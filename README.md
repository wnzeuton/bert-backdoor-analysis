# BERT Backdoor Analysis
Exploring Backdoor Attacks in BERT with Embedding Analysis and Neuron Interpretability.

## Overview

This repository explores a backdoor attack on a BERT-based text classifier using the AG News dataset. A small fraction of "Business" samples is poisoned with a text trigger, causing the model to misclassify them as "World." The notebook includes dataset poisoning, model training, and evaluation, along with PCA and 3D visualizations of embedding shifts. It also demonstrates steering vectors, neuron-level analysis, and partial mitigation of the backdoor.

## Features

- **Dataset Poisoning:** Inject a small fraction of "Business" samples with a text trigger to create backdoor examples.  
- **Model Training & Evaluation:** Train BERT-based classifiers at multiple poison rates and evaluate both clean accuracy and attack success rate (ASR).  
- **Embedding Visualization:** Explore latent space shifts using 2D PCA plots and interactive 3D visualizations of clean vs. poisoned embeddings.  
- **Steering Vector Analysis:** Extract and apply a linear vector that flips embeddings to the target class without using the text trigger.  
- **Neuron-Level Interpretability:** Identify key dimensions that carry the backdoor logic and analyze associated vocabulary.  
- **Partial Mitigation Experiments:** Test the effect of muting critical neurons on attack success and clean accuracy.  
