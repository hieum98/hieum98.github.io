---
layout: page
title: Event Relations and Causality
description: Document-level event relation extraction and event causality identification that capture long-range context.
importance: 4
github: https://github.com/hieum98/DisfusECI
related_publications: true
---

Understanding a document's events means recognizing how they relate, including which events cause which, often across sentences far apart. This work identifies the context that matters for each event pair.

- **Selecting the right context**: choosing optimal context sentences for event-event relation extraction {% cite man2022selecting %} ([code](https://github.com/hieumdt/SCS-EERE)), and identifying causality by generating important context words {% cite man-etal-2022-event %}.
- **Optimal transport and diffusion models**: hierarchical selection of important context with optimal transport {% cite man-etal-2024-hierarchical %} ([code](https://github.com/hieum98/HOTECI)), and context-to-label representation transformation with diffusion models {% cite man2024mastering %} ([code](https://github.com/hieum98/DisfusECI)).
- **Datasets and extraction**: a dataset for event detection in cybersecurity texts {% cite man-etal-2020-introducing %}, multilingual subevent relation extraction {% cite lai-etal-2022-multilingual %}, and contextualized soft prompts for event argument extraction {% cite nguyen-etal-2023-contextualized %}.
