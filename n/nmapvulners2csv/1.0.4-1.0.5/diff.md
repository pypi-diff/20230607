# Comparing `tmp/nmapvulners2csv-1.0.4.tar.gz` & `tmp/nmapvulners2csv-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmapvulners2csv-1.0.4.tar", max compression
+gzip compressed data, was "nmapvulners2csv-1.0.5.tar", max compression
```

## Comparing `nmapvulners2csv-1.0.4.tar` & `nmapvulners2csv-1.0.5.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    11356 2022-07-05 09:58:49.072517 nmapvulners2csv-1.0.4/LICENSE
--rw-r--r--   0        0        0     3058 2022-10-21 10:38:31.326310 nmapvulners2csv-1.0.4/assets/PYPI_README.md
--rw-r--r--   0        0        0       33 2022-07-05 11:13:08.130262 nmapvulners2csv-1.0.4/nmapvulners2csv/__init__.py
--rw-r--r--   0        0        0     6222 2022-10-21 10:24:44.126287 nmapvulners2csv-1.0.4/nmapvulners2csv/nmapvulners2csv.py
--rw-r--r--   0        0        0      540 2022-10-21 10:39:50.594312 nmapvulners2csv-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     4064 1970-01-01 00:00:00.000000 nmapvulners2csv-1.0.4/setup.py
--rw-r--r--   0        0        0     3887 1970-01-01 00:00:00.000000 nmapvulners2csv-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-07 16:19:32.458223 nmapvulners2csv-1.0.5/LICENSE
+-rw-r--r--   0        0        0     3058 2023-06-07 16:19:32.458223 nmapvulners2csv-1.0.5/assets/PYPI_README.md
+-rw-r--r--   0        0        0       33 2023-06-07 16:19:32.462223 nmapvulners2csv-1.0.5/nmapvulners2csv/__init__.py
+-rw-r--r--   0        0        0     6222 2023-06-07 16:19:32.462223 nmapvulners2csv-1.0.5/nmapvulners2csv/nmapvulners2csv.py
+-rw-r--r--   0        0        0      561 2023-06-07 16:19:32.462223 nmapvulners2csv-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3929 1970-01-01 00:00:00.000000 nmapvulners2csv-1.0.5/PKG-INFO
```

### Comparing `nmapvulners2csv-1.0.4/LICENSE` & `nmapvulners2csv-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nmapvulners2csv-1.0.4/assets/PYPI_README.md` & `nmapvulners2csv-1.0.5/assets/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `nmapvulners2csv-1.0.4/nmapvulners2csv/nmapvulners2csv.py` & `nmapvulners2csv-1.0.5/nmapvulners2csv/nmapvulners2csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import fire
 import requests
 from xml.etree import ElementTree
 from time import sleep
 from bs4 import BeautifulSoup
 from os import path, makedirs
 
-VERSION = '1.0.3'
+VERSION = '1.0.5'
 OUTPUT_DIR = "nmapvulners2csv_output" # Default value, can be changed with the '--dir' optional flag
 CSV_HEADERS = ['host', 'port', 'protocol', 'service', 'version','cpe', 'id_vuln', 'cvss', 'type', 'exploit', 'url', 'description']
 VULNERS_URL= "https://vulners.com/"
 
 vulners_base = lambda t: "{}{}".format(VULNERS_URL, t)
 vulners_endpoint = lambda t,id: "{}/{}".format(vulners_base(t), id)
```

### Comparing `nmapvulners2csv-1.0.4/pyproject.toml` & `nmapvulners2csv-1.0.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "nmapvulners2csv"
-version = "1.0.4"
+version = "1.0.5"
 authors = ["SecSI <dev@secsi.io>"]
 description = "Convert Nmap Vulners script output to CSV"
 license = "LICENSE"
 readme = "assets/PYPI_README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 beautifulsoup4 = "^4.11.1"
 bs4 = "^0.0.1"
 elementpath = "^3.0.2"
 fire = "^0.4.0"
 six = "^1.16.0"
 soupsieve = "^2.3.2.post1"
 termcolor = "^2.0.1"
+requests = "^2.31.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 nmapvulners2csv = 'nmapvulners2csv:main'
```

### Comparing `nmapvulners2csv-1.0.4/setup.py` & `nmapvulners2csv-1.0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,114 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nmapvulners2csv
+Version: 1.0.5
+Summary: Convert Nmap Vulners script output to CSV
+License: LICENSE
+Author: SecSI
+Author-email: dev@secsi.io
+Requires-Python: >=3.8,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
+Requires-Dist: bs4 (>=0.0.1,<0.0.2)
+Requires-Dist: elementpath (>=3.0.2,<4.0.0)
+Requires-Dist: fire (>=0.4.0,<0.5.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: six (>=1.16.0,<2.0.0)
+Requires-Dist: soupsieve (>=2.3.2.post1,<3.0.0)
+Requires-Dist: termcolor (>=2.0.1,<3.0.0)
+Description-Content-Type: text/markdown
+
+<h1 align="center">
+    <img src="https://raw.githubusercontent.com/cybersecsi/nmapvulners2csv/main/assets/logo-light-mode.png" alt= "nmapvulners2csv" width="300px">
+</h1>
+
+<p align="center">
+    <b>nmapvulners2csv</b>
+<p>
+
+
+<p align="center">
+  <a href="https://github.com/cybersecsi/nmapvulners2csv/blob/main/README.md"><img src="https://img.shields.io/badge/Documentation-complete-green.svg?style=flat"></a>
+  <a href="https://github.com/cybersecsi/nmapvulners2csv/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Apache2-blue.svg"></a>
+</p>
+
+## Table of Contents
+- [Getting Started](#getting-started)
+  - [Install](#install)
+  - [Run without installing](#run-without-installing)
+    - [Prerequisites](#prerequisites)
+  - [Evidences Description](#evidences-description)
+- [Contributing](#contributing)
+- [Credits](#credits)
+- [License](#license)
+
+##  Getting Started  
+Run nmap with enabled script Vulners and save xml output, for example:   
+```  
+nmap -sV --script vulners -oX <nmap_output.xml>  
+```  
+
+### Example
+The output of the tool is like the following:
+![Execution example](https://github.com/cybersecsi/nmapvulners2csv/raw/main/assets/usage.png)
+
+### Install & Run
+To install it you just need to run:
+```
+pip install nmapvulners2csv
+```
+
+### Run without installing
+
+#### Prerequisites   
+Install dependencies by using the following command:   
+``` 
+pip install -r requirements.txt
+chmod +x nmapvulners2csv/nmapvulners2csv.py
+```
+
+```   
+Usage: nmapvulners2csv.py NMAP_XML_FILE <flags>
+  optional flags:        --output | --descr
+  
+```  
+
+To run the converter:   
+```  
+nmapvulners2csv.py <nmap_output.xml>   
+``` 
+
+the script will generate a file output.csv in output dir. If you want to set the output file:   
+```   
+nmapvulners2csv.py <nmap_output.xml>  --output <output_csv_file> --dir <output_directory>
+``` 
+For multiple data:   
+```  
+for i in `ls -1 vulners*`; do python nmapvulners2csv.py $i ${i%%.xml}.csv ; done   
+``` 
+
+### Evidences Description  
+``nmapvulners2csv`` does not generate descriptions for vulnerabilities. You can add `--descr` flag to add descriptions in CSV.  The script scrapes description information from Vulners site. The command is more time-expensive and send several HTTP requests against Vulners website. Not tested for IP ban and network issues.     
+
+## Contributing
+
+Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+
+1. Fork the Project
+2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the Branch (`git push origin feature/AmazingFeature`)
+5. Open a Pull Request
+
+## Credits
+``nmapvulners2csv`` is proudly developed [@SecSI](https://secsi.io) by:
+- [Gaetano Perrone](https://github.com/giper45)
+- [NdA994](https://github.com/NdA994)
+- [Angelo Delicato](https://github.com/thelicato)
 
-packages = \
-['nmapvulners2csv']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['beautifulsoup4>=4.11.1,<5.0.0',
- 'bs4>=0.0.1,<0.0.2',
- 'elementpath>=3.0.2,<4.0.0',
- 'fire>=0.4.0,<0.5.0',
- 'six>=1.16.0,<2.0.0',
- 'soupsieve>=2.3.2.post1,<3.0.0',
- 'termcolor>=2.0.1,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['nmapvulners2csv = nmapvulners2csv:main']}
-
-setup_kwargs = {
-    'name': 'nmapvulners2csv',
-    'version': '1.0.4',
-    'description': 'Convert Nmap Vulners script output to CSV',
-    'long_description': '<h1 align="center">\n    <img src="https://raw.githubusercontent.com/cybersecsi/nmapvulners2csv/main/assets/logo-light-mode.png" alt= "nmapvulners2csv" width="300px">\n</h1>\n\n<p align="center">\n    <b>nmapvulners2csv</b>\n<p>\n\n\n<p align="center">\n  <a href="https://github.com/cybersecsi/nmapvulners2csv/blob/main/README.md"><img src="https://img.shields.io/badge/Documentation-complete-green.svg?style=flat"></a>\n  <a href="https://github.com/cybersecsi/nmapvulners2csv/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Apache2-blue.svg"></a>\n</p>\n\n## Table of Contents\n- [Getting Started](#getting-started)\n  - [Install](#install)\n  - [Run without installing](#run-without-installing)\n    - [Prerequisites](#prerequisites)\n  - [Evidences Description](#evidences-description)\n- [Contributing](#contributing)\n- [Credits](#credits)\n- [License](#license)\n\n##  Getting Started  \nRun nmap with enabled script Vulners and save xml output, for example:   \n```  \nnmap -sV --script vulners -oX <nmap_output.xml>  \n```  \n\n### Example\nThe output of the tool is like the following:\n![Execution example](https://github.com/cybersecsi/nmapvulners2csv/raw/main/assets/usage.png)\n\n### Install & Run\nTo install it you just need to run:\n```\npip install nmapvulners2csv\n```\n\n### Run without installing\n\n#### Prerequisites   \nInstall dependencies by using the following command:   \n``` \npip install -r requirements.txt\nchmod +x nmapvulners2csv/nmapvulners2csv.py\n```\n\n```   \nUsage: nmapvulners2csv.py NMAP_XML_FILE <flags>\n  optional flags:        --output | --descr\n  \n```  \n\nTo run the converter:   \n```  \nnmapvulners2csv.py <nmap_output.xml>   \n``` \n\nthe script will generate a file output.csv in output dir. If you want to set the output file:   \n```   \nnmapvulners2csv.py <nmap_output.xml>  --output <output_csv_file> --dir <output_directory>\n``` \nFor multiple data:   \n```  \nfor i in `ls -1 vulners*`; do python nmapvulners2csv.py $i ${i%%.xml}.csv ; done   \n``` \n\n### Evidences Description  \n``nmapvulners2csv`` does not generate descriptions for vulnerabilities. You can add `--descr` flag to add descriptions in CSV.  The script scrapes description information from Vulners site. The command is more time-expensive and send several HTTP requests against Vulners website. Not tested for IP ban and network issues.     \n\n## Contributing\n\nContributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.\n\n1. Fork the Project\n2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)\n3. Commit your Changes (`git commit -m \'Add some AmazingFeature\'`)\n4. Push to the Branch (`git push origin feature/AmazingFeature`)\n5. Open a Pull Request\n\n## Credits\n``nmapvulners2csv`` is proudly developed [@SecSI](https://secsi.io) by:\n- [Gaetano Perrone](https://github.com/giper45)\n- [NdA994](https://github.com/NdA994)\n- [Angelo Delicato](https://github.com/thelicato)\n\n## License\nDistributed under Apache 2 License. See `LICENSE` for more information. ',
-    'author': 'SecSI',
-    'author_email': 'dev@secsi.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
+## License
+Distributed under Apache 2 License. See `LICENSE` for more information.
```

#### html2text {}

```diff
@@ -1,53 +1,49 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['nmapvulners2csv'] package_data = \ {'': ['*']} install_requires = \
-['beautifulsoup4>=4.11.1,<5.0.0', 'bs4>=0.0.1,<0.0.2',
-'elementpath>=3.0.2,<4.0.0', 'fire>=0.4.0,<0.5.0', 'six>=1.16.0,<2.0.0',
-'soupsieve>=2.3.2.post1,<3.0.0', 'termcolor>=2.0.1,<3.0.0'] entry_points = \
-{'console_scripts': ['nmapvulners2csv = nmapvulners2csv:main']} setup_kwargs =
-{ 'name': 'nmapvulners2csv', 'version': '1.0.4', 'description': 'Convert Nmap
-Vulners script output to CSV', 'long_description': '
-                     ****** \n [nmapvulners2csv]\n ******
-\n\n
-                             \n nmapvulners2csv\n
-\n\n\n
-\n [https://img.shields.io/badge/Documentation-complete-green.svg?style=flat]\n
-           [https://img.shields.io/badge/License-Apache2-blue.svg]\n
-\n\n## Table of Contents\n- [Getting Started](#getting-started)\n - [Install]
-(#install)\n - [Run without installing](#run-without-installing)\n -
-[Prerequisites](#prerequisites)\n - [Evidences Description](#evidences-
-description)\n- [Contributing](#contributing)\n- [Credits](#credits)\n-
-[License](#license)\n\n## Getting Started \nRun nmap with enabled script
-Vulners and save xml output, for example: \n``` \nnmap -sV --script vulners -oX
-xml> \n``` \n\n### Example\nThe output of the tool is like the following:\n!
-[Execution example](https://github.com/cybersecsi/nmapvulners2csv/raw/main/
-assets/usage.png)\n\n### Install & Run\nTo install it you just need to run:
-\n```\npip install nmapvulners2csv\n```\n\n### Run without installing\n\n####
-Prerequisites \nInstall dependencies by using the following command: \n```
-\npip install -r requirements.txt\nchmod +x nmapvulners2csv/
-nmapvulners2csv.py\n```\n\n``` \nUsage: nmapvulners2csv.py NMAP_XML_FILE \n
-optional flags: --output | --descr\n \n``` \n\nTo run the converter: \n```
-\nnmapvulners2csv.py
-xml> \n``` \n\nthe script will generate a file output.csv in output dir. If you
-want to set the output file: \n``` \nnmapvulners2csv.py
-xml> --output  --dir \n``` \nFor multiple data: \n``` \nfor i in `ls -
-1 vulners*`; do python nmapvulners2csv.py $i ${i%%.xml}.csv ; done \n```
-\n\n### Evidences Description \n``nmapvulners2csv`` does not generate
-descriptions for vulnerabilities. You can add `--descr` flag to add
-descriptions in CSV. The script scrapes description information from Vulners
-site. The command is more time-expensive and send several HTTP requests against
-Vulners website. Not tested for IP ban and network issues. \n\n##
-Contributing\n\nContributions are what make the open source community such an
-amazing place to be learn, inspire, and create. Any contributions you make are
-**greatly appreciated**.\n\n1. Fork the Project\n2. Create your Feature Branch
-(`git checkout -b feature/AmazingFeature`)\n3. Commit your Changes (`git commit
--m \'Add some AmazingFeature\'`)\n4. Push to the Branch (`git push origin
-feature/AmazingFeature`)\n5. Open a Pull Request\n\n##
-Credits\n``nmapvulners2csv`` is proudly developed [@SecSI](https://secsi.io)
-by:\n- [Gaetano Perrone](https://github.com/giper45)\n- [NdA994](https://
-github.com/NdA994)\n- [Angelo Delicato](https://github.com/thelicato)\n\n##
-License\nDistributed under Apache 2 License. See `LICENSE` for more
-information. ', 'author': 'SecSI', 'author_email': 'dev@secsi.io',
-'maintainer': 'None', 'maintainer_email': 'None', 'url': 'None', 'packages':
-packages, 'package_data': package_data, 'install_requires': install_requires,
-'entry_points': entry_points, 'python_requires': '>=3.8,<4.0', } setup
-(**setup_kwargs)
+Metadata-Version: 2.1 Name: nmapvulners2csv Version: 1.0.5 Summary: Convert
+Nmap Vulners script output to CSV License: LICENSE Author: SecSI Author-email:
+dev@secsi.io Requires-Python: >=3.8,<4.0 Classifier: License :: Other/
+Proprietary License Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Dist: beautifulsoup4
+(>=4.11.1,<5.0.0) Requires-Dist: bs4 (>=0.0.1,<0.0.2) Requires-Dist:
+elementpath (>=3.0.2,<4.0.0) Requires-Dist: fire (>=0.4.0,<0.5.0) Requires-
+Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: six (>=1.16.0,<2.0.0) Requires-
+Dist: soupsieve (>=2.3.2.post1,<3.0.0) Requires-Dist: termcolor
+(>=2.0.1,<3.0.0) Description-Content-Type: text/markdown
+                        ****** [nmapvulners2csv] ******
+                                nmapvulners2csv
+  [https://img.shields.io/badge/Documentation-complete-green.svg?style=flat]
+            [https://img.shields.io/badge/License-Apache2-blue.svg]
+## Table of Contents - [Getting Started](#getting-started) - [Install]
+(#install) - [Run without installing](#run-without-installing) -
+[Prerequisites](#prerequisites) - [Evidences Description](#evidences-
+description) - [Contributing](#contributing) - [Credits](#credits) - [License]
+(#license) ## Getting Started Run nmap with enabled script Vulners and save xml
+output, for example: ``` nmap -sV --script vulners -oX
+xml> ``` ### Example The output of the tool is like the following: ![Execution
+example](https://github.com/cybersecsi/nmapvulners2csv/raw/main/assets/
+usage.png) ### Install & Run To install it you just need to run: ``` pip
+install nmapvulners2csv ``` ### Run without installing #### Prerequisites
+Install dependencies by using the following command: ``` pip install -
+r requirements.txt chmod +x nmapvulners2csv/nmapvulners2csv.py ``` ``` Usage:
+nmapvulners2csv.py NMAP_XML_FILE  optional flags: --output | --descr ``` To run
+the converter: ``` nmapvulners2csv.py
+xml> ``` the script will generate a file output.csv in output dir. If you want
+to set the output file: ``` nmapvulners2csv.py
+xml> --output  --dir  ``` For multiple data: ``` for i in `ls -1 vulners*`; do
+python nmapvulners2csv.py $i ${i%%.xml}.csv ; done ``` ### Evidences
+Description ``nmapvulners2csv`` does not generate descriptions for
+vulnerabilities. You can add `--descr` flag to add descriptions in CSV. The
+script scrapes description information from Vulners site. The command is more
+time-expensive and send several HTTP requests against Vulners website. Not
+tested for IP ban and network issues. ## Contributing Contributions are what
+make the open source community such an amazing place to be learn, inspire, and
+create. Any contributions you make are **greatly appreciated**. 1. Fork the
+Project 2. Create your Feature Branch (`git checkout -b feature/
+AmazingFeature`) 3. Commit your Changes (`git commit -m 'Add some
+AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
+AmazingFeature`) 5. Open a Pull Request ## Credits ``nmapvulners2csv`` is
+proudly developed [@SecSI](https://secsi.io) by: - [Gaetano Perrone](https://
+github.com/giper45) - [NdA994](https://github.com/NdA994) - [Angelo Delicato]
+(https://github.com/thelicato) ## License Distributed under Apache 2 License.
+See `LICENSE` for more information.
```

