# LLM-Inference-Acceleration

## Table of Contents

 - [About This Project](#about-this-project)
 - [Listing of Papers by Topics](#listing-of-papers-by-topics)
   - [Review](#review)
   - [Attention Mechanism](#attention-mechanism)
   - [Quantization](#quantization)
   - [KV Cache](#kv-cache)
   - [Continuous Batching](#continuous-batching)
   - [HW/SW Co-design](#hwsw-co-design)
   - [Framework/System/Architecture](#frameworksystemarchitecture)
   - [More](#more)

## About This Project
This project is dedicated to collecting and curating research papers focused on Large Language Model (LLM) inference acceleration. I hope to summarize and share the knowledge I gain during my self-learning journey.

It will be updated regularly. Contributions are welcome, so feel free to star or submit a pull request.

## Listing of Papers By Topics

Design Rule:
- Keywords: frequent academic terms for paper search.
- <mark>**Paper intro**: core idea/image with useful extensions are included for quick start. See example [[intro of SmoothQuant](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/quantization/smoothquant--accurate-and-efficient-post-training-quantization-for-large-language-models/README.md)].</mark>
- Citation: data for the papers is sourced from Google Scholar.

## Review
Last update of citation was on 28th July, 2024.

|Keywords | Title | Paper | Affiliation | Date | Citation|
|:---:|:---:|:---:|:---:|:---:|:---:|
|LLM Inference|**Towards Efficient Generative Large Language Model Serving: A Survey from Algorithms to Systems**|[[pdf](https://arxiv.org/abs/2312.15234)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/review/towards-efficient-generative-large-language-model-serving--a-survey-from-algorithms-to-systems/README.md)]|CMU|2023.12|36|
|LLM Inference|**A survey on efficient inference for large language models**|[[pdf](https://arxiv.org/abs/2404.14294)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/review/a-survey-on-efficient-inference-for-large-language-models/README.md)]|THU,  Infinigence-AI, SJTU etc|2024.04|14|

## Attention Mechanism
Last update of citation was on 20th Oct, 2024.

Upcoming topics include: FlashDecoding, QLoRA

|Keywords | Title | Paper | Affiliation | Date | Citation|
|:---:|:---:|:---:|:---:|:---:|:---:|
|MQA|**Fast Transformer Decoding: One Write-Head is All You Need**|[[pdf](https://arxiv.org/abs/1911.02150v1)]|Google|2019.11|176|
|GQA|**GQA: Training Generalized Multi-Query Transformer Models from Multi-Head Checkpoints** [EMNLP 2023]|[[pdf](https://arxiv.org/abs/2305.13245)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/attention-mechanism/gqa--training-generalized-multi-query-transformer-models-from-multi-head-checkpoints/README.md)]|Google|2023.05|174|
|ALiBi|**Train Short, Test Long: Attention with Linear Biases Enables Input Length Extrapolation** [ICLR 2022]|[[pdf](https://arxiv.org/abs/2108.12409)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/attention-mechanism/train-short--test-long--attention-with-linear-biases-enables-input-length-extrapolation/README.md)]|UW, Facebook, Allen Institute|2021.08|416|
|RoPE|**RoFormer: Enhanced Transformer with Rotary Position Embedding** [Neurocomputing 2024]|[[pdf](https://arxiv.org/abs/2104.09864)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/attention-mechanism/roformer--enhanced-transformer-with-rotary-position-embedding/README.md)]|Zhuiyi Technology|2021.04|937|
|CoPE|**Contextual Position Encoding: Learning to Count What's Important**|[[pdf](https://arxiv.org/abs/2405.18719)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/attention-mechanism/contextual-position-encoding--learning-to-count-what-s-important/README.md)]|Meta|2024.05|2|
|FlashAttention|**FlashAttention: Fast and Memory-Efficient Exact Attention with IO-Awareness** [NeurIPS 2022]|[[pdf](https://arxiv.org/abs/2205.14135)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/attention-mechanism/flashattention--fast-and-memory-efficient-exact-attention-with-io-awareness/README.md)]|Stanford, University at Buffalo|2022.05|915|
|FlashAttention2|**FlashAttention-2: Faster Attention with Better Parallelism and Work Partitioning**|[[pdf](https://arxiv.org/abs/2307.08691)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/attention-mechanism/flashattention-2--faster-attention-with-better-parallelism-and-work-partitioning/README.md)]|Princeton, Stanford|2023.07|281|
|Longformer|**Longformer: The Long-Document Transformer**|[[pdf](https://arxiv.org/abs/2004.05150)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/attention-mechanism/longformer--the-long-document-transformer/README.md)]|Allen Institute|2020.04|3605|
|Mistral|**Mistral 7B**|[[pdf](https://arxiv.org/abs/2310.06825)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/attention-mechanism/mistral-7b/README.md)]|Mistral|2023.10|313|
|StreamingLLM, Attention Sinks|**Efficient Streaming Language Models with Attention Sinks** [ICLR 2024]|[[pdf](https://arxiv.org/abs/2309.17453)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/attention-mechanism/efficient-streaming-language-models-with-attention-sinks/README.md)]|MIT, Meta, CMU etc|2023.09|146|
|LoRA|**LoRA: Low-Rank Adaptation of Large Language Models** [ICLR 2022]|[[pdf](https://arxiv.org/abs/2106.09685)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/attention-mechanism/lora--low-rank-adaptation-of-large-language-models/README.md)]|Microsoft|2021.06|4818|
|LISA|**LISA: Layerwise Importance Sampling for Memory-Efficient Large Language Model Fine-Tuning**|[[pdf](https://arxiv.org/abs/2403.17919)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/attention-mechanism/lisa--layerwise-importance-sampling-for-memory-efficient-large-language-model-fine-tuning/README.md)]|HKUST, UIUC|2024.03|2|
|HydraLoRA|**HydraLoRA: An Asymmetric LoRA Architecture for Efficient Fine-Tuning** [NIPS 2024]|[[pdf](https://arxiv.org/abs/2404.19245)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/attention-mechanism/hydralora--an-asymmetric-lora-architecture-for-efficient-fine-tuning/README.md)]|University of Macau, University of Texas at Austin, Cambridge|2024.04|2|

## Quantization
Last update of citation was on 5th July, 2024.

Upcoming topics include: QLoRA

|Keywords | Title | Paper | Affiliation | Date | Citation|
|:---:|:---:|:---:|:---:|:---:|:---:|
|LLM.int8|**LLM.int8(): 8-bit Matrix Multiplication for Transformers at Scale** [NeurIPS 2022]|[[pdf](https://arxiv.org/abs/2208.07339)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/quantization/llm.int8----8-bit-matrix-multiplication-for-transformers-at-scale/README.md)]|UW, Facebook, Hugging Face etc|2022.08|554|
|SmoothQuant|**SmoothQuant: Accurate and Efficient Post-Training Quantization for Large Language Models** [ICML 2023]|[[pdf](https://arxiv.org/abs/2211.10438)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/quantization/smoothquant--accurate-and-efficient-post-training-quantization-for-large-language-models/README.md)]|MIT, NVIDIA|2022.11|382|
|AWQ|**AWQ: Activation-aware Weight Quantization for LLM Compression and Acceleration** [MLSys 2024]|[[pdf](https://arxiv.org/abs/2306.00978)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/quantization/awq--activation-aware-weight-quantization-for-llm-compression-and-acceleration/README.md)]|MIT, SJTU, NVIDIA etc|2023.06|235|
|OneBit|**OneBit: Towards Extremely Low-bit Large Language Models**|[[pdf](https://arxiv.org/abs/2402.11295)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/quantization/onebit--towards-extremely-low-bit-large-language-models/README.md)]|THU, HIT|2024.02|4|
|OneBit|**The Era of 1-bit LLMs: All Large Language Models are in 1.58 Bits**|[[pdf](https://arxiv.org/abs/2402.17764)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/quantization/the-era-of-1-bit-llms--all-large-language-models-are-in-1.58-bits/README.md)]|Microsoft, UCAS|2024.02|39|

## KV Cache
Last update of citation was on 25th July, 2024.

|Keywords | Title | Paper | Affiliation | Date | Citation|
|:---:|:---:|:---:|:---:|:---:|:---:|
|vLLM, PagedAttention|**Efficient Memory Management for Large Language Model Serving with PagedAttention** [SOSP 2023]|[[pdf](https://arxiv.org/abs/2309.06180)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/kv-cache/efficient-memory-management-for-large-language-model-serving-with-pagedattention/README.md)]|UC Berkeley, Stanford, UC San Diego|2023.09|496|


## Continuous Batching
Last update of citation was on 5th August, 2024.

|Keywords | Title | Paper | Affiliation | Date | Citation|
|:---:|:---:|:---:|:---:|:---:|:---:|
|Cellular Batching|**Low latency rnn inference with cellular batching** [EuroSys 2018]|[[pdf](https://madsys.cs.tsinghua.edu.cn/publication/low-latency-rnn-inference-with-cellular-batching/EUROSYS2018-gao.pdf)]|THU, NYU|2018.04|97|
|ORCA|**Orca: A Distributed Serving System for Transformer-Based Generative Models** [OSDI 2022]|[[pdf](https://www.usenix.org/conference/osdi22/presentation/yu)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/continuous-batching/orca--a-distributed-serving-system-for-transformer-based-generative-models/README.md)]|SNU, FriendliAI|2022.07|195|
|SARATHI|**SARATHI: Efficient LLM Inference by Piggybacking Decodes with Chunked Prefills**|[[pdf](https://arxiv.org/abs/2308.16369)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/continuous-batching/sarathi--efficient-llm-inference-by-piggybacking-decodes-with-chunked-prefills/README.md)]|Microsoft, GIT|2023.08|36|

## HW/SW Co-design

## Framework/System/Architecture

## More
Last update of citation was on 8th August, 2024.

|Keywords | Title | Paper | Affiliation | Date | Citation|
|:---:|:---:|:---:|:---:|:---:|:---:|
|Block Transformer|**Block Transformer: Global-to-Local Language Modeling for Fast Inference**|[[pdf](https://arxiv.org/abs/2406.02657)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/more/block-transformer--global-to-local-language-modeling-for-fast-inference/README.md)]|KAIST, LG, Google|2024.06|2|
|TTT|**Learning to (Learn at Test Time): RNNs with Expressive Hidden States**|[[pdf](https://arxiv.org/abs/2407.04620)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/more/learning-to--learn-at-test-time---rnns-with-expressive-hidden-states/README.md)]|Stanford, UC San Diego, UC Berkeley etc|2024.07|3|
|LazyLLM|**LazyLLM: Dynamic Token Pruning for Efficient Long Context LLM Inference**|[[pdf](https://arxiv.org/abs/2407.14057)] [[intro](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/more/lazyllm--dynamic-token-pruning-for-efficient-long-context-llm-inference/README.md)]|Apple, Meta|2024.07||