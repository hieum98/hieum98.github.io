---
layout: page
title: LLM Embeddings for Multilingual Retrieval
description: Turning large language models into text embedding models that hold up across tasks and languages.
importance: 2
github: https://github.com/nlp-uoregon/ullme
related_publications: true
---

Embedding models built on large language models set the state of the art for dense retrieval, but they are trained mostly on English. This work makes them easier to build and extends them to other languages.

- **ULLME** {% cite man2024ullmeunifiedframeworklarge %}: an open-source framework (1.5B to 8B checkpoints) that unifies contrastive and generation-augmented training. It beats LLM2Vec trained on the same data by 1.2 to 2.0 points on MTEB. [Code](https://github.com/nlp-uoregon/ullme)
- **LUSIFER** {% cite man2025lusiferlanguageuniversalspace %}: adapts an English-centric LLM embedding model to other languages with English-only training, by connecting a multilingual encoder to it through a small set of trainable parameters. It beats E5-Mistral by 3.19 points on average across 14 languages. [Code](https://github.com/hieum98/lusifer)
- **Multilingual data and evaluation**: CulturaX {% cite nguyen-etal-2024-culturax %}, a cleaned multilingual dataset for training LLMs in 167 languages ([dataset](https://huggingface.co/datasets/uonlp/CulturaX)), and an evaluation of ChatGPT on multilingual NLP tasks {% cite lai-etal-2023-chatgpt %}.
