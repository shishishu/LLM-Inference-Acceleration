# LoRA: Low-Rank Adaptation of Large Language Models

## Core Idea
Conclusions:
- LoRA can reduce the number of trainable parameters by 10,000 times and the GPU memory requirement by 3 times
- no additional inference latency (unlike adapters)
  - could switch to different downstream work: W - BA + B'A'
- apply LoRA to Wq and Wv in most experiments

[kimi] LoRA中的低秩思想是基于对过参数化模型内在维度的理解，以及在深度学习中应用低秩矩阵分解的先前研究。这些理论和实证研究为LoRA提供了支持，表明通过低秩更新可以有效地调整大型预训练模型以适应新任务，而无需对所有参数进行昂贵的全参数微调。

## Core Image
![Figure 1](fig.1.JPG)

## Useful Extensions