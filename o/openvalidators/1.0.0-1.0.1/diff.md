# Comparing `tmp/openvalidators-1.0.0.tar.gz` & `tmp/openvalidators-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openvalidators-1.0.0.tar", last modified: Tue Jun  6 18:55:11 2023, max compression
+gzip compressed data, was "openvalidators-1.0.1.tar", last modified: Wed Jun  7 17:40:29 2023, max compression
```

## Comparing `openvalidators-1.0.0.tar` & `openvalidators-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-06 18:55:11.691594 openvalidators-1.0.0/
--rw-r--r--   0 pedroferreira   (501) staff       (20)     1087 2023-06-05 21:08:43.000000 openvalidators-1.0.0/LICENSE
--rw-r--r--   0 pedroferreira   (501) staff       (20)     8971 2023-06-06 18:55:11.691160 openvalidators-1.0.0/PKG-INFO
--rw-r--r--   0 pedroferreira   (501) staff       (20)     7757 2023-06-06 18:34:54.000000 openvalidators-1.0.0/README.md
-drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-06 18:55:11.690001 openvalidators-1.0.0/openvalidators/
--rw-r--r--   0 pedroferreira   (501) staff       (20)     1403 2023-06-06 18:37:57.000000 openvalidators-1.0.0/openvalidators/__init__.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     8660 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/config.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     4366 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/dendrite.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)    16782 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/forward.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)    13620 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/gating.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     2029 2023-06-05 21:08:43.000000 openvalidators-1.0.0/openvalidators/misc.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     3557 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/mock.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     6977 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/neuron.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)    10885 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/prompts.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     7927 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/reward.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     2547 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/run.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     9294 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/utils.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     2873 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/weights.py
-drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-06 18:55:11.690905 openvalidators-1.0.0/openvalidators.egg-info/
--rw-r--r--   0 pedroferreira   (501) staff       (20)     8971 2023-06-06 18:55:11.000000 openvalidators-1.0.0/openvalidators.egg-info/PKG-INFO
--rw-r--r--   0 pedroferreira   (501) staff       (20)      580 2023-06-06 18:55:11.000000 openvalidators-1.0.0/openvalidators.egg-info/SOURCES.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)        1 2023-06-06 18:55:11.000000 openvalidators-1.0.0/openvalidators.egg-info/dependency_links.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)       69 2023-06-06 18:55:11.000000 openvalidators-1.0.0/openvalidators.egg-info/entry_points.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)      130 2023-06-06 18:55:11.000000 openvalidators-1.0.0/openvalidators.egg-info/requires.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)       15 2023-06-06 18:55:11.000000 openvalidators-1.0.0/openvalidators.egg-info/top_level.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)       38 2023-06-06 18:55:11.691645 openvalidators-1.0.0/setup.cfg
--rw-r--r--   0 pedroferreira   (501) staff       (20)     3496 2023-06-06 18:47:52.000000 openvalidators-1.0.0/setup.py
+drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-07 17:40:29.243407 openvalidators-1.0.1/
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     1087 2023-06-05 21:08:43.000000 openvalidators-1.0.1/LICENSE
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     8951 2023-06-07 17:40:29.243276 openvalidators-1.0.1/PKG-INFO
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     7757 2023-06-06 18:34:54.000000 openvalidators-1.0.1/README.md
+drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-07 17:40:29.242505 openvalidators-1.0.1/openvalidators/
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     1403 2023-06-07 17:39:54.000000 openvalidators-1.0.1/openvalidators/__init__.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     8831 2023-06-07 17:39:54.000000 openvalidators-1.0.1/openvalidators/config.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     4366 2023-06-06 18:32:40.000000 openvalidators-1.0.1/openvalidators/dendrite.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)    16781 2023-06-07 17:39:54.000000 openvalidators-1.0.1/openvalidators/forward.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)    13620 2023-06-06 18:32:40.000000 openvalidators-1.0.1/openvalidators/gating.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     2029 2023-06-05 21:08:43.000000 openvalidators-1.0.1/openvalidators/misc.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     3557 2023-06-06 18:32:40.000000 openvalidators-1.0.1/openvalidators/mock.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     6977 2023-06-07 13:42:52.000000 openvalidators-1.0.1/openvalidators/neuron.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)    10885 2023-06-06 18:32:40.000000 openvalidators-1.0.1/openvalidators/prompts.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     7927 2023-06-06 18:32:40.000000 openvalidators-1.0.1/openvalidators/reward.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     2547 2023-06-07 13:42:52.000000 openvalidators-1.0.1/openvalidators/run.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     9413 2023-06-07 17:39:54.000000 openvalidators-1.0.1/openvalidators/utils.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     2912 2023-06-07 17:39:54.000000 openvalidators-1.0.1/openvalidators/weights.py
+drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-07 17:40:29.243115 openvalidators-1.0.1/openvalidators.egg-info/
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     8951 2023-06-07 17:40:29.000000 openvalidators-1.0.1/openvalidators.egg-info/PKG-INFO
+-rw-r--r--   0 pedroferreira   (501) staff       (20)      580 2023-06-07 17:40:29.000000 openvalidators-1.0.1/openvalidators.egg-info/SOURCES.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)        1 2023-06-07 17:40:29.000000 openvalidators-1.0.1/openvalidators.egg-info/dependency_links.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)       68 2023-06-07 17:40:29.000000 openvalidators-1.0.1/openvalidators.egg-info/entry_points.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)      143 2023-06-07 17:40:29.000000 openvalidators-1.0.1/openvalidators.egg-info/requires.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)       15 2023-06-07 17:40:29.000000 openvalidators-1.0.1/openvalidators.egg-info/top_level.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)       38 2023-06-07 17:40:29.243440 openvalidators-1.0.1/setup.cfg
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     3496 2023-06-06 18:47:52.000000 openvalidators-1.0.1/setup.py
```

### Comparing `openvalidators-1.0.0/LICENSE` & `openvalidators-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.0/PKG-INFO` & `openvalidators-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: openvalidators
-Version: 1.0.0
+Version: 1.0.1
 Summary: Openvalidators is a collection of open source validators for the Bittensor Network.
 Home-page: https://github.com/opentensor/validators
 Author: bittensor.com
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: MIT
 Keywords: bittensor,validator,ai,machine-learning,deep-learning,blockchain,pytorch,torch,neural-networks,cryptocurrency
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -159,9 +158,7 @@
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE 
 WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
```

### Comparing `openvalidators-1.0.0/README.md` & `openvalidators-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.0/openvalidators/__init__.py` & `openvalidators-1.0.1/openvalidators/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,9 +23,9 @@
 from . import neuron
 from . import prompts
 from . import reward
 from . import run
 from . import utils
 from . import weights
 
-__version__ = "1.0.0"
-__spec_version__ = 1000
+__version__ = "1.0.1"
+__spec_version__ = 1002
```

### Comparing `openvalidators-1.0.0/openvalidators/config.py` & `openvalidators-1.0.1/openvalidators/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         default="cuda" if torch.cuda.is_available() else "cpu",
     )
 
     parser.add_argument(
         "--neuron.num_concurrent_forwards",
         type=int,
         help="The number of concurrent forwards running at any time.",
-        default=5,
+        default=1,
     )
     parser.add_argument(
         "--neuron.disable_set_weights",
         action="store_true",
         help="Disables setting weights.",
         default=False,
     )
@@ -121,31 +121,31 @@
         help="Follow up query timeout.",
         default=10,
     )
     parser.add_argument(
         "--neuron.followup_sample_size",
         type=int,
         help="How many miners to query for the follow up prompt.",
-        default=10,
+        default=50,
     )
 
     parser.add_argument("--neuron.answer_timeout", type=float, help="Answer query timeout.", default=10)
     parser.add_argument(
         "--neuron.answer_sample_size",
         type=int,
         help="How many miners to query for the answer.",
-        default=10,
+        default=50,
     )
 
     parser.add_argument("--neuron.scoring_timeout", type=float, help="Scoring query timeout", default=10)
     parser.add_argument(
         "--neuron.scoring_sample_size",
         type=int,
         help="How many miners to query for the scoring prompt.",
-        default=10,
+        default=2,
     )
 
     parser.add_argument(
         "--neuron.epoch_length_override",
         type=int,
         help="Override the default epoch length (how often we set weights).",
         default=0,
@@ -248,14 +248,20 @@
     )
     parser.add_argument(
         "--neuron.nsfw_filter",
         action="store_true",
         help="If set, filter out not-safe-for-work messages.",
         default=False,
     )
+    parser.add_argument(
+        "--neuron.outsource_scoring",
+        action="store_true",
+        help="If set, enable outsourced scoring.",
+        default=False,
+    )
 
 
 def config(cls):
     parser = argparse.ArgumentParser()
     bt.wallet.add_args(parser)
     bt.subtensor.add_args(parser)
     bt.logging.add_args(parser)
```

### Comparing `openvalidators-1.0.0/openvalidators/dendrite.py` & `openvalidators-1.0.1/openvalidators/dendrite.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.0/openvalidators/forward.py` & `openvalidators-1.0.1/openvalidators/forward.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,25 +20,24 @@
 import wandb
 import torch
 import random
 import asyncio
 import bittensor as bt
 
 from loguru import logger
-from typing import List, Tuple, Union
+from typing import List, Union, Dict
 from openvalidators.misc import ttl_get_block
 from openvalidators.prompts import (
     extract_score,
     followup_request_template,
     answer_scoring_template,
     followup_scoring_template,
 )
 from openvalidators.utils import check_uid_availability
 
-
 def get_random_uids(self, k: int, exclude: List[int] = None) -> torch.LongTensor:
     """Returns k available random uids from the metagraph.
     Args:
         k (int): Number of uids to return.
         exclude (List[int]): List of uids to exclude from the random sampling.
     Returns:
         uids (torch.LongTensor): Randomly sampled available uids.
@@ -71,17 +70,16 @@
     """
     len_check = len(response.completion) > min_len
     filter_check = not (self.config.neuron.nsfw_filter and is_nsfw(self, response.completion, nsfw_bound_score))
 
     return len_check and filter_check
 
 
-async def scoring_completions(
-    self, prompt: str, scoring_template: str, responses: List[bt.DendriteCall], exclude_uids: List[int] = None
-) -> Tuple[torch.FloatTensor, List[List[int]], List[List[str]], List[List[int]]]:
+async def scoring_completions(self, prompt: str, scoring_template: str, responses: List[bt.DendriteCall],
+                              exclude_uids: List[int] = None) -> Dict:
     """Using the prompt and call responses, outsource prompt-based scoring to network,
        return scoring average for each response.
 
     Args:
         prompt (str):
             Prompt to use for the reward model.
         scoring_template (str):
@@ -158,16 +156,27 @@
         all_scoring_values[i] = scoring_values
 
         # Scoring average for completion.
         successful_scoring_values = [value for value in scoring_values if value]
         if len(successful_scoring_values) > 0:
             filled_scores[i] = sum(successful_scoring_values) / len(successful_scoring_values)
 
-    # Return all scoring details.
-    return filled_scores, all_scoring_uids, all_scoring_completions, all_scoring_values
+    # Determine best completion.
+    completions = [resp.completion for resp in responses]
+    best_completion = completions[filled_scores.argmax(dim=0)].strip()
+
+    # Scoring dictionary for wandb.
+    scoring_dict = {
+        f"scorings": filled_scores,
+        f"scoring_uids": all_scoring_uids,
+        f"scoring_completions": all_scoring_completions,
+        f"scoring_values": all_scoring_values,
+        f"best_completion": best_completion,
+    }
+    return scoring_dict
 
 
 def reward_completions(self, prompt: str, responses: List[bt.DendriteCall]) -> torch.FloatTensor:
     """Using the prompt and call responses returns rewards for each response.
 
     Args:
         prompt (str):
@@ -196,14 +205,15 @@
         completions_with_prompt=completions_with_prompt,
         completions_without_prompt=completions_without_prompt,
         difference=True,
         shift=self.config.neuron.reward_shift,
     ).to(self.device)
 
     # Fill scores with zeros for non successful responses.
+    successful_rewards = successful_rewards.softmax( 0 )
     filled_rewards = torch.zeros(len(responses), dtype=torch.float32)
     for idx, reward in zip(successful_completions_indices, successful_rewards):
         filled_rewards[idx] = reward
 
     # Return the filled rewards.
     return filled_rewards
 
@@ -281,21 +291,18 @@
     )
     # Reward model evaluation.
     followup_rewards = reward_completions(self, followup_prompt, followup_responses).to(self.device)
     followup_completions = [comp.completion for comp in followup_responses]
     best_followup = followup_completions[followup_rewards.argmax(dim=0)].strip()
 
     # Prompt-based scoring via network. Prohibits self-scoring.
-    (
-        followup_scorings,
-        followup_scoring_uids,
-        followup_scoring_completions,
-        followup_scoring_values,
-    ) = await scoring_completions(self, bootstrap_prompt, followup_scoring_template, followup_responses, followup_uids)
-    best_followup_scoring = followup_completions[followup_scorings.argmax(dim=0)].strip()
+    if self.config.neuron.outsource_scoring:
+        followup_scoring = await scoring_completions(self, prompt=bootstrap_prompt,
+                                                     scoring_template=followup_scoring_template,
+                                                     responses=followup_responses, exclude_uids=followup_uids)
 
     # Backward call sends reward info back to followup_uids.
     _followup_backward = await self.dendrite_pool.async_backward(
         uids=followup_uids,
         roles=["user"],
         messages=[followup_prompt],
         completions=followup_completions,
@@ -307,27 +314,25 @@
     answer_uids = get_random_uids(self, k=self.config.neuron.answer_sample_size, exclude=followup_uids).to(self.device)
     answer_responses = await self.dendrite_pool.async_forward(
         uids=answer_uids,
         roles=["user"],
         messages=[answer_prompt],
         timeout=self.config.neuron.answer_timeout,
     )
+
+    reward_prompt = f"Question: {best_followup}\n"
     # Reward model evaluation.
-    answer_rewards = reward_completions(self, answer_prompt, answer_responses).to(self.device)
+    answer_rewards = reward_completions(self, reward_prompt, answer_responses).to(self.device)
     answer_completions = [ans.completion for ans in answer_responses]
     best_answer = answer_completions[answer_rewards.argmax(dim=0)].strip()
 
     # Prompt-based scoring via network. Prohibits self-scoring.
-    (
-        answer_scorings,
-        answer_scoring_uids,
-        answer_scoring_completions,
-        answer_scoring_values,
-    ) = await scoring_completions(self, answer_prompt, answer_scoring_template, answer_responses, answer_uids)
-    best_answer_scoring = answer_completions[answer_scorings.argmax(dim=0)].strip()
+    if self.config.neuron.outsource_scoring:
+        answer_scoring = await scoring_completions(self, prompt=answer_prompt, scoring_template=answer_scoring_template,
+                                                   responses=answer_responses, exclude_uids=answer_uids)
 
     # Backward call sends reward info back to answer_uids.
     _answer_backward = await self.dendrite_pool.async_backward(
         uids=answer_uids,
         roles=["user"],
         messages=[answer_prompt],
         completions=answer_completions,
@@ -358,41 +363,35 @@
         "gating_loss": gating_loss.item(),
         "gating_scorings": scores[answer_uids].tolist(),
         "base_prompt": bootstrap_prompt,
         "followup_uids": followup_uids.tolist(),
         "followup_completions": followup_completions,
         "followup_times": [comp.elapsed_time for comp in followup_responses],
         "followup_rewards": followup_rewards.tolist(),
-        "followup_scorings": followup_scorings,
-        "followup_scoring_uids": followup_scoring_uids,
-        "followup_scoring_completions": followup_scoring_completions,
-        "followup_scoring_values": followup_scoring_values,
-        "best_followup_scoring": best_followup_scoring,
         "best_followup": best_followup,
         "best_answer": best_answer,
         "answer_prompt": answer_prompt,
         "answer_uids": answer_uids.tolist(),
         "answer_completions": answer_completions,
         "answer_times": [ans.elapsed_time for ans in answer_responses],
         "answer_rewards": answer_rewards.tolist(),
-        "answer_scorings": answer_scorings,
-        "answer_scoring_uids": answer_scoring_uids,
-        "answer_scoring_completions": answer_scoring_completions,
-        "answer_scoring_values": answer_scoring_values,
-        "best_answer_scoring": best_answer_scoring,
     }
 
     if self.config.neuron.nsfw_filter:
         event.update(
             {
                 "followup_nsfw_scores": [is_nsfw(self, comp, return_score=True) for comp in followup_completions],
                 "answer_nsfw_scores": [is_nsfw(self, ans, return_score=True) for ans in answer_completions],
             }
         )
 
+    if self.config.neuron.outsource_scoring:
+        event.update({f'followup_{k}': v for k, v in followup_scoring.items()})
+        event.update({f'answer_{k}': v for k, v in answer_scoring.items()})
+
     bt.logging.debug("step:", str(event))
     # Log to wandb.
     if not self.config.wandb.off:
 
         if self.step % self.config.wandb.weights_step_length == 0:
             event["moving_averaged_scores"] = self.moving_averaged_scores.tolist()
             bt.logging.debug("logging weights")
```

### Comparing `openvalidators-1.0.0/openvalidators/gating.py` & `openvalidators-1.0.1/openvalidators/gating.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.0/openvalidators/misc.py` & `openvalidators-1.0.1/openvalidators/misc.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.0/openvalidators/mock.py` & `openvalidators-1.0.1/openvalidators/mock.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.0/openvalidators/neuron.py` & `openvalidators-1.0.1/openvalidators/neuron.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.0/openvalidators/prompts.py` & `openvalidators-1.0.1/openvalidators/prompts.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.0/openvalidators/reward.py` & `openvalidators-1.0.1/openvalidators/reward.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.0/openvalidators/run.py` & `openvalidators-1.0.1/openvalidators/run.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.0/openvalidators/utils.py` & `openvalidators-1.0.1/openvalidators/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,21 +27,23 @@
 def should_reinit_wandb(self):
     # Check if wandb run needs to be rolled over.
     return not self.config.wandb.off and self.step and self.step % self.config.wandb.run_step_length == 0
 
 
 def init_wandb(self, reinit=False):
     """Starts a new wandb run."""
-    tags = [self.wallet.hotkey.ss58_address, openvalidators.__version__]
+    tags = [self.wallet.hotkey.ss58_address, openvalidators.__version__, openvalidators.__spec_version__]
     if self.config.mock:
         tags.append("mock")
     if self.config.neuron.use_custom_gating_model:
         tags.append("custom_gating_model")
     if self.config.neuron.nsfw_filter:
         tags.append("nsfw_filter")
+    if self.config.neuron.outsource_scoring:
+        tags.append("outsource_scoring")
     if self.config.neuron.disable_set_weights:
         tags.append("disable_set_weights")
 
     self.wandb = wandb.init(
         anonymous="allow",
         reinit=reinit,
         project=self.config.wandb.project_name,
```

### Comparing `openvalidators-1.0.0/openvalidators/weights.py` & `openvalidators-1.0.1/openvalidators/weights.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,18 @@
         netuid=self.config.netuid,
         subtensor=self.subtensor,
         metagraph=self.metagraph,
     )
     bt.logging.trace("processed_weights", processed_weights)
     bt.logging.trace("processed_weight_uids", processed_weight_uids)
 
+    if not self.config.wandb.off:
+        wandb.log({"set_weights": list(zip(processed_weight_uids.tolist(), processed_weights.tolist()))})
+
     # Set the weights on chain via our subtensor connection.
-    wandb.log({"set_weights": list(zip(processed_weight_uids.tolist(), processed_weights.tolist()))})
     self.subtensor.set_weights(
         wallet=self.wallet,
         netuid=self.config.netuid,
         uids=processed_weight_uids,
         weights=processed_weights,
         wait_for_finalization=False,
         version_key=openvalidators.__spec_version__,
```

### Comparing `openvalidators-1.0.0/openvalidators.egg-info/PKG-INFO` & `openvalidators-1.0.1/openvalidators.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: openvalidators
-Version: 1.0.0
+Version: 1.0.1
 Summary: Openvalidators is a collection of open source validators for the Bittensor Network.
 Home-page: https://github.com/opentensor/validators
 Author: bittensor.com
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: MIT
 Keywords: bittensor,validator,ai,machine-learning,deep-learning,blockchain,pytorch,torch,neural-networks,cryptocurrency
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -159,9 +158,7 @@
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE 
 WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
```

### Comparing `openvalidators-1.0.0/openvalidators.egg-info/SOURCES.txt` & `openvalidators-1.0.1/openvalidators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.0/setup.py` & `openvalidators-1.0.1/setup.py`

 * *Files identical despite different names*

