# Comparing `tmp/BaseDT-0.0.5.tar.gz` & `tmp/BaseDT-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseDT-0.0.5.tar", last modified: Fri May  5 09:47:48 2023, max compression
+gzip compressed data, was "BaseDT-0.0.6.tar", last modified: Wed Jun  7 06:28:57 2023, max compression
```

## Comparing `BaseDT-0.0.5.tar` & `BaseDT-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-05 09:47:48.000000 BaseDT-0.0.5/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-05 09:47:48.000000 BaseDT-0.0.5/BaseDT/
--rw-rw-r--   0 user      (1001) user      (1001)        0 2023-04-26 07:17:02.000000 BaseDT-0.0.5/BaseDT/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)    16851 2023-05-05 09:45:53.000000 BaseDT-0.0.5/BaseDT/data.py
--rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-04-26 07:17:02.000000 BaseDT-0.0.5/BaseDT/data_image.py
--rw-rw-r--   0 user      (1001) user      (1001)    31309 2023-04-26 07:17:02.000000 BaseDT-0.0.5/BaseDT/dataset.py
--rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-04-26 07:17:02.000000 BaseDT-0.0.5/BaseDT/io.py
--rw-rw-r--   0 user      (1001) user      (1001)     6986 2023-04-26 07:19:34.000000 BaseDT-0.0.5/BaseDT/plot.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-05 09:47:48.000000 BaseDT-0.0.5/BaseDT.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      314 2023-05-05 09:47:48.000000 BaseDT-0.0.5/BaseDT.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      316 2023-05-05 09:47:48.000000 BaseDT-0.0.5/BaseDT.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-05-05 09:47:48.000000 BaseDT-0.0.5/BaseDT.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       49 2023-05-05 09:47:48.000000 BaseDT-0.0.5/BaseDT.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        7 2023-05-05 09:47:48.000000 BaseDT-0.0.5/BaseDT.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-02-02 07:26:47.000000 BaseDT-0.0.5/BaseDT.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDT-0.0.5/MANIFEST.in
--rw-rw-r--   0 user      (1001) user      (1001)      314 2023-05-05 09:47:48.000000 BaseDT-0.0.5/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       49 2023-05-05 09:43:00.000000 BaseDT-0.0.5/install_requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-05-05 09:47:48.000000 BaseDT-0.0.5/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     4245 2023-05-05 09:47:43.000000 BaseDT-0.0.5/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-07 06:28:57.369519 BaseDT-0.0.6/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-07 06:28:57.365519 BaseDT-0.0.6/BaseDT/
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2023-04-26 07:17:02.000000 BaseDT-0.0.6/BaseDT/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)    31622 2023-06-07 06:26:00.000000 BaseDT-0.0.6/BaseDT/data.py
+-rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-04-26 07:17:02.000000 BaseDT-0.0.6/BaseDT/data_image.py
+-rw-rw-r--   0 user      (1001) user      (1001)    36851 2023-06-07 06:19:04.000000 BaseDT-0.0.6/BaseDT/dataset.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-04-26 07:17:02.000000 BaseDT-0.0.6/BaseDT/io.py
+-rw-rw-r--   0 user      (1001) user      (1001)    12752 2023-06-06 05:32:46.000000 BaseDT-0.0.6/BaseDT/plot.py
+-rw-rw-r--   0 user      (1001) user      (1001)     7577 2023-06-05 14:43:34.000000 BaseDT-0.0.6/BaseDT/utils.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-07 06:28:57.369519 BaseDT-0.0.6/BaseDT.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-07 06:28:57.000000 BaseDT-0.0.6/BaseDT.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      332 2023-06-07 06:28:57.000000 BaseDT-0.0.6/BaseDT.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-07 06:28:57.000000 BaseDT-0.0.6/BaseDT.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       43 2023-06-07 06:28:57.000000 BaseDT-0.0.6/BaseDT.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        7 2023-06-07 06:28:57.000000 BaseDT-0.0.6/BaseDT.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-02-02 07:26:47.000000 BaseDT-0.0.6/BaseDT.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDT-0.0.6/MANIFEST.in
+-rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-07 06:28:57.369519 BaseDT-0.0.6/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       42 2023-05-31 10:06:54.000000 BaseDT-0.0.6/install_requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-06-07 06:28:57.369519 BaseDT-0.0.6/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     4245 2023-06-07 06:14:46.000000 BaseDT-0.0.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `BaseDT-0.0.5/BaseDT/data.py` & `BaseDT-0.0.6/BaseDT/data_image.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 # 导入工具库
 import numpy as np
-import matplotlib.pyplot as plt
 import cv2
-import jieba
-from sklearn.feature_extraction.text import CountVectorizer
-from sklearn.feature_extraction import DictVectorizer
 import numbers
 
 class ImageData(object):
     '''
     目前支持图片路径, np array, 文本
     后续支持 PIL
     '''
@@ -38,20 +34,18 @@
 
     def get_attribute(self, n):
         if n in self.__dict__:
             return self.__dict__[n]
         else:
             return None
 
-    def __init__(self, data_source, **kwargs):
+    def __init__(self, data_source,**kwargs):
         self.vct = None
         self.data_source = data_source
-        # 装在默认参数进入私有变量列表
         self.__dict__.update(self._defaults)
-        # 将关键词参数装入私有变量列表
         for name, value in kwargs.items():
             setattr(self, name, value)
 
         if type(self.data_source) == str:
             self.value = cv2.imdecode(np.fromfile((self.data_source),dtype=np.uint8),-1)
         if type(self.data_source) == np.ndarray:
             self.value = self.data_source
@@ -60,38 +54,34 @@
             pass
         self.value = self.value.astype(self.get_attribute("data_type"))
         self.raw_value = self.value
         if self.get_attribute("backbone"):
             # for key, value in self._backbone_args[self.get_attribute("backbone")].items():
             #     print(key,value)
             self.value = ImageData(data_source, **self._backbone_args[self.get_attribute("backbone")]).value
-            self.__dict__.update(self._backbone_args[self.get_attribute("backbone")])#更新私有变量列表
         else:
-            if self.get_attribute("to_rgb") == False and len(self.value.shape)>=3:
+            if self.get_attribute("to_rgb") == False:
                 self._rgb2gray()
-            elif self.get_attribute("to_rgb") == True:
+            else:
                 self._to3channel()
-            #需要考虑各种操作顺序的灵活性，循环遍历私有变量列表来实现
-            for key in self.__dict__.keys():
-                if key == "size" or key == "size_keep_ratio":
-                    size = self.get_attribute("size")
-                    size_keep_ratio = self.get_attribute("size_keep_ratio")
-                    self._resize(size, size_keep_ratio)
-                if key == "crop_size":
-                    crop_size = self.get_attribute("crop_size")
-                    self._crop(crop_size)
-                if key == "normalize":
-                    #TODO 需检查维度
-                    if self.get_attribute("normalize") == True:
-                        mean = self.get_attribute("mean")
-                        std = self.get_attribute("std")
-                        self._normalize(mean, std)
-                if key == "pad_size_divisor":
-                    pad_size_divisor = self.get_attribute("pad_size_divisor")
-                    self._pad(size_divisor=pad_size_divisor)
+            if self.get_attribute("size") or self.get_attribute("size_keep_ratio"):
+                size = self.get_attribute("size")
+                size_keep_ratio = self.get_attribute("size_keep_ratio")
+                self._resize(size, size_keep_ratio)
+            if self.get_attribute("crop_size"):
+                crop_size = self.get_attribute("crop_size")
+                self._crop(crop_size)
+            if self.get_attribute("normalize")==True:
+                #TODO 需检查维度
+                mean = self.get_attribute("mean")
+                std = self.get_attribute("std")
+                self._normalize(mean, std)
+            if self.get_attribute("pad_size_divisor"):
+                pad_size_divisor = self.get_attribute("pad_size_divisor")
+                self._pad(size_divisor=pad_size_divisor)
 
     def to_tensor(self):
         if self.get_attribute("to_rgb"):
             return np.expand_dims(np.transpose(self.value, (2,0,1)), 0)
         else:
             return np.expand_dims(np.expand_dims(self.value, 0), 0)
 
@@ -285,145 +275,28 @@
             border_type[padding_mode],
             value=pad_val)
         self.value = img
 
     def _flip(self):
         pass
 
-    def show(self, raw = False):
-        if raw: img = self.raw_value
-        else: img = self.value
-        if len(img.shape) == 3:
-            img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-        plt.imshow(img)
-        plt.show()
+    def show(self, raw = False, win_name='', wait_time=0):
+        if raw: cv2.imshow(win_name, self.raw_value)
+        else: cv2.imshow(win_name, self.value)
+        if wait_time == 0:  # prevent from hanging if windows was closed
+            while True:
+                ret = cv2.waitKey(1)
+
+                closed = cv2.getWindowProperty(win_name, cv2.WND_PROP_VISIBLE) < 1
+                # if user closed window or if some key pressed
+                if closed or ret != -1:
+                    break
+        else:
+            ret = cv2.waitKey(wait_time)
 
-    def map_orig_coords(self, boxes):
-        #TODO 暂时只支持box的映射，后续应该支持单纯的坐标映射
+    def map_orig_coords(self, box):
         original_w, original_h = self.raw_value.shape[:2]
         processed_w, processed_h = self.value.shape[:2]
+        x1, y1, x2, y2, score = box
         sx, sy = original_w / processed_w, original_h / processed_h
-        new_boxes = np.array([]).reshape(0, 5)
-        for box in boxes:
-            new_box = [box[0] * sy, box[1] * sx, box[2] * sy, box[3] * sx, box[4]]
-            new_boxes = np.concatenate([new_boxes, [new_box]], axis=0)
-        return new_boxes
-
-class TextData(object):
-    _defaults = {
-        "data_type": 'uint8',
-        # 文本默认属性
-        "vct": {"str": CountVectorizer(), "dict": DictVectorizer()},
-    }
-
-    def get_attribute(self, n):
-        if n in self.__dict__:
-            return self.__dict__[n]
-        else:
-            return None
-
-    def __init__(self, data_source, **kwargs):
-        self.vct = None
-        self.data_source = data_source
-        self.__dict__.update(self._defaults)
-        for name, value in kwargs.items():
-            setattr(self, name, value)
-
-        # 这里的data_source不可以是文件
-        self.raw_value = self.data_source
-        self.value = self.raw_value
-        if type(self.raw_value) == dict or type(self.raw_value[0]) == dict:
-            self.text_type = "dict"
-            if type(self.raw_value) == dict: self.value = [self.raw_value]
-        elif type(self.raw_value) == str or type(self.raw_value[0]) == str:
-            self.text_type = "str"
-            if type(self.raw_value) == str: self.value = [self.raw_value]
-        else:
-            # TODO 检查合法性
-            pass
-        if self.get_attribute("vectorize") == True:
-            self.value = self.vectorizer(self.get_attribute("chinese"), self.get_attribute("fitted"))
-
-    def vectorizer(self, chinese = False, fitted = False):
-        '''
-        支持单文本及多文本
-        :param text: 允许raw txt输入以及半处理数据例如字典输入
-        :return: 词向量矩阵（词向量组成的矩阵）
-        '''
-        txt_cnt = None
-        text_type = self.text_type
-        texts = self.value
-
-        if chinese:
-            for i in range(len(texts)):
-                texts[i] = self._chinese_cut(texts[i])
-        #过滤
-        # for i in range(len(texts)):
-        #     texts[i] = re.sub('[^\u4e00-\u9fa5a-zA-Z0-9\sP]+', '', texts[i])
-        if text_type == "dict":
-            if not fitted: txt_cnt = self.vct[text_type].fit_transform(texts)
-            if fitted: txt_cnt = self.vct[self.text_type].transform(texts)
-
-        if text_type=="str":
-            if not fitted: txt_cnt = self.vct[text_type].fit_transform(texts)
-            if fitted: txt_cnt = self.vct[text_type].transform(texts)
-        return txt_cnt.A
-
-    def fit(self, texts = ""):
-        '''
-        生成词汇表，支持单文本及多文本
-        :param text:
-        :return:
-        '''
-        text_type = self.text_type
-        self.vct[text_type] = self.vct[text_type].fit(texts)
-
-    def get_feature_names(self):
-        texts = self.value
-        text_type = self.text_type
-        return self.vct[text_type].get_feature_names_out()
-
-    def _chinese_cut(self, text):
-        '''
-        单文本操作
-        :param text:
-        :return: 返回字符串
-        '''
-        words = list(jieba.cut(text))
-        text = "/ ".join(words)
-        # text = "".join(words)
-        return text
-
-    def to_tensor(self):
-        pass
-   
-class ModelData(object):
-
-    def __init__(self, path):
-        self.path = path
+        return x1 * sx, y1 * sy, x2 * sx, y2 * sy, score
 
-    def get_labels(self):
-        assert isinstance(self.path, str)
-        file_path = self.path
-        class_name = []
-        key = 'CLASSES'
-        if file_path[-3:] == 'txt':
-            with open(file_path, 'r') as f:
-                class_name = [tag.strip() for tag in f.readlines()]
-        elif file_path[-3:] == 'pth':
-            import torch
-            state_dict = torch.load(file_path, map_location=torch.device('cpu'))
-            if key in state_dict['meta']:
-                class_name = state_dict['meta'][key]
-        elif file_path[-4:] == 'onnx':
-            import onnxruntime
-            sess = onnxruntime.InferenceSession(file_path)
-            model_meta = sess.get_modelmeta()
-            if key in model_meta.custom_metadata_map:
-                unicode_string = model_meta.custom_metadata_map[key]
-                class_name = unicode_string.split('|')
-        else:
-            file_allow = ['txt', 'pth', 'onnx']
-            print('This function currently supports file formats in {}, please check the path'.format(file_allow))
-        if len(class_name) == 0:
-            print('Class_name in model is empty. Please use model generate by MMEdu')
-        return class_name
```

### Comparing `BaseDT-0.0.5/BaseDT/dataset.py` & `BaseDT-0.0.6/BaseDT/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -739,7 +739,134 @@
             try:
                 self.check_cls()
                 self.print_folder_structure(self.dataset_path)
             except Exception as e:
                 print(e)
 
 
+def split_tab_dataset(data_path, data_column,label_column=[-1],train_val_ratio=0.8,random_seed=42):
+
+    # 读取提取后的特征和标签
+    data = np.loadtxt(data_path, dtype=float, delimiter=',',skiprows=1,usecols=data_column)
+    label =  np.loadtxt(data_path, dtype=float, delimiter=',',skiprows=1,usecols=label_column)
+
+    # 设置随机种子，以获得可复现的划分结果
+    np.random.seed(random_seed)
+    state = np.random.get_state()
+    np.random.shuffle(data)
+    np.random.set_state(state)
+    np.random.shuffle(label)
+
+    
+    # 计算训练集验证集大小
+    train_size = int(len(data) * train_val_ratio)
+    val_size = int(len(data)) - train_size
+    print("正在划分数据集，比例为 train:val = {}:{}".format(train_val_ratio, round(1.0-train_val_ratio,3)))
+    print("实际数据量为 train:val = {}:{}".format(train_size, val_size))
+    print("划分中......")
+    train_x = data[:train_size]
+    train_y = label[:train_size]
+    val_x = data[train_size:]
+    val_y = label[train_size:]
+    # print(val_x, val_y)
+
+    # import numpy as np
+    # # 将 feature_data和labels拼接成一个数组
+    if len(train_x.shape) == 1:
+        train_x = train_x.reshape(-1,1)
+    if len(train_y.shape) == 1:
+        train_y = train_y.reshape(-1,1)
+    if len(val_x.shape) == 1:
+        val_x = val_x.reshape(-1,1)
+    if len(val_y.shape) == 1:
+        val_y = val_y.reshape(-1,1)
+    # print(len(train_x.shape),len(train_y.shape))
+
+    data_np_train = np.concatenate((train_x, train_y), axis=1)
+    # print(data_np_train)
+    data_np_val = np.concatenate((val_x, val_y), axis=1)
+    # # 添加表头
+    if isinstance(data_column, int):
+        len_data = 1
+    else:
+        len_data = len(data_column)
+    len_label = 1 if isinstance(label_column, int) else len(label_column)
+    header = [f"Feature {i+1}" for i in range(len_data)] + [f"Label {i+1}" for i in range(len_label)] # 设置表头的列名
+    train_data_with_header = np.vstack([header, data_np_train])  # 将表头和数据数组合并
+    val_data_with_header = np.vstack([header, data_np_val])
+    print("划分完毕！")
+    # # 保存为 CSV 文件
+    file_name = data_path.rsplit(".",1)
+    train_file = file_name[0]+"_train."+file_name[1]
+    val_file = file_name[0]+"_val."+file_name[1]
+    np.savetxt(train_file, train_data_with_header, delimiter=",", fmt="%s")
+    np.savetxt(val_file, val_data_with_header, delimiter=",", fmt="%s")
+    print("训练集保存至{}，验证集保存至{}。".format(train_file, val_file))
+    return train_x,train_y, val_x, val_y
+
+def split_tab_dataset_class(data_path, data_column,label_column=[-1],train_val_ratio=0.8,random_seed=42):
+    # 读取提取后的特征和标签
+    data = np.loadtxt(data_path, dtype=float, delimiter=',',skiprows=1,usecols=data_column)
+    label =  np.loadtxt(data_path, dtype=float, delimiter=',',skiprows=1,usecols=label_column)
+    # 获得所有标签
+    label_unique = np.unique(label)
+    # 设置随机数种子
+    np.random.seed(random_seed)
+    # 按类别划分数据集
+    for id, i in enumerate(label_unique):
+        # 获得随机种子状态，确保数据和标签以相同的顺序打乱
+        state = np.random.get_state()
+        np.random.shuffle(data)
+        np.random.set_state(state)
+        np.random.shuffle(label)
+        label_i = label[label == i]
+        data_i = data[label == i]
+        train_size = int(len(data_i) * train_val_ratio)
+        train_xi = data_i[:train_size]
+        train_yi = label_i[:train_size]
+        val_xi = data_i[train_size:]
+        val_yi = label_i[train_size:]
+        if id == 0:
+            train_x,train_y, val_x, val_y = train_xi,train_yi,val_xi,val_yi
+            continue
+        train_x = np.concatenate((train_x,train_xi), axis=0)
+        train_y = np.concatenate((train_y,train_yi), axis=0)
+        val_x = np.concatenate((val_x,val_xi), axis=0)
+        val_y = np.concatenate((val_y,val_yi), axis=0)
+
+    # 目前按照类别顺序，需再次打乱
+    state = np.random.get_state()
+    np.random.shuffle(val_x)
+    np.random.set_state(state)
+    np.random.shuffle(val_y)
+    np.random.set_state(state)
+    np.random.shuffle(train_x)
+    np.random.set_state(state)
+    np.random.shuffle(train_y)
+    # 拼接data和label之前确保形状一致可拼接
+    if len(train_x.shape) == 1:
+        train_x = train_x.reshape(-1,1)
+    if len(train_y.shape) == 1:
+        train_y = train_y.reshape(-1,1)
+    if len(val_x.shape) == 1:
+        val_x = val_x.reshape(-1,1)
+    if len(val_y.shape) == 1:
+        val_y = val_y.reshape(-1,1)
+    # 将 data和label拼接成一个数组
+    np_train = np.concatenate((train_x, train_y), axis=1)
+    np_val = np.concatenate((val_x, val_y), axis=1)
+    # 添加表头
+    len_data = 1 if isinstance(data_column, int) else len(data_column)
+    len_label = 1 if isinstance(label_column, int) else len(label_column)
+    header = [f"Feature {i+1}" for i in range(len_data)] + [f"Label {i+1}" for i in range(len_label)] # 设置表头的列名
+    # 将表头和数据数组合并
+    train_data_with_header = np.vstack([header, np_train])  
+    val_data_with_header = np.vstack([header, np_val])
+    # 保存为 CSV 文件
+    file_name = data_path.rsplit(".",1)
+    train_file = file_name[0]+"_train."+file_name[1]
+    val_file = file_name[0]+"_val."+file_name[1]
+    np.savetxt(train_file, train_data_with_header, delimiter=",", fmt="%s")
+    np.savetxt(val_file, val_data_with_header, delimiter=",", fmt="%s")
+
+    return train_x,train_y, val_x, val_y
+
```

### Comparing `BaseDT-0.0.5/BaseDT/io.py` & `BaseDT-0.0.6/BaseDT/io.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.5/setup.py` & `BaseDT-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 yield item
 
     packages = list(gen_packages_items())
     return packages
 
 setup(
     name='BaseDT',
-    version='0.0.5',
+    version='0.0.6',
     # version='0.0.1rc1',
     description='BaseDT is a data-processing  tool including data, dataset, io and plot.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
```

