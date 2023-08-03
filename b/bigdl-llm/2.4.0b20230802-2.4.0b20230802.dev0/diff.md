# Comparing `tmp/bigdl_llm-2.4.0b20230802-py3-none-win_amd64.whl.zip` & `tmp/bigdl_llm-2.4.0b20230802.dev0-py3-none-manylinux2010_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,89 +1,87 @@
-Zip file size: 2510314 bytes, number of entries: 87
--rw-------  2.0 unx      956 b- defN 23-Aug-02 08:46 bigdl/__init__.py
--rw-------  2.0 unx      914 b- defN 23-Aug-02 08:46 bigdl/llm/__init__.py
--rw-------  2.0 unx     6809 b- defN 23-Aug-02 08:46 bigdl/llm/convert_model.py
--rw-------  2.0 unx     1067 b- defN 23-Aug-02 08:46 bigdl/llm/models.py
--rw-rw-r--  2.0 unx     2772 b- defN 23-Aug-02 08:46 bigdl/llm/cli/llm-chat.ps1
--rwxrwxr-x  2.0 unx     3012 b- defN 23-Aug-02 08:46 bigdl/llm/cli/llm-cli.ps1
--rw-rw-r--  2.0 unx      216 b- defN 23-Aug-02 08:46 bigdl/llm/cli/prompts/chat-with-llm.txt
--rw-------  2.0 unx      994 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/__init__.py
--rw-------  2.0 unx     5378 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/convert.py
--rw-------  2.0 unx     6255 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/convert_model.py
--rw-------  2.0 unx     5183 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/quantize.py
--rw-------  2.0 unx      874 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/model/__init__.py
--rw-------  2.0 unx      900 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/model/bloom/__init__.py
--rw-------  2.0 unx    17895 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/model/bloom/bloom.py
--rw-------  2.0 unx     7311 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/model/bloom/bloom_cpp.py
--rw-------  2.0 unx      910 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/model/generation/__init__.py
--rw-------  2.0 unx     6250 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/model/generation/utils.py
--rw-------  2.0 unx      925 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/model/gptneox/__init__.py
--rw-------  2.0 unx    46965 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/model/gptneox/gptneox.py
--rw-------  2.0 unx    25853 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/model/gptneox/gptneox_cpp.py
--rw-------  2.0 unx     4194 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/model/gptneox/gptneox_types.py
--rw-------  2.0 unx      921 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/model/llama/__init__.py
--rw-------  2.0 unx    54567 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/model/llama/llama.py
--rw-------  2.0 unx    33541 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/model/llama/llama_cpp.py
--rw-------  2.0 unx     4207 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/model/llama/llama_types.py
--rw-------  2.0 unx      908 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/model/starcoder/__init__.py
--rw-------  2.0 unx    18336 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/model/starcoder/starcoder.py
--rw-------  2.0 unx     7479 b- defN 23-Aug-02 08:46 bigdl/llm/ggml/model/starcoder/starcoder_cpp.py
--rw-------  2.0 unx      874 b- defN 23-Aug-02 08:46 bigdl/llm/gptq/__init__.py
--rw-------  2.0 unx      874 b- defN 23-Aug-02 08:46 bigdl/llm/gptq/convert/__init__.py
--rw-------  2.0 unx    10737 b- defN 23-Aug-02 08:46 bigdl/llm/gptq/convert/convert_gptq_to_ggml.py
--rw-------  2.0 unx      874 b- defN 23-Aug-02 08:46 bigdl/llm/langchain/__init__.py
--rw-------  2.0 unx     1051 b- defN 23-Aug-02 08:46 bigdl/llm/langchain/embeddings/__init__.py
--rw-------  2.0 unx     7039 b- defN 23-Aug-02 08:46 bigdl/llm/langchain/embeddings/bigdlllm.py
--rw-------  2.0 unx     5917 b- defN 23-Aug-02 08:46 bigdl/llm/langchain/embeddings/transformersembeddings.py
--rw-------  2.0 unx     1414 b- defN 23-Aug-02 08:46 bigdl/llm/langchain/llms/__init__.py
--rw-------  2.0 unx    12672 b- defN 23-Aug-02 08:46 bigdl/llm/langchain/llms/bigdlllm.py
--rw-------  2.0 unx     7162 b- defN 23-Aug-02 08:46 bigdl/llm/langchain/llms/transformersllm.py
--rw-------  2.0 unx     7371 b- defN 23-Aug-02 08:46 bigdl/llm/langchain/llms/transformerspipelinellm.py
--rw-------  2.0 unx    36352 b- defN 23-Aug-02 13:18 bigdl/llm/libs/bloom-api.dll
--rw-------  2.0 unx   359936 b- defN 23-Aug-02 13:18 bigdl/llm/libs/bloom.dll
--rw-------  2.0 unx    24576 b- defN 23-Aug-02 13:18 bigdl/llm/libs/gptneox-api.dll
--rw-------  2.0 unx   429568 b- defN 23-Aug-02 13:18 bigdl/llm/libs/gptneox.dll
--rw-------  2.0 unx   360448 b- defN 23-Aug-02 13:18 bigdl/llm/libs/libbloom_vnni.dll
--rw-------  2.0 unx   430080 b- defN 23-Aug-02 13:18 bigdl/llm/libs/libgptneox_vnni.dll
--rw-------  2.0 unx   425472 b- defN 23-Aug-02 13:18 bigdl/llm/libs/libllama_vnni.dll
--rw-------  2.0 unx   452608 b- defN 23-Aug-02 13:18 bigdl/llm/libs/libstarcoder_vnni.dll
--rw-------  2.0 unx    25088 b- defN 23-Aug-02 13:18 bigdl/llm/libs/llama-api.dll
--rw-------  2.0 unx   424960 b- defN 23-Aug-02 13:18 bigdl/llm/libs/llama.dll
--rw-------  2.0 unx   102912 b- defN 23-Aug-02 13:18 bigdl/llm/libs/main-bloom.exe
--rw-------  2.0 unx   712704 b- defN 23-Aug-02 13:18 bigdl/llm/libs/main-chatglm_vnni.exe
--rw-------  2.0 unx    98816 b- defN 23-Aug-02 13:18 bigdl/llm/libs/main-gptneox.exe
--rw-------  2.0 unx   100352 b- defN 23-Aug-02 13:18 bigdl/llm/libs/main-llama.exe
--rw-------  2.0 unx   157184 b- defN 23-Aug-02 13:18 bigdl/llm/libs/main-starcoder.exe
--rw-------  2.0 unx   116224 b- defN 23-Aug-02 13:18 bigdl/llm/libs/quantize-bloom.exe
--rw-------  2.0 unx   116736 b- defN 23-Aug-02 13:18 bigdl/llm/libs/quantize-bloom_vnni.exe
--rw-------  2.0 unx    97280 b- defN 23-Aug-02 13:18 bigdl/llm/libs/quantize-gptneox.exe
--rw-------  2.0 unx    97792 b- defN 23-Aug-02 13:18 bigdl/llm/libs/quantize-gptneox_vnni.exe
--rw-------  2.0 unx   101888 b- defN 23-Aug-02 13:18 bigdl/llm/libs/quantize-llama.exe
--rw-------  2.0 unx   102400 b- defN 23-Aug-02 13:18 bigdl/llm/libs/quantize-llama_vnni.exe
--rw-------  2.0 unx   116736 b- defN 23-Aug-02 13:18 bigdl/llm/libs/quantize-starcoder.exe
--rw-------  2.0 unx   117248 b- defN 23-Aug-02 13:18 bigdl/llm/libs/quantize-starcoder_vnni.exe
--rw-------  2.0 unx    21504 b- defN 23-Aug-02 13:18 bigdl/llm/libs/starcoder-api.dll
--rw-------  2.0 unx   451584 b- defN 23-Aug-02 13:18 bigdl/llm/libs/starcoder.dll
--rw-------  2.0 unx      780 b- defN 23-Aug-02 08:46 bigdl/llm/transformers/__init__.py
--rw-------  2.0 unx     5498 b- defN 23-Aug-02 08:46 bigdl/llm/transformers/convert.py
--rw-------  2.0 unx     8660 b- defN 23-Aug-02 08:46 bigdl/llm/transformers/linear_quant.py
--rw-------  2.0 unx    10414 b- defN 23-Aug-02 08:46 bigdl/llm/transformers/model.py
--rw-------  2.0 unx     3609 b- defN 23-Aug-02 08:46 bigdl/llm/transformers/modelling_bigdl.py
--rw-------  2.0 unx     5301 b- defN 23-Aug-02 08:46 bigdl/llm/transformers/utils.py
--rw-------  2.0 unx      584 b- defN 23-Aug-02 08:46 bigdl/llm/transformers/models/__init__.py
--rw-------  2.0 unx     9264 b- defN 23-Aug-02 08:46 bigdl/llm/transformers/models/llama.py
--rw-------  2.0 unx      896 b- defN 23-Aug-02 08:46 bigdl/llm/utils/__init__.py
--rw-------  2.0 unx    17954 b- defN 23-Aug-02 08:46 bigdl/llm/utils/convert_chatglm.py
--rw-------  2.0 unx    64300 b- defN 23-Aug-02 08:46 bigdl/llm/utils/convert_util.py
--rw-------  2.0 unx     2102 b- defN 23-Aug-02 08:46 bigdl/llm/utils/isa_checker.py
--rw-------  2.0 unx     2062 b- defN 23-Aug-02 08:46 bigdl/llm/utils/utils.py
--rw-------  2.0 unx      988 b- defN 23-Aug-02 08:46 bigdl/llm/utils/common/__init__.py
--rw-------  2.0 unx     2874 b- defN 23-Aug-02 08:46 bigdl/llm/utils/common/lazyimport.py
--rw-------  2.0 unx     1763 b- defN 23-Aug-02 08:46 bigdl/llm/utils/common/log4Error.py
--rwxrwxr-x  2.0 unx     2772 b- defN 23-Aug-02 08:46 bigdl_llm-2.4.0b20230802.data/scripts/llm-chat.ps1
--rwxrwxr-x  2.0 unx     3012 b- defN 23-Aug-02 08:46 bigdl_llm-2.4.0b20230802.data/scripts/llm-cli.ps1
--rw-------  2.0 unx      895 b- defN 23-Aug-02 13:18 bigdl_llm-2.4.0b20230802.dist-info/METADATA
--rw-------  2.0 unx       98 b- defN 23-Aug-02 13:18 bigdl_llm-2.4.0b20230802.dist-info/WHEEL
--rw-------  2.0 unx       62 b- defN 23-Aug-02 13:18 bigdl_llm-2.4.0b20230802.dist-info/entry_points.txt
--rw-------  2.0 unx        6 b- defN 23-Aug-02 13:18 bigdl_llm-2.4.0b20230802.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     8005 b- defN 23-Aug-02 13:18 bigdl_llm-2.4.0b20230802.dist-info/RECORD
-87 files, 5953924 bytes uncompressed, 2497538 bytes compressed:  58.1%
+Zip file size: 3751952 bytes, number of entries: 85
+-rw-rw-r--  2.0 unx      956 b- defN 23-May-31 07:26 bigdl/__init__.py
+-rw-rw-r--  2.0 unx      914 b- defN 23-Jun-28 07:10 bigdl/llm/__init__.py
+-rw-rw-r--  2.0 unx     6809 b- defN 23-Aug-02 06:54 bigdl/llm/convert_model.py
+-rw-rw-r--  2.0 unx     1067 b- defN 23-Jun-28 07:11 bigdl/llm/models.py
+-rwxrwxr-x  2.0 unx     2251 b- defN 23-Aug-02 09:07 bigdl/llm/cli/llm-chat
+-rw-rw-r--  2.0 unx     2772 b- defN 23-Jul-31 05:59 bigdl/llm/cli/llm-chat.ps1
+-rwxrwxr-x  2.0 unx     2629 b- defN 23-Aug-02 09:07 bigdl/llm/cli/llm-cli
+-rwxrwxr-x  2.0 unx     3012 b- defN 23-Aug-02 06:54 bigdl/llm/cli/llm-cli.ps1
+-rw-rw-r--  2.0 unx      216 b- defN 23-Jul-04 12:07 bigdl/llm/cli/prompts/chat-with-llm.txt
+-rw-rw-r--  2.0 unx      994 b- defN 23-Jun-14 03:58 bigdl/llm/ggml/__init__.py
+-rw-rw-r--  2.0 unx     5378 b- defN 23-Aug-02 06:54 bigdl/llm/ggml/convert.py
+-rw-rw-r--  2.0 unx     6255 b- defN 23-Aug-02 06:54 bigdl/llm/ggml/convert_model.py
+-rw-rw-r--  2.0 unx     5183 b- defN 23-Jul-18 02:57 bigdl/llm/ggml/quantize.py
+-rw-rw-r--  2.0 unx      874 b- defN 23-Jun-02 03:52 bigdl/llm/ggml/model/__init__.py
+-rw-rw-r--  2.0 unx      900 b- defN 23-Jun-05 03:22 bigdl/llm/ggml/model/bloom/__init__.py
+-rw-rw-r--  2.0 unx    17895 b- defN 23-Jul-18 02:57 bigdl/llm/ggml/model/bloom/bloom.py
+-rw-rw-r--  2.0 unx     7311 b- defN 23-Jul-31 05:59 bigdl/llm/ggml/model/bloom/bloom_cpp.py
+-rw-rw-r--  2.0 unx      910 b- defN 23-Jun-06 08:26 bigdl/llm/ggml/model/generation/__init__.py
+-rw-rw-r--  2.0 unx     6250 b- defN 23-Jul-31 05:59 bigdl/llm/ggml/model/generation/utils.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-02 03:52 bigdl/llm/ggml/model/gptneox/__init__.py
+-rw-rw-r--  2.0 unx    46965 b- defN 23-Jul-18 02:57 bigdl/llm/ggml/model/gptneox/gptneox.py
+-rw-rw-r--  2.0 unx    25853 b- defN 23-Jul-31 05:59 bigdl/llm/ggml/model/gptneox/gptneox_cpp.py
+-rw-rw-r--  2.0 unx     4194 b- defN 23-Jun-02 03:52 bigdl/llm/ggml/model/gptneox/gptneox_types.py
+-rw-rw-r--  2.0 unx      921 b- defN 23-Jun-01 06:05 bigdl/llm/ggml/model/llama/__init__.py
+-rw-rw-r--  2.0 unx    54567 b- defN 23-Jul-18 02:57 bigdl/llm/ggml/model/llama/llama.py
+-rw-rw-r--  2.0 unx    33541 b- defN 23-Jul-31 05:59 bigdl/llm/ggml/model/llama/llama_cpp.py
+-rw-rw-r--  2.0 unx     4207 b- defN 23-Jun-02 03:52 bigdl/llm/ggml/model/llama/llama_types.py
+-rw-rw-r--  2.0 unx      908 b- defN 23-Jun-28 07:11 bigdl/llm/ggml/model/starcoder/__init__.py
+-rw-rw-r--  2.0 unx    18336 b- defN 23-Jul-18 02:57 bigdl/llm/ggml/model/starcoder/starcoder.py
+-rw-rw-r--  2.0 unx     7479 b- defN 23-Jul-31 05:59 bigdl/llm/ggml/model/starcoder/starcoder_cpp.py
+-rw-rw-r--  2.0 unx      874 b- defN 23-Jun-28 07:10 bigdl/llm/gptq/__init__.py
+-rw-rw-r--  2.0 unx      874 b- defN 23-Jun-28 07:10 bigdl/llm/gptq/convert/__init__.py
+-rw-rw-r--  2.0 unx    10737 b- defN 23-Jun-28 07:11 bigdl/llm/gptq/convert/convert_gptq_to_ggml.py
+-rw-rw-r--  2.0 unx      874 b- defN 23-Jun-14 03:58 bigdl/llm/langchain/__init__.py
+-rw-rw-r--  2.0 unx     1051 b- defN 23-Jul-18 02:57 bigdl/llm/langchain/embeddings/__init__.py
+-rw-rw-r--  2.0 unx     7039 b- defN 23-Jul-18 02:57 bigdl/llm/langchain/embeddings/bigdlllm.py
+-rw-rw-r--  2.0 unx     5917 b- defN 23-Jul-18 02:57 bigdl/llm/langchain/embeddings/transformersembeddings.py
+-rw-rw-r--  2.0 unx     1414 b- defN 23-Jul-18 02:57 bigdl/llm/langchain/llms/__init__.py
+-rw-rw-r--  2.0 unx    12672 b- defN 23-Jul-18 02:57 bigdl/llm/langchain/llms/bigdlllm.py
+-rw-rw-r--  2.0 unx     7162 b- defN 23-Jul-31 05:59 bigdl/llm/langchain/llms/transformersllm.py
+-rw-rw-r--  2.0 unx     7371 b- defN 23-Jul-18 02:57 bigdl/llm/langchain/llms/transformerspipelinellm.py
+-rwxrwxr-x  2.0 unx   139056 b- defN 23-Aug-03 02:02 bigdl/llm/libs/libbloom-api.so
+-rwxrwxr-x  2.0 unx   500536 b- defN 23-Aug-03 02:01 bigdl/llm/libs/libbloom_avx2.so
+-rwxrwxr-x  2.0 unx   500536 b- defN 23-Aug-03 02:01 bigdl/llm/libs/libbloom_avx512.so
+-rwxrwxr-x  2.0 unx    23664 b- defN 23-Aug-03 02:02 bigdl/llm/libs/libgptneox-api.so
+-rwxrwxr-x  2.0 unx   535368 b- defN 23-Aug-03 02:01 bigdl/llm/libs/libgptneox_avx2.so
+-rwxrwxr-x  2.0 unx   535368 b- defN 23-Aug-03 02:01 bigdl/llm/libs/libgptneox_avx512.so
+-rwxrwxr-x  2.0 unx    23696 b- defN 23-Aug-03 02:02 bigdl/llm/libs/libllama-api.so
+-rwxrwxr-x  2.0 unx   539448 b- defN 23-Aug-03 02:00 bigdl/llm/libs/libllama_avx2.so
+-rwxrwxr-x  2.0 unx   539448 b- defN 23-Aug-03 02:01 bigdl/llm/libs/libllama_avx512.so
+-rwxrwxr-x  2.0 unx    21984 b- defN 23-Aug-03 02:02 bigdl/llm/libs/libstarcoder-api.so
+-rwxrwxr-x  2.0 unx   657880 b- defN 23-Aug-03 02:01 bigdl/llm/libs/libstarcoder_avx2.so
+-rwxrwxr-x  2.0 unx   657880 b- defN 23-Aug-03 02:01 bigdl/llm/libs/libstarcoder_avx512.so
+-rwxrwxr-x  2.0 unx   188984 b- defN 23-Aug-03 02:02 bigdl/llm/libs/main-bloom
+-rwxrwxr-x  2.0 unx  1715504 b- defN 23-Aug-03 02:02 bigdl/llm/libs/main-chatglm_vnni
+-rwxrwxr-x  2.0 unx   175512 b- defN 23-Aug-03 02:02 bigdl/llm/libs/main-gptneox
+-rwxrwxr-x  2.0 unx   175440 b- defN 23-Aug-03 02:02 bigdl/llm/libs/main-llama
+-rwxrwxr-x  2.0 unx   314400 b- defN 23-Aug-03 02:02 bigdl/llm/libs/main-starcoder
+-rwxrwxr-x  2.0 unx   469256 b- defN 23-Aug-03 02:01 bigdl/llm/libs/quantize-bloom
+-rwxrwxr-x  2.0 unx   477640 b- defN 23-Aug-03 02:01 bigdl/llm/libs/quantize-gptneox
+-rwxrwxr-x  2.0 unx   477968 b- defN 23-Aug-03 02:01 bigdl/llm/libs/quantize-llama
+-rwxrwxr-x  2.0 unx   491480 b- defN 23-Aug-03 02:02 bigdl/llm/libs/quantize-starcoder
+-rw-rw-r--  2.0 unx      780 b- defN 23-Jul-19 03:04 bigdl/llm/transformers/__init__.py
+-rw-rw-r--  2.0 unx     5498 b- defN 23-Jul-31 05:59 bigdl/llm/transformers/convert.py
+-rw-rw-r--  2.0 unx     8660 b- defN 23-Jul-31 05:59 bigdl/llm/transformers/linear_quant.py
+-rw-rw-r--  2.0 unx    10414 b- defN 23-Aug-02 09:08 bigdl/llm/transformers/model.py
+-rw-rw-r--  2.0 unx     3609 b- defN 23-Jul-18 02:57 bigdl/llm/transformers/modelling_bigdl.py
+-rw-rw-r--  2.0 unx     5301 b- defN 23-Jul-31 05:59 bigdl/llm/transformers/utils.py
+-rw-rw-r--  2.0 unx      584 b- defN 23-Aug-02 06:54 bigdl/llm/transformers/models/__init__.py
+-rw-rw-r--  2.0 unx     9264 b- defN 23-Aug-02 06:54 bigdl/llm/transformers/models/llama.py
+-rw-rw-r--  2.0 unx      896 b- defN 23-Jun-02 07:39 bigdl/llm/utils/__init__.py
+-rw-rw-r--  2.0 unx    17954 b- defN 23-Aug-02 06:54 bigdl/llm/utils/convert_chatglm.py
+-rw-rw-r--  2.0 unx    64300 b- defN 23-Aug-02 06:54 bigdl/llm/utils/convert_util.py
+-rw-rw-r--  2.0 unx     2102 b- defN 23-Jul-31 05:59 bigdl/llm/utils/isa_checker.py
+-rw-rw-r--  2.0 unx     2018 b- defN 23-Aug-02 09:07 bigdl/llm/utils/utils.py
+-rw-rw-r--  2.0 unx      988 b- defN 23-Aug-02 09:08 bigdl/llm/utils/common/__init__.py
+-rw-rw-r--  2.0 unx     2874 b- defN 23-Jun-14 03:58 bigdl/llm/utils/common/lazyimport.py
+-rw-rw-r--  2.0 unx     1763 b- defN 23-Aug-02 09:08 bigdl/llm/utils/common/log4Error.py
+-rwxrwxr-x  2.0 unx     2251 b- defN 23-Aug-02 09:07 bigdl_llm-2.4.0b20230802.dev0.data/scripts/llm-chat
+-rwxrwxr-x  2.0 unx     2629 b- defN 23-Aug-02 09:07 bigdl_llm-2.4.0b20230802.dev0.data/scripts/llm-cli
+-rw-rw-r--  2.0 unx      902 b- defN 23-Aug-03 02:02 bigdl_llm-2.4.0b20230802.dev0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      109 b- defN 23-Aug-03 02:02 bigdl_llm-2.4.0b20230802.dev0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       61 b- defN 23-Aug-03 02:02 bigdl_llm-2.4.0b20230802.dev0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        6 b- defN 23-Aug-03 02:02 bigdl_llm-2.4.0b20230802.dev0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     7805 b- defN 23-Aug-03 02:02 bigdl_llm-2.4.0b20230802.dev0.dist-info/RECORD
+85 files, 9638273 bytes uncompressed, 3739496 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -6,17 +6,23 @@
 
 Filename: bigdl/llm/convert_model.py
 Comment: 
 
 Filename: bigdl/llm/models.py
 Comment: 
 
+Filename: bigdl/llm/cli/llm-chat
+Comment: 
+
 Filename: bigdl/llm/cli/llm-chat.ps1
 Comment: 
 
+Filename: bigdl/llm/cli/llm-cli
+Comment: 
+
 Filename: bigdl/llm/cli/llm-cli.ps1
 Comment: 
 
 Filename: bigdl/llm/cli/prompts/chat-with-llm.txt
 Comment: 
 
 Filename: bigdl/llm/ggml/__init__.py
@@ -111,87 +117,75 @@
 
 Filename: bigdl/llm/langchain/llms/transformersllm.py
 Comment: 
 
 Filename: bigdl/llm/langchain/llms/transformerspipelinellm.py
 Comment: 
 
-Filename: bigdl/llm/libs/bloom-api.dll
-Comment: 
-
-Filename: bigdl/llm/libs/bloom.dll
-Comment: 
-
-Filename: bigdl/llm/libs/gptneox-api.dll
-Comment: 
-
-Filename: bigdl/llm/libs/gptneox.dll
-Comment: 
-
-Filename: bigdl/llm/libs/libbloom_vnni.dll
+Filename: bigdl/llm/libs/libbloom-api.so
 Comment: 
 
-Filename: bigdl/llm/libs/libgptneox_vnni.dll
+Filename: bigdl/llm/libs/libbloom_avx2.so
 Comment: 
 
-Filename: bigdl/llm/libs/libllama_vnni.dll
+Filename: bigdl/llm/libs/libbloom_avx512.so
 Comment: 
 
-Filename: bigdl/llm/libs/libstarcoder_vnni.dll
+Filename: bigdl/llm/libs/libgptneox-api.so
 Comment: 
 
-Filename: bigdl/llm/libs/llama-api.dll
+Filename: bigdl/llm/libs/libgptneox_avx2.so
 Comment: 
 
-Filename: bigdl/llm/libs/llama.dll
+Filename: bigdl/llm/libs/libgptneox_avx512.so
 Comment: 
 
-Filename: bigdl/llm/libs/main-bloom.exe
+Filename: bigdl/llm/libs/libllama-api.so
 Comment: 
 
-Filename: bigdl/llm/libs/main-chatglm_vnni.exe
+Filename: bigdl/llm/libs/libllama_avx2.so
 Comment: 
 
-Filename: bigdl/llm/libs/main-gptneox.exe
+Filename: bigdl/llm/libs/libllama_avx512.so
 Comment: 
 
-Filename: bigdl/llm/libs/main-llama.exe
+Filename: bigdl/llm/libs/libstarcoder-api.so
 Comment: 
 
-Filename: bigdl/llm/libs/main-starcoder.exe
+Filename: bigdl/llm/libs/libstarcoder_avx2.so
 Comment: 
 
-Filename: bigdl/llm/libs/quantize-bloom.exe
+Filename: bigdl/llm/libs/libstarcoder_avx512.so
 Comment: 
 
-Filename: bigdl/llm/libs/quantize-bloom_vnni.exe
+Filename: bigdl/llm/libs/main-bloom
 Comment: 
 
-Filename: bigdl/llm/libs/quantize-gptneox.exe
+Filename: bigdl/llm/libs/main-chatglm_vnni
 Comment: 
 
-Filename: bigdl/llm/libs/quantize-gptneox_vnni.exe
+Filename: bigdl/llm/libs/main-gptneox
 Comment: 
 
-Filename: bigdl/llm/libs/quantize-llama.exe
+Filename: bigdl/llm/libs/main-llama
 Comment: 
 
-Filename: bigdl/llm/libs/quantize-llama_vnni.exe
+Filename: bigdl/llm/libs/main-starcoder
 Comment: 
 
-Filename: bigdl/llm/libs/quantize-starcoder.exe
+Filename: bigdl/llm/libs/quantize-bloom
 Comment: 
 
-Filename: bigdl/llm/libs/quantize-starcoder_vnni.exe
+Filename: bigdl/llm/libs/quantize-gptneox
 Comment: 
 
-Filename: bigdl/llm/libs/starcoder-api.dll
+Filename: bigdl/llm/libs/quantize-llama
 Comment: 
 
-Filename: bigdl/llm/libs/starcoder.dll
+Filename: bigdl/llm/libs/quantize-starcoder
 Comment: 
 
 Filename: bigdl/llm/transformers/__init__.py
 Comment: 
 
 Filename: bigdl/llm/transformers/convert.py
 Comment: 
@@ -234,29 +228,29 @@
 
 Filename: bigdl/llm/utils/common/lazyimport.py
 Comment: 
 
 Filename: bigdl/llm/utils/common/log4Error.py
 Comment: 
 
-Filename: bigdl_llm-2.4.0b20230802.data/scripts/llm-chat.ps1
+Filename: bigdl_llm-2.4.0b20230802.dev0.data/scripts/llm-chat
 Comment: 
 
-Filename: bigdl_llm-2.4.0b20230802.data/scripts/llm-cli.ps1
+Filename: bigdl_llm-2.4.0b20230802.dev0.data/scripts/llm-cli
 Comment: 
 
-Filename: bigdl_llm-2.4.0b20230802.dist-info/METADATA
+Filename: bigdl_llm-2.4.0b20230802.dev0.dist-info/METADATA
 Comment: 
 
-Filename: bigdl_llm-2.4.0b20230802.dist-info/WHEEL
+Filename: bigdl_llm-2.4.0b20230802.dev0.dist-info/WHEEL
 Comment: 
 
-Filename: bigdl_llm-2.4.0b20230802.dist-info/entry_points.txt
+Filename: bigdl_llm-2.4.0b20230802.dev0.dist-info/entry_points.txt
 Comment: 
 
-Filename: bigdl_llm-2.4.0b20230802.dist-info/top_level.txt
+Filename: bigdl_llm-2.4.0b20230802.dev0.dist-info/top_level.txt
 Comment: 
 
-Filename: bigdl_llm-2.4.0b20230802.dist-info/RECORD
+Filename: bigdl_llm-2.4.0b20230802.dev0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bigdl/llm/utils/utils.py

```diff
@@ -40,20 +40,18 @@
     if sys.platform.startswith("linux") or sys.platform == "darwin":
         lib_ext = ".so"
     elif sys.platform == "win32":
         lib_ext = ".dll"
     else:
         invalidInputError(False, "Unsupported platform.")
 
-    cpuflags = get_cpu_flags()
-
     # Construct the paths to the possible shared library names (python/llm/src/bigdl/llm/libs)
     _base_path = pathlib.Path(__file__).parent.parent.resolve()
     _base_path = _base_path / 'libs'
     # Searching for the library in the current directory under the name "lib{lib_base_name}"
     # (default name for llmcpp) and "{lib_base_name}" (default name for this repo)
     _lib_paths = [
-        _base_path / f"lib{lib_base_name}{cpuflags}{lib_ext}",
-        _base_path / f"{lib_base_name}{cpuflags}{lib_ext}",
+        _base_path / f"lib{lib_base_name}-api{lib_ext}",
+        _base_path / f"{lib_base_name}-api{lib_ext}",
     ]
 
     return _base_path, _lib_paths
```

## Comparing `bigdl_llm-2.4.0b20230802.data/scripts/llm-cli.ps1` & `bigdl/llm/cli/llm-cli`

 * *Files 27% similar despite different names*

```diff
@@ -1,114 +1,113 @@
-$llm_dir = (Split-Path -Parent (python -c "import bigdl.llm;print(bigdl.llm.__file__)"))
-$lib_dir = Join-Path $llm_dir "libs"
+#!/bin/bash
 
-
-$vnni_enable = ((python -c "from bigdl.llm.utils.isa_checker import check_avx_vnni;print(check_avx_vnni())").ToLower() -eq "true")
-$model_family = ""
-$threads = 8
-$n_predict = 128
+# Default values
+model_family=""
+threads=8
+n_predict=128
+
+
+llm_dir="$(dirname "$(python -c "import bigdl.llm;print(bigdl.llm.__file__)")")"
+lib_dir="$llm_dir/libs"
+
+function get_avx_flags() {
+  avx="avx2"
+  if command -v lscpu &>/dev/null; then
+    msg=$(lscpu)
+    if [[ $msg == *"avx512_vnni"* ]]; then
+      avx="avx512"
+    fi
+  else
+    echo "lscpu command not found. Please make sure it is installed."
+  fi
+  echo $avx
+}
 
 # Function to display help message
-function Display-Help
-{
-    Write-Host "usage: ./llm-cli.ps1 -x MODEL_FAMILY [-h] [args]"
-    Write-Host ""
-    Write-Host "options:"
-    Write-Host "  -h, --help           show this help message"
-    Write-Host "  -x, --model_family {llama,bloom,gptneox,starcoder,chatglm}"
-    Write-Host "                       family name of model"
-    Write-Host "  -t N, --threads N    number of threads to use during computation (default: 8)"
-    Write-Host "  -n N, --n_predict N  number of tokens to predict (default: 128, -1 = infinity)"
-    Write-Host "  args                 parameters passed to the specified model function"
-}
-
-function llama
-{
-    $exec_file = "main-llama.exe"
-    $command = "$lib_dir/$exec_file -t $threads -n $n_predict $filteredArguments"
-    Write-Host "$command"
-    Invoke-Expression $command
-}
-
-function bloom
-{
-    $exec_file = "main-bloom.exe"
-    $command = "$lib_dir/$exec_file -t $threads -n $n_predict $filteredArguments"
-    Write-Host "$command"
-    Invoke-Expression $command
-}
-
-function gptneox
-{
-    $exec_file = "main-gptneox.exe"
-    $command = "$lib_dir/$exec_file -t $threads -n $n_predict $filteredArguments"
-    Write-Host "$command"
-    Invoke-Expression $command
-}
-
-function starcoder
-{
-    $exec_file = "main-starcoder.exe"
-    $command = "$lib_dir/$exec_file -t $threads -n $n_predict $filteredArguments"
-    Write-Host "$command"
-    Invoke-Expression $command
-}
-
-function chatglm
-{
-    $exec_file = "main-chatglm_vnni.exe"
-    $command = "$lib_dir/$exec_file -t $threads -n $n_predict $filteredArguments"
-    Write-Host "$command"
-    Invoke-Expression $command
+function display_help {
+  echo "usage: ./llm-cli.sh -x MODEL_FAMILY [-h] [args]"
+  echo ""
+  echo "options:"
+  echo "  -h, --help           show this help message"
+  echo "  -x, --model_family {llama,bloom,gptneox,starcoder,chatglm}"
+  echo "                       family name of model"
+  echo "  -t N, --threads N    number of threads to use during computation (default: 8)"
+  echo "  -n N, --n_predict N  number of tokens to predict (default: 128, -1 = infinity)"
+  echo "  args                 parameters passed to the specified model function"
+}
+
+function llama {
+  command="$lib_dir/main-llama -t $threads -n $n_predict ${filteredArguments[*]}"
+  echo "$command"
+  eval "$command"
+}
+
+function bloom {
+  command="$lib_dir/main-bloom -t $threads -n $n_predict ${filteredArguments[*]}"
+  echo "$command"
+  eval "$command"
+}
+
+function gptneox {
+  command="$lib_dir/main-gptneox -t $threads -n $n_predict ${filteredArguments[*]}"
+  echo "$command"
+  eval "$command"
+}
+
+function starcoder {
+  command="$lib_dir/main-starcoder -t $threads -n $n_predict ${filteredArguments[*]}"
+  echo "$command"
+  eval "$command"
+}
+
+function chatglm {
+  command="$lib_dir/main-chatglm_vnni -t $threads -n $n_predict ${filteredArguments[*]}"
+  echo "$command"
+  eval "$command"
 }
 
-
 # Remove model_family/x parameter
-$filteredArguments = @()
-for ($i = 0; $i -lt $args.Length; $i++) {
-    if ($args[$i] -eq '--model_family' -or $args[$i] -eq '--model-family' -or $args[$i] -eq '-x')
-    {
-        if ($i + 1 -lt $args.Length -and $args[$i + 1] -notlike '-*')
-        {
-            $i++
-            $model_family = $args[$i]
-        }
-    }
-    elseif ($args[$i] -eq '--threads' -or $args[$i] -eq '-t')
-    {
-        $i++
-        $threads = $args[$i]
-    }
-    elseif ($args[$i] -eq '--n_predict' -or $args[$i] -eq '--n-predict' -or $args[$i] -eq '-n')
-    {
-        $i++
-        $n_predict = $args[$i]
-    }
-    else
-    {
-        $filteredArguments += "`'" + $args[$i] + "`'"
-    }
-}
+filteredArguments=()
+while [[ $# -gt 0 ]]; do
+  case "$1" in
+  -h | --help)
+    display_help
+    filteredArguments+=("'$1'")
+    shift
+    ;;
+  -x | --model_family | --model-family)
+    model_family="$2"
+    shift 2
+    ;;
+  -t | --threads)
+    threads="$2"
+    shift 2
+    ;;
+  -n | --n_predict | --n-predict)
+    n_predict="$2"
+    shift 2
+    ;;
+  *)
+    filteredArguments+=("'$1'")
+    shift
+    ;;
+  esac
+done
+
+avx_flag=$(get_avx_flags)
+echo "AVX Flags: $avx_flag"
 
 # Perform actions based on the model_family
-switch ($model_family)
-{
-    "llama" {
-        llama
-    }
-    "bloom" {
-        bloom
-    }
-    "gptneox" {
-        gptneox
-    }
-    "starcoder" {
-        starcoder
-    }
-    "chatglm" {
-        chatglm
-    }
-    default {
-        Write-Host "Invalid model_family: $model_family"
-        Display-Help
-    }
-}
+if [[ "$model_family" == "llama" ]]; then
+  llama
+elif [[ "$model_family" == "bloom" ]]; then
+  bloom
+elif [[ "$model_family" == "gptneox" ]]; then
+  gptneox
+elif [[ "$model_family" == "starcoder" ]]; then
+  starcoder
+elif [[ "$model_family" == "chatglm" ]]; then
+  chatglm
+else
+  echo "Invalid model_family: $model_family"
+  display_help
+fi
```

## Comparing `bigdl_llm-2.4.0b20230802.dist-info/METADATA` & `bigdl_llm-2.4.0b20230802.dev0.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigdl-llm
-Version: 2.4.0b20230802
+Version: 2.4.0b20230802.dev0
 Summary: Large Language Model Develop Toolkit
 Home-page: https://github.com/intel-analytics/BigDL
 Author: BigDL Authors
 Author-email: bigdl-user-group@googlegroups.com
 License: Apache License, Version 2.0
 Platform: windows
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,10 +18,8 @@
 Requires-Dist: torch ; extra == 'all'
 Requires-Dist: transformers ; extra == 'all'
 Requires-Dist: sentencepiece ; extra == 'all'
 Requires-Dist: accelerate ; extra == 'all'
 Requires-Dist: tabulate ; extra == 'all'
 
 
-BigDL LLM
-
-
+    BigDL LLM
```

## Comparing `bigdl_llm-2.4.0b20230802.dist-info/RECORD` & `bigdl_llm-2.4.0b20230802.dev0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 bigdl/__init__.py,sha256=9RhNOlx9rGC96ZLIJFCFSApoifpjHoayBKx7N9ZKSno,956
 bigdl/llm/__init__.py,sha256=t7e6iUPBEa2EPLhZHm9sm-4SiyLrOZh184HJ-dpdyfc,914
 bigdl/llm/convert_model.py,sha256=aO56x8M7MMIoK-gMGc1ZD5qRnzXkV9Jw-Y1KhqFP2Bc,6809
 bigdl/llm/models.py,sha256=M9W7VwFmiEXQ_HedzmSztRoIUNjFKW-ybvTvSXBPtb8,1067
+bigdl/llm/cli/llm-chat,sha256=BMwl3KyooUjF5U3l4eZIlnbe4zl2KZ6XDIKi79-3CU4,2251
 bigdl/llm/cli/llm-chat.ps1,sha256=PpUox9_gWYhERqZazhIRJnAzAHbp6l2JzwPy633AVLQ,2772
+bigdl/llm/cli/llm-cli,sha256=1dKHGO9uyRQBa2_-Ksi0kkCUNn1vKcnJztC2gktwLEM,2629
 bigdl/llm/cli/llm-cli.ps1,sha256=gyq9Fcv4frezJoNqQkNjPlGOVfusa-QN0zBO7VWRHjU,3012
 bigdl/llm/cli/prompts/chat-with-llm.txt,sha256=PpSyd4FQQd-T7ptfXL9jZp7dgstevu1fsxWFa0IQ5Oc,216
 bigdl/llm/ggml/__init__.py,sha256=Flc31gOq42SIKILIniO8i7Zp_is1A3uKRcqBM7TFK1g,994
 bigdl/llm/ggml/convert.py,sha256=0t13SJxnd5ajRHD8YVv1G1FnU36aP3LYl2ApPV4gJuQ,5378
 bigdl/llm/ggml/convert_model.py,sha256=Q-NdOp_TA8hVXzBzi8jA1tUk_8uRJ9TgE1JNX64Ykc0,6255
 bigdl/llm/ggml/quantize.py,sha256=E5EOgx67uKcWvd3wxVHVlb65aN-Xq0kHrXee9c9FbOs,5183
 bigdl/llm/ggml/model/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
@@ -33,55 +35,51 @@
 bigdl/llm/langchain/embeddings/__init__.py,sha256=ARJpCQZJ4bN7aCdCN0Fe7iVkJPXWgLzM24Gxkmmp924,1051
 bigdl/llm/langchain/embeddings/bigdlllm.py,sha256=dFn2LX7sO5KGKaVIj15YruBRaHagll_HaQfxdikzCdU,7039
 bigdl/llm/langchain/embeddings/transformersembeddings.py,sha256=9ryHKPnV5dboWAogpTWfdCz29W7xD52tqWqU9jfzLbY,5917
 bigdl/llm/langchain/llms/__init__.py,sha256=GEmxa4Qu87PLlSAviSzWIAp-ZM8LPyFb44abR3jFQqI,1414
 bigdl/llm/langchain/llms/bigdlllm.py,sha256=_vVQsai2Drh0uoPhU97hX30pBdH948WeUoAB_4VtYWg,12672
 bigdl/llm/langchain/llms/transformersllm.py,sha256=r6EKzLf_qgXIwmvOf_LPQ0uRDMLiw8DUHpJJv4w-3ZM,7162
 bigdl/llm/langchain/llms/transformerspipelinellm.py,sha256=9Cnhibr6TXTuZn1ZCkdWFD_KPdZFW67XE0BG5dxQZoo,7371
-bigdl/llm/libs/bloom-api.dll,sha256=VIlLTuugwtLSRuKzdf40Otp8IdOLvugZrA5-YPw3eAc,36352
-bigdl/llm/libs/bloom.dll,sha256=2NQGG61gCjwtAIsGP3v12hw_di13GaqORuiP7mFrV0Q,359936
-bigdl/llm/libs/gptneox-api.dll,sha256=uvO_QdHOkeh7Dt1b6IyMk2trYT_nTByOuwYGA78JPkA,24576
-bigdl/llm/libs/gptneox.dll,sha256=HurthJ4aX3E_b_3jnmWlw39_DGgGW44J7H2Bs8nJgQA,429568
-bigdl/llm/libs/libbloom_vnni.dll,sha256=FNOZkGF_NvksBP2-YRM7gZjpmnEo6lCQaa5ByKULL7k,360448
-bigdl/llm/libs/libgptneox_vnni.dll,sha256=AYmXYsg3AdXFVTTUAism12ipt4ZCjG8Zp0l32I3INsM,430080
-bigdl/llm/libs/libllama_vnni.dll,sha256=nFjmdw6lorUvWPOE1qWKSCB8od8DPp9adYJSuGBisRU,425472
-bigdl/llm/libs/libstarcoder_vnni.dll,sha256=-ZNKthS59ihNUVykfQofajA3kc8EzOrQwuAv5pdbTV0,452608
-bigdl/llm/libs/llama-api.dll,sha256=gKyg6ZLRXnRLeOvMWvyKsmjCYzxfl8IsVScOXXKKKUQ,25088
-bigdl/llm/libs/llama.dll,sha256=3-ZFmT2Yj1rN5wm_r91sbxFP3_n0HC-DJ0vDkkm0OmA,424960
-bigdl/llm/libs/main-bloom.exe,sha256=d7Ns7H5dg3lEJttgX9MIV1FuopFpPDkSkSc_buJ_uNA,102912
-bigdl/llm/libs/main-chatglm_vnni.exe,sha256=3nT4BYAvUbM-5fCzGbQsTpKxPz09qfFKZDUk51ZwgrA,712704
-bigdl/llm/libs/main-gptneox.exe,sha256=OVcRZGVWXX3hcZizzR7jCK-gYeB4U2KwEM5fpjeCGbE,98816
-bigdl/llm/libs/main-llama.exe,sha256=48SuFN2vWPy6_mBt-JtIDQ_gmVhfLl-HHGBfTdDTqbc,100352
-bigdl/llm/libs/main-starcoder.exe,sha256=arG99iVBkaxJ0cN4xDIRMPlHXmvMt9rLgJZTbKRVLPU,157184
-bigdl/llm/libs/quantize-bloom.exe,sha256=PtFkpBtk_QlTT6OMlH3ptomUZfXRWc1v4kGhLuUNWnY,116224
-bigdl/llm/libs/quantize-bloom_vnni.exe,sha256=imZYXmMTGsXR1uY3jEnwT7AROoj9khafKE9xJOyuSCk,116736
-bigdl/llm/libs/quantize-gptneox.exe,sha256=LUk2Z3eYrDNAxXg10_DekKWhBlApkyQv-WAhfzMnb3c,97280
-bigdl/llm/libs/quantize-gptneox_vnni.exe,sha256=eIeKavIGH3lkO3cxv86RHcWeoBCkzZDyqCbn6qzP7Q8,97792
-bigdl/llm/libs/quantize-llama.exe,sha256=KED9AgfP9TTb-Wx_7SId8T-NzGb1vGF11_d0sLpgdHY,101888
-bigdl/llm/libs/quantize-llama_vnni.exe,sha256=2orfPceHUw8LCFF0MFu20o-OUlDqO_6ou-pJdDd7i6Y,102400
-bigdl/llm/libs/quantize-starcoder.exe,sha256=vxDL3v1SlwnwC28m53FMMCzvs60Sa_ivq3emKwrv-3A,116736
-bigdl/llm/libs/quantize-starcoder_vnni.exe,sha256=zzfEolIirC7tQtJ5O9ghlQk-UtJnfSs2AaSvr5p4vrY,117248
-bigdl/llm/libs/starcoder-api.dll,sha256=DH2iA0x-zqMEXPe1fE1NFNLVPu4GzH509lLG_9MAn7o,21504
-bigdl/llm/libs/starcoder.dll,sha256=yIZh8MaHK7movgI2qjwbG4R013EjbQXqtcRbzzoLrdI,451584
+bigdl/llm/libs/libbloom-api.so,sha256=c0GHDHf13_YN116_FRhBjL6ehzOkXPq110ndU2xXH5E,139056
+bigdl/llm/libs/libbloom_avx2.so,sha256=nwyqXL3pbQf8xyZespKoUOECPZWiZAVq3tyPk0ro8EY,500536
+bigdl/llm/libs/libbloom_avx512.so,sha256=OmNkxic9Ahe0K6QYQhgqPxjifG9xq5w1vprxRot_zwg,500536
+bigdl/llm/libs/libgptneox-api.so,sha256=wv-Mlyk-85uX8QuBRiPwWV-5iEtF0LL7QLq-tf0iOts,23664
+bigdl/llm/libs/libgptneox_avx2.so,sha256=MXnltaB3VYPb3Qg_TBcSCgoC8OwdDUNgdI7NdaX38wI,535368
+bigdl/llm/libs/libgptneox_avx512.so,sha256=vl4KQ7JBk0zbM3wsS8QC-geim-5T_xjiWK3uo1TicFI,535368
+bigdl/llm/libs/libllama-api.so,sha256=GVGakRdRKAnKcxATUGJydTvtgsTcVfCgLGG0P0_5M7U,23696
+bigdl/llm/libs/libllama_avx2.so,sha256=JJXh1KFljYgL6v6VHuWYihEzpx7ppWentuoOuCFhX54,539448
+bigdl/llm/libs/libllama_avx512.so,sha256=R2FgUBkO35_GP61gl0ZNQdMB-who8diV4Kj_nUbNtQw,539448
+bigdl/llm/libs/libstarcoder-api.so,sha256=frkDRgRXsFCTw1DEDIgVWP1R1XdPuRzzaFpAc-FpYwM,21984
+bigdl/llm/libs/libstarcoder_avx2.so,sha256=bk-2bEJAvR2zhtI49bV8_vmX3sAl-KCjReuGnWNxc7c,657880
+bigdl/llm/libs/libstarcoder_avx512.so,sha256=_eOu_s-5HXkH9XMVamcntzmIeFooax583hymkn4GxlE,657880
+bigdl/llm/libs/main-bloom,sha256=H77AnNSabbbxq4mwdmrW-FuYV19AGfl7bti7maHMBPk,188984
+bigdl/llm/libs/main-chatglm_vnni,sha256=T500OEUdzYx6Nw840zf4kLKL88HSq-tc_SwX6CEmKVo,1715504
+bigdl/llm/libs/main-gptneox,sha256=TnTKO54LQTGXktXwgSSuFPKjwvB7D6KvqRJBcpYm56A,175512
+bigdl/llm/libs/main-llama,sha256=TeN7zzS1CMLSEQ6pGcNK6WxpLXHtuhPzqgoUTHd64_M,175440
+bigdl/llm/libs/main-starcoder,sha256=j0W7XsQENbCVLTQG2NPRfvlZFgWvKoL1Ubrrs8xWGA8,314400
+bigdl/llm/libs/quantize-bloom,sha256=n9_b9sk4NqnFJoTAZ8IX6ppRCuHIVg4319WOs9tXb6Q,469256
+bigdl/llm/libs/quantize-gptneox,sha256=qD5KTbWT-gCru1ZZD-Hc_d7lq2k0Up-dlQJKW8ezFrg,477640
+bigdl/llm/libs/quantize-llama,sha256=KsiBCSczDWfNAhqyHPEdn_OvTqC-C3VGDMpPHCWlmKc,477968
+bigdl/llm/libs/quantize-starcoder,sha256=sTgyOtyEX3AymbDScqGeCAb_Y-iRn8A9hrT67-hLHVw,491480
 bigdl/llm/transformers/__init__.py,sha256=XVoiHO6rr_FAgRvYVlo5DneDAmaGTBPAsd42zUMx1eg,780
 bigdl/llm/transformers/convert.py,sha256=lYX7BWRArEbqAOMroiPiLfnb1Ak08WVpC5XxBcPMOA8,5498
 bigdl/llm/transformers/linear_quant.py,sha256=3nWmFQXUpBHEG3NIFmy69T4Db1XWnaKuVbpE6vSkQjg,8660
 bigdl/llm/transformers/model.py,sha256=6fxx2RG9zH67KR9WrPg_Ol1-fqr-qxStaaKRvXZVCLI,10414
 bigdl/llm/transformers/modelling_bigdl.py,sha256=uxkU1C1dxPNh4g7NDae7AC-07pbZa7bA7T1uKI0vP0g,3609
 bigdl/llm/transformers/utils.py,sha256=bL5vvsfVklXt9YEQvzO55XuzwBAvQqUAwkfXaA863G0,5301
 bigdl/llm/transformers/models/__init__.py,sha256=tp2DcVkKg1-QvdYk7DY7rZvQWCDQ4ZjU8NAQ7Fclrpg,584
 bigdl/llm/transformers/models/llama.py,sha256=N2wmcKQ7vIUTCPtkUa0Lmv6Tf_ApYFfyKiEMOMGP_MM,9264
 bigdl/llm/utils/__init__.py,sha256=f_oavwQog8Wd1fSIebb-KgA61UKSzcOgw4cBxMHyS_w,896
 bigdl/llm/utils/convert_chatglm.py,sha256=RzuxWo5c3MKqH8pxW8ddw3nx2s6goXhSc2V17HBD80k,17954
 bigdl/llm/utils/convert_util.py,sha256=ukcnBBILLDPLELRld9q9AV5ijFMOch-CMqC8M9wdF6Y,64300
 bigdl/llm/utils/isa_checker.py,sha256=qqm6fguUz8Vxq6uOJeewLtefwphGzEcMIn7CQsX2vhw,2102
-bigdl/llm/utils/utils.py,sha256=NyCqzywDJMMYcyrHdZpZ3a_oAUstXh1769AehhzqwF4,2062
+bigdl/llm/utils/utils.py,sha256=11R2GNuz7SMPhHzgEao-2TiUaAnVvytvOiHK7zYrZfY,2018
 bigdl/llm/utils/common/__init__.py,sha256=pV_8I-oa8RrHSCJg6ADBY_Tre6vXCqAMyhfpj1UhvYE,988
 bigdl/llm/utils/common/lazyimport.py,sha256=TVDp-rtc6IHopmlS9WEIgP5GKg5i0iWGm8khPwG4jTo,2874
 bigdl/llm/utils/common/log4Error.py,sha256=8UgIpEJYQasQO4gMOWO22nsOgr14w1emAJy4ts1VOb0,1763
-bigdl_llm-2.4.0b20230802.data/scripts/llm-chat.ps1,sha256=PpUox9_gWYhERqZazhIRJnAzAHbp6l2JzwPy633AVLQ,2772
-bigdl_llm-2.4.0b20230802.data/scripts/llm-cli.ps1,sha256=gyq9Fcv4frezJoNqQkNjPlGOVfusa-QN0zBO7VWRHjU,3012
-bigdl_llm-2.4.0b20230802.dist-info/METADATA,sha256=N32CWbPSgD1Qzi0XFnYaZMQxgKBjefRzq72_iH6TV6Q,895
-bigdl_llm-2.4.0b20230802.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-bigdl_llm-2.4.0b20230802.dist-info/entry_points.txt,sha256=FClDfgRtVDhPPUsMDgDOZvqNZTS_vBpqhJvYkv0YzLM,62
-bigdl_llm-2.4.0b20230802.dist-info/top_level.txt,sha256=iGuLfZARD_qANcIMfy0tbbrC3EtCg6BSiH8icc3dLWs,6
-bigdl_llm-2.4.0b20230802.dist-info/RECORD,,
+bigdl_llm-2.4.0b20230802.dev0.data/scripts/llm-chat,sha256=BMwl3KyooUjF5U3l4eZIlnbe4zl2KZ6XDIKi79-3CU4,2251
+bigdl_llm-2.4.0b20230802.dev0.data/scripts/llm-cli,sha256=1dKHGO9uyRQBa2_-Ksi0kkCUNn1vKcnJztC2gktwLEM,2629
+bigdl_llm-2.4.0b20230802.dev0.dist-info/METADATA,sha256=x6vIqHqH7qLm2KqZMZUrm6yF8ysCDqfB7o1thRkmndQ,902
+bigdl_llm-2.4.0b20230802.dev0.dist-info/WHEEL,sha256=QyVW29td8kQUmwJkwP_jcy6j1729n0g4-qDh7fl0mPw,109
+bigdl_llm-2.4.0b20230802.dev0.dist-info/entry_points.txt,sha256=rq4b1Rv6QNt4_gh1MY5D-Z4WOqAip1y4NqgaRMT2Pw4,61
+bigdl_llm-2.4.0b20230802.dev0.dist-info/top_level.txt,sha256=iGuLfZARD_qANcIMfy0tbbrC3EtCg6BSiH8icc3dLWs,6
+bigdl_llm-2.4.0b20230802.dev0.dist-info/RECORD,,
```

