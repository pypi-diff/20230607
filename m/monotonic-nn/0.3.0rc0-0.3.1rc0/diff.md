# Comparing `tmp/monotonic-nn-0.3.0rc0.tar.gz` & `tmp/monotonic-nn-0.3.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monotonic-nn-0.3.0rc0.tar", last modified: Mon Jun  5 12:35:27 2023, max compression
+gzip compressed data, was "monotonic-nn-0.3.1rc0.tar", last modified: Wed Jun  7 07:07:44 2023, max compression
```

## Comparing `monotonic-nn-0.3.0rc0.tar` & `monotonic-nn-0.3.1rc0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:35:27.573294 monotonic-nn-0.3.0rc0/
--rw-r--r--   0 davor     (1000) davor     (1000)    20848 2023-06-05 07:35:04.000000 monotonic-nn-0.3.0rc0/LICENSE
--rw-r--r--   0 davor     (1000) davor     (1000)      111 2023-06-05 07:35:04.000000 monotonic-nn-0.3.0rc0/MANIFEST.in
--rw-rw-r--   0 davor     (1000) davor     (1000)    10660 2023-06-05 12:35:27.573294 monotonic-nn-0.3.0rc0/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)     9516 2023-06-05 12:24:54.000000 monotonic-nn-0.3.0rc0/README.md
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:35:27.573294 monotonic-nn-0.3.0rc0/airt/
--rw-rw-r--   0 davor     (1000) davor     (1000)       22 2023-06-05 12:25:53.000000 monotonic-nn-0.3.0rc0/airt/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:35:27.573294 monotonic-nn-0.3.0rc0/airt/_components/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-05 12:25:53.000000 monotonic-nn-0.3.0rc0/airt/_components/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)      320 2023-06-05 12:25:52.000000 monotonic-nn-0.3.0rc0/airt/_components/helpers.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    31430 2023-06-05 12:25:53.000000 monotonic-nn-0.3.0rc0/airt/_components/mono_dense_layer.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     9926 2023-06-05 12:25:53.000000 monotonic-nn-0.3.0rc0/airt/_modidx.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:35:27.573294 monotonic-nn-0.3.0rc0/airt/keras/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-05 12:25:53.000000 monotonic-nn-0.3.0rc0/airt/keras/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    14087 2023-06-05 12:25:52.000000 monotonic-nn-0.3.0rc0/airt/keras/experiments.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:35:27.573294 monotonic-nn-0.3.0rc0/airt/keras/layers/
--rw-rw-r--   0 davor     (1000) davor     (1000)      344 2023-06-05 12:25:53.000000 monotonic-nn-0.3.0rc0/airt/keras/layers/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:35:27.573294 monotonic-nn-0.3.0rc0/monotonic_nn.egg-info/
--rw-rw-r--   0 davor     (1000) davor     (1000)    10660 2023-06-05 12:35:27.000000 monotonic-nn-0.3.0rc0/monotonic_nn.egg-info/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)      510 2023-06-05 12:35:27.000000 monotonic-nn-0.3.0rc0/monotonic_nn.egg-info/SOURCES.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 12:35:27.000000 monotonic-nn-0.3.0rc0/monotonic_nn.egg-info/dependency_links.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)       30 2023-06-05 12:35:27.000000 monotonic-nn-0.3.0rc0/monotonic_nn.egg-info/entry_points.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 07:37:05.000000 monotonic-nn-0.3.0rc0/monotonic_nn.egg-info/not-zip-safe
--rw-rw-r--   0 davor     (1000) davor     (1000)      268 2023-06-05 12:35:27.000000 monotonic-nn-0.3.0rc0/monotonic_nn.egg-info/requires.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        5 2023-06-05 12:35:27.000000 monotonic-nn-0.3.0rc0/monotonic_nn.egg-info/top_level.txt
--rw-r--r--   0 davor     (1000) davor     (1000)      919 2023-06-05 12:34:58.000000 monotonic-nn-0.3.0rc0/settings.ini
--rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-05 12:35:27.573294 monotonic-nn-0.3.0rc0/setup.cfg
--rw-r--r--   0 davor     (1000) davor     (1000)     3157 2023-06-05 12:32:50.000000 monotonic-nn-0.3.0rc0/setup.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:07:44.830350 monotonic-nn-0.3.1rc0/
+-rw-rw-r--   0 davor     (1000) davor     (1000)    20848 2023-06-05 13:19:26.000000 monotonic-nn-0.3.1rc0/LICENSE
+-rw-rw-r--   0 davor     (1000) davor     (1000)      111 2023-06-05 13:19:26.000000 monotonic-nn-0.3.1rc0/MANIFEST.in
+-rw-rw-r--   0 davor     (1000) davor     (1000)    12001 2023-06-07 07:07:44.830350 monotonic-nn-0.3.1rc0/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10857 2023-06-06 14:04:51.000000 monotonic-nn-0.3.1rc0/README.md
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:07:44.830350 monotonic-nn-0.3.1rc0/airt/
+-rw-rw-r--   0 davor     (1000) davor     (1000)      367 2023-06-07 07:07:07.000000 monotonic-nn-0.3.1rc0/airt/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:07:44.830350 monotonic-nn-0.3.1rc0/airt/_components/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-07 07:07:07.000000 monotonic-nn-0.3.1rc0/airt/_components/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)      320 2023-06-07 07:07:07.000000 monotonic-nn-0.3.1rc0/airt/_components/helpers.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    31436 2023-06-07 07:07:07.000000 monotonic-nn-0.3.1rc0/airt/_components/mono_dense_layer.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     9935 2023-06-07 07:07:07.000000 monotonic-nn-0.3.1rc0/airt/_modidx.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:07:44.830350 monotonic-nn-0.3.1rc0/airt/keras/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-07 07:07:07.000000 monotonic-nn-0.3.1rc0/airt/keras/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    14089 2023-06-07 07:07:07.000000 monotonic-nn-0.3.1rc0/airt/keras/experiments.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:07:44.830350 monotonic-nn-0.3.1rc0/airt/keras/layers/
+-rw-rw-r--   0 davor     (1000) davor     (1000)      344 2023-06-07 07:07:07.000000 monotonic-nn-0.3.1rc0/airt/keras/layers/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:07:44.830350 monotonic-nn-0.3.1rc0/monotonic_nn.egg-info/
+-rw-rw-r--   0 davor     (1000) davor     (1000)    12001 2023-06-07 07:07:44.000000 monotonic-nn-0.3.1rc0/monotonic_nn.egg-info/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)      510 2023-06-07 07:07:44.000000 monotonic-nn-0.3.1rc0/monotonic_nn.egg-info/SOURCES.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-07 07:07:44.000000 monotonic-nn-0.3.1rc0/monotonic_nn.egg-info/dependency_links.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)       30 2023-06-07 07:07:44.000000 monotonic-nn-0.3.1rc0/monotonic_nn.egg-info/entry_points.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 18:05:47.000000 monotonic-nn-0.3.1rc0/monotonic_nn.egg-info/not-zip-safe
+-rw-rw-r--   0 davor     (1000) davor     (1000)      268 2023-06-07 07:07:44.000000 monotonic-nn-0.3.1rc0/monotonic_nn.egg-info/requires.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        5 2023-06-07 07:07:44.000000 monotonic-nn-0.3.1rc0/monotonic_nn.egg-info/top_level.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)      919 2023-06-07 07:07:01.000000 monotonic-nn-0.3.1rc0/settings.ini
+-rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-07 07:07:44.830350 monotonic-nn-0.3.1rc0/setup.cfg
+-rw-rw-r--   0 davor     (1000) davor     (1000)     3157 2023-06-05 13:19:26.000000 monotonic-nn-0.3.1rc0/setup.py
```

### Comparing `monotonic-nn-0.3.0rc0/LICENSE` & `monotonic-nn-0.3.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.3.0rc0/PKG-INFO` & `monotonic-nn-0.3.1rc0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,68 @@
-Metadata-Version: 2.1
-Name: monotonic-nn
-Version: 0.3.0rc0
-Summary: Monotonic Neural Networks
-Home-page: https://github.com/airtai/monotonic-nn
-Author: AIRT Technologies d.o.o.
-Author-email: info@airt.ai
-License: Creative Commons License
-Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
-Project-URL: CI, https://github.com/airtai/monotonic-nn/actions
-Project-URL: Documentation, https://monotonic.airt.ai/
-Project-URL: Tutorial, https://colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb
-Keywords: tensorflow keras monotone "monotonic neural networks" "dense layer"
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: Free for non-commercial use
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: experiments
-License-File: LICENSE
-
 Constrained Monotonic Neural Networks
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-This Python library implements Monotonic Dense Layer as described in
+## Running in Google Colab
+
+You can execute this interactive tutorial in Google Colab by clicking
+the button below:
+
+<a href="https://colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb" target=”_blank”>
+<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab" />
+</a>
+
+## Summary
+
+This Python library implements Constrained Monotonic Neural Networks as
+described in:
+
 Davor Runje, Sharath M. Shankaranarayana, “Constrained Monotonic Neural
-Networks” \[[PDF](https://arxiv.org/pdf/2205.11775.pdf)\].
+Networks”, in Proceedings of the 40th International Conference on
+Machine Learning, 2023. \[[PDF](https://arxiv.org/pdf/2205.11775.pdf)\].
+
+#### Abstract
+
+Wider adoption of neural networks in many critical domains such as
+finance and healthcare is being hindered by the need to explain their
+predictions and to impose additional constraints on them. Monotonicity
+constraint is one of the most requested properties in real-world
+scenarios and is the focus of this paper. One of the oldest ways to
+construct a monotonic fully connected neural network is to constrain
+signs on its weights. Unfortunately, this construction does not work
+with popular non-saturated activation functions as it can only
+approximate convex functions. We show this shortcoming can be fixed by
+constructing two additional activation functions from a typical
+unsaturated monotonic activation function and employing each of them on
+the part of neurons. Our experiments show this approach of building
+monotonic neural networks has better accuracy when compared to other
+state-of-the-art methods, while being the simplest one in the sense of
+having the least number of parameters, and not requiring any
+modifications to the learning procedure or post-learning steps. Finally,
+we prove it can approximate any continuous monotone function on a
+compact subset of $\mathbb{R}^n$.
+
+#### Citation
 
 If you use this library, please cite:
 
 ``` title="bibtex"
 @inproceedings{runje2023,
   title={Constrained Monotonic Neural Networks},
   author={Davor Runje and Sharath M. Shankaranarayana},
   booktitle={Proceedings of the 40th {International Conference on Machine Learning}},
   year={2023}
 }
 ```
 
+## Python package
+
 This package contains an implementation of our Monotonic Dense Layer
-[`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
+[`MonoDense`](https://monotonic.airt.ai/0.3.0/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
 (Constrained Monotonic Fully Connected Layer). Below is the figure from
 the paper for reference.
 
 In the code, the variable `monotonicity_indicator` corresponds to **t**
 in the figure and parameters `is_convex`, `is_concave` and
 `activation_weights` are used to calculate the activation selector **s**
 as follows:
@@ -64,40 +76,33 @@
   and $\tilde{s}$, respecively. E.g. if `activation_weights = (2, 2, 1)`
   and `units = 10`, then
 
 $$
 (\breve{s}, \hat{s}, \tilde{s}) = (4, 4, 2)
 $$
 
-![mono-dense-layer-diagram](https://github.com/airtai/monotonic-nn/raw/main/nbs/images/mono-dense-layer-diagram.png)
-
-## Running in Google Colab
-
-You can start this interactive tutorial in Google Colab by clicking the
-button below:
-
-<a href="https://colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb" target=”_blank”>
-<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab" />
-</a>
+![mono-dense-layer-diagram](https://monotonic.airt.ai/0.3.0/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
 
-## Install
+### Install
 
 ``` sh
 pip install monotonic-nn
 ```
 
-## How to use
+### How to use
 
 In this example, we’ll assume we have a simple dataset with three inputs
 values $x_1$, $x_2$ and $x_3$ sampled from the normal distribution,
 while the output value $y$ is calculated according to the following
 formula before adding Gaussian noise to it:
 
 $y = x_1^3 + \sin\left(\frac{x_2}{2 \pi}\right) + e^{-x_3}$
 
+<style type="text/css">
+</style>
 <table id="T_37b51">
   <thead>
     <tr>
       <th id="T_37b51_level0_col0" class="col_heading level0 col0" >x0</th>
       <th id="T_37b51_level0_col1" class="col_heading level0 col1" >x1</th>
       <th id="T_37b51_level0_col2" class="col_heading level0 col2" >x2</th>
       <th id="T_37b51_level0_col3" class="col_heading level0 col3" >y</th>
@@ -134,35 +139,35 @@
       <td id="T_37b51_row4_col2" class="data row4 col2" >0.467509</td>
       <td id="T_37b51_row4_col3" class="data row4 col3" >0.780875</td>
     </tr>
   </tbody>
 </table>
 
 Now, we’ll use the
-[`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
+[`MonoDense`](https://airtai.github.io/monotonic-nn/monodenselayer.html#monodense)
 layer instead of `Dense` layer to build a simple monotonic network. By
 default, the
-[`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
+[`MonoDense`](https://airtai.github.io/monotonic-nn/monodenselayer.html#monodense)
 layer assumes the output of the layer is monotonically increasing with
 all inputs. This assumtion is always true for all layers except possibly
 the first one. For the first layer, we use `monotonicity_indicator` to
 specify which input parameters are monotonic and to specify are they
 increasingly or decreasingly monotonic:
 
 - set 1 for increasingly monotonic parameter,
 
 - set -1 for decreasingly monotonic parameter, and
 
 - set 0 otherwise.
 
 In our case, the `monotonicity_indicator` is `[1, 0, -1]` because $y$
-is: 
+is:
 
 - monotonically increasing w.r.t. $x_1$
-$\left(\frac{\partial y}{x_1} = 3 {x_1}^2 \geq 0\right)$, and
+  $\left(\frac{\partial y}{x_1} = 3 {x_1}^2 \geq 0\right)$, and
 
 - monotonically decreasing w.r.t. $x_3$
   $\left(\frac{\partial y}{x_3} = - e^{-x_2} \leq 0\right)$.
 
 ``` python
 from tensorflow.keras import Sequential
 from tensorflow.keras.layers import Dense, Input
```

#### html2text {}

```diff
@@ -1,63 +1,64 @@
-Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.0rc0 Summary: Monotonic
-Neural Networks Home-page: https://github.com/airtai/monotonic-nn Author: AIRT
-Technologies d.o.o. Author-email: info@airt.ai License: Creative Commons
-License Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
-Project-URL: CI, https://github.com/airtai/monotonic-nn/actions Project-URL:
-Documentation, https://monotonic.airt.ai/ Project-URL: Tutorial, https://
-colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb
-Keywords: tensorflow keras monotone "monotonic neural networks" "dense layer"
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Developers Classifier: Natural Language :: English Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: License :: Free for non-
-commercial use Requires-Python: >=3.8 Description-Content-Type: text/markdown
-Provides-Extra: dev Provides-Extra: experiments License-File: LICENSE
-Constrained Monotonic Neural Networks ================  This Python library
-implements Monotonic Dense Layer as described in Davor Runje, Sharath M.
-Shankaranarayana, âConstrained Monotonic Neural Networksâ \[[PDF](https://
-arxiv.org/pdf/2205.11775.pdf)\]. If you use this library, please cite: ```
+Constrained Monotonic Neural Networks ================  ## Running in Google
+Colab You can execute this interactive tutorial in Google Colab by clicking the
+button below: [Open_in_Colab] ## Summary This Python library implements
+Constrained Monotonic Neural Networks as described in: Davor Runje, Sharath M.
+Shankaranarayana, âConstrained Monotonic Neural Networksâ, in Proceedings
+of the 40th International Conference on Machine Learning, 2023. \[[PDF](https:/
+/arxiv.org/pdf/2205.11775.pdf)\]. #### Abstract Wider adoption of neural
+networks in many critical domains such as finance and healthcare is being
+hindered by the need to explain their predictions and to impose additional
+constraints on them. Monotonicity constraint is one of the most requested
+properties in real-world scenarios and is the focus of this paper. One of the
+oldest ways to construct a monotonic fully connected neural network is to
+constrain signs on its weights. Unfortunately, this construction does not work
+with popular non-saturated activation functions as it can only approximate
+convex functions. We show this shortcoming can be fixed by constructing two
+additional activation functions from a typical unsaturated monotonic activation
+function and employing each of them on the part of neurons. Our experiments
+show this approach of building monotonic neural networks has better accuracy
+when compared to other state-of-the-art methods, while being the simplest one
+in the sense of having the least number of parameters, and not requiring any
+modifications to the learning procedure or post-learning steps. Finally, we
+prove it can approximate any continuous monotone function on a compact subset
+of $\mathbb{R}^n$. #### Citation If you use this library, please cite: ```
 title="bibtex" @inproceedings{runje2023, title={Constrained Monotonic Neural
 Networks}, author={Davor Runje and Sharath M. Shankaranarayana}, booktitle=
 {Proceedings of the 40th {International Conference on Machine Learning}}, year=
-{2023} } ``` This package contains an implementation of our Monotonic Dense
-Layer [`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/
-MonoDense/#airt.keras.layers.MonoDense) (Constrained Monotonic Fully Connected
-Layer). Below is the figure from the paper for reference. In the code, the
-variable `monotonicity_indicator` corresponds to **t** in the figure and
-parameters `is_convex`, `is_concave` and `activation_weights` are used to
-calculate the activation selector **s** as follows: - if `is_convex` or
+{2023} } ``` ## Python package This package contains an implementation of our
+Monotonic Dense Layer [`MonoDense`](https://monotonic.airt.ai/0.3.0/api/airt/
+keras/layers/MonoDense/#airt.keras.layers.MonoDense) (Constrained Monotonic
+Fully Connected Layer). Below is the figure from the paper for reference. In
+the code, the variable `monotonicity_indicator` corresponds to **t** in the
+figure and parameters `is_convex`, `is_concave` and `activation_weights` are
+used to calculate the activation selector **s** as follows: - if `is_convex` or
 `is_concave` is **True**, then the activation selector **s** will be (`units`,
 0, 0) and (0, `units`, 0), respecively. - if both `is_convex` or `is_concave`
 is **False**, then the `activation_weights` represent ratios between $\breve
 {s}$, $\hat{s}$ and $\tilde{s}$, respecively. E.g. if `activation_weights = (2,
 2, 1)` and `units = 10`, then $$ (\breve{s}, \hat{s}, \tilde{s}) = (4, 4, 2) $$
-![mono-dense-layer-diagram](https://github.com/airtai/monotonic-nn/raw/main/
-nbs/images/mono-dense-layer-diagram.png) ## Running in Google Colab You can
-start this interactive tutorial in Google Colab by clicking the button below:
-[Open_in_Colab] ## Install ``` sh pip install monotonic-nn ``` ## How to use In
-this example, weâll assume we have a simple dataset with three inputs values
-$x_1$, $x_2$ and $x_3$ sampled from the normal distribution, while the output
-value $y$ is calculated according to the following formula before adding
-Gaussian noise to it: $y = x_1^3 + \sin\left(\frac{x_2}{2 \pi}\right) + e^{-
-x_3}$
+![mono-dense-layer-diagram](https://monotonic.airt.ai/0.3.0/api/airt/keras/
+layers/MonoDense/#airt.keras.layers.MonoDense) ### Install ``` sh pip install
+monotonic-nn ``` ### How to use In this example, weâll assume we have a
+simple dataset with three inputs values $x_1$, $x_2$ and $x_3$ sampled from the
+normal distribution, while the output value $y$ is calculated according to the
+following formula before adding Gaussian noise to it: $y = x_1^3 + \sin\left
+(\frac{x_2}{2 \pi}\right) + e^{-x_3}$
 x0        x1        x2        y
 0.304717  -1.039984 0.750451  0.234541
 0.940565  -1.951035 -1.302180 4.199094
 0.127840  -0.316243 -0.016801 0.834086
 -0.853044 0.879398  0.777792  -0.093359
 0.066031  1.127241  0.467509  0.780875
-Now, weâll use the [`MonoDense`](https://monotonic.airt.ai/latest/api/airt/
-keras/layers/MonoDense/#airt.keras.layers.MonoDense) layer instead of `Dense`
-layer to build a simple monotonic network. By default, the [`MonoDense`](https:
-//monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/
-#airt.keras.layers.MonoDense) layer assumes the output of the layer is
-monotonically increasing with all inputs. This assumtion is always true for all
-layers except possibly the first one. For the first layer, we use
+Now, weâll use the [`MonoDense`](https://airtai.github.io/monotonic-nn/
+monodenselayer.html#monodense) layer instead of `Dense` layer to build a simple
+monotonic network. By default, the [`MonoDense`](https://airtai.github.io/
+monotonic-nn/monodenselayer.html#monodense) layer assumes the output of the
+layer is monotonically increasing with all inputs. This assumtion is always
+true for all layers except possibly the first one. For the first layer, we use
 `monotonicity_indicator` to specify which input parameters are monotonic and to
 specify are they increasingly or decreasingly monotonic: - set 1 for
 increasingly monotonic parameter, - set -1 for decreasingly monotonic
 parameter, and - set 0 otherwise. In our case, the `monotonicity_indicator` is
 `[1, 0, -1]` because $y$ is: - monotonically increasing w.r.t. $x_1$ $\left
 (\frac{\partial y}{x_1} = 3 {x_1}^2 \geq 0\right)$, and - monotonically
 decreasing w.r.t. $x_3$ $\left(\frac{\partial y}{x_3} = - e^{-x_2} \leq
```

### Comparing `monotonic-nn-0.3.0rc0/README.md` & `monotonic-nn-0.3.1rc0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,95 @@
+Metadata-Version: 2.1
+Name: monotonic-nn
+Version: 0.3.1rc0
+Summary: Monotonic Neural Networks
+Home-page: https://github.com/airtai/monotonic-nn
+Author: AIRT Technologies d.o.o.
+Author-email: info@airt.ai
+License: Creative Commons License
+Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
+Project-URL: CI, https://github.com/airtai/monotonic-nn/actions
+Project-URL: Documentation, https://monotonic.airt.ai/
+Project-URL: Tutorial, https://colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb
+Keywords: tensorflow keras monotone "monotonic neural networks" "dense layer"
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: Free for non-commercial use
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: experiments
+License-File: LICENSE
+
 Constrained Monotonic Neural Networks
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-This Python library implements Monotonic Dense Layer as described in
+## Running in Google Colab
+
+You can execute this interactive tutorial in Google Colab by clicking
+the button below:
+
+<a href="https://colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb" target=”_blank”>
+<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab" />
+</a>
+
+## Summary
+
+This Python library implements Constrained Monotonic Neural Networks as
+described in:
+
 Davor Runje, Sharath M. Shankaranarayana, “Constrained Monotonic Neural
-Networks” \[[PDF](https://arxiv.org/pdf/2205.11775.pdf)\].
+Networks”, in Proceedings of the 40th International Conference on
+Machine Learning, 2023. \[[PDF](https://arxiv.org/pdf/2205.11775.pdf)\].
+
+#### Abstract
+
+Wider adoption of neural networks in many critical domains such as
+finance and healthcare is being hindered by the need to explain their
+predictions and to impose additional constraints on them. Monotonicity
+constraint is one of the most requested properties in real-world
+scenarios and is the focus of this paper. One of the oldest ways to
+construct a monotonic fully connected neural network is to constrain
+signs on its weights. Unfortunately, this construction does not work
+with popular non-saturated activation functions as it can only
+approximate convex functions. We show this shortcoming can be fixed by
+constructing two additional activation functions from a typical
+unsaturated monotonic activation function and employing each of them on
+the part of neurons. Our experiments show this approach of building
+monotonic neural networks has better accuracy when compared to other
+state-of-the-art methods, while being the simplest one in the sense of
+having the least number of parameters, and not requiring any
+modifications to the learning procedure or post-learning steps. Finally,
+we prove it can approximate any continuous monotone function on a
+compact subset of $\mathbb{R}^n$.
+
+#### Citation
 
 If you use this library, please cite:
 
 ``` title="bibtex"
 @inproceedings{runje2023,
   title={Constrained Monotonic Neural Networks},
   author={Davor Runje and Sharath M. Shankaranarayana},
   booktitle={Proceedings of the 40th {International Conference on Machine Learning}},
   year={2023}
 }
 ```
 
+## Python package
+
 This package contains an implementation of our Monotonic Dense Layer
-[`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
+[`MonoDense`](https://monotonic.airt.ai/0.3.0/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
 (Constrained Monotonic Fully Connected Layer). Below is the figure from
 the paper for reference.
 
 In the code, the variable `monotonicity_indicator` corresponds to **t**
 in the figure and parameters `is_convex`, `is_concave` and
 `activation_weights` are used to calculate the activation selector **s**
 as follows:
@@ -37,40 +103,33 @@
   and $\tilde{s}$, respecively. E.g. if `activation_weights = (2, 2, 1)`
   and `units = 10`, then
 
 $$
 (\breve{s}, \hat{s}, \tilde{s}) = (4, 4, 2)
 $$
 
-![mono-dense-layer-diagram](https://github.com/airtai/monotonic-nn/raw/main/nbs/images/mono-dense-layer-diagram.png)
-
-## Running in Google Colab
-
-You can start this interactive tutorial in Google Colab by clicking the
-button below:
-
-<a href="https://colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb" target=”_blank”>
-<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab" />
-</a>
+![mono-dense-layer-diagram](https://monotonic.airt.ai/0.3.0/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
 
-## Install
+### Install
 
 ``` sh
 pip install monotonic-nn
 ```
 
-## How to use
+### How to use
 
 In this example, we’ll assume we have a simple dataset with three inputs
 values $x_1$, $x_2$ and $x_3$ sampled from the normal distribution,
 while the output value $y$ is calculated according to the following
 formula before adding Gaussian noise to it:
 
 $y = x_1^3 + \sin\left(\frac{x_2}{2 \pi}\right) + e^{-x_3}$
 
+<style type="text/css">
+</style>
 <table id="T_37b51">
   <thead>
     <tr>
       <th id="T_37b51_level0_col0" class="col_heading level0 col0" >x0</th>
       <th id="T_37b51_level0_col1" class="col_heading level0 col1" >x1</th>
       <th id="T_37b51_level0_col2" class="col_heading level0 col2" >x2</th>
       <th id="T_37b51_level0_col3" class="col_heading level0 col3" >y</th>
@@ -107,35 +166,35 @@
       <td id="T_37b51_row4_col2" class="data row4 col2" >0.467509</td>
       <td id="T_37b51_row4_col3" class="data row4 col3" >0.780875</td>
     </tr>
   </tbody>
 </table>
 
 Now, we’ll use the
-[`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
+[`MonoDense`](https://airtai.github.io/monotonic-nn/monodenselayer.html#monodense)
 layer instead of `Dense` layer to build a simple monotonic network. By
 default, the
-[`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
+[`MonoDense`](https://airtai.github.io/monotonic-nn/monodenselayer.html#monodense)
 layer assumes the output of the layer is monotonically increasing with
 all inputs. This assumtion is always true for all layers except possibly
 the first one. For the first layer, we use `monotonicity_indicator` to
 specify which input parameters are monotonic and to specify are they
 increasingly or decreasingly monotonic:
 
 - set 1 for increasingly monotonic parameter,
 
 - set -1 for decreasingly monotonic parameter, and
 
 - set 0 otherwise.
 
 In our case, the `monotonicity_indicator` is `[1, 0, -1]` because $y$
-is: 
+is:
 
 - monotonically increasing w.r.t. $x_1$
-$\left(\frac{\partial y}{x_1} = 3 {x_1}^2 \geq 0\right)$, and
+  $\left(\frac{\partial y}{x_1} = 3 {x_1}^2 \geq 0\right)$, and
 
 - monotonically decreasing w.r.t. $x_3$
   $\left(\frac{\partial y}{x_3} = - e^{-x_2} \leq 0\right)$.
 
 ``` python
 from tensorflow.keras import Sequential
 from tensorflow.keras.layers import Dense, Input
```

#### html2text {}

```diff
@@ -1,48 +1,79 @@
-Constrained Monotonic Neural Networks ================  This Python library
-implements Monotonic Dense Layer as described in Davor Runje, Sharath M.
-Shankaranarayana, âConstrained Monotonic Neural Networksâ \[[PDF](https://
-arxiv.org/pdf/2205.11775.pdf)\]. If you use this library, please cite: ```
+Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.1rc0 Summary: Monotonic
+Neural Networks Home-page: https://github.com/airtai/monotonic-nn Author: AIRT
+Technologies d.o.o. Author-email: info@airt.ai License: Creative Commons
+License Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
+Project-URL: CI, https://github.com/airtai/monotonic-nn/actions Project-URL:
+Documentation, https://monotonic.airt.ai/ Project-URL: Tutorial, https://
+colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb
+Keywords: tensorflow keras monotone "monotonic neural networks" "dense layer"
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: Natural Language :: English Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: License :: Free for non-
+commercial use Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: experiments License-File: LICENSE
+Constrained Monotonic Neural Networks ================  ## Running in Google
+Colab You can execute this interactive tutorial in Google Colab by clicking the
+button below: [Open_in_Colab] ## Summary This Python library implements
+Constrained Monotonic Neural Networks as described in: Davor Runje, Sharath M.
+Shankaranarayana, âConstrained Monotonic Neural Networksâ, in Proceedings
+of the 40th International Conference on Machine Learning, 2023. \[[PDF](https:/
+/arxiv.org/pdf/2205.11775.pdf)\]. #### Abstract Wider adoption of neural
+networks in many critical domains such as finance and healthcare is being
+hindered by the need to explain their predictions and to impose additional
+constraints on them. Monotonicity constraint is one of the most requested
+properties in real-world scenarios and is the focus of this paper. One of the
+oldest ways to construct a monotonic fully connected neural network is to
+constrain signs on its weights. Unfortunately, this construction does not work
+with popular non-saturated activation functions as it can only approximate
+convex functions. We show this shortcoming can be fixed by constructing two
+additional activation functions from a typical unsaturated monotonic activation
+function and employing each of them on the part of neurons. Our experiments
+show this approach of building monotonic neural networks has better accuracy
+when compared to other state-of-the-art methods, while being the simplest one
+in the sense of having the least number of parameters, and not requiring any
+modifications to the learning procedure or post-learning steps. Finally, we
+prove it can approximate any continuous monotone function on a compact subset
+of $\mathbb{R}^n$. #### Citation If you use this library, please cite: ```
 title="bibtex" @inproceedings{runje2023, title={Constrained Monotonic Neural
 Networks}, author={Davor Runje and Sharath M. Shankaranarayana}, booktitle=
 {Proceedings of the 40th {International Conference on Machine Learning}}, year=
-{2023} } ``` This package contains an implementation of our Monotonic Dense
-Layer [`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/
-MonoDense/#airt.keras.layers.MonoDense) (Constrained Monotonic Fully Connected
-Layer). Below is the figure from the paper for reference. In the code, the
-variable `monotonicity_indicator` corresponds to **t** in the figure and
-parameters `is_convex`, `is_concave` and `activation_weights` are used to
-calculate the activation selector **s** as follows: - if `is_convex` or
+{2023} } ``` ## Python package This package contains an implementation of our
+Monotonic Dense Layer [`MonoDense`](https://monotonic.airt.ai/0.3.0/api/airt/
+keras/layers/MonoDense/#airt.keras.layers.MonoDense) (Constrained Monotonic
+Fully Connected Layer). Below is the figure from the paper for reference. In
+the code, the variable `monotonicity_indicator` corresponds to **t** in the
+figure and parameters `is_convex`, `is_concave` and `activation_weights` are
+used to calculate the activation selector **s** as follows: - if `is_convex` or
 `is_concave` is **True**, then the activation selector **s** will be (`units`,
 0, 0) and (0, `units`, 0), respecively. - if both `is_convex` or `is_concave`
 is **False**, then the `activation_weights` represent ratios between $\breve
 {s}$, $\hat{s}$ and $\tilde{s}$, respecively. E.g. if `activation_weights = (2,
 2, 1)` and `units = 10`, then $$ (\breve{s}, \hat{s}, \tilde{s}) = (4, 4, 2) $$
-![mono-dense-layer-diagram](https://github.com/airtai/monotonic-nn/raw/main/
-nbs/images/mono-dense-layer-diagram.png) ## Running in Google Colab You can
-start this interactive tutorial in Google Colab by clicking the button below:
-[Open_in_Colab] ## Install ``` sh pip install monotonic-nn ``` ## How to use In
-this example, weâll assume we have a simple dataset with three inputs values
-$x_1$, $x_2$ and $x_3$ sampled from the normal distribution, while the output
-value $y$ is calculated according to the following formula before adding
-Gaussian noise to it: $y = x_1^3 + \sin\left(\frac{x_2}{2 \pi}\right) + e^{-
-x_3}$
+![mono-dense-layer-diagram](https://monotonic.airt.ai/0.3.0/api/airt/keras/
+layers/MonoDense/#airt.keras.layers.MonoDense) ### Install ``` sh pip install
+monotonic-nn ``` ### How to use In this example, weâll assume we have a
+simple dataset with three inputs values $x_1$, $x_2$ and $x_3$ sampled from the
+normal distribution, while the output value $y$ is calculated according to the
+following formula before adding Gaussian noise to it: $y = x_1^3 + \sin\left
+(\frac{x_2}{2 \pi}\right) + e^{-x_3}$
 x0        x1        x2        y
 0.304717  -1.039984 0.750451  0.234541
 0.940565  -1.951035 -1.302180 4.199094
 0.127840  -0.316243 -0.016801 0.834086
 -0.853044 0.879398  0.777792  -0.093359
 0.066031  1.127241  0.467509  0.780875
-Now, weâll use the [`MonoDense`](https://monotonic.airt.ai/latest/api/airt/
-keras/layers/MonoDense/#airt.keras.layers.MonoDense) layer instead of `Dense`
-layer to build a simple monotonic network. By default, the [`MonoDense`](https:
-//monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/
-#airt.keras.layers.MonoDense) layer assumes the output of the layer is
-monotonically increasing with all inputs. This assumtion is always true for all
-layers except possibly the first one. For the first layer, we use
+Now, weâll use the [`MonoDense`](https://airtai.github.io/monotonic-nn/
+monodenselayer.html#monodense) layer instead of `Dense` layer to build a simple
+monotonic network. By default, the [`MonoDense`](https://airtai.github.io/
+monotonic-nn/monodenselayer.html#monodense) layer assumes the output of the
+layer is monotonically increasing with all inputs. This assumtion is always
+true for all layers except possibly the first one. For the first layer, we use
 `monotonicity_indicator` to specify which input parameters are monotonic and to
 specify are they increasingly or decreasingly monotonic: - set 1 for
 increasingly monotonic parameter, - set -1 for decreasingly monotonic
 parameter, and - set 0 otherwise. In our case, the `monotonicity_indicator` is
 `[1, 0, -1]` because $y$ is: - monotonically increasing w.r.t. $x_1$ $\left
 (\frac{\partial y}{x_1} = 3 {x_1}^2 \geq 0\right)$, and - monotonically
 decreasing w.r.t. $x_3$ $\left(\frac{\partial y}{x_3} = - e^{-x_2} \leq
```

### Comparing `monotonic-nn-0.3.0rc0/airt/_components/mono_dense_layer.py` & `monotonic-nn-0.3.1rc0/airt/_components/mono_dense_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         - if both  `is_convex` or `is_concave` is **False**, then the `activation_weights` represent ratios between $\\breve{s}$, $\\hat{s}$ and $\\tilde{s}$,
           respecively. E.g. if `activation_weights = (2, 2, 1)` and `units = 10`, then
 
     $$
     (\\breve{s}, \\hat{s}, \\tilde{s}) = (4, 4, 2)
     $$
 
-    ![mono-dense-layer-diagram.png](../../../images/nbs/images/mono-dense-layer-diagram.png)
+    ![mono-dense-layer-diagram.png](../../../../../images/nbs/images/mono-dense-layer-diagram.png)
 
     """
 
     def __init__(
         self,
         units: int,
         *,
```

### Comparing `monotonic-nn-0.3.0rc0/airt/_modidx.py` & `monotonic-nn-0.3.1rc0/airt/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,24 +36,24 @@
                                                                                                                    'airt/_components/mono_dense_layer.py'),
                                                    'airt._components.mono_dense_layer.get_monotonicity_indicator': ( 'monodenselayer.html#get_monotonicity_indicator',
                                                                                                                      'airt/_components/mono_dense_layer.py'),
                                                    'airt._components.mono_dense_layer.get_saturated_activation': ( 'monodenselayer.html#get_saturated_activation',
                                                                                                                    'airt/_components/mono_dense_layer.py'),
                                                    'airt._components.mono_dense_layer.replace_kernel_using_monotonicity_indicator': ( 'monodenselayer.html#replace_kernel_using_monotonicity_indicator',
                                                                                                                                       'airt/_components/mono_dense_layer.py')},
-            'airt.keras.experiments': { 'airt.keras.experiments.TestHyperModel': ( 'experiments.html#testhypermodel',
-                                                                                   'airt/keras/experiments.py'),
-                                        'airt.keras.experiments.TestHyperModel.__init__': ( 'experiments.html#testhypermodel.__init__',
-                                                                                            'airt/keras/experiments.py'),
-                                        'airt.keras.experiments.TestHyperModel.build': ( 'experiments.html#testhypermodel.build',
-                                                                                         'airt/keras/experiments.py'),
-                                        'airt.keras.experiments._DownloadProgressBar': ( 'experiments.html#_downloadprogressbar',
+            'airt.keras.experiments': { 'airt.keras.experiments._DownloadProgressBar': ( 'experiments.html#_downloadprogressbar',
                                                                                          'airt/keras/experiments.py'),
                                         'airt.keras.experiments._DownloadProgressBar.update_to': ( 'experiments.html#_downloadprogressbar.update_to',
                                                                                                    'airt/keras/experiments.py'),
+                                        'airt.keras.experiments._TestHyperModel': ( 'experiments.html#_testhypermodel',
+                                                                                    'airt/keras/experiments.py'),
+                                        'airt.keras.experiments._TestHyperModel.__init__': ( 'experiments.html#_testhypermodel.__init__',
+                                                                                             'airt/keras/experiments.py'),
+                                        'airt.keras.experiments._TestHyperModel.build': ( 'experiments.html#_testhypermodel.build',
+                                                                                          'airt/keras/experiments.py'),
                                         'airt.keras.experiments._build_mono_model_f': ( 'experiments.html#_build_mono_model_f',
                                                                                         'airt/keras/experiments.py'),
                                         'airt.keras.experiments._count_model_params': ( 'experiments.html#_count_model_params',
                                                                                         'airt/keras/experiments.py'),
                                         'airt.keras.experiments._create_model_stats': ( 'experiments.html#_create_model_stats',
                                                                                         'airt/keras/experiments.py'),
                                         'airt.keras.experiments._download_data': ( 'experiments.html#_download_data',
```

### Comparing `monotonic-nn-0.3.0rc0/airt/keras/experiments.py` & `monotonic-nn-0.3.1rc0/airt/keras/experiments.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         default_kwargs.update(**override_kwargs)
         model = build_model_f(**default_kwargs, **kwargs)
         return model
 
     return build_model_with_hp_f
 
 
-class TestHyperModel(HyperModel):
+class _TestHyperModel(HyperModel):
     def __init__(self, **kwargs: Any):
         self.kwargs = kwargs
 
     def build(self, hp: HyperParameters) -> Model:
         build_model_with_hp_f = _get_build_model_with_hp_f(
             _build_mono_model_f, **self.kwargs  # type: ignore
         )
@@ -279,15 +279,15 @@
 
     """
     tf.keras.utils.set_random_seed(seed)
 
     train_df, test_df = get_train_n_test_data(dataset_name)
     train_ds, test_ds = df2ds(train_df), df2ds(test_df)
 
-    oracle = TestHyperModel(
+    oracle = _TestHyperModel(
         monotonicity_indicator=monotonicity_indicator,
         hp_params_f=hp_params_f,
         final_activation=final_activation,
         loss=loss,
         metrics=metrics,
         train_ds=train_ds,
         batch_size=batch_size,
```

### Comparing `monotonic-nn-0.3.0rc0/monotonic_nn.egg-info/PKG-INFO` & `monotonic-nn-0.3.1rc0/monotonic_nn.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monotonic-nn
-Version: 0.3.0rc0
+Version: 0.3.1rc0
 Summary: Monotonic Neural Networks
 Home-page: https://github.com/airtai/monotonic-nn
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
 Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions
@@ -26,31 +26,70 @@
 License-File: LICENSE
 
 Constrained Monotonic Neural Networks
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-This Python library implements Monotonic Dense Layer as described in
+## Running in Google Colab
+
+You can execute this interactive tutorial in Google Colab by clicking
+the button below:
+
+<a href="https://colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb" target=”_blank”>
+<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab" />
+</a>
+
+## Summary
+
+This Python library implements Constrained Monotonic Neural Networks as
+described in:
+
 Davor Runje, Sharath M. Shankaranarayana, “Constrained Monotonic Neural
-Networks” \[[PDF](https://arxiv.org/pdf/2205.11775.pdf)\].
+Networks”, in Proceedings of the 40th International Conference on
+Machine Learning, 2023. \[[PDF](https://arxiv.org/pdf/2205.11775.pdf)\].
+
+#### Abstract
+
+Wider adoption of neural networks in many critical domains such as
+finance and healthcare is being hindered by the need to explain their
+predictions and to impose additional constraints on them. Monotonicity
+constraint is one of the most requested properties in real-world
+scenarios and is the focus of this paper. One of the oldest ways to
+construct a monotonic fully connected neural network is to constrain
+signs on its weights. Unfortunately, this construction does not work
+with popular non-saturated activation functions as it can only
+approximate convex functions. We show this shortcoming can be fixed by
+constructing two additional activation functions from a typical
+unsaturated monotonic activation function and employing each of them on
+the part of neurons. Our experiments show this approach of building
+monotonic neural networks has better accuracy when compared to other
+state-of-the-art methods, while being the simplest one in the sense of
+having the least number of parameters, and not requiring any
+modifications to the learning procedure or post-learning steps. Finally,
+we prove it can approximate any continuous monotone function on a
+compact subset of $\mathbb{R}^n$.
+
+#### Citation
 
 If you use this library, please cite:
 
 ``` title="bibtex"
 @inproceedings{runje2023,
   title={Constrained Monotonic Neural Networks},
   author={Davor Runje and Sharath M. Shankaranarayana},
   booktitle={Proceedings of the 40th {International Conference on Machine Learning}},
   year={2023}
 }
 ```
 
+## Python package
+
 This package contains an implementation of our Monotonic Dense Layer
-[`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
+[`MonoDense`](https://monotonic.airt.ai/0.3.0/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
 (Constrained Monotonic Fully Connected Layer). Below is the figure from
 the paper for reference.
 
 In the code, the variable `monotonicity_indicator` corresponds to **t**
 in the figure and parameters `is_convex`, `is_concave` and
 `activation_weights` are used to calculate the activation selector **s**
 as follows:
@@ -64,40 +103,33 @@
   and $\tilde{s}$, respecively. E.g. if `activation_weights = (2, 2, 1)`
   and `units = 10`, then
 
 $$
 (\breve{s}, \hat{s}, \tilde{s}) = (4, 4, 2)
 $$
 
-![mono-dense-layer-diagram](https://github.com/airtai/monotonic-nn/raw/main/nbs/images/mono-dense-layer-diagram.png)
-
-## Running in Google Colab
-
-You can start this interactive tutorial in Google Colab by clicking the
-button below:
-
-<a href="https://colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb" target=”_blank”>
-<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab" />
-</a>
+![mono-dense-layer-diagram](https://monotonic.airt.ai/0.3.0/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
 
-## Install
+### Install
 
 ``` sh
 pip install monotonic-nn
 ```
 
-## How to use
+### How to use
 
 In this example, we’ll assume we have a simple dataset with three inputs
 values $x_1$, $x_2$ and $x_3$ sampled from the normal distribution,
 while the output value $y$ is calculated according to the following
 formula before adding Gaussian noise to it:
 
 $y = x_1^3 + \sin\left(\frac{x_2}{2 \pi}\right) + e^{-x_3}$
 
+<style type="text/css">
+</style>
 <table id="T_37b51">
   <thead>
     <tr>
       <th id="T_37b51_level0_col0" class="col_heading level0 col0" >x0</th>
       <th id="T_37b51_level0_col1" class="col_heading level0 col1" >x1</th>
       <th id="T_37b51_level0_col2" class="col_heading level0 col2" >x2</th>
       <th id="T_37b51_level0_col3" class="col_heading level0 col3" >y</th>
@@ -134,35 +166,35 @@
       <td id="T_37b51_row4_col2" class="data row4 col2" >0.467509</td>
       <td id="T_37b51_row4_col3" class="data row4 col3" >0.780875</td>
     </tr>
   </tbody>
 </table>
 
 Now, we’ll use the
-[`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
+[`MonoDense`](https://airtai.github.io/monotonic-nn/monodenselayer.html#monodense)
 layer instead of `Dense` layer to build a simple monotonic network. By
 default, the
-[`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
+[`MonoDense`](https://airtai.github.io/monotonic-nn/monodenselayer.html#monodense)
 layer assumes the output of the layer is monotonically increasing with
 all inputs. This assumtion is always true for all layers except possibly
 the first one. For the first layer, we use `monotonicity_indicator` to
 specify which input parameters are monotonic and to specify are they
 increasingly or decreasingly monotonic:
 
 - set 1 for increasingly monotonic parameter,
 
 - set -1 for decreasingly monotonic parameter, and
 
 - set 0 otherwise.
 
 In our case, the `monotonicity_indicator` is `[1, 0, -1]` because $y$
-is: 
+is:
 
 - monotonically increasing w.r.t. $x_1$
-$\left(\frac{\partial y}{x_1} = 3 {x_1}^2 \geq 0\right)$, and
+  $\left(\frac{\partial y}{x_1} = 3 {x_1}^2 \geq 0\right)$, and
 
 - monotonically decreasing w.r.t. $x_3$
   $\left(\frac{\partial y}{x_3} = - e^{-x_2} \leq 0\right)$.
 
 ``` python
 from tensorflow.keras import Sequential
 from tensorflow.keras.layers import Dense, Input
```

#### html2text {}

```diff
@@ -1,63 +1,79 @@
-Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.0rc0 Summary: Monotonic
+Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.1rc0 Summary: Monotonic
 Neural Networks Home-page: https://github.com/airtai/monotonic-nn Author: AIRT
 Technologies d.o.o. Author-email: info@airt.ai License: Creative Commons
 License Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions Project-URL:
 Documentation, https://monotonic.airt.ai/ Project-URL: Tutorial, https://
 colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb
 Keywords: tensorflow keras monotone "monotonic neural networks" "dense layer"
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: License :: Free for non-
 commercial use Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Provides-Extra: dev Provides-Extra: experiments License-File: LICENSE
-Constrained Monotonic Neural Networks ================  This Python library
-implements Monotonic Dense Layer as described in Davor Runje, Sharath M.
-Shankaranarayana, âConstrained Monotonic Neural Networksâ \[[PDF](https://
-arxiv.org/pdf/2205.11775.pdf)\]. If you use this library, please cite: ```
+Constrained Monotonic Neural Networks ================  ## Running in Google
+Colab You can execute this interactive tutorial in Google Colab by clicking the
+button below: [Open_in_Colab] ## Summary This Python library implements
+Constrained Monotonic Neural Networks as described in: Davor Runje, Sharath M.
+Shankaranarayana, âConstrained Monotonic Neural Networksâ, in Proceedings
+of the 40th International Conference on Machine Learning, 2023. \[[PDF](https:/
+/arxiv.org/pdf/2205.11775.pdf)\]. #### Abstract Wider adoption of neural
+networks in many critical domains such as finance and healthcare is being
+hindered by the need to explain their predictions and to impose additional
+constraints on them. Monotonicity constraint is one of the most requested
+properties in real-world scenarios and is the focus of this paper. One of the
+oldest ways to construct a monotonic fully connected neural network is to
+constrain signs on its weights. Unfortunately, this construction does not work
+with popular non-saturated activation functions as it can only approximate
+convex functions. We show this shortcoming can be fixed by constructing two
+additional activation functions from a typical unsaturated monotonic activation
+function and employing each of them on the part of neurons. Our experiments
+show this approach of building monotonic neural networks has better accuracy
+when compared to other state-of-the-art methods, while being the simplest one
+in the sense of having the least number of parameters, and not requiring any
+modifications to the learning procedure or post-learning steps. Finally, we
+prove it can approximate any continuous monotone function on a compact subset
+of $\mathbb{R}^n$. #### Citation If you use this library, please cite: ```
 title="bibtex" @inproceedings{runje2023, title={Constrained Monotonic Neural
 Networks}, author={Davor Runje and Sharath M. Shankaranarayana}, booktitle=
 {Proceedings of the 40th {International Conference on Machine Learning}}, year=
-{2023} } ``` This package contains an implementation of our Monotonic Dense
-Layer [`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/
-MonoDense/#airt.keras.layers.MonoDense) (Constrained Monotonic Fully Connected
-Layer). Below is the figure from the paper for reference. In the code, the
-variable `monotonicity_indicator` corresponds to **t** in the figure and
-parameters `is_convex`, `is_concave` and `activation_weights` are used to
-calculate the activation selector **s** as follows: - if `is_convex` or
+{2023} } ``` ## Python package This package contains an implementation of our
+Monotonic Dense Layer [`MonoDense`](https://monotonic.airt.ai/0.3.0/api/airt/
+keras/layers/MonoDense/#airt.keras.layers.MonoDense) (Constrained Monotonic
+Fully Connected Layer). Below is the figure from the paper for reference. In
+the code, the variable `monotonicity_indicator` corresponds to **t** in the
+figure and parameters `is_convex`, `is_concave` and `activation_weights` are
+used to calculate the activation selector **s** as follows: - if `is_convex` or
 `is_concave` is **True**, then the activation selector **s** will be (`units`,
 0, 0) and (0, `units`, 0), respecively. - if both `is_convex` or `is_concave`
 is **False**, then the `activation_weights` represent ratios between $\breve
 {s}$, $\hat{s}$ and $\tilde{s}$, respecively. E.g. if `activation_weights = (2,
 2, 1)` and `units = 10`, then $$ (\breve{s}, \hat{s}, \tilde{s}) = (4, 4, 2) $$
-![mono-dense-layer-diagram](https://github.com/airtai/monotonic-nn/raw/main/
-nbs/images/mono-dense-layer-diagram.png) ## Running in Google Colab You can
-start this interactive tutorial in Google Colab by clicking the button below:
-[Open_in_Colab] ## Install ``` sh pip install monotonic-nn ``` ## How to use In
-this example, weâll assume we have a simple dataset with three inputs values
-$x_1$, $x_2$ and $x_3$ sampled from the normal distribution, while the output
-value $y$ is calculated according to the following formula before adding
-Gaussian noise to it: $y = x_1^3 + \sin\left(\frac{x_2}{2 \pi}\right) + e^{-
-x_3}$
+![mono-dense-layer-diagram](https://monotonic.airt.ai/0.3.0/api/airt/keras/
+layers/MonoDense/#airt.keras.layers.MonoDense) ### Install ``` sh pip install
+monotonic-nn ``` ### How to use In this example, weâll assume we have a
+simple dataset with three inputs values $x_1$, $x_2$ and $x_3$ sampled from the
+normal distribution, while the output value $y$ is calculated according to the
+following formula before adding Gaussian noise to it: $y = x_1^3 + \sin\left
+(\frac{x_2}{2 \pi}\right) + e^{-x_3}$
 x0        x1        x2        y
 0.304717  -1.039984 0.750451  0.234541
 0.940565  -1.951035 -1.302180 4.199094
 0.127840  -0.316243 -0.016801 0.834086
 -0.853044 0.879398  0.777792  -0.093359
 0.066031  1.127241  0.467509  0.780875
-Now, weâll use the [`MonoDense`](https://monotonic.airt.ai/latest/api/airt/
-keras/layers/MonoDense/#airt.keras.layers.MonoDense) layer instead of `Dense`
-layer to build a simple monotonic network. By default, the [`MonoDense`](https:
-//monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/
-#airt.keras.layers.MonoDense) layer assumes the output of the layer is
-monotonically increasing with all inputs. This assumtion is always true for all
-layers except possibly the first one. For the first layer, we use
+Now, weâll use the [`MonoDense`](https://airtai.github.io/monotonic-nn/
+monodenselayer.html#monodense) layer instead of `Dense` layer to build a simple
+monotonic network. By default, the [`MonoDense`](https://airtai.github.io/
+monotonic-nn/monodenselayer.html#monodense) layer assumes the output of the
+layer is monotonically increasing with all inputs. This assumtion is always
+true for all layers except possibly the first one. For the first layer, we use
 `monotonicity_indicator` to specify which input parameters are monotonic and to
 specify are they increasingly or decreasingly monotonic: - set 1 for
 increasingly monotonic parameter, - set -1 for decreasingly monotonic
 parameter, and - set 0 otherwise. In our case, the `monotonicity_indicator` is
 `[1, 0, -1]` because $y$ is: - monotonically increasing w.r.t. $x_1$ $\left
 (\frac{\partial y}{x_1} = 3 {x_1}^2 \geq 0\right)$, and - monotonically
 decreasing w.r.t. $x_3$ $\left(\frac{\partial y}{x_3} = - e^{-x_2} \leq
```

### Comparing `monotonic-nn-0.3.0rc0/settings.ini` & `monotonic-nn-0.3.1rc0/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = monotonic-nn
 lib_name = %(repo)s
-version = 0.3.0rc0
+version = 0.3.1rc0
 min_python = 3.8
 license = cc
 
 ### nbdev ###
 doc_path = _docs
 lib_path = airt
 nbs_path = nbs
```

### Comparing `monotonic-nn-0.3.0rc0/setup.py` & `monotonic-nn-0.3.1rc0/setup.py`

 * *Files identical despite different names*

