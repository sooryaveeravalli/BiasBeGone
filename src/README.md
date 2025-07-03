# BiasBeGone

**Locating and Mitigating Bias in LLMs via Causal Tracing and Null-Space Model Editing**

For more details, please refer to our [project proposal](https://www.overleaf.com/project/67cb26425cd7603f3dadd2ea) on Overleaf.

## Overview

Large Language Models (LLMs) have shown impressive capabilities in natural language understanding and generation. However, they are prone to learning and reinforcing social biases, which can lead to unfair, discriminatory, or harmful outputs. Traditional bias mitigation techniques, such as fine-tuning and prompt engineering, often require extensive resources, increase computational costs, or risk degrading the model's overall performance. 

To address this, our project proposes a novel Bias Mitigation Algorithm using Model Editing that efficiently locates and mitigates bias in LLMs through targeted interventions. Our approach combines causal tracing techniques with null-space projection methods to identify and modify biased knowledge representations while preserving model accuracy on benign queries.

## Problem Statement

Bias in LLMs often arises from pre-existing patterns in training data, resulting in skewed associations that reinforce stereotypes or propagate social inequalities. Traditional mitigation strategies like fine-tuning or prompt engineering either demand significant computational resources or are vulnerable to adversarial manipulation. Moreover, mitigating bias often risks distorting useful, unbiased knowledge, compromising the model's effectiveness.

Our project addresses this challenge by:
- **Implementing causal tracing** to precisely locate layers that encode biased associations.
- **Applying null-space projection** to modify these biased components while preserving the model's preserved knowledge and reasoning capabilities.

This combined approach aims to deliver a scalable, efficient, and robust method for bias mitigation that avoids the pitfalls of traditional techniques.

## Baselines

To evaluate the effectiveness of our proposed approach, we will compare it against the following baseline methods:
- **Parameter-Efficient Fine-Tuning (e.g., LoRA, Adapter-Tuning):** Methods that modify a small subset of parameters to reduce model bias without extensive retraining.
- **MEMIT (Mass-Editing Memory in Transformers):** A method designed for efficiently editing LLM knowledge by modifying model weights to encode new facts or mitigate biases with minimal side effects.
- **DAMA (Debiasing Algorithm through Model Adaptations):** A state-of-the-art method that employs causal tracing and orthogonal projection to mitigate biased knowledge representations.
