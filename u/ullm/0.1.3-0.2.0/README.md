# Comparing `tmp/ullm-0.1.3.tar.gz` & `tmp/ullm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ullm-0.1.3.tar", last modified: Fri May 10 05:36:31 2024, max compression
+gzip compressed data, was "ullm-0.2.0.tar", last modified: Wed May 15 03:05:51 2024, max compression
```

## Comparing `ullm-0.1.3.tar` & `ullm-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:36:31.579472 ullm-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    17699 2024-05-10 05:36:31.579472 ullm-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16928 2024-05-10 05:36:22.000000 ullm-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-10 05:36:22.000000 ullm-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 05:36:31.579472 ullm-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:36:31.575472 ullm-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-10 05:36:22.000000 ullm-0.1.3/tests/test_openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:36:31.579472 ullm-0.1.3/ullm/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/alibaba.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/baichuan.py
--rw-r--r--   0 runner    (1001) docker     (127)    23260 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/baidu.py
--rw-r--r--   0 runner    (1001) docker     (127)    19510 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/deepseek.py
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/iflytek.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/minimax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/moonshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)    14266 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/openrouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/stepfun.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/zero_one.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-10 05:36:22.000000 ullm-0.1.3/ullm/zhipu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:36:31.579472 ullm-0.1.3/ullm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17699 2024-05-10 05:36:31.000000 ullm-0.1.3/ullm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-10 05:36:31.000000 ullm-0.1.3/ullm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 05:36:31.000000 ullm-0.1.3/ullm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 05:36:31.000000 ullm-0.1.3/ullm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-10 05:36:31.000000 ullm-0.1.3/ullm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 05:36:31.000000 ullm-0.1.3/ullm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:05:51.079203 ullm-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    18344 2024-05-15 03:05:51.079203 ullm-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17549 2024-05-15 03:05:47.000000 ullm-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-15 03:05:47.000000 ullm-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 03:05:51.079203 ullm-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:05:51.071203 ullm-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-15 03:05:47.000000 ullm-0.2.0/tests/test_openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:05:51.079203 ullm-0.2.0/ullm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/alibaba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/baichuan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23260 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19678 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/deepseek.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/iflytek.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/minimax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/moonshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14332 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8432 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/openrouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/skywork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/stepfun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/together.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/zero_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-15 03:05:47.000000 ullm-0.2.0/ullm/zhipu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:05:51.079203 ullm-0.2.0/ullm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18344 2024-05-15 03:05:51.000000 ullm-0.2.0/ullm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-15 03:05:51.000000 ullm-0.2.0/ullm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 03:05:51.000000 ullm-0.2.0/ullm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 03:05:51.000000 ullm-0.2.0/ullm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-15 03:05:51.000000 ullm-0.2.0/ullm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 03:05:51.000000 ullm-0.2.0/ullm.egg-info/top_level.txt
```

### Comparing `ullm-0.1.3/PKG-INFO` & `ullm-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ullm
-Version: 0.1.3
+Version: 0.2.0
 Summary: A unified interface for local Large Language Model(LLM) models and online LLM providers.
 Author-email: Linusp <linusp1024@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/monsternlp/ullm
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -14,20 +14,21 @@
 Requires-Dist: arrow
 Requires-Dist: websocket-client
 Requires-Dist: requests
 Requires-Dist: python-magic
 Requires-Dist: click
 Requires-Dist: deepmerge
 Requires-Dist: jsonschema
+Requires-Dist: tabulate
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 <h1 align="center">ullm</h1>
-<p align="center">A unified interface for local Large Language Model(LLM) models and online LLM providers.</p>
+<p align="center">A unified interface for local Large Language Models(LLM) and online LLM providers.</p>
 <h4 align="center">
     <a href="https://pypi.org/project/ullm/" target="_blank">
         <img src="https://shields.io/pypi/v/ullm.svg" alt="PyPI Version">
     </a>
     <a href="https://github.com/monsternlp/ullm/actions/workflows/pre-commit.yaml" target="_blank">
         <img src="https://shields.io/github/actions/workflow/status/monsternlp/ullm/pre-commit.yaml?label=pre-commit" alt="Pre-commit status">
     </a>
@@ -65,20 +66,22 @@
   - [print-example](#print-example)
   - [chat](#chat)
 
 <!-- /TOC -->
 
 ## 功能与特性
 
-- 支持 OpenAI 等 18 个在线 LLM 服务，详见「[在线服务](#在线服务)」一节
+- 支持 OpenAI 等 21 个在线 LLM 服务，详见「[在线服务](#在线服务)」一节
 - 支持和 OpenAI 接口兼容的自建服务
 - 支持 Ollama API
 - 配置化的使用方式，为所有不同模型及服务提供统一的初始化方式，详见「[使用](#使用)」一节
 - [ ] 本地模型支持
+- [ ] 归一化模型名称
 - [ ] 为所有模型支持工具调用（对原本不支持的通过自定义 prompt 模板实现）
+- [ ] 为不同模型适配对应的 tokenizer，以获得 tokens 数量解决某些 remote model 不返回 tokens 数量的问题
 - [ ] 模型配置的管理
 - [ ] 多模型路由
 - [ ] 单元测试
 - [ ] 完善文档
 - [ ] 实现流式接口
 
 ## 支持模型
@@ -93,25 +96,28 @@
 |------|-------------------|----------|--------------|------------------------|--------------|
 | [零一万物](https://platform.lingyiwanwu.com/docs)     | 01ai              |        3 |            1 |                      0 |            0 |
 | [阿里巴巴](https://help.aliyun.com/zh/dashscope/developer-reference/model-square/?spm=a2c4g.11186623.0.0.1cca23edHYSGqT)      | alibaba           |       44 |            4 |                      6 |            6 |
 | [Anthropic](https://docs.anthropic.com/claude/reference/getting-started-with-the-api)     | anthropic         |        3 |            3 |                      3 |            0 |
 | [Azure OpenAI](https://learn.microsoft.com/en-us/azure/ai-services/openai/reference#chat-completions)     | azure-openai      |       20 |            4 |                     11 |            0 |
 | [百川智能](https://platform.baichuan-ai.com/docs/api)     | baichuan          |        4 |            0 |                      0 |            2 |
 | [百度](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Nlks5zkzu)     | baidu             |       46 |            0 |                     24 |           12 |
+| [Cloudflare Workers AI](https://developers.cloudflare.com/workers-ai/get-started/rest-api/) | cloudflare        |       35 |               0 |             0 |               0 |
 | [Cohere](https://docs.cohere.com/reference/about)     | cohere            |       12 |            0 |                      4 |            6 |
 | [DeepSeek](https://platform.deepseek.com/docs)     | deepseek          |        2 |            0 |                      0 |            0 |
 | [Google](https://ai.google.dev/gemini-api/docs)     | google            |        3 |            2 |                      2 |            0 |
 | [Groq](https://console.groq.com/docs/quickstart)     | groq              |        4 |            0 |                      4 |            0 |
 | [科大讯飞](https://www.xfyun.cn/doc/spark/%E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E.html)     | iflytek           |        4 |            0 |                      2 |            0 |
 | [MiniMax](https://www.minimaxi.com/document/algorithm-concept?id=6433f37594878d408fc8295d)     | minimax           |        5 |            0 |                      5 |            0 |
 | [Moonshot](https://platform.moonshot.cn/docs/api/chat#%E5%9F%BA%E6%9C%AC%E4%BF%A1%E6%81%AF)     | moonshot          |        3 |            0 |                      3 |            0 |
 | [OpenAI](https://platform.openai.com/docs/api-reference/chat)      | openai            |       20 |            4 |                     11 |            0 |
 | [OpenRouter](https://openrouter.ai/docs)     | openrouter        |      127 |           13 |                    127 |            4 |
 | [Perplexity](https://docs.perplexity.ai/docs/getting-started)     | perplexity        |        7 |            0 |                      0 |            2 |
+| [天工](https://model-platform.tiangong.cn/api-reference) | skywork           |        1 |               0 |             0 |               0 |
 | [阶跃星辰](https://platform.stepfun.com/docs/Chat/chat-completion-create)     | stepfun           |        3 |            1 |                      0 |            0 |
+| [Together AI](https://docs.together.ai/docs/quickstart) | together          |       58 |               0 |            58 |               0 |
 | [智谱](https://open.bigmodel.cn/dev/api)     | zhipu             |        5 |            1 |                      4 |            2 |
 | OpenAI 接口兼容的服务     | openai-compatible |          |              |                        |              |
 | Ollama API     | ollama            |          |              |                        |              |
 
 
 ## 安装
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: ullm Version: 0.1.3 Summary: A unified interface
+Metadata-Version: 2.1 Name: ullm Version: 0.2.0 Summary: A unified interface
 for local Large Language Model(LLM) models and online LLM providers. Author-
 email: Linusp
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/monsternlp/
 ullm Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.8 Description-Content-Type: text/markdown Requires-Dist: pydantic
 Requires-Dist: arrow Requires-Dist: websocket-client Requires-Dist: requests
 Requires-Dist: python-magic Requires-Dist: click Requires-Dist: deepmerge
-Requires-Dist: jsonschema Provides-Extra: test Requires-Dist: pytest; extra ==
-"test" Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: jsonschema Requires-Dist: tabulate Provides-Extra: test
+Requires-Dist: pytest; extra == "test" Requires-Dist: pytest-cov; extra ==
+"test"
                               ************ uullllmm ************
- A unified interface for local Large Language Model(LLM) models and online LLM
+    A unified interface for local Large Language Models(LLM) and online LLM
                                   providers.
             ****** _[[_PP_yy_PP_II_ _VV_ee_rr_ss_ii_oo_nn_]]_[[_PP_rr_ee_--_cc_oo_mm_mm_ii_tt_ _ss_tt_aa_tt_uu_ss_]]_[[_BB_uu_ii_ll_dd_ _ss_tt_aa_tt_uu_ss_]] ******
 ullm å¸æè½ä¸ºæ¬å°æ¨¡åä»¥åä¼å¤å¨çº¿ LLM
 æå¡æä¾ç»ä¸çè°ç¨æ¹å¼ï¼ä½¿å¾å¼åèè½å¤æ çå°å¨ä¸åæ¨¡åæ
 LLM æå¡ä¹é´åæ¢ï¼èæ éæ´æ¹ä»£ç ã > [!NOTE] >
 æ¬é¡¹ç®åªä¸æ³¨äºä¸ºä¸å LLM
 æ¨¡åææå¡çåºç¡çæåè½æä¾ç»ä¸æ¥å£ï¼åæ¬éç¨ççæãèå¤©æ¥å£ä»¥åæåºç¡çå·¥å·è°ç¨ãè§è§çè§£åè½ï¼å¨æ­¤ä¹å¤çå¶ä»ç¸å³åè½å¦
@@ -25,53 +26,59 @@
 [åè½ä¸ç¹æ§](#åè½ä¸ç¹æ§) - [æ¯ææ¨¡å](#æ¯ææ¨¡å) -
 [æ¬å°æ¨¡å](#æ¬å°æ¨¡å) - [å¨çº¿æå¡](#å¨çº¿æå¡) - [å®è£]
 (#å®è£) - [ä½¿ç¨](#ä½¿ç¨) - [åå»ºæ¨¡åéç½®](#åå»ºæ¨¡åéç½®) -
 [å®ä¾åæ¨¡å](#å®ä¾åæ¨¡å) - [è®¾ç½®çæåæ°](#è®¾ç½®çæåæ°)
 - [çæææ¬](#çæææ¬) - [èå¤©](#èå¤©) - [å½ä»¤è¡](#å½ä»¤è¡) -
 [list-providers](#list-providers) - [list-models](#list-models) - [print-
 example](#print-example) - [chat](#chat) ## åè½ä¸ç¹æ§ - æ¯æ OpenAI ç­
-18 ä¸ªå¨çº¿ LLM æå¡ï¼è¯¦è§ã[å¨çº¿æå¡](#å¨çº¿æå¡)ãä¸è -
+21 ä¸ªå¨çº¿ LLM æå¡ï¼è¯¦è§ã[å¨çº¿æå¡](#å¨çº¿æå¡)ãä¸è -
 æ¯æå OpenAI æ¥å£å¼å®¹çèªå»ºæå¡ - æ¯æ Ollama API -
 éç½®åçä½¿ç¨æ¹å¼ï¼ä¸ºææä¸åæ¨¡ååæå¡æä¾ç»ä¸çåå§åæ¹å¼ï¼è¯¦è§ã
-[ä½¿ç¨](#ä½¿ç¨)ãä¸è - [ ] æ¬å°æ¨¡åæ¯æ - [ ]
-ä¸ºæææ¨¡åæ¯æå·¥å·è°ç¨ï¼å¯¹åæ¬ä¸æ¯æçéè¿èªå®ä¹ prompt
-æ¨¡æ¿å®ç°ï¼ - [ ] æ¨¡åéç½®çç®¡ç - [ ] å¤æ¨¡åè·¯ç± - [ ]
+[ä½¿ç¨](#ä½¿ç¨)ãä¸è - [ ] æ¬å°æ¨¡åæ¯æ - [ ] å½ä¸åæ¨¡ååç§°
+- [ ] ä¸ºæææ¨¡åæ¯æå·¥å·è°ç¨ï¼å¯¹åæ¬ä¸æ¯æçéè¿èªå®ä¹
+prompt æ¨¡æ¿å®ç°ï¼ - [ ] ä¸ºä¸åæ¨¡åééå¯¹åºç
+tokenizerï¼ä»¥è·å¾ tokens æ°éè§£å³æäº remote model ä¸è¿å tokens
+æ°éçé®é¢ - [ ] æ¨¡åéç½®çç®¡ç - [ ] å¤æ¨¡åè·¯ç± - [ ]
 ååæµè¯ - [ ] å®åææ¡£ - [ ] å®ç°æµå¼æ¥å£ ## æ¯ææ¨¡å ###
 æ¬å°æ¨¡å TBD ### å¨çº¿æå¡ | å¹³å° | Provider ID | æ¨¡åæ°é |
 è§è§æ¨¡åæ°é | æ¯æå·¥å·è°ç¨çæ¨¡åæ°é | èç½æ¨¡åæ°é |
 |------|-------------------|----------|--------------|------------------------
 |--------------| | [é¶ä¸ä¸ç©](https://platform.lingyiwanwu.com/docs) | 01ai
 | 3 | 1 | 0 | 0 | | [é¿éå·´å·´](https://help.aliyun.com/zh/dashscope/
 developer-reference/model-square/?spm=a2c4g.11186623.0.0.1cca23edHYSGqT) |
 alibaba | 44 | 4 | 6 | 6 | | [Anthropic](https://docs.anthropic.com/claude/
 reference/getting-started-with-the-api) | anthropic | 3 | 3 | 3 | 0 | | [Azure
 OpenAI](https://learn.microsoft.com/en-us/azure/ai-services/openai/
 reference#chat-completions) | azure-openai | 20 | 4 | 11 | 0 | | [ç¾å·æºè½]
 (https://platform.baichuan-ai.com/docs/api) | baichuan | 4 | 0 | 0 | 2 | |
 [ç¾åº¦](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Nlks5zkzu) | baidu | 46 |
-0 | 24 | 12 | | [Cohere](https://docs.cohere.com/reference/about) | cohere | 12
-| 0 | 4 | 6 | | [DeepSeek](https://platform.deepseek.com/docs) | deepseek | 2 |
-0 | 0 | 0 | | [Google](https://ai.google.dev/gemini-api/docs) | google | 3 | 2
-| 2 | 0 | | [Groq](https://console.groq.com/docs/quickstart) | groq | 4 | 0 | 4
-| 0 | | [ç§å¤§è®¯é£](https://www.xfyun.cn/doc/spark/
+0 | 24 | 12 | | [Cloudflare Workers AI](https://developers.cloudflare.com/
+workers-ai/get-started/rest-api/) | cloudflare | 35 | 0 | 0 | 0 | | [Cohere]
+(https://docs.cohere.com/reference/about) | cohere | 12 | 0 | 4 | 6 | |
+[DeepSeek](https://platform.deepseek.com/docs) | deepseek | 2 | 0 | 0 | 0 | |
+[Google](https://ai.google.dev/gemini-api/docs) | google | 3 | 2 | 2 | 0 | |
+[Groq](https://console.groq.com/docs/quickstart) | groq | 4 | 0 | 4 | 0 | |
+[ç§å¤§è®¯é£](https://www.xfyun.cn/doc/spark/
 %E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E.html) | iflytek | 4 | 0 | 2 | 0 | |
 [MiniMax](https://www.minimaxi.com/document/algorithm-
 concept?id=6433f37594878d408fc8295d) | minimax | 5 | 0 | 5 | 0 | | [Moonshot]
 (https://platform.moonshot.cn/docs/api/
 chat#%E5%9F%BA%E6%9C%AC%E4%BF%A1%E6%81%AF) | moonshot | 3 | 0 | 3 | 0 | |
 [OpenAI](https://platform.openai.com/docs/api-reference/chat) | openai | 20 | 4
 | 11 | 0 | | [OpenRouter](https://openrouter.ai/docs) | openrouter | 127 | 13 |
 127 | 4 | | [Perplexity](https://docs.perplexity.ai/docs/getting-started) |
-perplexity | 7 | 0 | 0 | 2 | | [é¶è·æè¾°](https://platform.stepfun.com/
-docs/Chat/chat-completion-create) | stepfun | 3 | 1 | 0 | 0 | | [æºè°±](https:
-//open.bigmodel.cn/dev/api) | zhipu | 5 | 1 | 4 | 2 | | OpenAI
-æ¥å£å¼å®¹çæå¡ | openai-compatible | | | | | | Ollama API | ollama | | |
-| | ## å®è£ ```shell pip install ullm ``` ## ä½¿ç¨ ### åå»ºæ¨¡åéç½®
-ç¤ºä¾: ```python model_config = { # required fields "type": 'remote', "model":
-'gpt-3.5-turbo', "provider": 'openai', "api_key": 'sk-
+perplexity | 7 | 0 | 0 | 2 | | [å¤©å·¥](https://model-platform.tiangong.cn/api-
+reference) | skywork | 1 | 0 | 0 | 0 | | [é¶è·æè¾°](https://
+platform.stepfun.com/docs/Chat/chat-completion-create) | stepfun | 3 | 1 | 0 |
+0 | | [Together AI](https://docs.together.ai/docs/quickstart) | together | 58 |
+0 | 58 | 0 | | [æºè°±](https://open.bigmodel.cn/dev/api) | zhipu | 5 | 1 | 4 |
+2 | | OpenAI æ¥å£å¼å®¹çæå¡ | openai-compatible | | | | | | Ollama API |
+ollama | | | | | ## å®è£ ```shell pip install ullm ``` ## ä½¿ç¨ ###
+åå»ºæ¨¡åéç½® ç¤ºä¾: ```python model_config = { # required fields "type":
+'remote', "model": 'gpt-3.5-turbo', "provider": 'openai', "api_key": 'sk-
 ************************************************', # optional fields
 "max_tokens": 4096, "max_input_tokens": 1024, "max_output_tokens": 1024,
 "temperature": 0.8, "top_p": 1.0, "top_k": 50, "stop_sequences": ['stop1',
 'stop2'], "http_proxy": 'https://example-proxy.com', } ```
 æ¨¡åéç½®ä¸­å¿é¡»æå®è¿ä¸ä¸ªå­æ®µ - type: æå®æ¨¡åä¸ºæ¬å°æ¨¡å
 (`local`)è¿æ¯å¨çº¿æ¨¡å(`remote`)ï¼ç®åä»å®ç°äº remote - provider:
 æå®æ¨¡åæä¾æ¹ï¼è§åé¢ã[æ¯ææ¨¡å]
```

### Comparing `ullm-0.1.3/README.md` & `ullm-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <h1 align="center">ullm</h1>
-<p align="center">A unified interface for local Large Language Model(LLM) models and online LLM providers.</p>
+<p align="center">A unified interface for local Large Language Models(LLM) and online LLM providers.</p>
 <h4 align="center">
     <a href="https://pypi.org/project/ullm/" target="_blank">
         <img src="https://shields.io/pypi/v/ullm.svg" alt="PyPI Version">
     </a>
     <a href="https://github.com/monsternlp/ullm/actions/workflows/pre-commit.yaml" target="_blank">
         <img src="https://shields.io/github/actions/workflow/status/monsternlp/ullm/pre-commit.yaml?label=pre-commit" alt="Pre-commit status">
     </a>
@@ -41,20 +41,22 @@
   - [print-example](#print-example)
   - [chat](#chat)
 
 <!-- /TOC -->
 
 ## 功能与特性
 
-- 支持 OpenAI 等 18 个在线 LLM 服务，详见「[在线服务](#在线服务)」一节
+- 支持 OpenAI 等 21 个在线 LLM 服务，详见「[在线服务](#在线服务)」一节
 - 支持和 OpenAI 接口兼容的自建服务
 - 支持 Ollama API
 - 配置化的使用方式，为所有不同模型及服务提供统一的初始化方式，详见「[使用](#使用)」一节
 - [ ] 本地模型支持
+- [ ] 归一化模型名称
 - [ ] 为所有模型支持工具调用（对原本不支持的通过自定义 prompt 模板实现）
+- [ ] 为不同模型适配对应的 tokenizer，以获得 tokens 数量解决某些 remote model 不返回 tokens 数量的问题
 - [ ] 模型配置的管理
 - [ ] 多模型路由
 - [ ] 单元测试
 - [ ] 完善文档
 - [ ] 实现流式接口
 
 ## 支持模型
@@ -69,25 +71,28 @@
 |------|-------------------|----------|--------------|------------------------|--------------|
 | [零一万物](https://platform.lingyiwanwu.com/docs)     | 01ai              |        3 |            1 |                      0 |            0 |
 | [阿里巴巴](https://help.aliyun.com/zh/dashscope/developer-reference/model-square/?spm=a2c4g.11186623.0.0.1cca23edHYSGqT)      | alibaba           |       44 |            4 |                      6 |            6 |
 | [Anthropic](https://docs.anthropic.com/claude/reference/getting-started-with-the-api)     | anthropic         |        3 |            3 |                      3 |            0 |
 | [Azure OpenAI](https://learn.microsoft.com/en-us/azure/ai-services/openai/reference#chat-completions)     | azure-openai      |       20 |            4 |                     11 |            0 |
 | [百川智能](https://platform.baichuan-ai.com/docs/api)     | baichuan          |        4 |            0 |                      0 |            2 |
 | [百度](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Nlks5zkzu)     | baidu             |       46 |            0 |                     24 |           12 |
+| [Cloudflare Workers AI](https://developers.cloudflare.com/workers-ai/get-started/rest-api/) | cloudflare        |       35 |               0 |             0 |               0 |
 | [Cohere](https://docs.cohere.com/reference/about)     | cohere            |       12 |            0 |                      4 |            6 |
 | [DeepSeek](https://platform.deepseek.com/docs)     | deepseek          |        2 |            0 |                      0 |            0 |
 | [Google](https://ai.google.dev/gemini-api/docs)     | google            |        3 |            2 |                      2 |            0 |
 | [Groq](https://console.groq.com/docs/quickstart)     | groq              |        4 |            0 |                      4 |            0 |
 | [科大讯飞](https://www.xfyun.cn/doc/spark/%E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E.html)     | iflytek           |        4 |            0 |                      2 |            0 |
 | [MiniMax](https://www.minimaxi.com/document/algorithm-concept?id=6433f37594878d408fc8295d)     | minimax           |        5 |            0 |                      5 |            0 |
 | [Moonshot](https://platform.moonshot.cn/docs/api/chat#%E5%9F%BA%E6%9C%AC%E4%BF%A1%E6%81%AF)     | moonshot          |        3 |            0 |                      3 |            0 |
 | [OpenAI](https://platform.openai.com/docs/api-reference/chat)      | openai            |       20 |            4 |                     11 |            0 |
 | [OpenRouter](https://openrouter.ai/docs)     | openrouter        |      127 |           13 |                    127 |            4 |
 | [Perplexity](https://docs.perplexity.ai/docs/getting-started)     | perplexity        |        7 |            0 |                      0 |            2 |
+| [天工](https://model-platform.tiangong.cn/api-reference) | skywork           |        1 |               0 |             0 |               0 |
 | [阶跃星辰](https://platform.stepfun.com/docs/Chat/chat-completion-create)     | stepfun           |        3 |            1 |                      0 |            0 |
+| [Together AI](https://docs.together.ai/docs/quickstart) | together          |       58 |               0 |            58 |               0 |
 | [智谱](https://open.bigmodel.cn/dev/api)     | zhipu             |        5 |            1 |                      4 |            2 |
 | OpenAI 接口兼容的服务     | openai-compatible |          |              |                        |              |
 | Ollama API     | ollama            |          |              |                        |              |
 
 
 ## 安装
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
                               ************ uullllmm ************
- A unified interface for local Large Language Model(LLM) models and online LLM
+    A unified interface for local Large Language Models(LLM) and online LLM
                                   providers.
             ****** _[[_PP_yy_PP_II_ _VV_ee_rr_ss_ii_oo_nn_]]_[[_PP_rr_ee_--_cc_oo_mm_mm_ii_tt_ _ss_tt_aa_tt_uu_ss_]]_[[_BB_uu_ii_ll_dd_ _ss_tt_aa_tt_uu_ss_]] ******
 ullm å¸æè½ä¸ºæ¬å°æ¨¡åä»¥åä¼å¤å¨çº¿ LLM
 æå¡æä¾ç»ä¸çè°ç¨æ¹å¼ï¼ä½¿å¾å¼åèè½å¤æ çå°å¨ä¸åæ¨¡åæ
 LLM æå¡ä¹é´åæ¢ï¼èæ éæ´æ¹ä»£ç ã > [!NOTE] >
 æ¬é¡¹ç®åªä¸æ³¨äºä¸ºä¸å LLM
 æ¨¡åææå¡çåºç¡çæåè½æä¾ç»ä¸æ¥å£ï¼åæ¬éç¨ççæãèå¤©æ¥å£ä»¥åæåºç¡çå·¥å·è°ç¨ãè§è§çè§£åè½ï¼å¨æ­¤ä¹å¤çå¶ä»ç¸å³åè½å¦
@@ -14,53 +14,59 @@
 [åè½ä¸ç¹æ§](#åè½ä¸ç¹æ§) - [æ¯ææ¨¡å](#æ¯ææ¨¡å) -
 [æ¬å°æ¨¡å](#æ¬å°æ¨¡å) - [å¨çº¿æå¡](#å¨çº¿æå¡) - [å®è£]
 (#å®è£) - [ä½¿ç¨](#ä½¿ç¨) - [åå»ºæ¨¡åéç½®](#åå»ºæ¨¡åéç½®) -
 [å®ä¾åæ¨¡å](#å®ä¾åæ¨¡å) - [è®¾ç½®çæåæ°](#è®¾ç½®çæåæ°)
 - [çæææ¬](#çæææ¬) - [èå¤©](#èå¤©) - [å½ä»¤è¡](#å½ä»¤è¡) -
 [list-providers](#list-providers) - [list-models](#list-models) - [print-
 example](#print-example) - [chat](#chat) ## åè½ä¸ç¹æ§ - æ¯æ OpenAI ç­
-18 ä¸ªå¨çº¿ LLM æå¡ï¼è¯¦è§ã[å¨çº¿æå¡](#å¨çº¿æå¡)ãä¸è -
+21 ä¸ªå¨çº¿ LLM æå¡ï¼è¯¦è§ã[å¨çº¿æå¡](#å¨çº¿æå¡)ãä¸è -
 æ¯æå OpenAI æ¥å£å¼å®¹çèªå»ºæå¡ - æ¯æ Ollama API -
 éç½®åçä½¿ç¨æ¹å¼ï¼ä¸ºææä¸åæ¨¡ååæå¡æä¾ç»ä¸çåå§åæ¹å¼ï¼è¯¦è§ã
-[ä½¿ç¨](#ä½¿ç¨)ãä¸è - [ ] æ¬å°æ¨¡åæ¯æ - [ ]
-ä¸ºæææ¨¡åæ¯æå·¥å·è°ç¨ï¼å¯¹åæ¬ä¸æ¯æçéè¿èªå®ä¹ prompt
-æ¨¡æ¿å®ç°ï¼ - [ ] æ¨¡åéç½®çç®¡ç - [ ] å¤æ¨¡åè·¯ç± - [ ]
+[ä½¿ç¨](#ä½¿ç¨)ãä¸è - [ ] æ¬å°æ¨¡åæ¯æ - [ ] å½ä¸åæ¨¡ååç§°
+- [ ] ä¸ºæææ¨¡åæ¯æå·¥å·è°ç¨ï¼å¯¹åæ¬ä¸æ¯æçéè¿èªå®ä¹
+prompt æ¨¡æ¿å®ç°ï¼ - [ ] ä¸ºä¸åæ¨¡åééå¯¹åºç
+tokenizerï¼ä»¥è·å¾ tokens æ°éè§£å³æäº remote model ä¸è¿å tokens
+æ°éçé®é¢ - [ ] æ¨¡åéç½®çç®¡ç - [ ] å¤æ¨¡åè·¯ç± - [ ]
 ååæµè¯ - [ ] å®åææ¡£ - [ ] å®ç°æµå¼æ¥å£ ## æ¯ææ¨¡å ###
 æ¬å°æ¨¡å TBD ### å¨çº¿æå¡ | å¹³å° | Provider ID | æ¨¡åæ°é |
 è§è§æ¨¡åæ°é | æ¯æå·¥å·è°ç¨çæ¨¡åæ°é | èç½æ¨¡åæ°é |
 |------|-------------------|----------|--------------|------------------------
 |--------------| | [é¶ä¸ä¸ç©](https://platform.lingyiwanwu.com/docs) | 01ai
 | 3 | 1 | 0 | 0 | | [é¿éå·´å·´](https://help.aliyun.com/zh/dashscope/
 developer-reference/model-square/?spm=a2c4g.11186623.0.0.1cca23edHYSGqT) |
 alibaba | 44 | 4 | 6 | 6 | | [Anthropic](https://docs.anthropic.com/claude/
 reference/getting-started-with-the-api) | anthropic | 3 | 3 | 3 | 0 | | [Azure
 OpenAI](https://learn.microsoft.com/en-us/azure/ai-services/openai/
 reference#chat-completions) | azure-openai | 20 | 4 | 11 | 0 | | [ç¾å·æºè½]
 (https://platform.baichuan-ai.com/docs/api) | baichuan | 4 | 0 | 0 | 2 | |
 [ç¾åº¦](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Nlks5zkzu) | baidu | 46 |
-0 | 24 | 12 | | [Cohere](https://docs.cohere.com/reference/about) | cohere | 12
-| 0 | 4 | 6 | | [DeepSeek](https://platform.deepseek.com/docs) | deepseek | 2 |
-0 | 0 | 0 | | [Google](https://ai.google.dev/gemini-api/docs) | google | 3 | 2
-| 2 | 0 | | [Groq](https://console.groq.com/docs/quickstart) | groq | 4 | 0 | 4
-| 0 | | [ç§å¤§è®¯é£](https://www.xfyun.cn/doc/spark/
+0 | 24 | 12 | | [Cloudflare Workers AI](https://developers.cloudflare.com/
+workers-ai/get-started/rest-api/) | cloudflare | 35 | 0 | 0 | 0 | | [Cohere]
+(https://docs.cohere.com/reference/about) | cohere | 12 | 0 | 4 | 6 | |
+[DeepSeek](https://platform.deepseek.com/docs) | deepseek | 2 | 0 | 0 | 0 | |
+[Google](https://ai.google.dev/gemini-api/docs) | google | 3 | 2 | 2 | 0 | |
+[Groq](https://console.groq.com/docs/quickstart) | groq | 4 | 0 | 4 | 0 | |
+[ç§å¤§è®¯é£](https://www.xfyun.cn/doc/spark/
 %E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E.html) | iflytek | 4 | 0 | 2 | 0 | |
 [MiniMax](https://www.minimaxi.com/document/algorithm-
 concept?id=6433f37594878d408fc8295d) | minimax | 5 | 0 | 5 | 0 | | [Moonshot]
 (https://platform.moonshot.cn/docs/api/
 chat#%E5%9F%BA%E6%9C%AC%E4%BF%A1%E6%81%AF) | moonshot | 3 | 0 | 3 | 0 | |
 [OpenAI](https://platform.openai.com/docs/api-reference/chat) | openai | 20 | 4
 | 11 | 0 | | [OpenRouter](https://openrouter.ai/docs) | openrouter | 127 | 13 |
 127 | 4 | | [Perplexity](https://docs.perplexity.ai/docs/getting-started) |
-perplexity | 7 | 0 | 0 | 2 | | [é¶è·æè¾°](https://platform.stepfun.com/
-docs/Chat/chat-completion-create) | stepfun | 3 | 1 | 0 | 0 | | [æºè°±](https:
-//open.bigmodel.cn/dev/api) | zhipu | 5 | 1 | 4 | 2 | | OpenAI
-æ¥å£å¼å®¹çæå¡ | openai-compatible | | | | | | Ollama API | ollama | | |
-| | ## å®è£ ```shell pip install ullm ``` ## ä½¿ç¨ ### åå»ºæ¨¡åéç½®
-ç¤ºä¾: ```python model_config = { # required fields "type": 'remote', "model":
-'gpt-3.5-turbo', "provider": 'openai', "api_key": 'sk-
+perplexity | 7 | 0 | 0 | 2 | | [å¤©å·¥](https://model-platform.tiangong.cn/api-
+reference) | skywork | 1 | 0 | 0 | 0 | | [é¶è·æè¾°](https://
+platform.stepfun.com/docs/Chat/chat-completion-create) | stepfun | 3 | 1 | 0 |
+0 | | [Together AI](https://docs.together.ai/docs/quickstart) | together | 58 |
+0 | 58 | 0 | | [æºè°±](https://open.bigmodel.cn/dev/api) | zhipu | 5 | 1 | 4 |
+2 | | OpenAI æ¥å£å¼å®¹çæå¡ | openai-compatible | | | | | | Ollama API |
+ollama | | | | | ## å®è£ ```shell pip install ullm ``` ## ä½¿ç¨ ###
+åå»ºæ¨¡åéç½® ç¤ºä¾: ```python model_config = { # required fields "type":
+'remote', "model": 'gpt-3.5-turbo', "provider": 'openai', "api_key": 'sk-
 ************************************************', # optional fields
 "max_tokens": 4096, "max_input_tokens": 1024, "max_output_tokens": 1024,
 "temperature": 0.8, "top_p": 1.0, "top_k": 50, "stop_sequences": ['stop1',
 'stop2'], "http_proxy": 'https://example-proxy.com', } ```
 æ¨¡åéç½®ä¸­å¿é¡»æå®è¿ä¸ä¸ªå­æ®µ - type: æå®æ¨¡åä¸ºæ¬å°æ¨¡å
 (`local`)è¿æ¯å¨çº¿æ¨¡å(`remote`)ï¼ç®åä»å®ç°äº remote - provider:
 æå®æ¨¡åæä¾æ¹ï¼è§åé¢ã[æ¯ææ¨¡å]
```

### Comparing `ullm-0.1.3/pyproject.toml` & `ullm-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [project]
 name = "ullm"
-version = "0.1.3"
+version = "0.2.0"
 description = "A unified interface for local Large Language Model(LLM) models and online LLM providers."
 authors = [
     {name = "Linusp", email = "linusp1024@gmail.com"},
 ]
 dependencies = [
     "pydantic",
     "arrow",
     "websocket-client",
     "requests",
     "python-magic",
     "click",
     "deepmerge",
     "jsonschema",
+    "tabulate",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 license = {text = "MIT"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `ullm-0.1.3/tests/test_openai.py` & `ullm-0.2.0/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.3/ullm/__init__.py` & `ullm-0.2.0/ullm/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,36 +7,40 @@
     GenerateConfig,
     LanguageModel,
     LocalLanguageModel,
     RemoteLanguageModel,
     ToolMessage,
     UserMessage,
 )
+from .cloudflare import CloudflareModel
 from .cohere import CohereModel
 from .deepseek import DeepSeekModel
 from .google import GoogleModel
 from .groq import GroqModel
 from .iflytek import IflyTekModel
 from .minimax import MiniMaxModel
 from .moonshot import MoonshotModel
 from .ollama import OllamaModel
 from .openai import AzureOpenAIModel, OpenAICompatibleModel, OpenAIModel
 from .openrouter import OpenRouterModel
 from .perplexity import PerplexityModel
+from .skywork import SkyWorkModel
 from .stepfun import StepFunModel
+from .together import TogetherAIModel
 from .zero_one import ZeroOneAIModel
 from .zhipu import ZhipuAIModel
 
 __all__ = [
     AlibabaModel,
     AnthropicModel,
     AssistantMessage,
     AzureOpenAIModel,
     BaichuanModel,
     BaiduModel,
+    CloudflareModel,
     CohereModel,
     DeepSeekModel,
     GenerateConfig,
     GoogleModel,
     GoogleModel,
     GroqModel,
     IflyTekModel,
@@ -46,13 +50,15 @@
     MoonshotModel,
     OllamaModel,
     OpenAICompatibleModel,
     OpenAIModel,
     OpenRouterModel,
     PerplexityModel,
     RemoteLanguageModel,
+    SkyWorkModel,
     StepFunModel,
+    TogetherAIModel,
     ToolMessage,
     UserMessage,
     ZeroOneAIModel,
     ZhipuAIModel,
 ]
```

### Comparing `ullm-0.1.3/ullm/alibaba.py` & `ullm-0.2.0/ullm/alibaba.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.3/ullm/anthropic.py` & `ullm-0.2.0/ullm/anthropic.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.3/ullm/baichuan.py` & `ullm-0.2.0/ullm/baichuan.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.3/ullm/baidu.py` & `ullm-0.2.0/ullm/baidu.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.3/ullm/base.py` & `ullm-0.2.0/ullm/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,14 +275,19 @@
     max_input_tokens: Optional[PositiveInt] = Field(None, examples=[1024, 2048])
     max_output_tokens: Optional[PositiveInt] = Field(None, examples=[1024, 4096])
     temperature: Optional[NonNegativeFloat] = Field(None, examples=[0.7, 0.8])
     top_p: Optional[NonNegativeFloat] = Field(None, le=1.0, examples=[1.0])
     top_k: Optional[NonNegativeInt] = Field(None, examples=[50, 100])
     stop_sequences: Optional[List[str]] = Field(None, examples=[["stop1", "stop2"]])
     http_proxy: Optional[HttpUrl] = Field(None, examples=["https://example-proxy.com"])
+    cf_account_id: Optional[SecretStr] = Field(
+        None,
+        description="Cloudflare Account ID",
+        examples=["fe18f2a883e6401c9ee72ab358714088"],
+    )
 
 
 class RemoteLanguageModelMetaInfo(BaseModel):
     model_config = ConfigDict(protected_namespaces=())
 
     api_url: Optional[AnyUrl] = Field("", description="TODO")
     model_api_url_mappings: Optional[Dict[str, AnyUrl]] = Field({}, description="TODO")
```

### Comparing `ullm-0.1.3/ullm/cli.py` & `ullm-0.2.0/ullm/cli.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.3/ullm/cohere.py` & `ullm-0.2.0/ullm/cohere.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.3/ullm/deepseek.py` & `ullm-0.2.0/ullm/deepseek.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.3/ullm/google.py` & `ullm-0.2.0/ullm/google.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.3/ullm/groq.py` & `ullm-0.2.0/ullm/groq.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.3/ullm/iflytek.py` & `ullm-0.2.0/ullm/iflytek.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.3/ullm/minimax.py` & `ullm-0.2.0/ullm/minimax.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.3/ullm/moonshot.py` & `ullm-0.2.0/ullm/moonshot.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.3/ullm/ollama.py` & `ullm-0.2.0/ullm/ollama.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.3/ullm/openai.py` & `ullm-0.2.0/ullm/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,34 +321,37 @@
             "gpt-4-0613",
             "gpt-4-1106-preview",
             "gpt-4-32k",
             "gpt-4-32k-0613",
             "gpt-4-turbo",
             "gpt-4-turbo-2024-04-09",
             "gpt-4-turbo-preview",
+            "gpt-4o",
         ],
         visual_language_models=[
             "gpt-4-vision-preview",
             "gpt-4-1106-vision-preview",
             "gpt-4-turbo",
             "gpt-4-turbo-2024-04-09",
+            "gpt-4o",
         ],
         # https://platform.openai.com/docs/guides/function-calling
         tool_models=[
             "gpt-3.5-turbo",
             "gpt-3.5-turbo-0125",
             "gpt-3.5-turbo-0613",
             "gpt-3.5-turbo-1106",
             "gpt-4",
             "gpt-4-0125-preview",
             "gpt-4-0613",
             "gpt-4-1106-preview",
             "gpt-4-turbo",
             "gpt-4-turbo-2024-04-09",
             "gpt-4-turbo-preview",
+            "gpt-4o",
         ],
         required_config_fields=["api_key"],
     )
 
 
 class AzureOpenAIRequestBody(OpenAIRequestBody):
     model: Optional[str] = Field(None, exclude=True)
```

### Comparing `ullm-0.1.3/ullm/openrouter.py` & `ullm-0.2.0/ullm/openrouter.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,14 +169,15 @@
         "openai/gpt-3.5-turbo-16k",
         "openai/gpt-3.5-turbo-instruct",
         "openai/gpt-4",
         "openai/gpt-4-32k",
         "openai/gpt-4-turbo",
         "openai/gpt-4-turbo-preview",
         "openai/gpt-4-vision-preview",
+        "openai/gpt-4o",
         "openchat/openchat-7b",
         "openchat/openchat-7b:free",
         "openrouter/auto",
         "openrouter/cinematika-7b",
         "openrouter/cinematika-7b:free",
         "perplexity/pplx-70b-chat",
         "perplexity/pplx-70b-online",
@@ -217,14 +218,15 @@
         "claude-3-sonnet",
         "claude-3-sonnet:beta",
         "firellava-13b",  # https://openrouter.ai/models/fireworks/firellava-13b
         "gemini-pro-vision",
         "gemini-pro-1.5",
         "gpt-4-turbo",
         "gpt-4-vision-preview",
+        "gpt-4o",
         "llava-13b",  # https://openrouter.ai/models/haotian-liu/llava-13b
         "nous-hermes-2-vision-7b",  # https://openrouter.ai/models/nousresearch/nous-hermes-2-vision-7b
     ]
     META = RemoteLanguageModelMetaInfo(
         api_url="https://openrouter.ai/api/v1/chat/completions",
         required_config_fields=["api_key"],
         language_models=set(_SUPPORTED_MODELS) - set(_VISUAL_MODELS),
```

### Comparing `ullm-0.1.3/ullm/perplexity.py` & `ullm-0.2.0/ullm/perplexity.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.3/ullm/stepfun.py` & `ullm-0.2.0/ullm/stepfun.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.3/ullm/zero_one.py` & `ullm-0.2.0/ullm/zero_one.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.3/ullm/zhipu.py` & `ullm-0.2.0/ullm/zhipu.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.3/ullm.egg-info/PKG-INFO` & `ullm-0.2.0/ullm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ullm
-Version: 0.1.3
+Version: 0.2.0
 Summary: A unified interface for local Large Language Model(LLM) models and online LLM providers.
 Author-email: Linusp <linusp1024@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/monsternlp/ullm
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -14,20 +14,21 @@
 Requires-Dist: arrow
 Requires-Dist: websocket-client
 Requires-Dist: requests
 Requires-Dist: python-magic
 Requires-Dist: click
 Requires-Dist: deepmerge
 Requires-Dist: jsonschema
+Requires-Dist: tabulate
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 <h1 align="center">ullm</h1>
-<p align="center">A unified interface for local Large Language Model(LLM) models and online LLM providers.</p>
+<p align="center">A unified interface for local Large Language Models(LLM) and online LLM providers.</p>
 <h4 align="center">
     <a href="https://pypi.org/project/ullm/" target="_blank">
         <img src="https://shields.io/pypi/v/ullm.svg" alt="PyPI Version">
     </a>
     <a href="https://github.com/monsternlp/ullm/actions/workflows/pre-commit.yaml" target="_blank">
         <img src="https://shields.io/github/actions/workflow/status/monsternlp/ullm/pre-commit.yaml?label=pre-commit" alt="Pre-commit status">
     </a>
@@ -65,20 +66,22 @@
   - [print-example](#print-example)
   - [chat](#chat)
 
 <!-- /TOC -->
 
 ## 功能与特性
 
-- 支持 OpenAI 等 18 个在线 LLM 服务，详见「[在线服务](#在线服务)」一节
+- 支持 OpenAI 等 21 个在线 LLM 服务，详见「[在线服务](#在线服务)」一节
 - 支持和 OpenAI 接口兼容的自建服务
 - 支持 Ollama API
 - 配置化的使用方式，为所有不同模型及服务提供统一的初始化方式，详见「[使用](#使用)」一节
 - [ ] 本地模型支持
+- [ ] 归一化模型名称
 - [ ] 为所有模型支持工具调用（对原本不支持的通过自定义 prompt 模板实现）
+- [ ] 为不同模型适配对应的 tokenizer，以获得 tokens 数量解决某些 remote model 不返回 tokens 数量的问题
 - [ ] 模型配置的管理
 - [ ] 多模型路由
 - [ ] 单元测试
 - [ ] 完善文档
 - [ ] 实现流式接口
 
 ## 支持模型
@@ -93,25 +96,28 @@
 |------|-------------------|----------|--------------|------------------------|--------------|
 | [零一万物](https://platform.lingyiwanwu.com/docs)     | 01ai              |        3 |            1 |                      0 |            0 |
 | [阿里巴巴](https://help.aliyun.com/zh/dashscope/developer-reference/model-square/?spm=a2c4g.11186623.0.0.1cca23edHYSGqT)      | alibaba           |       44 |            4 |                      6 |            6 |
 | [Anthropic](https://docs.anthropic.com/claude/reference/getting-started-with-the-api)     | anthropic         |        3 |            3 |                      3 |            0 |
 | [Azure OpenAI](https://learn.microsoft.com/en-us/azure/ai-services/openai/reference#chat-completions)     | azure-openai      |       20 |            4 |                     11 |            0 |
 | [百川智能](https://platform.baichuan-ai.com/docs/api)     | baichuan          |        4 |            0 |                      0 |            2 |
 | [百度](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Nlks5zkzu)     | baidu             |       46 |            0 |                     24 |           12 |
+| [Cloudflare Workers AI](https://developers.cloudflare.com/workers-ai/get-started/rest-api/) | cloudflare        |       35 |               0 |             0 |               0 |
 | [Cohere](https://docs.cohere.com/reference/about)     | cohere            |       12 |            0 |                      4 |            6 |
 | [DeepSeek](https://platform.deepseek.com/docs)     | deepseek          |        2 |            0 |                      0 |            0 |
 | [Google](https://ai.google.dev/gemini-api/docs)     | google            |        3 |            2 |                      2 |            0 |
 | [Groq](https://console.groq.com/docs/quickstart)     | groq              |        4 |            0 |                      4 |            0 |
 | [科大讯飞](https://www.xfyun.cn/doc/spark/%E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E.html)     | iflytek           |        4 |            0 |                      2 |            0 |
 | [MiniMax](https://www.minimaxi.com/document/algorithm-concept?id=6433f37594878d408fc8295d)     | minimax           |        5 |            0 |                      5 |            0 |
 | [Moonshot](https://platform.moonshot.cn/docs/api/chat#%E5%9F%BA%E6%9C%AC%E4%BF%A1%E6%81%AF)     | moonshot          |        3 |            0 |                      3 |            0 |
 | [OpenAI](https://platform.openai.com/docs/api-reference/chat)      | openai            |       20 |            4 |                     11 |            0 |
 | [OpenRouter](https://openrouter.ai/docs)     | openrouter        |      127 |           13 |                    127 |            4 |
 | [Perplexity](https://docs.perplexity.ai/docs/getting-started)     | perplexity        |        7 |            0 |                      0 |            2 |
+| [天工](https://model-platform.tiangong.cn/api-reference) | skywork           |        1 |               0 |             0 |               0 |
 | [阶跃星辰](https://platform.stepfun.com/docs/Chat/chat-completion-create)     | stepfun           |        3 |            1 |                      0 |            0 |
+| [Together AI](https://docs.together.ai/docs/quickstart) | together          |       58 |               0 |            58 |               0 |
 | [智谱](https://open.bigmodel.cn/dev/api)     | zhipu             |        5 |            1 |                      4 |            2 |
 | OpenAI 接口兼容的服务     | openai-compatible |          |              |                        |              |
 | Ollama API     | ollama            |          |              |                        |              |
 
 
 ## 安装
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: ullm Version: 0.1.3 Summary: A unified interface
+Metadata-Version: 2.1 Name: ullm Version: 0.2.0 Summary: A unified interface
 for local Large Language Model(LLM) models and online LLM providers. Author-
 email: Linusp
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/monsternlp/
 ullm Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.8 Description-Content-Type: text/markdown Requires-Dist: pydantic
 Requires-Dist: arrow Requires-Dist: websocket-client Requires-Dist: requests
 Requires-Dist: python-magic Requires-Dist: click Requires-Dist: deepmerge
-Requires-Dist: jsonschema Provides-Extra: test Requires-Dist: pytest; extra ==
-"test" Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: jsonschema Requires-Dist: tabulate Provides-Extra: test
+Requires-Dist: pytest; extra == "test" Requires-Dist: pytest-cov; extra ==
+"test"
                               ************ uullllmm ************
- A unified interface for local Large Language Model(LLM) models and online LLM
+    A unified interface for local Large Language Models(LLM) and online LLM
                                   providers.
             ****** _[[_PP_yy_PP_II_ _VV_ee_rr_ss_ii_oo_nn_]]_[[_PP_rr_ee_--_cc_oo_mm_mm_ii_tt_ _ss_tt_aa_tt_uu_ss_]]_[[_BB_uu_ii_ll_dd_ _ss_tt_aa_tt_uu_ss_]] ******
 ullm å¸æè½ä¸ºæ¬å°æ¨¡åä»¥åä¼å¤å¨çº¿ LLM
 æå¡æä¾ç»ä¸çè°ç¨æ¹å¼ï¼ä½¿å¾å¼åèè½å¤æ çå°å¨ä¸åæ¨¡åæ
 LLM æå¡ä¹é´åæ¢ï¼èæ éæ´æ¹ä»£ç ã > [!NOTE] >
 æ¬é¡¹ç®åªä¸æ³¨äºä¸ºä¸å LLM
 æ¨¡åææå¡çåºç¡çæåè½æä¾ç»ä¸æ¥å£ï¼åæ¬éç¨ççæãèå¤©æ¥å£ä»¥åæåºç¡çå·¥å·è°ç¨ãè§è§çè§£åè½ï¼å¨æ­¤ä¹å¤çå¶ä»ç¸å³åè½å¦
@@ -25,53 +26,59 @@
 [åè½ä¸ç¹æ§](#åè½ä¸ç¹æ§) - [æ¯ææ¨¡å](#æ¯ææ¨¡å) -
 [æ¬å°æ¨¡å](#æ¬å°æ¨¡å) - [å¨çº¿æå¡](#å¨çº¿æå¡) - [å®è£]
 (#å®è£) - [ä½¿ç¨](#ä½¿ç¨) - [åå»ºæ¨¡åéç½®](#åå»ºæ¨¡åéç½®) -
 [å®ä¾åæ¨¡å](#å®ä¾åæ¨¡å) - [è®¾ç½®çæåæ°](#è®¾ç½®çæåæ°)
 - [çæææ¬](#çæææ¬) - [èå¤©](#èå¤©) - [å½ä»¤è¡](#å½ä»¤è¡) -
 [list-providers](#list-providers) - [list-models](#list-models) - [print-
 example](#print-example) - [chat](#chat) ## åè½ä¸ç¹æ§ - æ¯æ OpenAI ç­
-18 ä¸ªå¨çº¿ LLM æå¡ï¼è¯¦è§ã[å¨çº¿æå¡](#å¨çº¿æå¡)ãä¸è -
+21 ä¸ªå¨çº¿ LLM æå¡ï¼è¯¦è§ã[å¨çº¿æå¡](#å¨çº¿æå¡)ãä¸è -
 æ¯æå OpenAI æ¥å£å¼å®¹çèªå»ºæå¡ - æ¯æ Ollama API -
 éç½®åçä½¿ç¨æ¹å¼ï¼ä¸ºææä¸åæ¨¡ååæå¡æä¾ç»ä¸çåå§åæ¹å¼ï¼è¯¦è§ã
-[ä½¿ç¨](#ä½¿ç¨)ãä¸è - [ ] æ¬å°æ¨¡åæ¯æ - [ ]
-ä¸ºæææ¨¡åæ¯æå·¥å·è°ç¨ï¼å¯¹åæ¬ä¸æ¯æçéè¿èªå®ä¹ prompt
-æ¨¡æ¿å®ç°ï¼ - [ ] æ¨¡åéç½®çç®¡ç - [ ] å¤æ¨¡åè·¯ç± - [ ]
+[ä½¿ç¨](#ä½¿ç¨)ãä¸è - [ ] æ¬å°æ¨¡åæ¯æ - [ ] å½ä¸åæ¨¡ååç§°
+- [ ] ä¸ºæææ¨¡åæ¯æå·¥å·è°ç¨ï¼å¯¹åæ¬ä¸æ¯æçéè¿èªå®ä¹
+prompt æ¨¡æ¿å®ç°ï¼ - [ ] ä¸ºä¸åæ¨¡åééå¯¹åºç
+tokenizerï¼ä»¥è·å¾ tokens æ°éè§£å³æäº remote model ä¸è¿å tokens
+æ°éçé®é¢ - [ ] æ¨¡åéç½®çç®¡ç - [ ] å¤æ¨¡åè·¯ç± - [ ]
 ååæµè¯ - [ ] å®åææ¡£ - [ ] å®ç°æµå¼æ¥å£ ## æ¯ææ¨¡å ###
 æ¬å°æ¨¡å TBD ### å¨çº¿æå¡ | å¹³å° | Provider ID | æ¨¡åæ°é |
 è§è§æ¨¡åæ°é | æ¯æå·¥å·è°ç¨çæ¨¡åæ°é | èç½æ¨¡åæ°é |
 |------|-------------------|----------|--------------|------------------------
 |--------------| | [é¶ä¸ä¸ç©](https://platform.lingyiwanwu.com/docs) | 01ai
 | 3 | 1 | 0 | 0 | | [é¿éå·´å·´](https://help.aliyun.com/zh/dashscope/
 developer-reference/model-square/?spm=a2c4g.11186623.0.0.1cca23edHYSGqT) |
 alibaba | 44 | 4 | 6 | 6 | | [Anthropic](https://docs.anthropic.com/claude/
 reference/getting-started-with-the-api) | anthropic | 3 | 3 | 3 | 0 | | [Azure
 OpenAI](https://learn.microsoft.com/en-us/azure/ai-services/openai/
 reference#chat-completions) | azure-openai | 20 | 4 | 11 | 0 | | [ç¾å·æºè½]
 (https://platform.baichuan-ai.com/docs/api) | baichuan | 4 | 0 | 0 | 2 | |
 [ç¾åº¦](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Nlks5zkzu) | baidu | 46 |
-0 | 24 | 12 | | [Cohere](https://docs.cohere.com/reference/about) | cohere | 12
-| 0 | 4 | 6 | | [DeepSeek](https://platform.deepseek.com/docs) | deepseek | 2 |
-0 | 0 | 0 | | [Google](https://ai.google.dev/gemini-api/docs) | google | 3 | 2
-| 2 | 0 | | [Groq](https://console.groq.com/docs/quickstart) | groq | 4 | 0 | 4
-| 0 | | [ç§å¤§è®¯é£](https://www.xfyun.cn/doc/spark/
+0 | 24 | 12 | | [Cloudflare Workers AI](https://developers.cloudflare.com/
+workers-ai/get-started/rest-api/) | cloudflare | 35 | 0 | 0 | 0 | | [Cohere]
+(https://docs.cohere.com/reference/about) | cohere | 12 | 0 | 4 | 6 | |
+[DeepSeek](https://platform.deepseek.com/docs) | deepseek | 2 | 0 | 0 | 0 | |
+[Google](https://ai.google.dev/gemini-api/docs) | google | 3 | 2 | 2 | 0 | |
+[Groq](https://console.groq.com/docs/quickstart) | groq | 4 | 0 | 4 | 0 | |
+[ç§å¤§è®¯é£](https://www.xfyun.cn/doc/spark/
 %E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E.html) | iflytek | 4 | 0 | 2 | 0 | |
 [MiniMax](https://www.minimaxi.com/document/algorithm-
 concept?id=6433f37594878d408fc8295d) | minimax | 5 | 0 | 5 | 0 | | [Moonshot]
 (https://platform.moonshot.cn/docs/api/
 chat#%E5%9F%BA%E6%9C%AC%E4%BF%A1%E6%81%AF) | moonshot | 3 | 0 | 3 | 0 | |
 [OpenAI](https://platform.openai.com/docs/api-reference/chat) | openai | 20 | 4
 | 11 | 0 | | [OpenRouter](https://openrouter.ai/docs) | openrouter | 127 | 13 |
 127 | 4 | | [Perplexity](https://docs.perplexity.ai/docs/getting-started) |
-perplexity | 7 | 0 | 0 | 2 | | [é¶è·æè¾°](https://platform.stepfun.com/
-docs/Chat/chat-completion-create) | stepfun | 3 | 1 | 0 | 0 | | [æºè°±](https:
-//open.bigmodel.cn/dev/api) | zhipu | 5 | 1 | 4 | 2 | | OpenAI
-æ¥å£å¼å®¹çæå¡ | openai-compatible | | | | | | Ollama API | ollama | | |
-| | ## å®è£ ```shell pip install ullm ``` ## ä½¿ç¨ ### åå»ºæ¨¡åéç½®
-ç¤ºä¾: ```python model_config = { # required fields "type": 'remote', "model":
-'gpt-3.5-turbo', "provider": 'openai', "api_key": 'sk-
+perplexity | 7 | 0 | 0 | 2 | | [å¤©å·¥](https://model-platform.tiangong.cn/api-
+reference) | skywork | 1 | 0 | 0 | 0 | | [é¶è·æè¾°](https://
+platform.stepfun.com/docs/Chat/chat-completion-create) | stepfun | 3 | 1 | 0 |
+0 | | [Together AI](https://docs.together.ai/docs/quickstart) | together | 58 |
+0 | 58 | 0 | | [æºè°±](https://open.bigmodel.cn/dev/api) | zhipu | 5 | 1 | 4 |
+2 | | OpenAI æ¥å£å¼å®¹çæå¡ | openai-compatible | | | | | | Ollama API |
+ollama | | | | | ## å®è£ ```shell pip install ullm ``` ## ä½¿ç¨ ###
+åå»ºæ¨¡åéç½® ç¤ºä¾: ```python model_config = { # required fields "type":
+'remote', "model": 'gpt-3.5-turbo', "provider": 'openai', "api_key": 'sk-
 ************************************************', # optional fields
 "max_tokens": 4096, "max_input_tokens": 1024, "max_output_tokens": 1024,
 "temperature": 0.8, "top_p": 1.0, "top_k": 50, "stop_sequences": ['stop1',
 'stop2'], "http_proxy": 'https://example-proxy.com', } ```
 æ¨¡åéç½®ä¸­å¿é¡»æå®è¿ä¸ä¸ªå­æ®µ - type: æå®æ¨¡åä¸ºæ¬å°æ¨¡å
 (`local`)è¿æ¯å¨çº¿æ¨¡å(`remote`)ï¼ç®åä»å®ç°äº remote - provider:
 æå®æ¨¡åæä¾æ¹ï¼è§åé¢ã[æ¯ææ¨¡å]
```

### Comparing `ullm-0.1.3/ullm.egg-info/SOURCES.txt` & `ullm-0.2.0/ullm.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 ullm/__init__.py
 ullm/alibaba.py
 ullm/anthropic.py
 ullm/baichuan.py
 ullm/baidu.py
 ullm/base.py
 ullm/cli.py
+ullm/cloudflare.py
 ullm/cohere.py
 ullm/deepseek.py
 ullm/google.py
 ullm/groq.py
 ullm/iflytek.py
 ullm/minimax.py
 ullm/moonshot.py
 ullm/ollama.py
 ullm/openai.py
 ullm/openrouter.py
 ullm/perplexity.py
+ullm/skywork.py
 ullm/stepfun.py
+ullm/together.py
 ullm/zero_one.py
 ullm/zhipu.py
 ullm.egg-info/PKG-INFO
 ullm.egg-info/SOURCES.txt
 ullm.egg-info/dependency_links.txt
 ullm.egg-info/entry_points.txt
 ullm.egg-info/requires.txt
```

