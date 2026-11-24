---
layout: default
title: Research
permalink: /research.html
---

[Home]({{ '/' | relative_url }}) | **Research** | [Projects]({{ '/projects.html' | relative_url }})

# Research

My research focuses on mechanistic interpretability: investigating the computations inside neural networks to better understand how they work. Through undergraduate research at UW–Eau Claire, I have explored both language-model representations and small networks that perform algorithmic tasks.

## Understanding Small Recurrent Neural Networks

*Undergraduate Research Assistant | OSRP | November 2026–present*

I am studying a small recurrent neural network from the Alignment Research Center's AlgZoo collection. The model processes a sequence of ten numbers and predicts the position of the second-largest number, using sixteen hidden neurons.

I examine its weights, hidden states, and output scores to investigate how it performs this task. Using heatmaps and controlled changes to input sequences, I explore how individual neurons respond and how information changes as the model processes a sequence. The goal is to develop a clearer explanation of its internal computation.

**Tools:** Python, PyTorch, Jupyter notebooks, Matplotlib, Seaborn

## Factual Representations During Roleplay

*Undergraduate Research Assistant | OSRP | June–August 2026*

I investigated how language models represent factual information during roleplay and when conversational topics change. I reproduced and extended published experiments using Gemma models and linear probes, which are classifiers trained on internal activations to test what information those activations contain.

I designed a topic-switch experiment to examine whether these representations returned toward their original factual patterns after the conversation changed direction. Across the model sizes tested, probe results indicated this return occurred after an average of one to two conversation turns.

I also built a 1,536-example dataset and ran experiments locally and on a university GPU cluster, using models ranging from 1B to 12B parameters.

**Tools:** Python, PyTorch, Hugging Face Transformers, scikit-learn, SLURM, CUDA, Linux/Bash

[View the research repository](https://github.com/gkrajnik/Mechanistic-Research)
