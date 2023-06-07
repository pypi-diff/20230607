# Comparing `tmp/openvalidators-1.0.1.tar.gz` & `tmp/openvalidators-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openvalidators-1.0.1.tar", last modified: Wed Jun  7 17:40:29 2023, max compression
+gzip compressed data, was "openvalidators-1.0.2.tar", last modified: Wed Jun  7 20:01:13 2023, max compression
```

## Comparing `openvalidators-1.0.1.tar` & `openvalidators-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-07 17:40:29.243407 openvalidators-1.0.1/
--rw-r--r--   0 pedroferreira   (501) staff       (20)     1087 2023-06-05 21:08:43.000000 openvalidators-1.0.1/LICENSE
--rw-r--r--   0 pedroferreira   (501) staff       (20)     8951 2023-06-07 17:40:29.243276 openvalidators-1.0.1/PKG-INFO
--rw-r--r--   0 pedroferreira   (501) staff       (20)     7757 2023-06-06 18:34:54.000000 openvalidators-1.0.1/README.md
-drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-07 17:40:29.242505 openvalidators-1.0.1/openvalidators/
--rw-r--r--   0 pedroferreira   (501) staff       (20)     1403 2023-06-07 17:39:54.000000 openvalidators-1.0.1/openvalidators/__init__.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     8831 2023-06-07 17:39:54.000000 openvalidators-1.0.1/openvalidators/config.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     4366 2023-06-06 18:32:40.000000 openvalidators-1.0.1/openvalidators/dendrite.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)    16781 2023-06-07 17:39:54.000000 openvalidators-1.0.1/openvalidators/forward.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)    13620 2023-06-06 18:32:40.000000 openvalidators-1.0.1/openvalidators/gating.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     2029 2023-06-05 21:08:43.000000 openvalidators-1.0.1/openvalidators/misc.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     3557 2023-06-06 18:32:40.000000 openvalidators-1.0.1/openvalidators/mock.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     6977 2023-06-07 13:42:52.000000 openvalidators-1.0.1/openvalidators/neuron.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)    10885 2023-06-06 18:32:40.000000 openvalidators-1.0.1/openvalidators/prompts.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     7927 2023-06-06 18:32:40.000000 openvalidators-1.0.1/openvalidators/reward.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     2547 2023-06-07 13:42:52.000000 openvalidators-1.0.1/openvalidators/run.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     9413 2023-06-07 17:39:54.000000 openvalidators-1.0.1/openvalidators/utils.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     2912 2023-06-07 17:39:54.000000 openvalidators-1.0.1/openvalidators/weights.py
-drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-07 17:40:29.243115 openvalidators-1.0.1/openvalidators.egg-info/
--rw-r--r--   0 pedroferreira   (501) staff       (20)     8951 2023-06-07 17:40:29.000000 openvalidators-1.0.1/openvalidators.egg-info/PKG-INFO
--rw-r--r--   0 pedroferreira   (501) staff       (20)      580 2023-06-07 17:40:29.000000 openvalidators-1.0.1/openvalidators.egg-info/SOURCES.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)        1 2023-06-07 17:40:29.000000 openvalidators-1.0.1/openvalidators.egg-info/dependency_links.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)       68 2023-06-07 17:40:29.000000 openvalidators-1.0.1/openvalidators.egg-info/entry_points.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)      143 2023-06-07 17:40:29.000000 openvalidators-1.0.1/openvalidators.egg-info/requires.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)       15 2023-06-07 17:40:29.000000 openvalidators-1.0.1/openvalidators.egg-info/top_level.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)       38 2023-06-07 17:40:29.243440 openvalidators-1.0.1/setup.cfg
--rw-r--r--   0 pedroferreira   (501) staff       (20)     3496 2023-06-06 18:47:52.000000 openvalidators-1.0.1/setup.py
+drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-07 20:01:13.358997 openvalidators-1.0.2/
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     1087 2023-06-05 21:08:43.000000 openvalidators-1.0.2/LICENSE
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     8971 2023-06-07 20:01:13.358866 openvalidators-1.0.2/PKG-INFO
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     7757 2023-06-06 18:34:54.000000 openvalidators-1.0.2/README.md
+drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-07 20:01:13.357876 openvalidators-1.0.2/openvalidators/
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     1403 2023-06-07 20:00:55.000000 openvalidators-1.0.2/openvalidators/__init__.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     8831 2023-06-07 17:58:23.000000 openvalidators-1.0.2/openvalidators/config.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     4366 2023-06-06 18:32:40.000000 openvalidators-1.0.2/openvalidators/dendrite.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)    16781 2023-06-07 20:00:41.000000 openvalidators-1.0.2/openvalidators/forward.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)    13620 2023-06-06 18:32:40.000000 openvalidators-1.0.2/openvalidators/gating.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     2029 2023-06-05 21:08:43.000000 openvalidators-1.0.2/openvalidators/misc.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     3557 2023-06-06 18:32:40.000000 openvalidators-1.0.2/openvalidators/mock.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     6977 2023-06-07 13:42:52.000000 openvalidators-1.0.2/openvalidators/neuron.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)    10885 2023-06-06 18:32:40.000000 openvalidators-1.0.2/openvalidators/prompts.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     7927 2023-06-06 18:32:40.000000 openvalidators-1.0.2/openvalidators/reward.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     2547 2023-06-07 13:42:52.000000 openvalidators-1.0.2/openvalidators/run.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     9418 2023-06-07 20:00:41.000000 openvalidators-1.0.2/openvalidators/utils.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     2912 2023-06-07 17:58:23.000000 openvalidators-1.0.2/openvalidators/weights.py
+drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-07 20:01:13.358692 openvalidators-1.0.2/openvalidators.egg-info/
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     8971 2023-06-07 20:01:13.000000 openvalidators-1.0.2/openvalidators.egg-info/PKG-INFO
+-rw-r--r--   0 pedroferreira   (501) staff       (20)      580 2023-06-07 20:01:13.000000 openvalidators-1.0.2/openvalidators.egg-info/SOURCES.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)        1 2023-06-07 20:01:13.000000 openvalidators-1.0.2/openvalidators.egg-info/dependency_links.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)       69 2023-06-07 20:01:13.000000 openvalidators-1.0.2/openvalidators.egg-info/entry_points.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)      143 2023-06-07 20:01:13.000000 openvalidators-1.0.2/openvalidators.egg-info/requires.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)       15 2023-06-07 20:01:13.000000 openvalidators-1.0.2/openvalidators.egg-info/top_level.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)       38 2023-06-07 20:01:13.359037 openvalidators-1.0.2/setup.cfg
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     3496 2023-06-06 18:47:52.000000 openvalidators-1.0.2/setup.py
```

### Comparing `openvalidators-1.0.1/LICENSE` & `openvalidators-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.1/PKG-INFO` & `openvalidators-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: openvalidators
-Version: 1.0.1
+Version: 1.0.2
 Summary: Openvalidators is a collection of open source validators for the Bittensor Network.
 Home-page: https://github.com/opentensor/validators
 Author: bittensor.com
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: MIT
 Keywords: bittensor,validator,ai,machine-learning,deep-learning,blockchain,pytorch,torch,neural-networks,cryptocurrency
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -158,7 +159,9 @@
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE 
 WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+
```

### Comparing `openvalidators-1.0.1/README.md` & `openvalidators-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.1/openvalidators/__init__.py` & `openvalidators-1.0.2/openvalidators/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,9 +23,9 @@
 from . import neuron
 from . import prompts
 from . import reward
 from . import run
 from . import utils
 from . import weights
 
-__version__ = "1.0.1"
-__spec_version__ = 1002
+__version__ = "1.0.2"
+__spec_version__ = 1003
```

### Comparing `openvalidators-1.0.1/openvalidators/config.py` & `openvalidators-1.0.2/openvalidators/config.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.1/openvalidators/dendrite.py` & `openvalidators-1.0.2/openvalidators/dendrite.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.1/openvalidators/forward.py` & `openvalidators-1.0.2/openvalidators/forward.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.1/openvalidators/gating.py` & `openvalidators-1.0.2/openvalidators/gating.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.1/openvalidators/misc.py` & `openvalidators-1.0.2/openvalidators/misc.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.1/openvalidators/mock.py` & `openvalidators-1.0.2/openvalidators/mock.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.1/openvalidators/neuron.py` & `openvalidators-1.0.2/openvalidators/neuron.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.1/openvalidators/prompts.py` & `openvalidators-1.0.2/openvalidators/prompts.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.1/openvalidators/reward.py` & `openvalidators-1.0.2/openvalidators/reward.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.1/openvalidators/run.py` & `openvalidators-1.0.2/openvalidators/run.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.1/openvalidators/utils.py` & `openvalidators-1.0.2/openvalidators/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 def should_reinit_wandb(self):
     # Check if wandb run needs to be rolled over.
     return not self.config.wandb.off and self.step and self.step % self.config.wandb.run_step_length == 0
 
 
 def init_wandb(self, reinit=False):
     """Starts a new wandb run."""
-    tags = [self.wallet.hotkey.ss58_address, openvalidators.__version__, openvalidators.__spec_version__]
+    tags = [self.wallet.hotkey.ss58_address, openvalidators.__version__, str(openvalidators.__spec_version__)]
     if self.config.mock:
         tags.append("mock")
     if self.config.neuron.use_custom_gating_model:
         tags.append("custom_gating_model")
     if self.config.neuron.nsfw_filter:
         tags.append("nsfw_filter")
     if self.config.neuron.outsource_scoring:
```

### Comparing `openvalidators-1.0.1/openvalidators/weights.py` & `openvalidators-1.0.2/openvalidators/weights.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.1/openvalidators.egg-info/PKG-INFO` & `openvalidators-1.0.2/openvalidators.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: openvalidators
-Version: 1.0.1
+Version: 1.0.2
 Summary: Openvalidators is a collection of open source validators for the Bittensor Network.
 Home-page: https://github.com/opentensor/validators
 Author: bittensor.com
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: MIT
 Keywords: bittensor,validator,ai,machine-learning,deep-learning,blockchain,pytorch,torch,neural-networks,cryptocurrency
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -158,7 +159,9 @@
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE 
 WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+
```

### Comparing `openvalidators-1.0.1/openvalidators.egg-info/SOURCES.txt` & `openvalidators-1.0.2/openvalidators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.1/setup.py` & `openvalidators-1.0.2/setup.py`

 * *Files identical despite different names*

