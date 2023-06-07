# Comparing `tmp/pyatp-1.1.1.tar.gz` & `tmp/pyatp-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatp-1.1.1.tar", max compression
+gzip compressed data, was "pyatp-1.1.2.tar", max compression
```

## Comparing `pyatp-1.1.1.tar` & `pyatp-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,392 @@
--rw-r--r--   0        0        0      471 2023-02-27 01:36:28.747490 pyatp-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       68 2023-02-23 14:58:07.782013 pyatp-1.1.1/src/atp/__init__.py
--rw-r--r--   0        0        0     6363 2023-02-26 07:49:40.027781 pyatp-1.1.1/src/atp/client.py
--rw-r--r--   0        0        0     4394 2022-11-16 03:39:20.958158 pyatp-1.1.1/src/atp/config.py
--rw-r--r--   0        0        0     1354 2022-10-31 06:28:07.824669 pyatp-1.1.1/src/atp/error.py
--rw-r--r--   0        0        0     1151 2023-02-23 14:45:51.373707 pyatp-1.1.1/src/atp/huggingface/datasets.py
--rw-r--r--   0        0        0     4448 2023-02-24 08:04:59.967139 pyatp-1.1.1/src/atp/huggingface/pipelines.py
--rw-r--r--   0        0        0     1153 2022-10-31 06:23:44.182652 pyatp-1.1.1/src/atp/pretrain/__init__.py
--rw-r--r--   0        0        0     1151 2022-10-31 02:59:44.406000 pyatp-1.1.1/src/atp/pretrain/av2vec/__init__.py
--rw-r--r--   0        0        0      290 2022-10-31 06:16:58.083767 pyatp-1.1.1/src/atp/pretrain/av2vec/av2vec.py
--rw-r--r--   0        0        0     1006 2022-11-16 02:45:12.155157 pyatp-1.1.1/src/atp/pretrain/av2vec/data.py
--rw-r--r--   0        0        0     1151 2022-10-31 02:59:44.406000 pyatp-1.1.1/src/atp/pretrain/voice2vec/__init__.py
--rw-r--r--   0        0        0     1357 2023-02-26 07:49:09.652036 pyatp-1.1.1/src/atp/pretrain/voice2vec/data.py
--rw-r--r--   0        0        0      299 2022-10-26 01:33:06.000000 pyatp-1.1.1/src/atp/pretrain/voice2vec/main.py
--rw-r--r--   0        0        0      290 2022-10-31 06:16:58.083000 pyatp-1.1.1/src/atp/pretrain/voice2vec/voice2vec.py
--rw-r--r--   0        0        0     3543 2023-02-26 07:50:00.444216 pyatp-1.1.1/src/atp/utils/aipass_client.py
--rw-r--r--   0        0        0      204 2022-10-26 01:33:06.000000 pyatp-1.1.1/src/atp/utils/exception.py
--rw-r--r--   0        0        0     1425 2022-09-08 02:50:41.716000 pyatp-1.1.1/src/atp/utils/log.py
--rw-r--r--   0        0        0     2168 2023-02-26 07:50:10.078208 pyatp-1.1.1/src/atp/utils/ne_utils.py
--rw-r--r--   0        0        0      769 2023-02-27 01:36:31.693333 pyatp-1.1.1/setup.py
--rw-r--r--   0        0        0      524 2023-02-27 01:36:31.693509 pyatp-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-08 09:45:37.719000 pyatp-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1057 2023-06-07 01:50:44.139361 pyatp-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1151 2023-05-26 01:51:19.942655 pyatp-1.1.2/src/ailab/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 01:43:21.707000 pyatp-1.1.2/src/ailab/atp_dataset/__init__.py
+-rw-r--r--   0        0        0     1189 2023-05-26 01:43:21.707000 pyatp-1.1.2/src/ailab/atp_dataset/ailab_api.py
+-rw-r--r--   0        0        0      392 2023-05-26 01:43:21.707000 pyatp-1.1.2/src/ailab/atp_dataset/constant.py
+-rw-r--r--   0        0        0     5428 2023-05-26 02:01:22.426564 pyatp-1.1.2/src/ailab/atp_dataset/dataset.py
+-rw-r--r--   0        0        0     1027 2023-05-26 01:43:21.707000 pyatp-1.1.2/src/ailab/atp_dataset/huggingface_api.py
+-rw-r--r--   0        0        0      323 2023-05-26 01:43:21.707000 pyatp-1.1.2/src/ailab/atp_dataset/modelscope_api.py
+-rw-r--r--   0        0        0        0 2023-05-26 01:43:21.707000 pyatp-1.1.2/src/ailab/atp_finetuner/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-26 01:43:21.707000 pyatp-1.1.2/src/ailab/atp_finetuner/accelerator/__init__.py
+-rw-r--r--   0        0        0     1826 2023-06-01 08:42:34.253000 pyatp-1.1.2/src/ailab/atp_finetuner/accelerator/accelerator.py
+-rw-r--r--   0        0        0      766 2023-05-26 01:43:21.707000 pyatp-1.1.2/src/ailab/atp_finetuner/build.py
+-rw-r--r--   0        0        0     2096 2023-05-26 02:21:36.014188 pyatp-1.1.2/src/ailab/atp_finetuner/constant.py
+-rw-r--r--   0        0        0      295 2023-05-26 01:43:21.708000 pyatp-1.1.2/src/ailab/atp_finetuner/datacollator/__init__.py
+-rw-r--r--   0        0        0     1552 2023-05-26 02:03:39.199534 pyatp-1.1.2/src/ailab/atp_finetuner/datacollator/datacollator.py
+-rw-r--r--   0        0        0      919 2023-05-26 02:34:48.583795 pyatp-1.1.2/src/ailab/atp_finetuner/datacollator/dc_for_alpaca.py
+-rw-r--r--   0        0        0     1760 2023-05-26 02:34:48.589949 pyatp-1.1.2/src/ailab/atp_finetuner/datacollator/dc_for_chatglm.py
+-rw-r--r--   0        0        0      885 2023-05-26 02:34:48.585577 pyatp-1.1.2/src/ailab/atp_finetuner/datacollator/dc_for_language.py
+-rw-r--r--   0        0        0      905 2023-05-26 02:34:48.588525 pyatp-1.1.2/src/ailab/atp_finetuner/datacollator/dc_for_token.py
+-rw-r--r--   0        0        0      855 2023-05-26 02:34:48.587131 pyatp-1.1.2/src/ailab/atp_finetuner/datacollator/dc_with_padding.py
+-rw-r--r--   0        0        0     1557 2023-06-01 08:42:34.253691 pyatp-1.1.2/src/ailab/atp_finetuner/finetuner.py
+-rw-r--r--   0        0        0       64 2023-05-26 01:43:21.708000 pyatp-1.1.2/src/ailab/atp_finetuner/metric/__init__.py
+-rw-r--r--   0        0        0      627 2023-05-26 02:34:59.536185 pyatp-1.1.2/src/ailab/atp_finetuner/metric/accury.py
+-rw-r--r--   0        0        0      425 2023-05-26 02:03:39.174407 pyatp-1.1.2/src/ailab/atp_finetuner/metric/metric.py
+-rw-r--r--   0        0        0       62 2023-05-26 01:43:21.708000 pyatp-1.1.2/src/ailab/atp_finetuner/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 01:43:21.708000 pyatp-1.1.2/src/ailab/atp_finetuner/model/cv/__init__.py
+-rw-r--r--   0        0        0      992 2023-05-26 02:03:39.205737 pyatp-1.1.2/src/ailab/atp_finetuner/model/model.py
+-rw-r--r--   0        0        0       80 2023-06-01 08:42:34.253788 pyatp-1.1.2/src/ailab/atp_finetuner/model/multimodel/__init__.py
+-rw-r--r--   0        0        0     3338 2023-06-01 08:42:34.253977 pyatp-1.1.2/src/ailab/atp_finetuner/model/multimodel/model_for_sd_lora.py
+-rw-r--r--   0        0        0     1068 2023-06-01 08:42:34.254154 pyatp-1.1.2/src/ailab/atp_finetuner/model/multimodel/vilt_for_vqa.py
+-rw-r--r--   0        0        0      277 2023-05-26 01:43:21.709000 pyatp-1.1.2/src/ailab/atp_finetuner/model/nlp/__init__.py
+-rw-r--r--   0        0        0      705 2023-05-26 02:03:39.194115 pyatp-1.1.2/src/ailab/atp_finetuner/model/nlp/model_for_chatglm.py
+-rw-r--r--   0        0        0     1602 2023-05-26 02:03:39.171860 pyatp-1.1.2/src/ailab/atp_finetuner/model/nlp/model_for_lora.py
+-rw-r--r--   0        0        0      723 2023-05-26 02:03:39.180833 pyatp-1.1.2/src/ailab/atp_finetuner/model/nlp/model_for_question_answer.py
+-rw-r--r--   0        0        0      733 2023-05-26 02:03:39.202174 pyatp-1.1.2/src/ailab/atp_finetuner/model/nlp/model_for_text_classification.py
+-rw-r--r--   0        0        0      733 2023-05-26 02:03:39.208106 pyatp-1.1.2/src/ailab/atp_finetuner/model/nlp/model_for_token_classification.py
+-rw-r--r--   0        0        0       78 2023-05-26 01:43:21.709000 pyatp-1.1.2/src/ailab/atp_finetuner/preprossor/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 01:43:21.709000 pyatp-1.1.2/src/ailab/atp_finetuner/preprossor/cv/__init__.py
+-rw-r--r--   0        0        0       88 2023-05-26 01:43:21.709000 pyatp-1.1.2/src/ailab/atp_finetuner/preprossor/multimodel/__init__.py
+-rw-r--r--   0        0        0     2934 2023-06-01 08:42:34.254278 pyatp-1.1.2/src/ailab/atp_finetuner/preprossor/multimodel/pc_for_sd_lora.py
+-rw-r--r--   0        0        0     3412 2023-06-01 08:42:34.254380 pyatp-1.1.2/src/ailab/atp_finetuner/preprossor/multimodel/pc_for_vilt_vqa.py
+-rw-r--r--   0        0        0      267 2023-05-26 01:43:21.709000 pyatp-1.1.2/src/ailab/atp_finetuner/preprossor/nlp/__init__.py
+-rw-r--r--   0        0        0     3062 2023-06-01 08:42:34.254467 pyatp-1.1.2/src/ailab/atp_finetuner/preprossor/nlp/pc_for_alpaca.py
+-rw-r--r--   0        0        0     2504 2023-06-01 08:42:34.254547 pyatp-1.1.2/src/ailab/atp_finetuner/preprossor/nlp/pc_for_chatglm.py
+-rw-r--r--   0        0        0     2702 2023-06-01 08:42:34.254626 pyatp-1.1.2/src/ailab/atp_finetuner/preprossor/nlp/pc_for_llama_cn.py
+-rw-r--r--   0        0        0     3509 2023-06-01 08:42:34.254707 pyatp-1.1.2/src/ailab/atp_finetuner/preprossor/nlp/question_answer_pc.py
+-rw-r--r--   0        0        0     1107 2023-06-01 08:42:34.254799 pyatp-1.1.2/src/ailab/atp_finetuner/preprossor/nlp/text_classification_pc.py
+-rw-r--r--   0        0        0     1091 2023-06-01 08:42:34.254882 pyatp-1.1.2/src/ailab/atp_finetuner/preprossor/preprossor.py
+-rw-r--r--   0        0        0       65 2023-05-26 01:43:21.710000 pyatp-1.1.2/src/ailab/atp_finetuner/trainer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 01:43:21.710000 pyatp-1.1.2/src/ailab/atp_finetuner/trainer/cv/__init__.py
+-rw-r--r--   0        0        0       88 2023-05-26 01:43:21.710000 pyatp-1.1.2/src/ailab/atp_finetuner/trainer/multimodel/__init__.py
+-rw-r--r--   0        0        0    10436 2023-06-01 08:42:34.255060 pyatp-1.1.2/src/ailab/atp_finetuner/trainer/multimodel/trainer_for_sd_lora.py
+-rw-r--r--   0        0        0     4244 2023-06-01 08:42:34.255151 pyatp-1.1.2/src/ailab/atp_finetuner/trainer/multimodel/trainer_for_vilt_vqa.py
+-rw-r--r--   0        0        0      276 2023-05-26 01:43:21.710000 pyatp-1.1.2/src/ailab/atp_finetuner/trainer/nlp/__init__.py
+-rw-r--r--   0        0        0     4865 2023-06-01 08:42:34.255241 pyatp-1.1.2/src/ailab/atp_finetuner/trainer/nlp/trainer_for_alpaca.py
+-rw-r--r--   0        0        0     6323 2023-06-01 08:42:34.255617 pyatp-1.1.2/src/ailab/atp_finetuner/trainer/nlp/trainer_for_chatglm.py
+-rw-r--r--   0        0        0     5110 2023-06-01 08:42:34.255722 pyatp-1.1.2/src/ailab/atp_finetuner/trainer/nlp/trainer_for_llama_cn.py
+-rw-r--r--   0        0        0     4090 2023-06-01 08:42:34.255810 pyatp-1.1.2/src/ailab/atp_finetuner/trainer/nlp/trainer_for_text_classification.py
+-rw-r--r--   0        0        0     4041 2023-06-01 08:42:34.256415 pyatp-1.1.2/src/ailab/atp_finetuner/trainer/nlp/traniner_for_question_answer.py
+-rw-r--r--   0        0        0     1594 2023-06-01 08:42:34.256512 pyatp-1.1.2/src/ailab/atp_finetuner/trainer/trainer.py
+-rw-r--r--   0        0        0      341 2023-06-06 06:46:33.737827 pyatp-1.1.2/src/ailab/buildkit/README.md
+-rw-r--r--   0        0        0     1148 2023-06-06 06:46:33.737928 pyatp-1.1.2/src/ailab/buildkit/__init__.py
+-rw-r--r--   0        0        0      293 2023-06-06 07:57:10.714617 pyatp-1.1.2/src/ailab/buildkit/base/Dockerfile
+-rw-r--r--   0        0        0       86 2023-06-06 07:58:04.834648 pyatp-1.1.2/src/ailab/buildkit/base/build.sh
+-rw-r--r--   0        0        0    11435 2023-06-06 07:53:21.547634 pyatp-1.1.2/src/ailab/buildkit/build.py
+-rw-r--r--   0        0        0      542 2023-06-06 06:46:33.738272 pyatp-1.1.2/src/ailab/buildkit/config.py
+-rw-r--r--   0        0        0      529 2023-06-06 06:46:33.738346 pyatp-1.1.2/src/ailab/buildkit/dotdict.py
+-rw-r--r--   0        0        0      610 2023-06-06 06:46:33.738426 pyatp-1.1.2/src/ailab/buildkit/error.py
+-rw-r--r--   0        0        0  2680354 2023-06-06 06:46:33.750086 pyatp-1.1.2/src/ailab/buildkit/get-pip.py
+-rw-r--r--   0        0        0     1249 2023-06-06 07:31:52.608041 pyatp-1.1.2/src/ailab/buildkit/templates/Dockerfile.j2
+-rw-r--r--   0        0        0     1148 2023-06-06 06:46:33.750461 pyatp-1.1.2/src/ailab/inference_wrapper/__init__.py
+-rw-r--r--   0        0        0      637 2023-03-02 05:17:14.587000 pyatp-1.1.2/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/Dockerfile
+-rw-r--r--   0        0        0      198 2023-03-02 05:17:14.586000 pyatp-1.1.2/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/README.md
+-rw-r--r--   0        0        0       53 2023-03-02 05:17:28.917000 pyatp-1.1.2/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/requirements.txt
+-rw-r--r--   0        0        0    95827 2023-03-02 05:17:14.588000 pyatp-1.1.2/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/wrapper/test_data/test.png
+-rw-r--r--   0        0        0      918 2023-03-02 08:23:57.053000 pyatp-1.1.2/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/wrapper/test_data/test.py
+-rw-r--r--   0        0        0     6286 2023-03-02 05:21:16.095000 pyatp-1.1.2/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/wrapper/wrapper.py
+-rw-r--r--   0        0        0       85 2023-03-21 05:26:30.958000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/README.md
+-rw-r--r--   0        0        0      637 2023-03-23 14:04:01.930000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/Dockerfile
+-rw-r--r--   0        0        0      182 2023-03-31 02:08:50.009000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/readme.md
+-rw-r--r--   0        0        0       84 2023-03-23 14:04:01.931000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/requirements.txt
+-rw-r--r--   0        0        0   178529 2023-03-23 14:04:01.931000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/wrapper/sketch-mountains-input.jpg
+-rw-r--r--   0        0        0     2992 2023-03-31 02:08:50.009000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-23 14:04:01.932000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/audio_diffusion/Dockerfile
+-rw-r--r--   0        0        0       84 2023-03-23 14:04:01.932000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/audio_diffusion/requirements.txt
+-rw-r--r--   0        0        0        0 2023-03-31 02:08:50.010000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/audio_diffusion/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-23 14:04:01.932000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/Dockerfile
+-rw-r--r--   0        0        0      144 2023-03-31 02:08:50.010000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/readme.md
+-rw-r--r--   0        0        0       84 2023-03-23 14:04:01.932000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/requirements.txt
+-rw-r--r--   0        0        0  1333615 2023-03-23 14:04:01.933000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/wrapper/horse.png
+-rw-r--r--   0        0        0     3303 2023-03-31 02:08:50.010000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-23 14:04:01.934000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/dance_diffusion/Dockerfile
+-rw-r--r--   0        0        0       84 2023-03-23 14:04:01.934000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/dance_diffusion/requirements.txt
+-rw-r--r--   0        0        0        0 2023-03-31 02:08:50.010000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/dance_diffusion/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-31 02:08:50.010000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/latency_diffusion/Dockerfile
+-rw-r--r--   0        0        0       84 2023-03-31 02:08:50.011000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/latency_diffusion/requirements.txt
+-rw-r--r--   0        0        0        0 2023-03-31 02:08:50.011000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/latency_diffusion/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-31 02:08:50.011000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/attend_and_excite/Dockerfile
+-rw-r--r--   0        0        0      260 2023-03-31 02:08:50.011000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/attend_and_excite/readme.md
+-rw-r--r--   0        0        0       84 2023-03-31 02:08:50.011000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/attend_and_excite/requirements.txt
+-rw-r--r--   0        0        0     3349 2023-03-31 02:08:50.011000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/attend_and_excite/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-31 02:08:50.011000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/Dockerfile
+-rw-r--r--   0        0        0      232 2023-03-31 02:08:50.011000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/readme.md
+-rw-r--r--   0        0        0       84 2023-03-31 02:08:50.011000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/requirements.txt
+-rw-r--r--   0        0        0   173131 2023-03-31 02:08:50.012000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/wrapper/000000039769.jpg
+-rw-r--r--   0        0        0     2997 2023-03-31 02:08:50.012000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-23 14:04:01.934000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/Dockerfile
+-rw-r--r--   0        0        0      194 2023-03-31 02:08:50.012000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/readme.md
+-rw-r--r--   0        0        0       84 2023-03-23 14:04:01.934000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/requirements.txt
+-rw-r--r--   0        0        0   178529 2023-03-23 14:04:01.935000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/wrapper/sketch-mountains-input.jpg
+-rw-r--r--   0        0        0     3045 2023-03-31 02:08:50.012000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-31 02:08:50.012000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/Dockerfile
+-rw-r--r--   0        0        0      213 2023-03-31 02:08:50.012000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/readme.md
+-rw-r--r--   0        0        0       84 2023-03-31 02:08:50.012000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/requirements.txt
+-rw-r--r--   0        0        0   404753 2023-03-31 02:08:50.014000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/wrapper/overture-creations-5sI6fQgYIuo.png
+-rw-r--r--   0        0        0    12106 2023-03-31 02:08:50.014000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/wrapper/overture-creations-5sI6fQgYIuo_mask.png
+-rw-r--r--   0        0        0     3375 2023-03-31 02:08:50.014000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-31 02:08:50.015000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/Dockerfile
+-rw-r--r--   0        0        0      231 2023-03-31 02:08:50.015000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/readme.md
+-rw-r--r--   0        0        0       84 2023-03-31 02:08:50.015000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/requirements.txt
+-rw-r--r--   0        0        0   408679 2023-03-31 02:08:50.016000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/wrapper/mountain.png
+-rw-r--r--   0        0        0     3076 2023-03-31 02:08:50.016000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-31 02:08:50.016000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/multi_diffusion/Dockerfile
+-rw-r--r--   0        0        0      319 2023-03-31 02:08:50.016000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/multi_diffusion/readme.md
+-rw-r--r--   0        0        0       84 2023-03-31 02:08:50.016000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/multi_diffusion/requirements.txt
+-rw-r--r--   0        0        0     3075 2023-03-31 02:08:50.016000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/multi_diffusion/wrapper/wrapper.py
+-rw-r--r--   0        0        0      159 2023-03-31 02:08:50.016000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/readme.md
+-rw-r--r--   0        0        0      637 2023-03-31 02:08:50.017000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/self_attention_guidance/Dockerfile
+-rw-r--r--   0        0        0      201 2023-03-31 02:08:50.017000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/self_attention_guidance/readme.md
+-rw-r--r--   0        0        0       84 2023-03-31 02:08:50.017000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/self_attention_guidance/requirements.txt
+-rw-r--r--   0        0        0     2958 2023-03-31 02:08:50.018000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/self_attention_guidance/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-31 02:08:50.018000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/Dockerfile
+-rw-r--r--   0        0        0      170 2023-03-31 02:08:50.018000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/readme.md
+-rw-r--r--   0        0        0       84 2023-03-31 02:08:50.018000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/requirements.txt
+-rw-r--r--   0        0        0    26358 2023-03-31 02:08:50.018000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/wrapper/low_res_cat.png
+-rw-r--r--   0        0        0     2992 2023-03-31 02:08:50.018000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-23 14:04:01.935000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/text_to_image/Dockerfile
+-rw-r--r--   0        0        0      158 2023-03-31 02:08:50.018000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/text_to_image/readme.md
+-rw-r--r--   0        0        0       84 2023-03-23 14:04:01.935000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/text_to_image/requirements.txt
+-rw-r--r--   0        0        0     2947 2023-03-23 14:04:01.935000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/text_to_image/wrapper/wrapper.py
+-rw-r--r--   0        0        0     2823 2023-03-21 05:26:30.958000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/README.md
+-rw-r--r--   0        0        0     1151 2023-06-06 06:46:33.750578 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/__init__.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.708000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/audio/audio_classification/Dockerfile
+-rw-r--r--   0        0        0       63 2023-03-19 14:49:24.708000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/audio/audio_classification/requirements.txt
+-rw-r--r--   0        0        0   383447 2023-03-19 14:49:24.709000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/audio/audio_classification/wrapper/mlk.flac
+-rw-r--r--   0        0        0     2360 2023-03-21 05:26:30.958000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/audio/audio_classification/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-02 05:19:51.931000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/audio/automatic-speech-recognition/Dockerfile
+-rw-r--r--   0        0        0       63 2023-03-02 05:19:51.931000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/audio/automatic-speech-recognition/requirements.txt
+-rw-r--r--   0        0        0   383447 2023-03-02 05:19:51.932000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/audio/automatic-speech-recognition/wrapper/mlk.flac
+-rw-r--r--   0        0        0     2619 2023-03-19 14:49:24.710000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/audio/automatic-speech-recognition/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.710000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.710000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/requirements.txt
+-rw-r--r--   0        0        0   173131 2023-03-19 14:49:24.710000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/wrapper/cat.jpg
+-rw-r--r--   0        0        0    10942 2023-03-19 14:49:24.711000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/wrapper/result_depth.jpeg
+-rw-r--r--   0        0        0     2899 2023-03-19 14:49:24.711000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.711000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/image_classification/Dockerfile
+-rw-r--r--   0        0        0       64 2023-03-19 14:49:24.711000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/image_classification/requirements.txt
+-rw-r--r--   0        0        0   434332 2023-03-19 14:49:24.712000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/image_classification/wrapper/img.png
+-rw-r--r--   0        0        0     2539 2023-03-19 14:49:24.712000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/image_classification/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.713000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/Dockerfile
+-rw-r--r--   0        0        0       98 2023-03-19 14:49:24.713000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/requirements.txt
+-rw-r--r--   0        0        0   173131 2023-03-19 14:49:24.713000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/cat.jpg
+-rw-r--r--   0        0        0     9565 2023-03-19 14:49:24.713000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_1.jpg
+-rw-r--r--   0        0        0     5000 2023-03-19 14:49:24.713000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_2.jpg
+-rw-r--r--   0        0        0     4937 2023-03-19 14:49:24.713000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_3.jpg
+-rw-r--r--   0        0        0    20405 2023-03-19 14:49:24.713000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_4.jpg
+-rw-r--r--   0        0        0    10041 2023-03-19 14:49:24.713000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_5.jpg
+-rw-r--r--   0        0        0    63187 2023-03-19 14:49:24.714000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/test_str_to_img.jpg
+-rw-r--r--   0        0        0     3164 2023-03-19 14:49:24.714000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.714000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/object_detection/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.714000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/object_detection/requirements.txt
+-rw-r--r--   0        0        0   173131 2023-03-19 14:49:24.714000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/object_detection/wrapper/cat.jpg
+-rw-r--r--   0        0        0     2433 2023-03-19 14:49:24.714000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/object_detection/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.714000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/video_classification/Dockerfile
+-rw-r--r--   0        0        0       64 2023-03-21 05:26:30.959000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/video_classification/requirements.txt
+-rw-r--r--   0        0        0     2897 2023-03-21 05:26:30.959000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/video_classification/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.718000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_image_classification/Dockerfile
+-rw-r--r--   0        0        0       63 2023-03-19 14:49:24.718000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_image_classification/requirements.txt
+-rw-r--r--   0        0        0   434332 2023-03-19 14:49:24.718000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_image_classification/wrapper/img.png
+-rw-r--r--   0        0        0     2754 2023-03-19 14:49:24.718000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_image_classification/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.718000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_object_detection/Dockerfile
+-rw-r--r--   0        0        0       64 2023-03-19 14:49:24.719000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_object_detection/requirements.txt
+-rw-r--r--   0        0        0   173131 2023-03-19 14:49:24.719000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_object_detection/wrapper/cat.jpg
+-rw-r--r--   0        0        0     2914 2023-03-19 14:49:24.719000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_object_detection/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-21 05:26:30.959000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/multimodal/document_question_answering/Dockerfile
+-rw-r--r--   0        0        0       75 2023-03-21 05:26:30.960000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/multimodal/document_question_answering/requirements.txt
+-rw-r--r--   0        0        0    76876 2023-03-21 05:26:30.960000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/multimodal/document_question_answering/wrapper/doc.png
+-rw-r--r--   0        0        0     2747 2023-03-21 05:26:30.960000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/multimodal/document_question_answering/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-21 05:26:30.960000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/multimodal/feature_extraction/Dockerfile
+-rw-r--r--   0        0        0       63 2023-03-21 05:26:30.961000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/multimodal/feature_extraction/requirements.txt
+-rw-r--r--   0        0        0     2404 2023-03-21 05:26:30.961000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/multimodal/feature_extraction/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-21 05:26:30.961000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/multimodal/image_to_text/Dockerfile
+-rw-r--r--   0        0        0       75 2023-03-21 05:26:30.961000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/multimodal/image_to_text/requirements.txt
+-rw-r--r--   0        0        0   173131 2023-03-21 05:26:30.962000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/multimodal/image_to_text/wrapper/cat.jpg
+-rw-r--r--   0        0        0     2454 2023-03-21 05:26:30.962000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/multimodal/image_to_text/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-21 05:26:30.962000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/multimodal/visual_question_answering/Dockerfile
+-rw-r--r--   0        0        0       75 2023-03-21 05:26:30.962000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/multimodal/visual_question_answering/requirements.txt
+-rw-r--r--   0        0        0   173131 2023-03-21 05:26:30.963000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/multimodal/visual_question_answering/wrapper/cat.jpg
+-rw-r--r--   0        0        0     2780 2023-03-21 05:26:30.963000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/multimodal/visual_question_answering/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.719000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/conversational/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.719000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/conversational/requirements.txt
+-rw-r--r--   0        0        0     2486 2023-03-19 14:49:24.719000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/conversational/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.719000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/fill_mask/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.719000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/fill_mask/requirements.txt
+-rw-r--r--   0        0        0     2386 2023-03-19 14:49:24.719000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/fill_mask/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.720000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/question_answering/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.720000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/question_answering/requirements.txt
+-rw-r--r--   0        0        0     2641 2023-03-19 14:49:24.720000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/question_answering/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-02 05:19:51.937000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/sentiment-analysis/Dockerfile
+-rw-r--r--   0        0        0      435 2023-03-02 05:19:51.937000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/sentiment-analysis/README.md
+-rw-r--r--   0        0        0       63 2023-03-02 05:19:51.938000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/sentiment-analysis/requirements.txt
+-rw-r--r--   0        0        0     2475 2023-03-19 14:49:24.720000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/sentiment-analysis/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.720000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/summarization/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.720000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/summarization/requirements.txt
+-rw-r--r--   0        0        0     3602 2023-03-19 14:49:24.720000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/summarization/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.720000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/table_question_answering/Dockerfile
+-rw-r--r--   0        0        0       92 2023-03-19 14:49:24.720000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/table_question_answering/requirements.txt
+-rw-r--r--   0        0        0     2832 2023-03-19 14:49:24.720000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/table_question_answering/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.720000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/text2text_generation/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.720000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/text2text_generation/requirements.txt
+-rw-r--r--   0        0        0     2410 2023-03-19 14:49:24.721000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/text2text_generation/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-02 05:19:51.938000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_classification/Dockerfile
+-rw-r--r--   0        0        0       64 2023-03-02 05:19:51.938000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_classification/requirements.txt
+-rw-r--r--   0        0        0        4 2023-06-06 06:46:33.750677 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_classification/wrapper/packages.txt
+-rw-r--r--   0        0        0       64 2023-03-02 05:19:51.938000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_classification/wrapper/requirements.txt
+-rw-r--r--   0        0        0     2421 2023-03-19 14:49:24.721000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_classification/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.721000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_generation/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.721000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_generation/requirements.txt
+-rw-r--r--   0        0        0     2678 2023-03-19 14:49:24.721000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_generation/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.721000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/token_classification/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.721000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/token_classification/requirements.txt
+-rw-r--r--   0        0        0     2523 2023-03-19 14:49:24.721000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/token_classification/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.721000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/translation/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.721000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/translation/requirements.txt
+-rw-r--r--   0        0        0     2392 2023-03-19 14:49:24.721000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/translation/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.721000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/zero_shot_classification/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.721000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/zero_shot_classification/requirements.txt
+-rw-r--r--   0        0        0     2711 2023-03-19 14:49:24.722000 pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/nlp/zero_shot_classification/wrapper/wrapper.py
+-rw-r--r--   0        0        0        6 2023-03-06 07:33:04.130000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/requirements.txt
+-rw-r--r--   0        0        0     3701 2023-03-06 08:14:31.141000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.dockerignore
+-rw-r--r--   0        0        0       75 2023-03-06 08:14:31.141000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.gitattributes
+-rw-r--r--   0        0        0     2938 2023-03-06 08:14:31.141000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      280 2023-03-06 08:14:31.141000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1803 2023-03-06 08:14:31.141000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0     1149 2023-03-06 08:14:31.141000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/ISSUE_TEMPLATE/question.yml
+-rw-r--r--   0        0        0      693 2023-03-06 08:14:31.141000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      441 2023-03-06 08:14:31.141000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/dependabot.yml
+-rw-r--r--   0        0        0     6789 2023-03-23 14:04:01.875000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/ci-testing.yml
+-rw-r--r--   0        0        0     2051 2023-03-06 08:14:31.142000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1572 2023-03-06 08:14:31.142000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/docker.yml
+-rw-r--r--   0        0        0     5434 2023-03-06 08:14:31.142000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/greetings.yml
+-rw-r--r--   0        0        0     2014 2023-03-06 08:14:31.142000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/stale.yml
+-rw-r--r--   0        0        0      707 2023-03-06 08:14:31.142000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/translate-readme.yml
+-rwxr-xr-x   0        0        0     3998 2023-03-06 08:14:31.142000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.gitignore
+-rw-r--r--   0        0        0     1747 2023-03-06 08:14:31.142000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      392 2023-03-06 08:14:31.142000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/CITATION.cff
+-rw-r--r--   0        0        0     4999 2023-03-06 08:14:31.142000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/CONTRIBUTING.md
+-rw-r--r--   0        0        0    35127 2023-03-06 08:14:31.142000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/LICENSE
+-rw-r--r--   0        0        0    40553 2023-03-06 08:14:31.142000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/README.md
+-rw-r--r--   0        0        0    39592 2023-03-06 08:14:31.143000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/README.zh-CN.md
+-rw-r--r--   0        0        0     7830 2023-03-06 08:14:31.143000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/benchmarks.py
+-rw-r--r--   0        0        0    11730 2023-03-06 08:14:31.143000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/predict.py
+-rw-r--r--   0        0        0    16383 2023-05-26 01:51:19.920034 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/train.py
+-rw-r--r--   0        0        0   103520 2023-03-06 08:14:31.143000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/tutorial.ipynb
+-rw-r--r--   0        0        0     8056 2023-03-06 08:14:31.143000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/val.py
+-rw-r--r--   0        0        0     2733 2023-03-06 08:14:31.144000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/Argoverse.yaml
+-rw-r--r--   0        0        0     1885 2023-03-06 08:14:31.144000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/GlobalWheat2020.yaml
+-rw-r--r--   0        0        0    18871 2023-03-06 08:14:31.144000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/ImageNet.yaml
+-rw-r--r--   0        0        0     9205 2023-03-06 08:14:31.144000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/Objects365.yaml
+-rw-r--r--   0        0        0     2341 2023-03-06 08:14:31.144000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/SKU-110K.yaml
+-rw-r--r--   0        0        0     3493 2023-03-06 08:14:31.144000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/VOC.yaml
+-rw-r--r--   0        0        0     2971 2023-03-06 08:14:31.144000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/VisDrone.yaml
+-rw-r--r--   0        0        0     2495 2023-03-06 08:14:31.144000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/coco.yaml
+-rw-r--r--   0        0        0     1868 2023-03-06 08:14:31.144000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/coco128-seg.yaml
+-rw-r--r--   0        0        0     1852 2023-03-06 08:14:31.144000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/coco128.yaml
+-rw-r--r--   0        0        0      673 2023-03-06 08:14:31.144000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.Objects365.yaml
+-rw-r--r--   0        0        0     1156 2023-03-06 08:14:31.144000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.VOC.yaml
+-rw-r--r--   0        0        0     1684 2023-03-06 08:14:31.144000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.no-augmentation.yaml
+-rw-r--r--   0        0        0     1683 2023-03-06 08:14:31.144000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.scratch-high.yaml
+-rw-r--r--   0        0        0     1691 2023-03-06 08:14:31.145000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.scratch-low.yaml
+-rw-r--r--   0        0        0     1685 2023-03-06 08:14:31.145000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.scratch-med.yaml
+-rw-r--r--   0        0        0   487438 2023-03-06 08:14:31.145000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/images/bus.jpg
+-rw-r--r--   0        0        0   168949 2023-03-06 08:14:31.146000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/images/zidane.jpg
+-rwxr-xr-x   0        0        0      640 2023-03-06 08:14:31.146000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/download_weights.sh
+-rwxr-xr-x   0        0        0     1566 2023-03-06 08:14:31.146000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/get_coco.sh
+-rwxr-xr-x   0        0        0      618 2023-03-06 08:14:31.146000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/get_coco128.sh
+-rwxr-xr-x   0        0        0     1671 2023-03-06 08:14:31.146000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/get_imagenet.sh
+-rw-r--r--   0        0        0     5170 2023-03-06 08:14:31.146000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/xView.yaml
+-rw-r--r--   0        0        0    14292 2023-03-06 08:14:31.146000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/detect.py
+-rw-r--r--   0        0        0    32063 2023-05-26 01:51:19.911068 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/export.py
+-rw-r--r--   0        0        0     7767 2023-05-26 01:51:19.923788 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/hubconf.py
+-rw-r--r--   0        0        0        0 2023-03-06 08:14:31.147000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/__init__.py
+-rw-r--r--   0        0        0    41702 2023-03-06 08:14:31.147000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/common.py
+-rw-r--r--   0        0        0     4319 2023-03-06 08:14:31.147000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/experimental.py
+-rw-r--r--   0        0        0     3335 2023-03-06 08:14:31.147000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/anchors.yaml
+-rw-r--r--   0        0        0     1567 2023-03-06 08:14:31.147000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov3-spp.yaml
+-rw-r--r--   0        0        0     1232 2023-03-06 08:14:31.147000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov3-tiny.yaml
+-rw-r--r--   0        0        0     1558 2023-03-06 08:14:31.147000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov3.yaml
+-rw-r--r--   0        0        0     1423 2023-03-06 08:14:31.147000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-bifpn.yaml
+-rw-r--r--   0        0        0     1214 2023-03-06 08:14:31.147000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-fpn.yaml
+-rw-r--r--   0        0        0     1687 2023-03-06 08:14:31.147000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p2.yaml
+-rw-r--r--   0        0        0     1349 2023-03-06 08:14:31.147000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p34.yaml
+-rw-r--r--   0        0        0     1741 2023-03-06 08:14:31.147000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p6.yaml
+-rw-r--r--   0        0        0     2122 2023-03-06 08:14:31.148000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p7.yaml
+-rw-r--r--   0        0        0     1407 2023-03-06 08:14:31.148000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-panet.yaml
+-rw-r--r--   0        0        0     1820 2023-03-06 08:14:31.148000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5l6.yaml
+-rw-r--r--   0        0        0     1822 2023-03-06 08:14:31.148000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5m6.yaml
+-rw-r--r--   0        0        0     1822 2023-03-06 08:14:31.148000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5n6.yaml
+-rw-r--r--   0        0        0     1497 2023-03-06 08:14:31.148000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s-LeakyReLU.yaml
+-rw-r--r--   0        0        0     1483 2023-03-06 08:14:31.148000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s-ghost.yaml
+-rw-r--r--   0        0        0     1441 2023-03-06 08:14:31.148000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s-transformer.yaml
+-rw-r--r--   0        0        0     1822 2023-03-06 08:14:31.148000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s6.yaml
+-rw-r--r--   0        0        0     1822 2023-03-06 08:14:31.148000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5x6.yaml
+-rw-r--r--   0        0        0     1411 2023-03-06 08:14:31.148000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5l-seg.yaml
+-rw-r--r--   0        0        0     1413 2023-03-06 08:14:31.148000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5m-seg.yaml
+-rw-r--r--   0        0        0     1413 2023-03-06 08:14:31.148000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5n-seg.yaml
+-rw-r--r--   0        0        0     1412 2023-03-06 08:14:31.148000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5s-seg.yaml
+-rw-r--r--   0        0        0     1413 2023-03-06 08:14:31.148000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5x-seg.yaml
+-rw-r--r--   0        0        0    27032 2023-05-26 01:51:19.958775 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/tf.py
+-rw-r--r--   0        0        0    17780 2023-05-26 01:51:19.931156 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolo.py
+-rw-r--r--   0        0        0     1401 2023-03-06 08:14:31.149000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5l.yaml
+-rw-r--r--   0        0        0     1403 2023-03-06 08:14:31.149000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5m.yaml
+-rw-r--r--   0        0        0     1403 2023-03-06 08:14:31.149000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5n.yaml
+-rw-r--r--   0        0        0     1403 2023-03-06 08:14:31.149000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5s.yaml
+-rw-r--r--   0        0        0     1403 2023-03-06 08:14:31.149000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5x.yaml
+-rw-r--r--   0        0        0     1593 2023-03-06 08:14:31.149000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/requirements.txt
+-rw-r--r--   0        0        0    15743 2023-03-06 08:14:31.149000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/predict.py
+-rw-r--r--   0        0        0    34678 2023-03-23 14:04:01.875000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/train.py
+-rw-r--r--   0        0        0    43293 2023-03-06 08:14:31.150000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/tutorial.ipynb
+-rw-r--r--   0        0        0    24005 2023-03-06 08:14:31.150000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/val.py
+-rw-r--r--   0        0        0     1727 2023-03-06 08:14:31.150000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/setup.cfg
+-rw-r--r--   0        0        0    33701 2023-03-06 08:14:31.150000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/train.py
+-rw-r--r--   0        0        0    54258 2023-03-06 08:14:31.150000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/tutorial.ipynb
+-rw-r--r--   0        0        0     2432 2023-03-06 08:14:31.150000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/__init__.py
+-rw-r--r--   0        0        0     3449 2023-03-06 08:14:31.151000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/activations.py
+-rw-r--r--   0        0        0    17030 2023-03-06 08:14:31.151000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/augmentations.py
+-rw-r--r--   0        0        0     7420 2023-03-06 08:14:31.151000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/autoanchor.py
+-rw-r--r--   0        0        0     3003 2023-05-26 01:51:19.914199 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/autobatch.py
+-rw-r--r--   0        0        0        0 2023-03-06 08:14:31.151000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/aws/__init__.py
+-rw-r--r--   0        0        0      780 2023-03-06 08:14:31.151000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/aws/mime.sh
+-rw-r--r--   0        0        0     1198 2023-03-06 08:14:31.151000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/aws/resume.py
+-rw-r--r--   0        0        0     1247 2023-03-06 08:14:31.151000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/aws/userdata.sh
+-rw-r--r--   0        0        0     2661 2023-03-06 08:14:31.151000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/callbacks.py
+-rw-r--r--   0        0        0    55779 2023-05-26 01:51:19.947412 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/dataloaders.py
+-rw-r--r--   0        0        0     2709 2023-03-06 08:14:31.152000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/docker/Dockerfile
+-rw-r--r--   0        0        0     1682 2023-03-06 08:14:31.152000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/docker/Dockerfile-arm64
+-rw-r--r--   0        0        0     1707 2023-03-06 08:14:31.152000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/docker/Dockerfile-cpu
+-rw-r--r--   0        0        0     4952 2023-03-06 08:14:31.152000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/downloads.py
+-rw-r--r--   0        0        0     1710 2023-03-06 08:14:31.152000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/flask_rest_api/README.md
+-rw-r--r--   0        0        0      368 2023-03-06 08:14:31.152000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/flask_rest_api/example_request.py
+-rw-r--r--   0        0        0     1439 2023-03-06 08:14:31.152000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/flask_rest_api/restapi.py
+-rw-r--r--   0        0        0    46844 2023-03-06 08:14:31.152000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/general.py
+-rw-r--r--   0        0        0      821 2023-03-06 08:14:31.152000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/google_app_engine/Dockerfile
+-rw-r--r--   0        0        0      187 2023-03-06 08:14:31.152000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/google_app_engine/additional_requirements.txt
+-rw-r--r--   0        0        0      174 2023-03-06 08:14:31.153000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/google_app_engine/app.yaml
+-rw-r--r--   0        0        0    16635 2023-03-06 08:14:31.153000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/__init__.py
+-rw-r--r--   0        0        0    10862 2023-03-06 08:14:31.153000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/clearml/README.md
+-rw-r--r--   0        0        0        0 2023-03-06 08:14:31.153000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/clearml/__init__.py
+-rw-r--r--   0        0        0     8034 2023-03-06 08:14:31.153000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/clearml/clearml_utils.py
+-rw-r--r--   0        0        0     5271 2023-03-06 08:14:31.153000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/clearml/hpo.py
+-rw-r--r--   0        0        0    10772 2023-03-06 08:14:31.153000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/README.md
+-rw-r--r--   0        0        0    18731 2023-03-06 08:14:31.153000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/__init__.py
+-rw-r--r--   0        0        0     4751 2023-03-06 08:14:31.153000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/comet_utils.py
+-rw-r--r--   0        0        0     6653 2023-03-06 08:14:31.153000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/hpo.py
+-rw-r--r--   0        0        0        0 2023-03-06 08:14:31.153000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/wandb/__init__.py
+-rw-r--r--   0        0        0     8252 2023-03-06 08:14:31.154000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/wandb/wandb_utils.py
+-rw-r--r--   0        0        0     9919 2023-03-06 08:14:31.154000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loss.py
+-rw-r--r--   0        0        0    14568 2023-03-06 08:14:31.154000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/metrics.py
+-rw-r--r--   0        0        0    24501 2023-05-26 01:51:19.940339 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/plots.py
+-rw-r--r--   0        0        0        0 2023-03-06 08:14:31.154000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/__init__.py
+-rw-r--r--   0        0        0     3756 2023-03-06 08:14:31.154000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/augmentations.py
+-rw-r--r--   0        0        0    13835 2023-03-06 08:14:31.154000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/dataloaders.py
+-rw-r--r--   0        0        0     5813 2023-03-23 14:04:01.876000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/general.py
+-rw-r--r--   0        0        0     8591 2023-03-23 14:04:01.876000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/loss.py
+-rw-r--r--   0        0        0     5457 2023-03-06 08:14:31.154000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/metrics.py
+-rw-r--r--   0        0        0     6386 2023-03-23 14:04:01.876000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/plots.py
+-rw-r--r--   0        0        0    19655 2023-05-26 01:51:19.900763 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/torch_utils.py
+-rw-r--r--   0        0        0     3634 2023-03-06 08:14:31.155000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/triton.py
+-rw-r--r--   0        0        0    20424 2023-03-06 08:14:31.155000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/val.py
+-rw-r--r--   0        0        0     4932 2023-03-06 08:24:07.583000 pyatp-1.1.2/src/ailab/inference_wrapper/yolo/wrapper/yolov5/wrapper.py
+-rw-r--r--   0        0        0     2007 2023-05-26 01:43:21.934000 pyatp-1.1.2/src/ailab/templates/README.md
+-rw-r--r--   0        0        0      542 2023-05-26 01:43:21.934000 pyatp-1.1.2/src/ailab/templates/alpaca.json
+-rw-r--r--   0        0        0      561 2023-05-26 01:43:21.934000 pyatp-1.1.2/src/ailab/templates/alpaca_legacy.json
+-rw-r--r--   0        0        0      281 2023-05-26 01:43:21.934000 pyatp-1.1.2/src/ailab/templates/alpaca_short.json
+-rw-r--r--   0        0        0      605 2023-05-26 01:43:21.934000 pyatp-1.1.2/src/ailab/templates/vigogne.json
+-rw-r--r--   0        0        0      239 2023-05-29 01:38:01.672199 pyatp-1.1.2/src/ailab/utils/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 01:38:01.672232 pyatp-1.1.2/src/ailab/utils/__init__.py
+-rw-r--r--   0        0        0     2384 2023-06-01 08:42:34.256596 pyatp-1.1.2/src/ailab/utils/callbacks.py
+-rw-r--r--   0        0        0     1669 2023-05-29 01:38:01.672407 pyatp-1.1.2/src/ailab/utils/prompter.py
+-rw-r--r--   0        0        0    33918 2023-05-29 01:38:01.672647 pyatp-1.1.2/src/ailab/utils/streampeft.py
+-rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 pyatp-1.1.2/PKG-INFO
```

### Comparing `pyatp-1.1.1/src/atp/error.py` & `pyatp-1.1.2/src/ailab/inference_wrapper/huggingface/transformers/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # coding:utf-8
 """ 
 @author: nivic ybyang7
 @license: Apache Licence 
-@file: config
-@time: 2022/10/31
+@file: __init__.py
+@time: 2023/06/05
 @contact: ybyang7@iflytek.com
 @site:  
 @software: PyCharm 
 
 # code is far away from bugs with the god animal protecting
     I love animals. They taste delicious.
               ┏┓      ┏┓
@@ -21,22 +21,12 @@
                 ┃  神兽保佑    ┣┓
                 ┃　永无BUG！   ┏┛
                 ┗┓┓┏━┳┓┏┛
                   ┃┫┫  ┃┫┫
                   ┗┻┛  ┗┻┛ 
 """
 
-
 #  Copyright (c) 2022. Lorem ipsum dolor sit amet, consectetur adipiscing elit.
 #  Morbi non lorem porttitor neque feugiat blandit. Ut vitae ipsum eget quam lacinia accumsan.
 #  Etiam sed turpis ac ipsum condimentum fringilla. Maecenas magna.
 #  Proin dapibus sapien vel ante. Aliquam erat volutpat. Pellentesque sagittis ligula eget metus.
 #  Vestibulum commodo. Ut rhoncus gravida arcu.
-
-
-class NoSuchModelError(Exception):
-    def __init__(self, errinfo):
-        super().__init__(self)  # 初始化父类
-        self.errorinfo = errinfo
-
-    def __str__(self):
-        return self.errorinfo
```

### Comparing `pyatp-1.1.1/src/atp/huggingface/datasets.py` & `pyatp-1.1.2/src/ailab/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # coding:utf-8
 """ 
 @author: nivic ybyang7
 @license: Apache Licence 
-@file: datasets.py
-@time: 2023/02/23
+@file: __init__.py
+@time: 2023/05/26
 @contact: ybyang7@iflytek.com
 @site:  
 @software: PyCharm 
 
 # code is far away from bugs with the god animal protecting
     I love animals. They taste delicious.
               ┏┓      ┏┓
```

### Comparing `pyatp-1.1.1/src/atp/pretrain/__init__.py` & `pyatp-1.1.2/src/ailab/buildkit/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # coding:utf-8
 """ 
 @author: nivic ybyang7
 @license: Apache Licence 
-@file: __init__.py
-@time: 2022/10/31
+@file: __init__
+@time: 2023/06/02
 @contact: ybyang7@iflytek.com
 @site:  
 @software: PyCharm 
 
 # code is far away from bugs with the god animal protecting
     I love animals. They taste delicious.
               ┏┓      ┏┓
@@ -26,9 +26,7 @@
 """
 
 #  Copyright (c) 2022. Lorem ipsum dolor sit amet, consectetur adipiscing elit.
 #  Morbi non lorem porttitor neque feugiat blandit. Ut vitae ipsum eget quam lacinia accumsan.
 #  Etiam sed turpis ac ipsum condimentum fringilla. Maecenas magna.
 #  Proin dapibus sapien vel ante. Aliquam erat volutpat. Pellentesque sagittis ligula eget metus.
 #  Vestibulum commodo. Ut rhoncus gravida arcu.
-
-
```

### Comparing `pyatp-1.1.1/src/atp/pretrain/av2vec/__init__.py` & `pyatp-1.1.2/src/ailab/inference_wrapper/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # coding:utf-8
 """ 
 @author: nivic ybyang7
 @license: Apache Licence 
-@file: __init__.py
-@time: 2022/10/31
+@file: __init__
+@time: 2023/06/05
 @contact: ybyang7@iflytek.com
 @site:  
 @software: PyCharm 
 
 # code is far away from bugs with the god animal protecting
     I love animals. They taste delicious.
               ┏┓      ┏┓
```

