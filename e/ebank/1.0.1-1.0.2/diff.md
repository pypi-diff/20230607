# Comparing `tmp/ebank-1.0.1.tar.gz` & `tmp/ebank-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebank-1.0.1.tar", last modified: Tue Jun  6 09:58:42 2023, max compression
+gzip compressed data, was "ebank-1.0.2.tar", last modified: Wed Jun  7 09:31:33 2023, max compression
```

## Comparing `ebank-1.0.1.tar` & `ebank-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 09:58:42.423133 ebank-1.0.1/
--rw-rw-rw-   0        0        0       52 2023-06-06 09:58:42.421328 ebank-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-06 09:58:42.362132 ebank-1.0.1/ebank/
--rw-rw-rw-   0        0        0        2 2023-06-06 05:27:42.000000 ebank-1.0.1/ebank/__init__.py
--rw-rw-rw-   0        0        0    24486 2023-06-06 05:27:42.000000 ebank-1.0.1/ebank/receipt.py
--rw-rw-rw-   0        0        0     4770 2023-06-06 09:45:38.000000 ebank-1.0.1/ebank/trans.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:58:42.417135 ebank-1.0.1/ebank/utils/
--rw-rw-rw-   0        0        0        2 2023-06-06 05:27:42.000000 ebank-1.0.1/ebank/utils/__init__.py
--rw-rw-rw-   0        0        0     2156 2023-06-06 09:41:09.000000 ebank-1.0.1/ebank/utils/baiduocr.py
--rw-rw-rw-   0        0        0     1516 2023-06-06 09:40:51.000000 ebank-1.0.1/ebank/utils/chaojiying.py
--rw-rw-rw-   0        0        0     2474 2023-06-06 05:27:42.000000 ebank-1.0.1/ebank/utils/filesearch.py
--rw-rw-rw-   0        0        0     4814 2023-06-06 07:10:48.000000 ebank-1.0.1/ebank/utils/sfun.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:58:42.386145 ebank-1.0.1/ebank.egg-info/
--rw-rw-rw-   0        0        0       52 2023-06-06 09:58:42.000000 ebank-1.0.1/ebank.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-06-06 09:58:42.000000 ebank-1.0.1/ebank.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 09:58:42.000000 ebank-1.0.1/ebank.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-06-06 09:58:42.000000 ebank-1.0.1/ebank.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-06 09:58:42.000000 ebank-1.0.1/ebank.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 09:58:42.423133 ebank-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      500 2023-06-06 09:58:34.000000 ebank-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 09:31:33.408348 ebank-1.0.2/
+-rw-rw-rw-   0        0        0       52 2023-06-07 09:31:33.407348 ebank-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-07 09:31:33.355345 ebank-1.0.2/ebank/
+-rw-rw-rw-   0        0        0        4 2023-06-07 07:25:49.000000 ebank-1.0.2/ebank/__init__.py
+-rw-rw-rw-   0        0        0     4766 2023-06-07 09:17:41.000000 ebank-1.0.2/ebank/balance.py
+-rw-rw-rw-   0        0        0     1211 2023-06-07 09:24:29.000000 ebank-1.0.2/ebank/constants.py
+-rw-rw-rw-   0        0        0    24486 2023-06-06 05:27:42.000000 ebank-1.0.2/ebank/receipt.py
+-rw-rw-rw-   0        0        0     6639 2023-06-07 08:48:28.000000 ebank-1.0.2/ebank/trans.py
+drwxrwxrwx   0        0        0        0 2023-06-07 09:31:33.404348 ebank-1.0.2/ebank/utils/
+-rw-rw-rw-   0        0        0        2 2023-06-06 05:27:42.000000 ebank-1.0.2/ebank/utils/__init__.py
+-rw-rw-rw-   0        0        0     2156 2023-06-06 09:41:09.000000 ebank-1.0.2/ebank/utils/baiduocr.py
+-rw-rw-rw-   0        0        0     1516 2023-06-06 09:40:51.000000 ebank-1.0.2/ebank/utils/chaojiying.py
+-rw-rw-rw-   0        0        0     2474 2023-06-06 05:27:42.000000 ebank-1.0.2/ebank/utils/filesearch.py
+-rw-rw-rw-   0        0        0     4816 2023-06-07 07:26:54.000000 ebank-1.0.2/ebank/utils/sfun.py
+drwxrwxrwx   0        0        0        0 2023-06-07 09:31:33.380405 ebank-1.0.2/ebank.egg-info/
+-rw-rw-rw-   0        0        0       52 2023-06-07 09:31:33.000000 ebank-1.0.2/ebank.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-06-07 09:31:33.000000 ebank-1.0.2/ebank.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 09:31:33.000000 ebank-1.0.2/ebank.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-06-07 09:31:33.000000 ebank-1.0.2/ebank.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-07 09:31:33.000000 ebank-1.0.2/ebank.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 09:31:33.409346 ebank-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      500 2023-06-07 09:14:50.000000 ebank-1.0.2/setup.py
```

### Comparing `ebank-1.0.1/ebank/receipt.py` & `ebank-1.0.2/ebank/receipt.py`

 * *Files identical despite different names*

### Comparing `ebank-1.0.1/ebank/trans.py` & `ebank-1.0.2/ebank/balance.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,153 +1,149 @@
 import sqlite3
 from abc import ABC, abstractmethod
+from datetime import datetime
+
+import constants as CONSTANTS
 from encoo.logger import Logger
 from utils import sfun
 
 
-class BaseTrans(ABC):
-
-    BANK_NAME_IDX = -3
-    BANK_NO_IDX = -1
-    SQLITE3_PATH = r"D:\Repos\ebanktool\ebank\ebank.db"
+class BaseBalance(ABC):
 
-    _logger = Logger("BaseTrans")
+    _logger = Logger("BaseBalance")
 
     def __init__(self, file_path, row_start_idx):
 
-        # 流水文件路径
+        # 文件路径
         self.file_path = file_path
         # 开始取数行索引
         self.row_start_idx = row_start_idx
 
         # 银行名称
         self.bank_name = ""
-
         # 本方户名
         self.acc_name = ""
-        # 本方账号
+        # 账号
         self.acc_no = ""
 
-        # 交易日期
-        self.trans_date = ""
-        # 流水号
-        self.flow_no = ""
-        # 收入金额
-        self.rec_amt = 0.00
-        # 支出金额
-        self.pay_amt = 0.00
-        # 余额
-        self.balance = 0.00
-
-        # 对方户名
-        self.other_acc_name = ""
-        # 对方账号
-        self.other_acc_no = ""
-        # 对方行名
-        self.other_bank_name = ""
-
-        # 用途
-        self.purpose = ""
-        # 摘要
-        self.abstract = ""
-        # 备注
-        self.remark = ""
-
-        # 回单路径
-        self.rct_path = ""
+        # 查询时间
+        self.query_date = ""
+        # 可用余额
+        self.balance = ""
+
+        # 币种
+        self.currency = ""
+        self.task_id = ""
 
         self.excel_sheet = sfun.read_xl(self.file_path)
         # 从文件路径中加载信息
         self.__from_filepath()
 
     def __from_filepath(self):
         """ 从路径中获取信息
-        D:\\Ouye\\12家银行流水回单\\渤海银行\\2022-11-07\\H_2017037908000158_2022-11-01~2022-11-04.xls
+        "D:\Repos\工商银行\20230604\工行江苏省分行1_20230605_余额.xlsx"
         """
         try:
             fps = self.file_path.split("\\")
-            self.bank_name = fps[self.BANK_NAME_IDX]
-            self.bank_no = sfun.get_curno(fps[self.BANK_NO_IDX])
+            self.bank_name = fps[CONSTANTS.BANK_NAME_IDX]
 
         except Exception as ex:
-            self._logger.error(f"BaseTrans __from_filepath {ex}")
+            self._logger.error(f"BaseBalance __from_filepath {ex}")
 
     @abstractmethod
-    def build_trans(self, row_idx) -> list[str]:
+    def build_self(self, row_idx):
         pass
 
     def extract(self) -> list[tuple]:
         row_list = []
-        self._logger.info(f"BaseTrans extract idx {self.row_start_idx}")
+
         try:
+            self.task_id = datetime.now().strftime("%Y%m%d%H%M%S")
             for row_idx in range(self.row_start_idx, self.excel_sheet.nrows):
-                # 依次按列取值
-                trans_row = self.build_trans(row_idx)
-                row_list.append(tuple(trans_row))
+                # 调用子类实现的方法
+                self.build_self(row_idx)
+
+                trans_row = (self.file_path,
+                             self.bank_name,
+                             self.acc_name,
+                             self.acc_no,
+                             self.balance,
+                             self.query_date,
+                             self.currency,
+                             self.task_id,
+                             datetime.now(),
+                             datetime.now(),
+                             1)
+
+                row_list.append(trans_row)
             # end for
         except Exception as ex:
             self._logger.error(f"BaseTrans extract  {ex}")
         # end try
         return row_list
 
     def to_sqlite(self) -> None:
         rows = self.extract()
-        self._logger.info(f"BaseTrans to_sqlite {rows}")
+        self._logger.info(f"BaseBalance to_sqlite {rows}")
         try:
-            conn = sqlite3.connect(self.SQLITE3_PATH)
+            conn = sqlite3.connect(CONSTANTS.SQLITE3_PATH)
             cur = conn.cursor()
-            sql = ' insert into trans(file_path,bank_name,acc_name,acc_no,trans_date,flow_no,rec_amt,pay_amt,' + \
-                ' balance,other_acc_name,other_acc_no,other_bank_name,purpose,abstract,remark,rct_path) ' + \
-                ' values(?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?)'
-
+            sql = CONSTANTS.SQL_INSERT_BALANCE
             cur.executemany(sql, rows)
             conn.commit()
 
             cur.close()
             conn.close()
         except Exception as ex:
-            self._logger.error(f"BaseTrans to_sqlite {ex}")
+            self._logger.error(f"BaseBalance to_sqlite {ex}")
 
 
-class BeiJingTrans(BaseTrans):
+class ICBCBalance(BaseBalance):
 
-    # 流水文件开始取数索引
-    ROW_START_IDX = 3
+    ''' 工商银行
+        账　号	币种	钞汇标志	账户属性	昨日余额	当前余额	可用余额	查询时间	操作
+        4301016509812100729	英镑	汇	基本账户	600,000.00	600,000.00	600,000.00	15:50:08	
+        4301016509813100767	港币	汇	基本账户	20,004,076.60	20,004,076.60	20,004,076.60	15:50:08'''
+
+    # 文件开始取数索引
+    ROW_START_IDX = 2
 
     def __init__(self, file_path, row_start_idx=ROW_START_IDX):
         super().__init__(file_path, row_start_idx)
 
-    def build_trans(self, row_idx) -> list[str]:
+    def build_self(self, row_idx):
+        sheet = self.excel_sheet
+        # 依次按列取值
+        self.acc_no = sheet.cell(row_idx, 0).value
+        self.acc_name = CONSTANTS.BANK_NO_DICT[self.acc_no]
+        self.balance = sheet.cell(row_idx, 6).value
+        self.query_date = sheet.cell(row_idx, 7).value
+        self.currency = sheet.cell(row_idx, 1).value
+        return self
+
+
+class HXBBalance(BaseBalance):
+
+    ''' 工商银行
+        序号	账户别名	账号	账户名称	币种	可用余额
+        1	未定义	12592000000000515	江苏银行股份有限公司无锡分行	人民币	10,211.33'''
+
+    # 文件开始取数索引
+    ROW_START_IDX = 1
+
+    def __init__(self, file_path, row_start_idx=ROW_START_IDX):
+        super().__init__(file_path, row_start_idx)
 
+    def build_self(self, row_idx):
         sheet = self.excel_sheet
         # 依次按列取值
-        row_trans_date = sheet.cell(row_idx, 4).value
-        row_flow_no = sheet.cell(row_idx, 2).value
-        row_rec_amt = sheet.cell(row_idx, 8).value
-        row_pay_amt = sheet.cell(row_idx, 7).value
-        row_balance = sheet.cell(row_idx, 9).value
-        row_ant_name = sheet.cell(row_idx, 10).value
-        row_ant_no = sheet.cell(row_idx, 11).value
-        row_purpose = sheet.cell(row_idx, 6).value
-        row_abstract = sheet.cell(row_idx, 13).value
-
-        return [self.file_path,
-                self.bank_name,
-                self.acc_name,
-                self.acc_no,
-                row_trans_date,
-                row_flow_no,
-                row_rec_amt,
-                row_pay_amt,
-                row_balance,
-                row_ant_name,
-                row_ant_no,
-                self.other_bank_name,
-                row_purpose,
-                row_abstract,
-                self.remark,
-                self.rct_path]
+        self.acc_no = sheet.cell(row_idx, 2).value
+        self.acc_name = CONSTANTS.BANK_NO_DICT[self.acc_no]
+        self.balance = sheet.cell(row_idx, 5).value
+        self.query_date = ""
+        self.currency = sheet.cell(row_idx, 4).value
+        return self
 
 
 if (__name__ == "__main__"):
-    bfr = BeiJingTrans(
-        r"D:\Ouye\12家银行流水回单\北京银行\东方付通信息技术有限公司\2022-11-07\H20000021408900101114394 2022-03-01~2022-03-10.xls").to_sqlite()
+    bfr = HXBBalance(
+        r"D:\Repos\华夏银行\20230606\华夏银行无锡分行_20230606_余额.xlsx").to_sqlite()
```

### Comparing `ebank-1.0.1/ebank/utils/baiduocr.py` & `ebank-1.0.2/ebank/utils/baiduocr.py`

 * *Files identical despite different names*

### Comparing `ebank-1.0.1/ebank/utils/chaojiying.py` & `ebank-1.0.2/ebank/utils/chaojiying.py`

 * *Files identical despite different names*

### Comparing `ebank-1.0.1/ebank/utils/filesearch.py` & `ebank-1.0.2/ebank/utils/filesearch.py`

 * *Files identical despite different names*

### Comparing `ebank-1.0.1/ebank/utils/sfun.py` & `ebank-1.0.2/ebank/utils/sfun.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,244 +58,244 @@
 00000390: 6461 7465 292e 7374 7266 7469 6d65 2822  date).strftime("
 000003a0: 2559 2d25 6d2d 2564 2229 0d0a 2020 2020  %Y-%m-%d")..    
 000003b0: 6578 6365 7074 3a0d 0a20 2020 2020 2020  except:..       
 000003c0: 2072 6574 7572 6e20 7472 616e 735f 6461   return trans_da
 000003d0: 7465 0d0a 0d0a 0d0a 6465 6620 6765 745f  te......def get_
 000003e0: 6375 726e 6f28 6669 6c65 5f6e 616d 6529  curno(file_name)
 000003f0: 3a0d 0a20 2020 2072 6567 6578 203d 2072  :..    regex = r
-00000400: 2228 3f3c 3d48 295c 642a 220d 0a20 2020  "(?<=H)\d*"..   
-00000410: 2066 696e 6473 203d 2072 652e 6669 6e64   finds = re.find
-00000420: 616c 6c28 7265 6765 782c 2066 696c 655f  all(regex, file_
-00000430: 6e61 6d65 290d 0a20 2020 2069 6620 6c65  name)..    if le
-00000440: 6e28 6669 6e64 7329 203e 2030 3a0d 0a20  n(finds) > 0:.. 
-00000450: 2020 2020 2020 2072 6574 7572 6e20 6669         return fi
-00000460: 6e64 735b 305d 0d0a 2020 2020 656c 7365  nds[0]..    else
-00000470: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
-00000480: 6e20 2222 0d0a 0d0a 0d0a 6465 6620 7265  n ""......def re
-00000490: 6164 5f78 6c28 786c 5f70 6174 682c 2073  ad_xl(xl_path, s
-000004a0: 6865 6574 5f69 6478 3d30 293a 0d0a 2020  heet_idx=0):..  
-000004b0: 2020 786c 7320 3d20 786c 7264 2e6f 7065    xls = xlrd.ope
-000004c0: 6e5f 776f 726b 626f 6f6b 2878 6c5f 7061  n_workbook(xl_pa
-000004d0: 7468 2c20 666f 726d 6174 7469 6e67 5f69  th, formatting_i
-000004e0: 6e66 6f3d 5472 7565 290d 0a20 2020 2073  nfo=True)..    s
-000004f0: 6865 6574 203d 2078 6c73 2e73 6865 6574  heet = xls.sheet
-00000500: 5f62 795f 696e 6465 7828 7368 6565 745f  _by_index(sheet_
-00000510: 6964 7829 0d0a 2020 2020 7265 7475 726e  idx)..    return
-00000520: 2073 6865 6574 0d0a 0d0a 0d0a 6465 6620   sheet......def 
-00000530: 7774 5f72 6374 5f65 7863 656c 2878 6c5f  wt_rct_excel(xl_
-00000540: 7061 7468 2c20 7263 745f 6c69 7374 2920  path, rct_list) 
-00000550: 2d3e 2073 7472 3a0d 0a0d 0a20 2020 2065  -> str:....    e
-00000560: 7863 656c 5f68 6561 6465 7220 3d20 5b22  xcel_header = ["
-00000570: e59b 9ee5 8d95 e6b5 81e6 b0b4 e58f b722  ..............."
-00000580: 2c20 22e6 8891 e696 b9e5 85ac e58f b8e5  , ".............
-00000590: 908d e7a7 b022 2c20 22e9 93b6 e8a1 8ce5  .....", ".......
-000005a0: 908d e7a7 b022 2c20 22e6 9cac e696 b9e9  .....", ".......
-000005b0: 93b6 e8a1 8ce8 b4a6 e58f b722 2c20 22e6  ...........", ".
-000005c0: 97a5 e69c 9f22 2c0d 0a20 2020 2020 2020  .....",..       
-000005d0: 2020 2020 2020 2020 2020 2020 2022 e694               "..
-000005e0: b6e5 85a5 e987 91e9 a29d 222c 2022 e694  ..........", "..
-000005f0: afe5 87ba e987 91e9 a29d 222c 2022 e4bd  ..........", "..
-00000600: 99e9 a29d 222c 2022 e5af b9e6 96b9 e688  ....", "........
-00000610: b7e5 908d 222c 2022 e5af b9e6 96b9 e8b4  ....", "........
-00000620: a6e5 8fb7 222c 2022 e794 a8e9 8094 222c  ....", "......",
-00000630: 2022 e691 98e8 a681 222c 2022 e59b 9ee5   "......", "....
-00000640: 8d95 e8b7 afe5 be84 225d 0d0a 0d0a 2020  ........"]....  
-00000650: 2020 786c 203d 2078 6c77 742e 576f 726b    xl = xlwt.Work
-00000660: 626f 6f6b 2865 6e63 6f64 696e 673d 2275  book(encoding="u
-00000670: 6674 2d38 2229 0d0a 2020 2020 7368 6565  ft-8")..    shee
-00000680: 7420 3d20 786c 2e61 6464 5f73 6865 6574  t = xl.add_sheet
-00000690: 2822 7368 6565 7431 222c 2063 656c 6c5f  ("sheet1", cell_
-000006a0: 6f76 6572 7772 6974 655f 6f6b 3d46 616c  overwrite_ok=Fal
-000006b0: 7365 290d 0a0d 0a20 2020 2063 6f6c 5f69  se)....    col_i
-000006c0: 6478 203d 2030 0d0a 2020 2020 666f 7220  dx = 0..    for 
-000006d0: 636f 6c5f 6e61 6d65 2069 6e20 6578 6365  col_name in exce
-000006e0: 6c5f 6865 6164 6572 3a0d 0a20 2020 2020  l_header:..     
-000006f0: 2020 2073 6865 6574 2e77 7269 7465 2830     sheet.write(0
-00000700: 2c20 636f 6c5f 6964 782c 2063 6f6c 5f6e  , col_idx, col_n
-00000710: 616d 6529 0d0a 2020 2020 2020 2020 636f  ame)..        co
-00000720: 6c5f 6964 7820 3d20 636f 6c5f 6964 782b  l_idx = col_idx+
-00000730: 310d 0a0d 0a20 2020 2072 6f77 5f69 6478  1....    row_idx
-00000740: 203d 2031 0d0a 2020 2020 666f 7220 7263   = 1..    for rc
-00000750: 7420 696e 2072 6374 5f6c 6973 743a 0d0a  t in rct_list:..
-00000760: 2020 2020 2020 2020 7368 6565 742e 7772          sheet.wr
-00000770: 6974 6528 726f 775f 6964 782c 2030 2c20  ite(row_idx, 0, 
-00000780: 7263 742e 666c 6f77 5f6e 6f29 2020 2320  rct.flow_no)  # 
-00000790: e6b5 81e6 b0b4 e58f b70d 0a20 2020 2020  ...........     
-000007a0: 2020 2073 6865 6574 2e77 7269 7465 2872     sheet.write(r
-000007b0: 6f77 5f69 6478 2c20 312c 2072 6374 2e63  ow_idx, 1, rct.c
-000007c0: 6f6d 7061 6e79 5f6e 616d 6529 0d0a 2020  ompany_name)..  
-000007d0: 2020 2020 2020 7368 6565 742e 7772 6974        sheet.writ
-000007e0: 6528 726f 775f 6964 782c 2032 2c20 7263  e(row_idx, 2, rc
-000007f0: 742e 6261 6e6b 5f6e 616d 6529 0d0a 2020  t.bank_name)..  
-00000800: 2020 2020 2020 7368 6565 742e 7772 6974        sheet.writ
-00000810: 6528 726f 775f 6964 782c 2033 2c20 7263  e(row_idx, 3, rc
-00000820: 742e 6375 725f 6e6f 290d 0a20 2020 2020  t.cur_no)..     
-00000830: 2020 2073 6865 6574 2e77 7269 7465 2872     sheet.write(r
-00000840: 6f77 5f69 6478 2c20 342c 2072 6374 2e74  ow_idx, 4, rct.t
-00000850: 7261 6e73 5f64 6174 6529 0d0a 2020 2020  rans_date)..    
-00000860: 2020 2020 7368 6565 742e 7772 6974 6528      sheet.write(
-00000870: 726f 775f 6964 782c 2035 2c20 7263 742e  row_idx, 5, rct.
-00000880: 7265 635f 616d 7429 0d0a 2020 2020 2020  rec_amt)..      
-00000890: 2020 7368 6565 742e 7772 6974 6528 726f    sheet.write(ro
-000008a0: 775f 6964 782c 2036 2c20 7263 742e 7061  w_idx, 6, rct.pa
-000008b0: 795f 616d 7429 0d0a 2020 2020 2020 2020  y_amt)..        
-000008c0: 7368 6565 742e 7772 6974 6528 726f 775f  sheet.write(row_
-000008d0: 6964 782c 2038 2c20 7263 742e 616e 745f  idx, 8, rct.ant_
-000008e0: 6e61 6d65 290d 0a20 2020 2020 2020 2073  name)..        s
-000008f0: 6865 6574 2e77 7269 7465 2872 6f77 5f69  heet.write(row_i
-00000900: 6478 2c20 392c 2072 6374 2e61 6e74 5f6e  dx, 9, rct.ant_n
-00000910: 6f29 0d0a 2020 2020 2020 2020 7368 6565  o)..        shee
-00000920: 742e 7772 6974 6528 726f 775f 6964 782c  t.write(row_idx,
-00000930: 2031 322c 2072 6374 2e66 696c 655f 7061   12, rct.file_pa
-00000940: 7468 290d 0a0d 0a20 2020 2020 2020 2072  th)....        r
-00000950: 6f77 5f69 6478 203d 2072 6f77 5f69 6478  ow_idx = row_idx
-00000960: 2b31 0d0a 0d0a 2020 2020 786c 2e73 6176  +1....    xl.sav
-00000970: 6528 786c 5f70 6174 6829 0d0a 2020 2020  e(xl_path)..    
-00000980: 7265 7475 726e 2078 6c5f 7061 7468 0d0a  return xl_path..
-00000990: 0d0a 0d0a 6465 6620 7774 5f62 616e 6b66  ....def wt_bankf
-000009a0: 6c6f 775f 6578 6365 6c28 786c 5f70 6174  low_excel(xl_pat
-000009b0: 682c 2062 616e 6b66 6c6f 775f 6c69 7374  h, bankflow_list
-000009c0: 2920 2d3e 2073 7472 3a0d 0a0d 0a20 2020  ) -> str:....   
-000009d0: 2065 7863 656c 5f68 6561 6465 7220 3d20   excel_header = 
-000009e0: 5b22 e585 ace5 8fb8 e590 8de7 a7b0 222c  ["............",
-000009f0: 2022 e993 b6e8 a18c e590 8de7 a7b0 222c   "............",
-00000a00: 2022 e69c ace6 96b9 e993 b6e8 a18c e8b4   "..............
-00000a10: a6e5 8fb7 222c 2022 e697 a5e6 9c9f 222c  ....", "......",
-00000a20: 2022 e6b5 81e6 b0b4 e58f b722 2c0d 0a20   ".........",.. 
-00000a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a40: 2020 2022 e694 b6e5 85a5 e987 91e9 a29d     "............
-00000a50: 222c 2022 e694 afe5 87ba e987 91e9 a29d  ", "............
-00000a60: 222c 2022 e4bd 99e9 a29d 222c 2022 e5af  ", "......", "..
-00000a70: b9e6 96b9 e688 b7e5 908d 222c 2022 e5af  ..........", "..
-00000a80: b9e6 96b9 e8b4 a6e5 8fb7 222c 2022 e794  ..........", "..
-00000a90: a8e9 8094 222c 0d0a 2020 2020 2020 2020  ....",..        
-00000aa0: 2020 2020 2020 2020 2020 2020 22e6 9198              "...
-00000ab0: e8a6 8122 2c20 22e7 94b5 e5ad 90e5 9b9e  ...", ".........
-00000ac0: e58d 9522 2c20 22e6 9c8d e58a a1e5 99a8  ...", ".........
-00000ad0: e59b 9ee5 8d95 e8b7 afe5 be84 222c 2022  ............", "
-00000ae0: 5372 7655 5549 4422 5d0d 0a0d 0a20 2020  SrvUUID"]....   
-00000af0: 2078 6c20 3d20 786c 7774 2e57 6f72 6b62   xl = xlwt.Workb
-00000b00: 6f6f 6b28 656e 636f 6469 6e67 3d22 7566  ook(encoding="uf
-00000b10: 742d 3822 290d 0a20 2020 2073 6865 6574  t-8")..    sheet
-00000b20: 203d 2078 6c2e 6164 645f 7368 6565 7428   = xl.add_sheet(
-00000b30: 2273 6865 6574 3122 2c20 6365 6c6c 5f6f  "sheet1", cell_o
-00000b40: 7665 7277 7269 7465 5f6f 6b3d 4661 6c73  verwrite_ok=Fals
-00000b50: 6529 0d0a 0d0a 2020 2020 636f 6c5f 6964  e)....    col_id
-00000b60: 7820 3d20 300d 0a20 2020 2066 6f72 2063  x = 0..    for c
-00000b70: 6f6c 5f6e 616d 6520 696e 2065 7863 656c  ol_name in excel
-00000b80: 5f68 6561 6465 723a 0d0a 2020 2020 2020  _header:..      
-00000b90: 2020 7368 6565 742e 7772 6974 6528 302c    sheet.write(0,
-00000ba0: 2063 6f6c 5f69 6478 2c20 636f 6c5f 6e61   col_idx, col_na
-00000bb0: 6d65 290d 0a20 2020 2020 2020 2063 6f6c  me)..        col
-00000bc0: 5f69 6478 203d 2063 6f6c 5f69 6478 2b31  _idx = col_idx+1
-00000bd0: 0d0a 0d0a 2020 2020 726f 775f 6964 7820  ....    row_idx 
-00000be0: 3d20 310d 0a20 2020 2066 6f72 2062 6620  = 1..    for bf 
-00000bf0: 696e 2062 616e 6b66 6c6f 775f 6c69 7374  in bankflow_list
-00000c00: 3a0d 0a20 2020 2020 2020 2073 6865 6574  :..        sheet
-00000c10: 2e77 7269 7465 2872 6f77 5f69 6478 2c20  .write(row_idx, 
-00000c20: 302c 2062 662e 636f 6d70 616e 795f 6e61  0, bf.company_na
-00000c30: 6d65 290d 0a20 2020 2020 2020 2073 6865  me)..        she
-00000c40: 6574 2e77 7269 7465 2872 6f77 5f69 6478  et.write(row_idx
-00000c50: 2c20 312c 2062 662e 6261 6e6b 5f6e 616d  , 1, bf.bank_nam
-00000c60: 6529 0d0a 2020 2020 2020 2020 7368 6565  e)..        shee
-00000c70: 742e 7772 6974 6528 726f 775f 6964 782c  t.write(row_idx,
-00000c80: 2032 2c20 6266 2e62 616e 6b5f 6e6f 290d   2, bf.bank_no).
-00000c90: 0a20 2020 2020 2020 2073 6865 6574 2e77  .        sheet.w
-00000ca0: 7269 7465 2872 6f77 5f69 6478 2c20 332c  rite(row_idx, 3,
-00000cb0: 2062 662e 7472 616e 735f 6461 7465 290d   bf.trans_date).
-00000cc0: 0a20 2020 2020 2020 2073 6865 6574 2e77  .        sheet.w
-00000cd0: 7269 7465 2872 6f77 5f69 6478 2c20 342c  rite(row_idx, 4,
-00000ce0: 2062 662e 666c 6f77 5f6e 6f29 0d0a 2020   bf.flow_no)..  
-00000cf0: 2020 2020 2020 7368 6565 742e 7772 6974        sheet.writ
-00000d00: 6528 726f 775f 6964 782c 2035 2c20 6266  e(row_idx, 5, bf
-00000d10: 2e72 6563 5f61 6d74 290d 0a20 2020 2020  .rec_amt)..     
-00000d20: 2020 2073 6865 6574 2e77 7269 7465 2872     sheet.write(r
-00000d30: 6f77 5f69 6478 2c20 362c 2062 662e 7061  ow_idx, 6, bf.pa
-00000d40: 795f 616d 7429 0d0a 2020 2020 2020 2020  y_amt)..        
-00000d50: 7368 6565 742e 7772 6974 6528 726f 775f  sheet.write(row_
-00000d60: 6964 782c 2037 2c20 6266 2e62 616c 616e  idx, 7, bf.balan
-00000d70: 6365 290d 0a20 2020 2020 2020 2073 6865  ce)..        she
-00000d80: 6574 2e77 7269 7465 2872 6f77 5f69 6478  et.write(row_idx
-00000d90: 2c20 382c 2062 662e 616e 745f 6e61 6d65  , 8, bf.ant_name
-00000da0: 290d 0a20 2020 2020 2020 2073 6865 6574  )..        sheet
-00000db0: 2e77 7269 7465 2872 6f77 5f69 6478 2c20  .write(row_idx, 
-00000dc0: 392c 2062 662e 616e 745f 6e6f 290d 0a20  9, bf.ant_no).. 
-00000dd0: 2020 2020 2020 2073 6865 6574 2e77 7269         sheet.wri
-00000de0: 7465 2872 6f77 5f69 6478 2c20 3130 2c20  te(row_idx, 10, 
-00000df0: 6266 2e70 7572 706f 7365 290d 0a20 2020  bf.purpose)..   
-00000e00: 2020 2020 2073 6865 6574 2e77 7269 7465       sheet.write
-00000e10: 2872 6f77 5f69 6478 2c20 3131 2c20 6266  (row_idx, 11, bf
-00000e20: 2e73 756d 6d61 7279 290d 0a0d 0a20 2020  .summary)....   
-00000e30: 2020 2020 2072 6f77 5f69 6478 203d 2072       row_idx = r
-00000e40: 6f77 5f69 6478 2b31 0d0a 0d0a 2020 2020  ow_idx+1....    
-00000e50: 786c 2e73 6176 6528 786c 5f70 6174 6829  xl.save(xl_path)
-00000e60: 0d0a 2020 2020 7265 7475 726e 2078 6c5f  ..    return xl_
-00000e70: 7061 7468 0d0a 0d0a 0d0a 6465 6620 7370  path......def sp
-00000e80: 6c69 745f 7064 6628 7064 665f 6669 6c65  lit_pdf(pdf_file
-00000e90: 2c20 6f75 7470 7574 5f64 6972 3d4e 6f6e  , output_dir=Non
-00000ea0: 6529 3a0d 0a20 2020 2066 5f6e 616d 6520  e):..    f_name 
-00000eb0: 3d20 6f73 2e70 6174 682e 6261 7365 6e61  = os.path.basena
-00000ec0: 6d65 2870 6466 5f66 696c 6529 0d0a 2020  me(pdf_file)..  
-00000ed0: 2020 6966 206f 7574 7075 745f 6469 7220    if output_dir 
-00000ee0: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
-00000ef0: 2020 6f75 7470 7574 5f64 6972 203d 206f    output_dir = o
-00000f00: 732e 7061 7468 2e6a 6f69 6e28 6f73 2e70  s.path.join(os.p
-00000f10: 6174 682e 6469 726e 616d 6528 7064 665f  ath.dirname(pdf_
-00000f20: 6669 6c65 292c 2022 7375 6270 6466 2229  file), "subpdf")
-00000f30: 0d0a 0d0a 2020 2020 7064 6673 203d 205b  ....    pdfs = [
-00000f40: 5d0d 0a20 2020 2074 7279 3a0d 0a20 2020  ]..    try:..   
-00000f50: 2020 2020 2069 6620 6f73 2e70 6174 682e       if os.path.
-00000f60: 6578 6973 7473 286f 7574 7075 745f 6469  exists(output_di
-00000f70: 7229 203d 3d20 4661 6c73 653a 0d0a 2020  r) == False:..  
-00000f80: 2020 2020 2020 2020 2020 6f73 2e6d 6b64            os.mkd
-00000f90: 6972 286f 7574 7075 745f 6469 7229 0d0a  ir(output_dir)..
-00000fa0: 2020 2020 2020 2020 7265 6164 6572 203d          reader =
-00000fb0: 2050 6466 5265 6164 6572 2870 6466 5f66   PdfReader(pdf_f
-00000fc0: 696c 6529 0d0a 2020 2020 2020 2020 666f  ile)..        fo
-00000fd0: 7220 696e 6465 7820 696e 2072 616e 6765  r index in range
-00000fe0: 286c 656e 2872 6561 6465 722e 7061 6765  (len(reader.page
-00000ff0: 7329 293a 0d0a 2020 2020 2020 2020 2020  s)):..          
-00001000: 2020 7772 6974 6572 203d 2050 6466 5772    writer = PdfWr
-00001010: 6974 6572 2829 0d0a 2020 2020 2020 2020  iter()..        
-00001020: 2020 2020 7061 6765 4f62 6a20 3d20 7265      pageObj = re
-00001030: 6164 6572 2e70 6167 6573 5b69 6e64 6578  ader.pages[index
-00001040: 5d0d 0a20 2020 2020 2020 2020 2020 2077  ]..            w
-00001050: 7269 7465 722e 6164 645f 7061 6765 2870  riter.add_page(p
-00001060: 6167 654f 626a 290d 0a20 2020 2020 2020  ageObj)..       
-00001070: 2020 2020 206e 6577 7061 7468 203d 206f       newpath = o
-00001080: 732e 7061 7468 2e6a 6f69 6e28 6f75 7470  s.path.join(outp
-00001090: 7574 5f64 6972 2c20 6622 7b69 6e64 6578  ut_dir, f"{index
-000010a0: 7d5f 7b66 5f6e 616d 657d 2229 0d0a 2020  }_{f_name}")..  
-000010b0: 2020 2020 2020 2020 2020 7769 7468 206f            with o
-000010c0: 7065 6e28 6e65 7770 6174 682c 2027 7762  pen(newpath, 'wb
-000010d0: 2729 2061 7320 6677 3a0d 0a20 2020 2020  ') as fw:..     
-000010e0: 2020 2020 2020 2020 2020 2077 7269 7465             write
-000010f0: 722e 7772 6974 6528 6677 290d 0a0d 0a20  r.write(fw).... 
-00001100: 2020 2020 2020 2020 2020 2070 6466 732e             pdfs.
-00001110: 6170 7065 6e64 286e 6577 7061 7468 290d  append(newpath).
-00001120: 0a20 2020 2065 7863 6570 7420 4578 6365  .    except Exce
-00001130: 7074 696f 6e20 6173 2065 3a0d 0a20 2020  ption as e:..   
-00001140: 2020 2020 2070 7269 6e74 2865 290d 0a0d       print(e)...
-00001150: 0a20 2020 2072 6574 7572 6e20 7064 6673  .    return pdfs
-00001160: 0d0a 0d0a 0d0a 6465 6620 6765 745f 6669  ......def get_fi
-00001170: 6c65 5f63 6f6e 7465 6e74 5f61 735f 6261  le_content_as_ba
-00001180: 7365 3634 2870 6174 682c 2075 726c 656e  se64(path, urlen
-00001190: 636f 6465 643d 4661 6c73 6529 3a0d 0a20  coded=False):.. 
-000011a0: 2020 2077 6974 6820 6f70 656e 2870 6174     with open(pat
-000011b0: 682c 2022 7262 2229 2061 7320 663a 0d0a  h, "rb") as f:..
-000011c0: 2020 2020 2020 2020 636f 6e74 656e 7420          content 
-000011d0: 3d20 6261 7365 3634 2e62 3634 656e 636f  = base64.b64enco
-000011e0: 6465 2866 2e72 6561 6428 2929 2e64 6563  de(f.read()).dec
-000011f0: 6f64 6528 2275 7466 3822 290d 0a20 2020  ode("utf8")..   
-00001200: 2020 2020 2069 6620 7572 6c65 6e63 6f64       if urlencod
-00001210: 6564 3a0d 0a20 2020 2020 2020 2020 2020  ed:..           
-00001220: 2063 6f6e 7465 6e74 203d 2075 726c 6c69   content = urlli
-00001230: 622e 7061 7273 652e 7175 6f74 655f 706c  b.parse.quote_pl
-00001240: 7573 2863 6f6e 7465 6e74 290d 0a20 2020  us(content)..   
-00001250: 2072 6574 7572 6e20 636f 6e74 656e 740d   return content.
-00001260: 0a0d 0a0d 0a69 6620 5f5f 6e61 6d65 5f5f  .....if __name__
-00001270: 203d 3d20 225f 5f6d 6169 6e5f 5f22 3a0d   == "__main__":.
-00001280: 0a20 2020 206b 7620 3d20 7b22 6b22 3a20  .    kv = {"k": 
-00001290: 2276 227d 0d0a 2020 2020 7072 696e 7428  "v"}..    print(
-000012a0: 6b76 2e67 6574 2822 6b22 2929 0d0a 2020  kv.get("k"))..  
-000012b0: 2020 7072 696e 7428 6b76 2e67 6574 2822    print(kv.get("
-000012c0: 6b73 7322 2c20 2273 7322 2929 0d0a       kss", "ss"))..
+00000400: 2228 3f3c 3d48 5f29 5c64 2a22 0d0a 2020  "(?<=H_)\d*"..  
+00000410: 2020 6669 6e64 7320 3d20 7265 2e66 696e    finds = re.fin
+00000420: 6461 6c6c 2872 6567 6578 2c20 6669 6c65  dall(regex, file
+00000430: 5f6e 616d 6529 0d0a 2020 2020 6966 206c  _name)..    if l
+00000440: 656e 2866 696e 6473 2920 3e20 303a 0d0a  en(finds) > 0:..
+00000450: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+00000460: 696e 6473 5b30 5d0d 0a20 2020 2065 6c73  inds[0]..    els
+00000470: 653a 0d0a 2020 2020 2020 2020 7265 7475  e:..        retu
+00000480: 726e 2022 220d 0a0d 0a0d 0a64 6566 2072  rn ""......def r
+00000490: 6561 645f 786c 2878 6c5f 7061 7468 2c20  ead_xl(xl_path, 
+000004a0: 7368 6565 745f 6964 783d 3029 3a0d 0a20  sheet_idx=0):.. 
+000004b0: 2020 2078 6c73 203d 2078 6c72 642e 6f70     xls = xlrd.op
+000004c0: 656e 5f77 6f72 6b62 6f6f 6b28 786c 5f70  en_workbook(xl_p
+000004d0: 6174 682c 2066 6f72 6d61 7474 696e 675f  ath, formatting_
+000004e0: 696e 666f 3d46 616c 7365 290d 0a20 2020  info=False)..   
+000004f0: 2073 6865 6574 203d 2078 6c73 2e73 6865   sheet = xls.she
+00000500: 6574 5f62 795f 696e 6465 7828 7368 6565  et_by_index(shee
+00000510: 745f 6964 7829 0d0a 2020 2020 7265 7475  t_idx)..    retu
+00000520: 726e 2073 6865 6574 0d0a 0d0a 0d0a 6465  rn sheet......de
+00000530: 6620 7774 5f72 6374 5f65 7863 656c 2878  f wt_rct_excel(x
+00000540: 6c5f 7061 7468 2c20 7263 745f 6c69 7374  l_path, rct_list
+00000550: 2920 2d3e 2073 7472 3a0d 0a0d 0a20 2020  ) -> str:....   
+00000560: 2065 7863 656c 5f68 6561 6465 7220 3d20   excel_header = 
+00000570: 5b22 e59b 9ee5 8d95 e6b5 81e6 b0b4 e58f  ["..............
+00000580: b722 2c20 22e6 8891 e696 b9e5 85ac e58f  .", "...........
+00000590: b8e5 908d e7a7 b022 2c20 22e9 93b6 e8a1  .......", ".....
+000005a0: 8ce5 908d e7a7 b022 2c20 22e6 9cac e696  .......", ".....
+000005b0: b9e9 93b6 e8a1 8ce8 b4a6 e58f b722 2c20  .............", 
+000005c0: 22e6 97a5 e69c 9f22 2c0d 0a20 2020 2020  "......",..     
+000005d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000005e0: e694 b6e5 85a5 e987 91e9 a29d 222c 2022  ............", "
+000005f0: e694 afe5 87ba e987 91e9 a29d 222c 2022  ............", "
+00000600: e4bd 99e9 a29d 222c 2022 e5af b9e6 96b9  ......", "......
+00000610: e688 b7e5 908d 222c 2022 e5af b9e6 96b9  ......", "......
+00000620: e8b4 a6e5 8fb7 222c 2022 e794 a8e9 8094  ......", "......
+00000630: 222c 2022 e691 98e8 a681 222c 2022 e59b  ", "......", "..
+00000640: 9ee5 8d95 e8b7 afe5 be84 225d 0d0a 0d0a  .........."]....
+00000650: 2020 2020 786c 203d 2078 6c77 742e 576f      xl = xlwt.Wo
+00000660: 726b 626f 6f6b 2865 6e63 6f64 696e 673d  rkbook(encoding=
+00000670: 2275 6674 2d38 2229 0d0a 2020 2020 7368  "uft-8")..    sh
+00000680: 6565 7420 3d20 786c 2e61 6464 5f73 6865  eet = xl.add_she
+00000690: 6574 2822 7368 6565 7431 222c 2063 656c  et("sheet1", cel
+000006a0: 6c5f 6f76 6572 7772 6974 655f 6f6b 3d46  l_overwrite_ok=F
+000006b0: 616c 7365 290d 0a0d 0a20 2020 2063 6f6c  alse)....    col
+000006c0: 5f69 6478 203d 2030 0d0a 2020 2020 666f  _idx = 0..    fo
+000006d0: 7220 636f 6c5f 6e61 6d65 2069 6e20 6578  r col_name in ex
+000006e0: 6365 6c5f 6865 6164 6572 3a0d 0a20 2020  cel_header:..   
+000006f0: 2020 2020 2073 6865 6574 2e77 7269 7465       sheet.write
+00000700: 2830 2c20 636f 6c5f 6964 782c 2063 6f6c  (0, col_idx, col
+00000710: 5f6e 616d 6529 0d0a 2020 2020 2020 2020  _name)..        
+00000720: 636f 6c5f 6964 7820 3d20 636f 6c5f 6964  col_idx = col_id
+00000730: 782b 310d 0a0d 0a20 2020 2072 6f77 5f69  x+1....    row_i
+00000740: 6478 203d 2031 0d0a 2020 2020 666f 7220  dx = 1..    for 
+00000750: 7263 7420 696e 2072 6374 5f6c 6973 743a  rct in rct_list:
+00000760: 0d0a 2020 2020 2020 2020 7368 6565 742e  ..        sheet.
+00000770: 7772 6974 6528 726f 775f 6964 782c 2030  write(row_idx, 0
+00000780: 2c20 7263 742e 666c 6f77 5f6e 6f29 2020  , rct.flow_no)  
+00000790: 2320 e6b5 81e6 b0b4 e58f b70d 0a20 2020  # ...........   
+000007a0: 2020 2020 2073 6865 6574 2e77 7269 7465       sheet.write
+000007b0: 2872 6f77 5f69 6478 2c20 312c 2072 6374  (row_idx, 1, rct
+000007c0: 2e63 6f6d 7061 6e79 5f6e 616d 6529 0d0a  .company_name)..
+000007d0: 2020 2020 2020 2020 7368 6565 742e 7772          sheet.wr
+000007e0: 6974 6528 726f 775f 6964 782c 2032 2c20  ite(row_idx, 2, 
+000007f0: 7263 742e 6261 6e6b 5f6e 616d 6529 0d0a  rct.bank_name)..
+00000800: 2020 2020 2020 2020 7368 6565 742e 7772          sheet.wr
+00000810: 6974 6528 726f 775f 6964 782c 2033 2c20  ite(row_idx, 3, 
+00000820: 7263 742e 6375 725f 6e6f 290d 0a20 2020  rct.cur_no)..   
+00000830: 2020 2020 2073 6865 6574 2e77 7269 7465       sheet.write
+00000840: 2872 6f77 5f69 6478 2c20 342c 2072 6374  (row_idx, 4, rct
+00000850: 2e74 7261 6e73 5f64 6174 6529 0d0a 2020  .trans_date)..  
+00000860: 2020 2020 2020 7368 6565 742e 7772 6974        sheet.writ
+00000870: 6528 726f 775f 6964 782c 2035 2c20 7263  e(row_idx, 5, rc
+00000880: 742e 7265 635f 616d 7429 0d0a 2020 2020  t.rec_amt)..    
+00000890: 2020 2020 7368 6565 742e 7772 6974 6528      sheet.write(
+000008a0: 726f 775f 6964 782c 2036 2c20 7263 742e  row_idx, 6, rct.
+000008b0: 7061 795f 616d 7429 0d0a 2020 2020 2020  pay_amt)..      
+000008c0: 2020 7368 6565 742e 7772 6974 6528 726f    sheet.write(ro
+000008d0: 775f 6964 782c 2038 2c20 7263 742e 616e  w_idx, 8, rct.an
+000008e0: 745f 6e61 6d65 290d 0a20 2020 2020 2020  t_name)..       
+000008f0: 2073 6865 6574 2e77 7269 7465 2872 6f77   sheet.write(row
+00000900: 5f69 6478 2c20 392c 2072 6374 2e61 6e74  _idx, 9, rct.ant
+00000910: 5f6e 6f29 0d0a 2020 2020 2020 2020 7368  _no)..        sh
+00000920: 6565 742e 7772 6974 6528 726f 775f 6964  eet.write(row_id
+00000930: 782c 2031 322c 2072 6374 2e66 696c 655f  x, 12, rct.file_
+00000940: 7061 7468 290d 0a0d 0a20 2020 2020 2020  path)....       
+00000950: 2072 6f77 5f69 6478 203d 2072 6f77 5f69   row_idx = row_i
+00000960: 6478 2b31 0d0a 0d0a 2020 2020 786c 2e73  dx+1....    xl.s
+00000970: 6176 6528 786c 5f70 6174 6829 0d0a 2020  ave(xl_path)..  
+00000980: 2020 7265 7475 726e 2078 6c5f 7061 7468    return xl_path
+00000990: 0d0a 0d0a 0d0a 6465 6620 7774 5f62 616e  ......def wt_ban
+000009a0: 6b66 6c6f 775f 6578 6365 6c28 786c 5f70  kflow_excel(xl_p
+000009b0: 6174 682c 2062 616e 6b66 6c6f 775f 6c69  ath, bankflow_li
+000009c0: 7374 2920 2d3e 2073 7472 3a0d 0a0d 0a20  st) -> str:.... 
+000009d0: 2020 2065 7863 656c 5f68 6561 6465 7220     excel_header 
+000009e0: 3d20 5b22 e585 ace5 8fb8 e590 8de7 a7b0  = ["............
+000009f0: 222c 2022 e993 b6e8 a18c e590 8de7 a7b0  ", "............
+00000a00: 222c 2022 e69c ace6 96b9 e993 b6e8 a18c  ", "............
+00000a10: e8b4 a6e5 8fb7 222c 2022 e697 a5e6 9c9f  ......", "......
+00000a20: 222c 2022 e6b5 81e6 b0b4 e58f b722 2c0d  ", ".........",.
+00000a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000a40: 2020 2020 2022 e694 b6e5 85a5 e987 91e9       "..........
+00000a50: a29d 222c 2022 e694 afe5 87ba e987 91e9  ..", "..........
+00000a60: a29d 222c 2022 e4bd 99e9 a29d 222c 2022  ..", "......", "
+00000a70: e5af b9e6 96b9 e688 b7e5 908d 222c 2022  ............", "
+00000a80: e5af b9e6 96b9 e8b4 a6e5 8fb7 222c 2022  ............", "
+00000a90: e794 a8e9 8094 222c 0d0a 2020 2020 2020  ......",..      
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 22e6                ".
+00000ab0: 9198 e8a6 8122 2c20 22e7 94b5 e5ad 90e5  .....", ".......
+00000ac0: 9b9e e58d 9522 2c20 22e6 9c8d e58a a1e5  .....", ".......
+00000ad0: 99a8 e59b 9ee5 8d95 e8b7 afe5 be84 222c  ..............",
+00000ae0: 2022 5372 7655 5549 4422 5d0d 0a0d 0a20   "SrvUUID"].... 
+00000af0: 2020 2078 6c20 3d20 786c 7774 2e57 6f72     xl = xlwt.Wor
+00000b00: 6b62 6f6f 6b28 656e 636f 6469 6e67 3d22  kbook(encoding="
+00000b10: 7566 742d 3822 290d 0a20 2020 2073 6865  uft-8")..    she
+00000b20: 6574 203d 2078 6c2e 6164 645f 7368 6565  et = xl.add_shee
+00000b30: 7428 2273 6865 6574 3122 2c20 6365 6c6c  t("sheet1", cell
+00000b40: 5f6f 7665 7277 7269 7465 5f6f 6b3d 4661  _overwrite_ok=Fa
+00000b50: 6c73 6529 0d0a 0d0a 2020 2020 636f 6c5f  lse)....    col_
+00000b60: 6964 7820 3d20 300d 0a20 2020 2066 6f72  idx = 0..    for
+00000b70: 2063 6f6c 5f6e 616d 6520 696e 2065 7863   col_name in exc
+00000b80: 656c 5f68 6561 6465 723a 0d0a 2020 2020  el_header:..    
+00000b90: 2020 2020 7368 6565 742e 7772 6974 6528      sheet.write(
+00000ba0: 302c 2063 6f6c 5f69 6478 2c20 636f 6c5f  0, col_idx, col_
+00000bb0: 6e61 6d65 290d 0a20 2020 2020 2020 2063  name)..        c
+00000bc0: 6f6c 5f69 6478 203d 2063 6f6c 5f69 6478  ol_idx = col_idx
+00000bd0: 2b31 0d0a 0d0a 2020 2020 726f 775f 6964  +1....    row_id
+00000be0: 7820 3d20 310d 0a20 2020 2066 6f72 2062  x = 1..    for b
+00000bf0: 6620 696e 2062 616e 6b66 6c6f 775f 6c69  f in bankflow_li
+00000c00: 7374 3a0d 0a20 2020 2020 2020 2073 6865  st:..        she
+00000c10: 6574 2e77 7269 7465 2872 6f77 5f69 6478  et.write(row_idx
+00000c20: 2c20 302c 2062 662e 636f 6d70 616e 795f  , 0, bf.company_
+00000c30: 6e61 6d65 290d 0a20 2020 2020 2020 2073  name)..        s
+00000c40: 6865 6574 2e77 7269 7465 2872 6f77 5f69  heet.write(row_i
+00000c50: 6478 2c20 312c 2062 662e 6261 6e6b 5f6e  dx, 1, bf.bank_n
+00000c60: 616d 6529 0d0a 2020 2020 2020 2020 7368  ame)..        sh
+00000c70: 6565 742e 7772 6974 6528 726f 775f 6964  eet.write(row_id
+00000c80: 782c 2032 2c20 6266 2e62 616e 6b5f 6e6f  x, 2, bf.bank_no
+00000c90: 290d 0a20 2020 2020 2020 2073 6865 6574  )..        sheet
+00000ca0: 2e77 7269 7465 2872 6f77 5f69 6478 2c20  .write(row_idx, 
+00000cb0: 332c 2062 662e 7472 616e 735f 6461 7465  3, bf.trans_date
+00000cc0: 290d 0a20 2020 2020 2020 2073 6865 6574  )..        sheet
+00000cd0: 2e77 7269 7465 2872 6f77 5f69 6478 2c20  .write(row_idx, 
+00000ce0: 342c 2062 662e 666c 6f77 5f6e 6f29 0d0a  4, bf.flow_no)..
+00000cf0: 2020 2020 2020 2020 7368 6565 742e 7772          sheet.wr
+00000d00: 6974 6528 726f 775f 6964 782c 2035 2c20  ite(row_idx, 5, 
+00000d10: 6266 2e72 6563 5f61 6d74 290d 0a20 2020  bf.rec_amt)..   
+00000d20: 2020 2020 2073 6865 6574 2e77 7269 7465       sheet.write
+00000d30: 2872 6f77 5f69 6478 2c20 362c 2062 662e  (row_idx, 6, bf.
+00000d40: 7061 795f 616d 7429 0d0a 2020 2020 2020  pay_amt)..      
+00000d50: 2020 7368 6565 742e 7772 6974 6528 726f    sheet.write(ro
+00000d60: 775f 6964 782c 2037 2c20 6266 2e62 616c  w_idx, 7, bf.bal
+00000d70: 616e 6365 290d 0a20 2020 2020 2020 2073  ance)..        s
+00000d80: 6865 6574 2e77 7269 7465 2872 6f77 5f69  heet.write(row_i
+00000d90: 6478 2c20 382c 2062 662e 616e 745f 6e61  dx, 8, bf.ant_na
+00000da0: 6d65 290d 0a20 2020 2020 2020 2073 6865  me)..        she
+00000db0: 6574 2e77 7269 7465 2872 6f77 5f69 6478  et.write(row_idx
+00000dc0: 2c20 392c 2062 662e 616e 745f 6e6f 290d  , 9, bf.ant_no).
+00000dd0: 0a20 2020 2020 2020 2073 6865 6574 2e77  .        sheet.w
+00000de0: 7269 7465 2872 6f77 5f69 6478 2c20 3130  rite(row_idx, 10
+00000df0: 2c20 6266 2e70 7572 706f 7365 290d 0a20  , bf.purpose).. 
+00000e00: 2020 2020 2020 2073 6865 6574 2e77 7269         sheet.wri
+00000e10: 7465 2872 6f77 5f69 6478 2c20 3131 2c20  te(row_idx, 11, 
+00000e20: 6266 2e73 756d 6d61 7279 290d 0a0d 0a20  bf.summary).... 
+00000e30: 2020 2020 2020 2072 6f77 5f69 6478 203d         row_idx =
+00000e40: 2072 6f77 5f69 6478 2b31 0d0a 0d0a 2020   row_idx+1....  
+00000e50: 2020 786c 2e73 6176 6528 786c 5f70 6174    xl.save(xl_pat
+00000e60: 6829 0d0a 2020 2020 7265 7475 726e 2078  h)..    return x
+00000e70: 6c5f 7061 7468 0d0a 0d0a 0d0a 6465 6620  l_path......def 
+00000e80: 7370 6c69 745f 7064 6628 7064 665f 6669  split_pdf(pdf_fi
+00000e90: 6c65 2c20 6f75 7470 7574 5f64 6972 3d4e  le, output_dir=N
+00000ea0: 6f6e 6529 3a0d 0a20 2020 2066 5f6e 616d  one):..    f_nam
+00000eb0: 6520 3d20 6f73 2e70 6174 682e 6261 7365  e = os.path.base
+00000ec0: 6e61 6d65 2870 6466 5f66 696c 6529 0d0a  name(pdf_file)..
+00000ed0: 2020 2020 6966 206f 7574 7075 745f 6469      if output_di
+00000ee0: 7220 6973 204e 6f6e 653a 0d0a 2020 2020  r is None:..    
+00000ef0: 2020 2020 6f75 7470 7574 5f64 6972 203d      output_dir =
+00000f00: 206f 732e 7061 7468 2e6a 6f69 6e28 6f73   os.path.join(os
+00000f10: 2e70 6174 682e 6469 726e 616d 6528 7064  .path.dirname(pd
+00000f20: 665f 6669 6c65 292c 2022 7375 6270 6466  f_file), "subpdf
+00000f30: 2229 0d0a 0d0a 2020 2020 7064 6673 203d  ")....    pdfs =
+00000f40: 205b 5d0d 0a20 2020 2074 7279 3a0d 0a20   []..    try:.. 
+00000f50: 2020 2020 2020 2069 6620 6f73 2e70 6174         if os.pat
+00000f60: 682e 6578 6973 7473 286f 7574 7075 745f  h.exists(output_
+00000f70: 6469 7229 203d 3d20 4661 6c73 653a 0d0a  dir) == False:..
+00000f80: 2020 2020 2020 2020 2020 2020 6f73 2e6d              os.m
+00000f90: 6b64 6972 286f 7574 7075 745f 6469 7229  kdir(output_dir)
+00000fa0: 0d0a 2020 2020 2020 2020 7265 6164 6572  ..        reader
+00000fb0: 203d 2050 6466 5265 6164 6572 2870 6466   = PdfReader(pdf
+00000fc0: 5f66 696c 6529 0d0a 2020 2020 2020 2020  _file)..        
+00000fd0: 666f 7220 696e 6465 7820 696e 2072 616e  for index in ran
+00000fe0: 6765 286c 656e 2872 6561 6465 722e 7061  ge(len(reader.pa
+00000ff0: 6765 7329 293a 0d0a 2020 2020 2020 2020  ges)):..        
+00001000: 2020 2020 7772 6974 6572 203d 2050 6466      writer = Pdf
+00001010: 5772 6974 6572 2829 0d0a 2020 2020 2020  Writer()..      
+00001020: 2020 2020 2020 7061 6765 4f62 6a20 3d20        pageObj = 
+00001030: 7265 6164 6572 2e70 6167 6573 5b69 6e64  reader.pages[ind
+00001040: 6578 5d0d 0a20 2020 2020 2020 2020 2020  ex]..           
+00001050: 2077 7269 7465 722e 6164 645f 7061 6765   writer.add_page
+00001060: 2870 6167 654f 626a 290d 0a20 2020 2020  (pageObj)..     
+00001070: 2020 2020 2020 206e 6577 7061 7468 203d         newpath =
+00001080: 206f 732e 7061 7468 2e6a 6f69 6e28 6f75   os.path.join(ou
+00001090: 7470 7574 5f64 6972 2c20 6622 7b69 6e64  tput_dir, f"{ind
+000010a0: 6578 7d5f 7b66 5f6e 616d 657d 2229 0d0a  ex}_{f_name}")..
+000010b0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+000010c0: 206f 7065 6e28 6e65 7770 6174 682c 2027   open(newpath, '
+000010d0: 7762 2729 2061 7320 6677 3a0d 0a20 2020  wb') as fw:..   
+000010e0: 2020 2020 2020 2020 2020 2020 2077 7269               wri
+000010f0: 7465 722e 7772 6974 6528 6677 290d 0a0d  ter.write(fw)...
+00001100: 0a20 2020 2020 2020 2020 2020 2070 6466  .            pdf
+00001110: 732e 6170 7065 6e64 286e 6577 7061 7468  s.append(newpath
+00001120: 290d 0a20 2020 2065 7863 6570 7420 4578  )..    except Ex
+00001130: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
+00001140: 2020 2020 2020 2070 7269 6e74 2865 290d         print(e).
+00001150: 0a0d 0a20 2020 2072 6574 7572 6e20 7064  ...    return pd
+00001160: 6673 0d0a 0d0a 0d0a 6465 6620 6765 745f  fs......def get_
+00001170: 6669 6c65 5f63 6f6e 7465 6e74 5f61 735f  file_content_as_
+00001180: 6261 7365 3634 2870 6174 682c 2075 726c  base64(path, url
+00001190: 656e 636f 6465 643d 4661 6c73 6529 3a0d  encoded=False):.
+000011a0: 0a20 2020 2077 6974 6820 6f70 656e 2870  .    with open(p
+000011b0: 6174 682c 2022 7262 2229 2061 7320 663a  ath, "rb") as f:
+000011c0: 0d0a 2020 2020 2020 2020 636f 6e74 656e  ..        conten
+000011d0: 7420 3d20 6261 7365 3634 2e62 3634 656e  t = base64.b64en
+000011e0: 636f 6465 2866 2e72 6561 6428 2929 2e64  code(f.read()).d
+000011f0: 6563 6f64 6528 2275 7466 3822 290d 0a20  ecode("utf8").. 
+00001200: 2020 2020 2020 2069 6620 7572 6c65 6e63         if urlenc
+00001210: 6f64 6564 3a0d 0a20 2020 2020 2020 2020  oded:..         
+00001220: 2020 2063 6f6e 7465 6e74 203d 2075 726c     content = url
+00001230: 6c69 622e 7061 7273 652e 7175 6f74 655f  lib.parse.quote_
+00001240: 706c 7573 2863 6f6e 7465 6e74 290d 0a20  plus(content).. 
+00001250: 2020 2072 6574 7572 6e20 636f 6e74 656e     return conten
+00001260: 740d 0a0d 0a0d 0a69 6620 5f5f 6e61 6d65  t......if __name
+00001270: 5f5f 203d 3d20 225f 5f6d 6169 6e5f 5f22  __ == "__main__"
+00001280: 3a0d 0a20 2020 206b 7620 3d20 7b22 6b22  :..    kv = {"k"
+00001290: 3a20 2276 227d 0d0a 2020 2020 7072 696e  : "v"}..    prin
+000012a0: 7428 6b76 2e67 6574 2822 6b22 2929 0d0a  t(kv.get("k"))..
+000012b0: 2020 2020 7072 696e 7428 6b76 2e67 6574      print(kv.get
+000012c0: 2822 6b73 7322 2c20 2273 7322 2929 0d0a  ("kss", "ss"))..
```

