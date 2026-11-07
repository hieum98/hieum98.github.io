---
layout: page
title: Memory for Retrieval-Augmented Reasoning
description: An explicit working memory that decides which retrieved evidence to keep, update, or discard during multi-hop reasoning.
importance: 1
github: https://github.com/amazon-science/state-aware-rag
related_publications: true
---

Multi-hop retrieval-augmented generation (RAG) has to keep a coherent picture of what it has found as the reasoning chain grows longer. This line of work gives the system an explicit working memory and learns how to manage it.

- **State-Aware RAG** {% cite man-etal-2026-reasoning %}: a trainable working memory (a Qwen3-4B extractor) that filters and updates retrieved evidence for multi-hop reasoning, with the retriever and generator frozen. The extractor is trained with LoRA SFT on about 70K MCTS-synthesized state-action pairs, then with GRPO using a Path-Outcome Dual Reward that also scores every reasoning step. It beats the best memory-augmented and RL-enhanced baselines by 8.6% and 9.3% on average across eight QA benchmarks. [Code](https://github.com/amazon-science/state-aware-rag)
- **Co-E** {% cite man2026coevolvinggraphtextmemory %}: keeps graph and text memory in sync during reasoning without any training. On an 8B open model, it beats comparable training-free baselines on six multi-hop QA benchmarks (+10.3 EM over HopRAG with GPT-4o on MuSiQue). [Code](https://github.com/hieum98/wemg)
