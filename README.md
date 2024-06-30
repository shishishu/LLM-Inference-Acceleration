# LLM-Inference-Acceleration

## Table of Contents

 - [About This Project](#about-this-project)
 - [Listing of Papers by Topics](#listing-of-papers-by-topics)
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
- **Paper Overview**: core idea/image with useful extensions are included for quick start.
- Citation: data for the papers is sourced from Google Scholar.

## Attention Mechanism
Last update of cititation was on 29th June, 2024.

Upcoming topics include: FlashDecoding

|Keywords | Title | Affiliation | Date | Cititaion|
|:---:|:---:|:---:|:---:|:---:|
|MQA|[Fast Transformer Decoding: One Write-Head is All You Need](https://arxiv.org/abs/1911.02150v1)|Google|2019.11|176|
|GQA|[EMNLP 2023] [GQA: Training Generalized Multi-Query Transformer Models from Multi-Head Checkpoints](https://arxiv.org/abs/2305.13245) [[Paper Overview](https://github.com/shishishu/LLM-Inference-Acceleration/blob/main/attention-mechanism/gqa--training-generalized-multi-query-transformer-models-from-multi-head-checkpoints/README.md)]|Google|2023.05|174|
|ALiBi|[ICLR 2022] [Train Short, Test Long: Attention with Linear Biases Enables Input Length Extrapolation](https://arxiv.org/abs/2108.12409)|UW, Facebook, Allen Institute|2021.08|416|
|RoPE|[Neurocomputing 2024] [RoFormer: Enhanced Transformer with Rotary Position Embedding](https://arxiv.org/abs/2104.09864)|Zhuiyi Technology|2021.04|937|
|CoPE|[Contextual Position Encoding: Learning to Count What's Important](https://arxiv.org/abs/2405.18719)|Meta|2024.05|2|
|FlashAttention|[NeurIPS 2022] [FlashAttention: Fast and Memory-Efficient Exact Attention with IO-Awareness](https://arxiv.org/abs/2205.14135)|Stanford, University at Buffalo|2022.05|915|
|FlashAttention2|[FlashAttention-2: Faster Attention with Better Parallelism and Work Partitioning](https://arxiv.org/abs/2307.08691)|Princeton, Stanford|2023.07|281|
|Longformer|[Longformer: The Long-Document Transformer](https://arxiv.org/abs/2004.05150)|Allen Institute|2020.04|3605|
|Mistral|[Mistral 7B](https://arxiv.org/abs/2310.06825)|Mistral|2023.10|313|
|StreamingLLM, Attention Sinks|[ICLR 2024] [Efficient Streaming Language Models with Attention Sinks](https://arxiv.org/abs/2309.17453)|MIT, Meta, CMU etc|2023.09|146|
|LoRA|[ICLR 2022] [LoRA: Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/2106.09685)|Microsoft|2021.06|4818|
|LISA|[LISA: Layerwise Importance Sampling for Memory-Efficient Large Language Model Fine-Tuning](https://arxiv.org/abs/2403.17919)|HKUST, UIUC|2024.03|2|

## Quantization

## KV Cache

## Continuous Batching

## HW/SW Co-design

## Framework/System/Architecture

## More
