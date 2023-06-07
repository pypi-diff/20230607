# Comparing `tmp/pydraughts-0.6.1.tar.gz` & `tmp/pydraughts-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydraughts-0.6.1.tar", last modified: Wed Nov 30 15:45:33 2022, max compression
+gzip compressed data, was "pydraughts-0.6.2.tar", last modified: Wed Jun  7 12:47:53 2023, max compression
```

## Comparing `pydraughts-0.6.1.tar` & `pydraughts-0.6.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2022-11-30 15:45:33.665490 pydraughts-0.6.1/
--rw-rw-rw-   0        0        0     1082 2022-11-30 15:36:31.000000 pydraughts-0.6.1/LICENSE
--rw-rw-rw-   0        0        0       46 2022-11-30 15:36:31.000000 pydraughts-0.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5393 2022-11-30 15:45:33.665490 pydraughts-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     4147 2022-11-30 15:36:31.000000 pydraughts-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2022-11-30 15:45:33.420334 pydraughts-0.6.1/draughts/
--rw-rw-rw-   0        0        0    12623 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/PDN.py
--rw-rw-rw-   0        0        0      242 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-30 15:45:33.482871 pydraughts-0.6.1/draughts/ballot_files/
--rw-rw-rw-   0        0        0   350063 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/ballot_files/11_english.json
--rw-rw-rw-   0        0        0   191861 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/ballot_files/11_italian.json
--rw-rw-rw-   0        0        0    17530 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/ballot_files/150russian_and_brazilian.json
--rw-rw-rw-   0        0        0     5225 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/ballot_files/2move_english.json
--rw-rw-rw-   0        0        0    21036 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/ballot_files/3move_english.json
--rw-rw-rw-   0        0        0   104689 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/ballot_files/4move_english.json
--rw-rw-rw-   0        0        0   388564 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/ballot_files/5move_english.json
--rw-rw-rw-   0        0        0    95519 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/ballot_files/brazilian.json
--rw-rw-rw-   0        0        0    96764 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/ballot_files/russian.json
--rw-rw-rw-   0        0        0     2185 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/ballots.py
--rw-rw-rw-   0        0        0    11930 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/convert.py
-drwxrwxrwx   0        0        0        0 2022-11-30 15:45:33.534486 pydraughts-0.6.1/draughts/core/
--rw-rw-rw-   0        0        0        0 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/core/__init__.py
--rw-rw-rw-   0        0        0     7019 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/core/board.py
--rw-rw-rw-   0        0        0     2635 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/core/board_initializer.py
--rw-rw-rw-   0        0        0     3406 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/core/board_searcher.py
--rw-rw-rw-   0        0        0    35852 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/core/game.py
--rw-rw-rw-   0        0        0    19525 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/core/move.py
--rw-rw-rw-   0        0        0    28869 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/core/piece.py
--rw-rw-rw-   0        0        0    17684 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/core/variant.py
--rw-rw-rw-   0        0        0     1218 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/engine.py
-drwxrwxrwx   0        0        0        0 2022-11-30 15:45:33.556105 pydraughts-0.6.1/draughts/engines/
--rw-rw-rw-   0        0        0        0 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/engines/__init__.py
--rw-rw-rw-   0        0        0     6447 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/engines/checkerboard.py
-drwxrwxrwx   0        0        0        0 2022-11-30 15:45:33.587357 pydraughts-0.6.1/draughts/engines/checkerboard_extra/
--rw-rw-rw-   0        0        0        0 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/engines/checkerboard_extra/__init__.py
--rw-rw-rw-   0        0        0     5506 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/engines/checkerboard_extra/engine_64.py
--rw-rw-rw-   0        0        0     1241 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/engines/checkerboard_extra/engine_client.py
--rw-rw-rw-   0        0        0     5191 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/engines/checkerboard_extra/engine_server.py
--rw-rw-rw-   0        0        0     4405 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/engines/checkerboard_extra/get_checker_board.py
--rw-rw-rw-   0        0        0     6895 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/engines/dxp.py
-drwxrwxrwx   0        0        0        0 2022-11-30 15:45:33.602985 pydraughts-0.6.1/draughts/engines/dxp_communication/
--rw-rw-rw-   0        0        0        0 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/engines/dxp_communication/__init__.py
--rw-rw-rw-   0        0        0     8583 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/engines/dxp_communication/dxp_classes.py
--rw-rw-rw-   0        0        0    13312 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/engines/dxp_communication/dxp_run.py
--rw-rw-rw-   0        0        0    10797 2022-11-30 15:36:31.000000 pydraughts-0.6.1/draughts/engines/hub.py
-drwxrwxrwx   0        0        0        0 2022-11-30 15:45:33.618609 pydraughts-0.6.1/other_licenses/
--rw-rw-rw-   0        0        0     1111 2022-11-30 15:36:31.000000 pydraughts-0.6.1/other_licenses/ImparaAI checkers LICENSE
--rw-rw-rw-   0        0        0     1075 2022-11-30 15:36:31.000000 pydraughts-0.6.1/other_licenses/akalverboer DXC100_draughts_client LICENSE
--rw-rw-rw-   0        0        0     1073 2022-11-30 15:36:31.000000 pydraughts-0.6.1/other_licenses/fishnet LICENSE.txt
-drwxrwxrwx   0        0        0        0 2022-11-30 15:45:33.649862 pydraughts-0.6.1/pydraughts.egg-info/
--rw-rw-rw-   0        0        0     5393 2022-11-30 15:45:33.000000 pydraughts-0.6.1/pydraughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1538 2022-11-30 15:45:33.000000 pydraughts-0.6.1/pydraughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-30 15:45:33.000000 pydraughts-0.6.1/pydraughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2022-11-30 15:45:33.000000 pydraughts-0.6.1/pydraughts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-30 15:45:33.000000 pydraughts-0.6.1/pydraughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-11-30 15:36:31.000000 pydraughts-0.6.1/pyproject.toml
--rw-rw-rw-   0        0        0     1217 2022-11-30 15:45:33.665490 pydraughts-0.6.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-07 12:47:53.712388 pydraughts-0.6.2/
+-rw-rw-rw-   0        0        0     1078 2023-06-07 12:45:22.000000 pydraughts-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0       46 2023-06-07 12:42:58.000000 pydraughts-0.6.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5393 2023-06-07 12:47:53.713387 pydraughts-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4147 2023-06-07 12:42:58.000000 pydraughts-0.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 12:47:53.461323 pydraughts-0.6.2/draughts/
+-rw-rw-rw-   0        0        0    12623 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/PDN.py
+-rw-rw-rw-   0        0        0      238 2023-06-07 12:45:00.000000 pydraughts-0.6.2/draughts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 12:47:53.532343 pydraughts-0.6.2/draughts/ballot_files/
+-rw-rw-rw-   0        0        0   350063 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballot_files/11_english.json
+-rw-rw-rw-   0        0        0   191861 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballot_files/11_italian.json
+-rw-rw-rw-   0        0        0    17530 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballot_files/150russian_and_brazilian.json
+-rw-rw-rw-   0        0        0     5225 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballot_files/2move_english.json
+-rw-rw-rw-   0        0        0    21036 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballot_files/3move_english.json
+-rw-rw-rw-   0        0        0   104689 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballot_files/4move_english.json
+-rw-rw-rw-   0        0        0   388564 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballot_files/5move_english.json
+-rw-rw-rw-   0        0        0    95519 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballot_files/brazilian.json
+-rw-rw-rw-   0        0        0    96764 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballot_files/russian.json
+-rw-rw-rw-   0        0        0     2185 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballots.py
+-rw-rw-rw-   0        0        0    11930 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/convert.py
+drwxrwxrwx   0        0        0        0 2023-06-07 12:47:53.585355 pydraughts-0.6.2/draughts/core/
+-rw-rw-rw-   0        0        0        0 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/core/__init__.py
+-rw-rw-rw-   0        0        0     7019 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/core/board.py
+-rw-rw-rw-   0        0        0     2635 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/core/board_initializer.py
+-rw-rw-rw-   0        0        0     3406 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/core/board_searcher.py
+-rw-rw-rw-   0        0        0    35852 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/core/game.py
+-rw-rw-rw-   0        0        0    19525 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/core/move.py
+-rw-rw-rw-   0        0        0    28954 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/core/piece.py
+-rw-rw-rw-   0        0        0    17684 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/core/variant.py
+-rw-rw-rw-   0        0        0     1218 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engine.py
+drwxrwxrwx   0        0        0        0 2023-06-07 12:47:53.618363 pydraughts-0.6.2/draughts/engines/
+-rw-rw-rw-   0        0        0        0 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/__init__.py
+-rw-rw-rw-   0        0        0     6447 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/checkerboard.py
+drwxrwxrwx   0        0        0        0 2023-06-07 12:47:53.648370 pydraughts-0.6.2/draughts/engines/checkerboard_extra/
+-rw-rw-rw-   0        0        0        0 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/checkerboard_extra/__init__.py
+-rw-rw-rw-   0        0        0     5506 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/checkerboard_extra/engine_64.py
+-rw-rw-rw-   0        0        0     1133 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/checkerboard_extra/engine_client.py
+-rw-rw-rw-   0        0        0     5091 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/checkerboard_extra/engine_server.py
+-rw-rw-rw-   0        0        0     4405 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/checkerboard_extra/get_checker_board.py
+-rw-rw-rw-   0        0        0     7267 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/dxp.py
+drwxrwxrwx   0        0        0        0 2023-06-07 12:47:53.665373 pydraughts-0.6.2/draughts/engines/dxp_communication/
+-rw-rw-rw-   0        0        0        0 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/dxp_communication/__init__.py
+-rw-rw-rw-   0        0        0     8959 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/dxp_communication/dxp_classes.py
+-rw-rw-rw-   0        0        0    14219 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/dxp_communication/dxp_run.py
+-rw-rw-rw-   0        0        0    10797 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/hub.py
+drwxrwxrwx   0        0        0        0 2023-06-07 12:47:53.681378 pydraughts-0.6.2/other_licenses/
+-rw-rw-rw-   0        0        0     1111 2023-06-07 12:42:58.000000 pydraughts-0.6.2/other_licenses/ImparaAI checkers LICENSE
+-rw-rw-rw-   0        0        0     1075 2023-06-07 12:42:58.000000 pydraughts-0.6.2/other_licenses/akalverboer DXC100_draughts_client LICENSE
+-rw-rw-rw-   0        0        0     1073 2023-06-07 12:42:58.000000 pydraughts-0.6.2/other_licenses/fishnet LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 12:47:53.707385 pydraughts-0.6.2/pydraughts.egg-info/
+-rw-rw-rw-   0        0        0     5393 2023-06-07 12:47:53.000000 pydraughts-0.6.2/pydraughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1538 2023-06-07 12:47:53.000000 pydraughts-0.6.2/pydraughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 12:47:53.000000 pydraughts-0.6.2/pydraughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-07 12:47:53.000000 pydraughts-0.6.2/pydraughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-07 12:47:53.000000 pydraughts-0.6.2/pydraughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-06-07 12:42:58.000000 pydraughts-0.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1217 2023-06-07 12:47:53.716388 pydraughts-0.6.2/setup.cfg
```

### Comparing `pydraughts-0.6.1/LICENSE` & `pydraughts-0.6.2/other_licenses/akalverboer DXC100_draughts_client LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021-2022 AttackingOrDefending
+Copyright (c) 2018  Arthur Kalverboer
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pydraughts-0.6.1/PKG-INFO` & `pydraughts-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydraughts
-Version: 0.6.1
+Version: 0.6.2
 Summary: A draughts library for Python with move generation, PDN reading and writing, engine communication and balloted openings
 Home-page: https://github.com/AttackingOrDefending/pydraughts
 Author: AttackingOrDefending
 Project-URL: Bug Tracker, https://github.com/AttackingOrDefending/pydraughts/issues
 Keywords: checkers,draughts,game,fen,pdn
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -65,15 +65,15 @@
 * Make a move
 ```python
 move = Move(board, steps_move=[34, 30])
 board.push(move)
 
 # Multi-capture
 board2 = Board(fen="W:WK40:B19,29")
-board2.push(Move(board2), pdn_move='40x14')
+board2.push(Move(board2, pdn_move='40x14'))
 ```
 * Get a visual representation of the board
 ```python
 print(board)
 
 """
    | b |   | b |   | b |   | b |   | b
```

### Comparing `pydraughts-0.6.1/README.md` & `pydraughts-0.6.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 * Make a move
 ```python
 move = Move(board, steps_move=[34, 30])
 board.push(move)
 
 # Multi-capture
 board2 = Board(fen="W:WK40:B19,29")
-board2.push(Move(board2), pdn_move='40x14')
+board2.push(Move(board2, pdn_move='40x14'))
 ```
 * Get a visual representation of the board
 ```python
 print(board)
 
 """
    | b |   | b |   | b |   | b |   | b
```

### Comparing `pydraughts-0.6.1/draughts/PDN.py` & `pydraughts-0.6.2/draughts/PDN.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/ballot_files/11_english.json` & `pydraughts-0.6.2/draughts/ballot_files/11_english.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/ballot_files/11_italian.json` & `pydraughts-0.6.2/draughts/ballot_files/11_italian.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/ballot_files/150russian_and_brazilian.json` & `pydraughts-0.6.2/draughts/ballot_files/150russian_and_brazilian.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/ballot_files/2move_english.json` & `pydraughts-0.6.2/draughts/ballot_files/2move_english.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/ballot_files/3move_english.json` & `pydraughts-0.6.2/draughts/ballot_files/3move_english.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/ballot_files/4move_english.json` & `pydraughts-0.6.2/draughts/ballot_files/4move_english.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/ballot_files/5move_english.json` & `pydraughts-0.6.2/draughts/ballot_files/5move_english.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/ballot_files/brazilian.json` & `pydraughts-0.6.2/draughts/ballot_files/brazilian.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/ballot_files/russian.json` & `pydraughts-0.6.2/draughts/ballot_files/russian.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/ballots.py` & `pydraughts-0.6.2/draughts/ballots.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/convert.py` & `pydraughts-0.6.2/draughts/convert.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/core/board.py` & `pydraughts-0.6.2/draughts/core/board.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/core/board_initializer.py` & `pydraughts-0.6.2/draughts/core/board_initializer.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/core/board_searcher.py` & `pydraughts-0.6.2/draughts/core/board_searcher.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/core/game.py` & `pydraughts-0.6.2/draughts/core/game.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/core/move.py` & `pydraughts-0.6.2/draughts/core/move.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/core/piece.py` & `pydraughts-0.6.2/draughts/core/piece.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,16 @@
     def reset_for_new_board(self) -> None:
         """Reset possible moves to None."""
         self.possible_capture_moves: Optional[List[List[int]]] = None
         self.possible_positional_moves: Optional[List[List[int]]] = None
 
     def get_square(self, row: int, column: int) -> Optional[int]:
         """Get the square given the row and column."""
-        return self.board.position_layout.get(row, {}).get(column)
+        board_row: dict[int, Optional[int]] = self.board.position_layout.get(row, {})
+        return board_row.get(column)
 
     def is_movable(self, captures: List[int]) -> bool:
         """Get if the piece can move."""
         return bool((self.get_possible_capture_moves(captures) or self.get_possible_positional_moves()) and not self.captured)
 
     def capture(self) -> None:
         """Flag the piece as captured."""
@@ -348,15 +349,16 @@
         """Get all adjacent positions of the piece."""
         # In some variants men can't capture backwards
         criteria = bool(capture or self.king) if self.men_can_capture_backwards else bool(self.king)
         return self.get_directional_adjacent_positions(forward=True, capture=capture) + (self.get_directional_adjacent_positions(forward=False, capture=capture) if criteria else [])
 
     def get_column(self) -> int:
         """Get the piece's column."""
-        return (self.position - 1) % self.board.width
+        width: int = self.board.width
+        return (self.position - 1) % width
 
     def get_row(self) -> int:
         """Get the piece's row."""
         return self.get_row_from_position(self.position)
 
     def is_on_enemy_home_row(self) -> bool:
         """Get if the piece is on the enemy's home row (used for promotions)."""
```

### Comparing `pydraughts-0.6.1/draughts/core/variant.py` & `pydraughts-0.6.2/draughts/core/variant.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/engine.py` & `pydraughts-0.6.2/draughts/engine.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/engines/checkerboard.py` & `pydraughts-0.6.2/draughts/engines/checkerboard.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/engines/checkerboard_extra/engine_64.py` & `pydraughts-0.6.2/draughts/engines/checkerboard_extra/engine_64.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/engines/checkerboard_extra/engine_client.py` & `pydraughts-0.6.2/draughts/engines/checkerboard_extra/engine_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,18 +6,16 @@
 
 
 class Engine32(Client64):
     """64 bit client to communicate with the 32 bit server that is running the old Checkerboard engine."""
     def __init__(self, command: str) -> None:
 
         command = command.replace('\\', '\\\\')
-        with open(os.path.join(os.path.dirname(__file__), 'engine_name.txt'), 'w') as file:
-            file.write(command)
 
-        super(Engine32, self).__init__(module32='engine_server', append_sys_path=os.path.dirname(__file__))
+        super(Engine32, self).__init__(module32='engine_server', append_sys_path=os.path.dirname(__file__), dll_name=command)
 
     def enginecommand(self, command: str) -> Tuple[bytes, int]:
         """Send an enginecommand to the engine."""
         return self.request32('enginecommand', command)
 
     def getmove(self, game: draughts.Board, maxtime: Union[int, float, None] = None, time: Union[int, float, None] = None, increment: Union[int, float, None] = None, movetime: Union[int, float, None] = None) -> Tuple[Optional[str], bytes, Dict[str, Any], int]:
         """Send a getmove to the engine."""
```

### Comparing `pydraughts-0.6.1/draughts/engines/checkerboard_extra/engine_server.py` & `pydraughts-0.6.2/draughts/engines/checkerboard_extra/engine_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,20 @@
 import draughts
 from draughts.engines.checkerboard_extra.get_checker_board import get_board, from_board
 import os
 from typing import Tuple, Optional, Union, Dict, Any
 
 from msl.loadlib import Server32
 
-with open(os.path.join(os.path.dirname(__file__), 'engine_name.txt')) as file:
-    DLL_name = file.read()
-
 
 class Engine32Server(Server32):
     """32 bit server to run old Checkerboard engines."""
 
     def __init__(self, host: str, port: int, **kwargs: Any) -> None:
-        super(Engine32Server, self).__init__(DLL_name, 'windll', host, port)
+        super(Engine32Server, self).__init__(kwargs["dll_name"], 'windll', host, port)
 
     def enginecommand(self, command: str) -> Tuple[bytes, int]:
         """Send an enginecommand to the engine."""
         output = ctypes.create_string_buffer(b'', 1024)
         result = self.lib.enginecommand(ctypes.create_string_buffer(bytes(command.encode('ascii')), 256), output)
         return output.value, result
```

### Comparing `pydraughts-0.6.1/draughts/engines/checkerboard_extra/get_checker_board.py` & `pydraughts-0.6.2/draughts/engines/checkerboard_extra/get_checker_board.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/draughts/engines/dxp.py` & `pydraughts-0.6.2/draughts/engines/dxp.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         self.wait_to_open_time = 10
         self.ENGINE = ENGINE
         self.info: Dict[str, Any] = {}
         self.id: Dict[str, str] = {}
         self.console = dxp.tConsoleHandler
         self.receiver = dxp.tReceiveHandler
         self.game_started = False
-        self._last_move = None
         self.exit = False
 
         self.configure(options)
 
         if not self.engine_opened:
             cwd = cwd or os.getcwd()
             cwd = os.path.realpath(os.path.expanduser(cwd))
@@ -48,14 +47,15 @@
             command = ' '.join(command)
             self.command = command
             self.p = self._open_process(command, cwd)
             self.engine_receive_thread = threading.Thread(target=self._recv)
             self.engine_receive_thread.start()
 
         self.start_time = time.perf_counter_ns()
+        self.quit_time = 0
 
     def setoption(self, name: str, value: Union[str, int, bool]) -> None:
         """Set a DXP option."""
         if name == 'engine-opened':
             self.engine_opened = value
         elif name == 'ip':
             self.ip = str(value)
@@ -98,30 +98,36 @@
 
         with _popen_lock:  # Work around Python 2 Popen race condition
             return subprocess.Popen(command, **kwargs)
 
     def kill_process(self) -> None:
         """Kill the engine process."""
         if not self.engine_opened:
+            wait_time = self.quit_time / 1e9 + 10 - time.perf_counter_ns() / 1e9
+            logger.debug(f'wait time before killing: {wait_time}')
+            if wait_time > 0:
+                time.sleep(wait_time)
             self.exit = True
             try:
                 # Windows
+                logger.debug("Killing Windows.")
                 self.p.send_signal(signal.CTRL_BREAK_EVENT)
             except AttributeError:
                 # Unix
+                logger.debug("Killing UNIX.")
                 os.killpg(self.p.pid, signal.SIGKILL)
 
             self.p.communicate()
             self.engine_receive_thread.join()
 
     def _connect(self) -> None:
         """Connect to the engine."""
         if not self.engine_opened:
             wait_time = self.start_time / 1e9 + self.wait_to_open_time - time.perf_counter_ns() / 1e9
-            logger.debug(f'wait time: {wait_time}')
+            logger.debug(f'wait time before connecting: {wait_time}')
             if wait_time > 0:
                 time.sleep(wait_time)
         self.console.run_command(f'connect {self.ip} {self.port}')
 
     def _start(self, board: draughts.Board, time: int) -> None:
         """Start the game."""
         self._connect()
@@ -158,18 +164,17 @@
                 return dxp.accepted
 
     def _recv_move(self) -> Optional[List[List[int]]]:
         """Receive the engine move."""
         while True:
             if not dxp.tReceiveHandler.isListening:
                 break
-            if self._last_move != dxp.last_move:
-                self._last_move = dxp.last_move
-                logger.debug(f'new last move: {self._last_move}')
-                return self._last_move
+            if dxp.last_move_changed:
+                logger.debug(f'new last move: {dxp.last_move.board_move}')
+                return dxp.last_move
 
     def play(self, board: draughts.Board) -> Any:
         """Engine search."""
         if not self.game_started:
             self._start(board, self.initial_time)
             self.game_started = True
         if board.move_stack:
@@ -179,7 +184,9 @@
             self.console.run_command(f'sm {move}')
         best_move = self._recv_move()
         return draughts.engine.PlayResult(best_move, None, {})
 
     def quit(self) -> None:
         """Quit the engine."""
         self.console.run_command('gameend 0')
+        self.console.run_command("disconn")
+        self.quit_time = time.perf_counter_ns()
```

### Comparing `pydraughts-0.6.1/draughts/engines/dxp_communication/dxp_classes.py` & `pydraughts-0.6.2/draughts/engines/dxp_communication/dxp_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,39 +27,43 @@
         """Get the color of the playing side."""
         return DXP_WHITE if self.pos.turn == draughts.WHITE else DXP_BLACK
 
 
 class MySocket:
     def __init__(self) -> None:
         self.sock = None
+        self.closed = False
 
     def open(self) -> MySocket:
         """Open the socket."""
         try:
             self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+            self.closed = False
         except Exception:
             self.sock = None
             raise Exception("socket exception: failed to open")
         return self
 
     def connect(self, host: str, port: int) -> MySocket:
         """Connect to the engine."""
         self.sock.settimeout(10)  # timeout for connection
         try:
             self.sock.connect((host, port))
         except socket.error as msg:
             self.sock = None
-            raise Exception("connection exception: failed to connect")
+            raise Exception(f"connection exception: failed to connect ({msg}).")
         if self.sock is not None:
             self.sock.settimeout(None)  # default
         return self
 
     def send(self, msg: str) -> None:
         """Send a message to the engine."""
         try:
+            logger.debug(f"socket send: {msg}")
             self.sock.send(bytes(msg, 'utf-8') + b"\0")
         except Exception:
             raise Exception("send exception: no connection")
         return None
 
     def receive(self) -> str:
         """Receive a message from the engine."""
@@ -83,17 +87,23 @@
         msg = msg.replace("\0", "")  # remove all null chars
 
         # Use strip to remove all whitespace at the start and end.
         # Including spaces, tabs, newlines and carriage returns.
         msg = msg.strip()
         return msg
 
-    def __del__(self):
-        if self.sock:
+    def close(self):
+        if self.sock and not self.closed:
+            self.closed = True
+            self.sock.shutdown(socket.SHUT_RDWR)
             self.sock.close()
+            self.sock = None
+
+    def __del__(self):
+        self.close()
 
 
 class DamExchange:
     def parse(self, msg: str) -> Dict[str, Union[str, List[str]]]:
         """Parse an incoming DXP message."""
         # Parse incoming DXP message. Returns relevant items depending on mtype.
         result: Dict[str, Union[str, List[str]]] = {}
```

### Comparing `pydraughts-0.6.1/draughts/engines/dxp_communication/dxp_run.py` & `pydraughts-0.6.2/draughts/engines/dxp_communication/dxp_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 import threading
 import logging
 from draughts.engines.dxp_communication.dxp_classes import DamExchange, MySocket, GameStatus, DXP_WHITE, DXP_BLACK
 from draughts import Move
 from typing import Union
 
 last_move = None
+last_move_changed = False
 accepted = None
+gameend_sent = False
 
 logger = logging.getLogger("pydraughts")
 
 
 class ConsoleHandler:
     def __init__(self) -> None:
         self.isRunning = False  # not used
 
     def run_command(self, comm: str) -> None:
         """Send a command to the DXP engine."""
 
         global current, mySock, lock
-        global accepted, last_move
+        global accepted, last_move, last_move_changed, gameend_sent
         logger.debug(f'comm {comm}')
 
         if comm.startswith('q') or comm.startswith('ex'):  # quit/exit
             logger.debug(f"Command terminate program: {comm.strip()}")
             # os._exit(1)  # does no cleanups
 
         elif comm.startswith('setup'):
@@ -56,38 +58,39 @@
             if current.started and current.myColor != current.get_color():
                 logger.debug("Move not allowed; server has to move")
                 return
             logger.debug(f"Command step move piece: {comm.strip()}")
             str_steps = comm.strip().split()[1].split('-')
             steps = list(map(int, str_steps))
 
-            lock.acquire()  # LOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCK
+            lock.acquire() # LOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCK
             if current.started and current.myColor == current.get_color():
                 timeSpend = 0  # time spend for this move (future)
 
                 board_move = []
                 for index in range(1, len(steps)):
                     board_move.append([steps[index - 1], steps[index]])
                 captures = []
                 for move in current.pos.legal_moves():
                     if move.steps_move == steps:
                         captures = move.captures
                         break
+                last_move_changed = False
                 msg = dxp.msg_move(steps, captures, timeSpend)
                 logger.debug(f'MOVE: {board_move}')
 
                 try:
                     mySock.send(msg)
                     logger.debug(f"snd MOVE: {msg}")
                 except Exception as err:
                     logger.debug(f"Error sending move: {err}")
                     return
 
                 current.pos.push(Move(board_move=board_move))
-            lock.release()  # LOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCK
+            lock.release() # LOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCK
 
         elif comm.startswith('conn'):
             if mySock.sock is not None:
                 logger.debug("Already connected")
                 return
             if current.started:
                 logger.debug("Game marked as started. First exit to start a new game.")
@@ -108,14 +111,23 @@
                 logger.debug(f"Error trying to connect: {err}")
                 return
 
             if mySock.sock is not None:  # connected
                 if not tReceiveHandler.isListening:
                     tReceiveHandler.start()
 
+        elif comm.startswith("disconn"):
+            try:
+                mySock.close()
+                logger.debug(f"Successfully closed socket.")
+            except Exception as err:
+                mySock.sock = None
+                logger.debug(f"Error trying to close socket: {err}")
+                return
+
         elif comm.startswith('chat'):
             if len(comm.split()) == 1:
                 return
             if len(comm.split()) > 1:
                 _, txt = comm.split(' ', 1)  # strip first word
                 txt = txt.strip()  # trim whitespace
                 logger.debug(f"Command send chat message: {comm.strip()}")
@@ -129,15 +141,17 @@
 
         elif comm.startswith('gamereq'):
             if current.started:
                 logger.debug("Game already started; gamereq not allowed")
                 return
             logger.debug(f"Command request new game: {comm.strip()}")
             last_move = None
+            last_move_changed = False
             accepted = None
+            gameend_sent = False
             myColor = "W"  # default
             gameTime = "120"  # default
             numMoves = "50"  # default
             if len(comm.split()) == 2:
                 _, myColor = comm.split()
             if len(comm.split()) == 3:
                 _, myColor, gameTime = comm.split()
@@ -163,14 +177,16 @@
             if current.started and current.myColor != current.get_color():
                 logger.debug("Message gameend not allowed; wait until your turn")
                 return
             if len(comm.split()) == 2:
                 _, reason = comm.split()
             else:
                 reason = "0"
+            accepted = None
+            gameend_sent = True
             msg = dxp.msg_gameend(reason)
 
             try:
                 mySock.send(msg)
                 logger.debug(f"snd GAMEEND: {msg}")
             except Exception as err:
                 logger.debug(f"Error sending gameend message: {err}")
@@ -196,70 +212,74 @@
     def run(self) -> None:
         """Start the receiver. It receives the moves from the DXP engine."""
         # Handling incoming messages from server.
         # Excutes when thread started. Overriding python threading.Thread.run()
 
         logger.debug("ReceiveHandler started")
         global current, mySock, lock
-        global accepted, last_move
+        global accepted, last_move, last_move_changed, gameend_sent
         self.isListening = True
         logger.debug("DXP Client starts listening")
         while True:
             try:
                 message = mySock.receive()  # wait for message
             except Exception as err:
                 logger.debug(f"Error {err}")
+                mySock.close()
                 break
 
             lock.acquire()  # LOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCK
             message = message[0:127]  # DXP max length
             dxpData = dxp.parse(message)
             if dxpData["type"] == "C":
                 logger.debug(f"rcv CHAT: {message}")
                 logger.debug(f"\nChat message: {dxpData['text']}")
 
             elif dxpData["type"] == "A":
                 logger.debug(f"rcv GAMEACC: {message}")
                 if dxpData["accCode"] == "0":
-                    current.started = True
                     current.myColor = current.myColor  # as requested
                     current.engineName = dxpData["engineName"]
                     logger.debug(f"\nGame request accepted by {dxpData['engineName']}")
                     accepted = True
+                    gameend_sent = False
+                    current.started = True
                 else:
-                    current.started = False
                     logger.debug(f"\nGame request NOT accepted by {dxpData['engineName']} Reason: {dxpData['accCode']}")
                     accepted = False
+                    current.started = False
 
             elif dxpData["type"] == "E":
                 logger.debug(f"rcv GAMEEND: {message}")
                 logger.debug(f"\nRequest end of game accepted. Reason: {dxpData['reason']} Stop: {dxpData['stop']}")
                 # Confirm game end by sending message back (if not sent by me)
-                if current.started:
-                    current.started = False
+                if current.started and not gameend_sent:
                     current.result = dxpData["reason"]
                     msg = dxp.msg_gameend(dxpData["reason"])
                     mySock.send(msg)
                     logger.debug(f"snd GAMEEND: {msg}")
+                    gameend_sent = True
+                    current.started = False
 
             elif dxpData["type"] == "M":
                 logger.debug(f"rcv MOVE: {message}")
                 steps = [dxpData['from'], dxpData['to']]
                 nsteps = list(map(int, steps))
                 ntakes = list(map(int, dxpData['captures']))
                 ntakes = list(map(lambda pos: str(pos).zfill(2), sorted(ntakes)))
                 correct_move = None
                 for move in current.pos.legal_moves():
                     if move.hub_position_move == f"{str(nsteps[0]).zfill(2)}{str(nsteps[-1]).zfill(2)}{''.join(ntakes)}":
                         correct_move = move
 
                 if correct_move is not None:
                     last_move = correct_move
-                    logger.debug(f"\nMove received: {correct_move.steps_move}")
+                    logger.debug(f"Move received: {correct_move.steps_move}")
                     current.pos.push(correct_move)
+                    last_move_changed = True
                 else:
                     logger.debug(f"Error: received move is illegal [{message}]")
 
             elif dxpData["type"] == "B":
                 # For the time being do not confirm request from server: send message back.
                 logger.debug(f"rcv BACKREQ: {message}")
                 accCode = "1"  # 0: BACK YES; 1: BACK NO; 2: CONTINUE
@@ -279,15 +299,18 @@
             else:
                 logger.debug(f"rcv UNKNOWN: {message}")
                 logger.debug(f"\nrcv Unknown message: {message}")
 
             lock.release()  # LOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCKLOCK
 
         self.isListening = False
-        logger.error("Listening stopped; connection broken")
+        if mySock.closed:
+            logger.debug("Listening stopped; connection broken")
+        else:
+            logger.error("Listening stopped; connection broken")
         logger.debug("Connection broken; receiveHandler stopped. ")
         logger.debug("Save your data and exit program to start again. ")
         return None
 
 
 dxp = DamExchange()  # global, singleton
 mySock = MySocket()  # global, singleton
```

### Comparing `pydraughts-0.6.1/draughts/engines/hub.py` & `pydraughts-0.6.2/draughts/engines/hub.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/other_licenses/ImparaAI checkers LICENSE` & `pydraughts-0.6.2/other_licenses/ImparaAI checkers LICENSE`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/other_licenses/akalverboer DXC100_draughts_client LICENSE` & `pydraughts-0.6.2/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018  Arthur Kalverboer
+Copyright (c) 2021-2022 Ioannis Pantidis
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pydraughts-0.6.1/other_licenses/fishnet LICENSE.txt` & `pydraughts-0.6.2/other_licenses/fishnet LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/pydraughts.egg-info/PKG-INFO` & `pydraughts-0.6.2/pydraughts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydraughts
-Version: 0.6.1
+Version: 0.6.2
 Summary: A draughts library for Python with move generation, PDN reading and writing, engine communication and balloted openings
 Home-page: https://github.com/AttackingOrDefending/pydraughts
 Author: AttackingOrDefending
 Project-URL: Bug Tracker, https://github.com/AttackingOrDefending/pydraughts/issues
 Keywords: checkers,draughts,game,fen,pdn
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -65,15 +65,15 @@
 * Make a move
 ```python
 move = Move(board, steps_move=[34, 30])
 board.push(move)
 
 # Multi-capture
 board2 = Board(fen="W:WK40:B19,29")
-board2.push(Move(board2), pdn_move='40x14')
+board2.push(Move(board2, pdn_move='40x14'))
 ```
 * Get a visual representation of the board
 ```python
 print(board)
 
 """
    | b |   | b |   | b |   | b |   | b
```

### Comparing `pydraughts-0.6.1/pydraughts.egg-info/SOURCES.txt` & `pydraughts-0.6.2/pydraughts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.1/setup.cfg` & `pydraughts-0.6.2/setup.cfg`

 * *Files identical despite different names*

