---
layout: page
title: Robust Authorship Representations
description: Style representations for authorship attribution and machine-generated text detection that hold up across genres, topics, and languages (IARPA HIATUS).
importance: 3
github: https://github.com/hieum98/avae
related_publications: true
---

As part of the IARPA HIATUS program, I developed authorship attribution and machine-generated text detection methods that stay robust when genre, topic, or language shifts. RTX BBN Technologies, the team lead, selected my style embedding model for the team's submission to the program's evaluations.

- **Counterfactual augmentation** {% cite man2024counterfactual %}: learns authorship representations that are robust to topic and genre shifts. Released as [ERLAS](https://huggingface.co/Hieuman/erlas) on Hugging Face (3,900+ downloads). [Code](https://github.com/ManHieu/ERLAS)
- **EAVAE** {% cite man-etal-2026-explainable %}: a variational autoencoder with separate style and content encoders, plus a discriminator that explains its decisions in natural language. State of the art on Amazon Reviews, PAN21, and HRS. [Code](https://github.com/hieum98/avae)
- **Team systems**: the ALERT system for cross-domain machine-generated text detection {% cite kandula-etal-2025-bbn %} and a combination of neural and large-margin contrastive criteria for authorship attribution {% cite kandula2024improved %}.
