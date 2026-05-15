# Introduction to Hugging Face Transformers

This project serves as a comprehensive technical guide for developers and AI enthusiasts looking to master the Hugging Face Transformers ecosystem. It covers the essential workflows for modern Natural Language Processing (NLP), from raw text processing to implementing state-of-the-art deep learning models.

## Project Overview

Hugging Face has revolutionized NLP by providing a standardized interface for using Transformer-based architectures. This repository demonstrates the core components of the library, focusing on practical implementation and architectural understanding.

## Core Concepts Covered

### 1. The AutoClasses Ecosystem

One of the most powerful features of the library is the AutoClass system. We explore how to use generic classes to automatically fetch the correct model architecture and configuration based on the model name, facilitating seamless experimentation with different pre-trained weights.

### 2. Tokenization and Data Preparation

Understanding how machines "read" text is crucial. The project covers:

    Subword tokenization (WordPiece) used by BERT.

    Special tokens such as [CLS] for classification and [SEP] for sequence separation.

    Converting text to PyTorch tensors with proper padding and truncation for model compatibility.

### 3. Masked Language Modeling (MLM)

Implementation of BERT for fill-mask tasks, demonstrating the model's bidirectional understanding of context by predicting hidden words within a sentence.

### 4. Generative AI with GPT-2

An exploration of Causal Language Modeling. We demonstrate how to use GPT-2 for text generation, including advanced decoding techniques like preventing repetition (no_repeat_ngram_size) and controlling output length.

### 5. Multilingual Sentiment Analysis

Implementation of sequence classification using a multilingual BERT model. This section shows how to transform model outputs (logits) into human-interpretable probability scores and star ratings using Softmax and Argmax operations.

## Technical Requirements

To run the provided scripts, you will need:

    Python 3.10+

    Transformers Library

    PyTorch

    Hugging Face Hub API (for programmatic model searching)

## How to Use

    Exploration: Start with the basic tokenization scripts to understand data structures.

    Inference: Run the classification and generation modules to see the pre-trained models in action.

    Customization: Replace the model names with any compatible checkpoint from the Hugging Face Model Hub to test different languages or specialized domains.

## Learning Objectives

By following the code in this repository, you will understand:

    How to bridge the gap between raw text and deep learning tensors.

    The difference between Encoder-only (BERT) and Decoder-only (GPT) architectures.

    How to perform inference efficiently without calculating gradients for production-ready code.
