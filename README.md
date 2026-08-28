# Multi-VLM Debate for Multimodal Science Question Answering

This project explores whether debates among multiple vision-language models (VLMs) can improve multimodal reasoning for science question answering. The main idea is to use multiple VLMs, scene-graph representations, and a debate framework to answer complex questions that require both image and text understanding.

## Overview

Multimodal reasoning requires a model to make decisions using information from multiple modalities, such as images and text. Although existing vision-language models have shown strong performance, they often rely heavily on the text modality and may fail to capture spatial relationships in images.

To address this issue, this project investigates a multi-model debate framework. Instead of relying on a single VLM, multiple VLMs generate and challenge responses using scene-graph-based image representations. The goal is to encourage more reliable reasoning and reduce model-specific bias.

## Research Goal

The goal of this project is to study whether using multiple VLMs in a debate setting improves performance on multimodal science question-answering tasks.

Specifically, this project asks:

- Can multiple VLMs improve answer accuracy through debate?
- Can scene graphs help VLMs reason better about objects and spatial relationships?
- How does interaction between different VLMs affect the quality of responses?
- Does multi-model debate outperform single-model VLM reasoning?

## Datasets

This project plans to evaluate the framework on multimodal science question-answering benchmarks, including:

- **ScienceQA**
- **MMBench**

These datasets contain questions that require both visual understanding and textual reasoning.

## Methodology

The project follows these main steps:

1. **Dataset Processing**
   - Load multimodal question-answering datasets.
   - Extract image, question, answer choices, and ground-truth labels.

2. **Scene Graph Extraction**
   - Generate scene-graph representations from images.
   - Use object and relationship information to support visual reasoning.

3. **Multi-VLM Debate**
   - Use multiple vision-language models to generate initial answers.
   - Allow models to compare, critique, and revise their responses.
   - Aggregate final answers after the debate process.

4. **Evaluation**
   - Compare final predictions with ground-truth answers.
   - Use accuracy as the primary evaluation metric.
   - Compare multi-VLM debate performance with single-model VLM baselines.

