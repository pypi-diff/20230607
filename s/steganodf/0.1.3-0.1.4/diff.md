# Comparing `tmp/steganodf-0.1.3.tar.gz` & `tmp/steganodf-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steganodf-0.1.3.tar", max compression
+gzip compressed data, was "steganodf-0.1.4.tar", max compression
```

## Comparing `steganodf-0.1.3.tar` & `steganodf-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      837 2023-05-29 22:52:55.771268 steganodf-0.1.3/README.md
--rw-r--r--   0        0        0      447 2023-06-05 23:36:54.384112 steganodf-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5967 2023-06-05 22:30:27.037481 steganodf-0.1.3/steganodf/__init__.py
--rw-r--r--   0        0        0     2053 2023-06-05 23:29:15.344116 steganodf-0.1.3/steganodf/__main__.py
--rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 steganodf-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      949 2023-06-07 21:12:25.438851 steganodf-0.1.4/README.md
+-rw-r--r--   0        0        0      447 2023-06-07 21:13:24.565518 steganodf-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5967 2023-06-05 22:30:27.037481 steganodf-0.1.4/steganodf/__init__.py
+-rw-r--r--   0        0        0     2460 2023-06-07 20:59:43.455525 steganodf-0.1.4/steganodf/__main__.py
+-rw-r--r--   0        0        0     1450 1970-01-01 00:00:00.000000 steganodf-0.1.4/PKG-INFO
```

### Comparing `steganodf-0.1.3/steganodf/__init__.py` & `steganodf-0.1.4/steganodf/__init__.py`

 * *Files identical despite different names*

### Comparing `steganodf-0.1.3/steganodf/__main__.py` & `steganodf-0.1.4/steganodf/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,69 +5,71 @@
 
 supported_format = {
         ".csv" : (pd.read_csv, pd.DataFrame.to_csv),
         ".parquet": (pd.read_parquet, pd.DataFrame.to_parquet)
         }
 
 
-def encode(input_file:Path, output_file:Path, payload:str):
+def encode(input_file:Path, output_file:Path, message:str, password:None|str = None):
 
     extension = input_file.suffix
     
     if extension not in supported_format:
         raise Exception("File Format is not supported")
     
     reader, writer  = supported_format[extension]
     df = reader(input_file)
-    encoded_df  = st.encode_pandas(df, payload)
+    encoded_df  = st.encode_pandas(df, message, password=password)
     
     writer(encoded_df, output_file, index=None)
     
 
 
-def decode(input_file:Path):
+def decode(input_file:Path, password:None|str):
 
     extension = input_file.suffix
     
     if extension not in supported_format:
         raise Exception("File Format is not supported")
     
     reader, _ = supported_format[extension]
 
     df = reader(input_file)
     
-    message = st.decode_pandas(df)
+    message = st.decode_pandas(df, password=password)
     return message
 
     
-def cli():
+def cli(args):
 
     parser = argparse.ArgumentParser(prog='steganodf', description="a Tool to hide a message in a tabular file")
     subparsers = parser.add_subparsers(dest='command')
 
     # Sous-commande "encode"
     encode_parser = subparsers.add_parser('encode', help='Encode a file')
     encode_parser.add_argument('--input', "-i", type=Path, required=True, help='source file (csv,parquet)')
     encode_parser.add_argument('--output',"-o", type=Path,required=True, help='File with the hidding message (csv,parquet)')
-    encode_parser.add_argument('--payload',"-p", type=str, required=True, help='Payload message')
+    encode_parser.add_argument('--message',"-m", type=str, required=True, help='Payload message')
+    encode_parser.add_argument('--password',"-p", type=str, required=False, help='Use a password')
 
     # Sous-commande "decode"
     decode_parser = subparsers.add_parser('decode', help='File with the hidding message (csv or parquet)')
     decode_parser.add_argument('--input', "-i", type=Path,required=True, help='Input file')
+    decode_parser.add_argument('--password', "-p", type=str,required=False, help='Use a password')
 
-    args = parser.parse_args()
+    parsed_args = parser.parse_args(args)
 
-    if args.command == 'encode':
-        encode(args.input, args.output, args.payload)
-    elif args.command == 'decode':
-        print(decode(args.input))
+    if parsed_args.command == 'encode':
+        encode(parsed_args.input, parsed_args.output, parsed_args.message,parsed_args.password)
+    elif parsed_args.command == 'decode':
+        print(decode(parsed_args.input, parsed_args.password))
     else:
         parser.print_help()
     
 
 
 
 if __name__ == "__main__":
+    import sys
 
-
-    cli()
+    cli(sys.argv[1:])
```

### Comparing `steganodf-0.1.3/PKG-INFO` & `steganodf-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 Metadata-Version: 2.1
 Name: steganodf
-Version: 0.1.3
+Version: 0.1.4
 Summary: Functions to add steganographic message to a dataframe with row permutation
 Author: Sacha Schutz
 Author-email: sacha@labsquare.org
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 
 # Steganodf 
 
-Steganodf is a tool to hide a secret message in a pandas dataframe by swapping lines. 
-It works with permutation of block of 6 lines (720 combinaisons) to store 1 byte. 
+This is a Python tool for hiding a secret message in a tabulated file ( e.g: CSV file ) .
+It works by swapping blocks of 6 lines, each capable of storing 1 bytes ( 6! > 255 bits ) 
 
-The dataframe is first sorted by the computed hash of each line. You can also use HMAC 
-if you give a password. This prevents the attacker from finding the secret message. 
-Indexes of each block of 6 lines are used as the source of permutation. A byte is then encoded 
-as the n-th permutation. 
+The dataframe is first sorted by the computed hash of each line. HMAC is also supported if you provide a password.
+This method does not alter the data, but the watermark is easily sterilized.
 
 
 # Installation 
 
 ```
 pip install steganodf
 ```
 
 # Usage 
 
+## From command line 
+```bash 
+
+steganodf encode -i iris.csv -o iris.w.csv -m hello -p password
+steganodf decode -i iris.w.csv -p password
+
+```
+
+## From Python
 
 ```python
 import steganodf 
 
  
 df = pd.read_csv("https://gist.githubusercontent.com/netj/8836201/raw/6f9306ad21398ea43cba4f7d537619d0e07d5ae3/iris.csv")
 
-# Encode a message
-new_df = steganodf.encode_pandas(df, "made by steganodf")
+# Hide your message 
+new_df = steganodf.encode_pandas(df, "made by steganodf", password="secret")
 
-# Decode a message 
-message = steganodf.decode_pandas(df)
+# Extract your message 
+message = steganodf.decode_pandas(df, password="secret")
 
 ```
```

