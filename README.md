# AI Generated Text Detection using LORA based fine tuning of LLM Models

## Overview

This project addresses SemEval 2024 Task 8 Subtask A, which involves binary classification of text as either human-written or machine-generated. It leverages transformer-based models—RoBERTa, BART, and GPT-2—and applies parameter-efficient fine-tuning with LoRA to improve classification accuracy and computational efficiency. The system is tested on both familiar and unfamiliar domains using the official SemEval dataset and demonstrates strong generalization across varying text sources and styles.

Notably, RoBERTa fine-tuned with LoRA achieved an F1-score of 0.96 on AI-generated content in the familiar domain, while BART with LoRA performed best in the unfamiliar domain with an F1-score of 0.88, demonstrating strong generalization and adaptability across varying contexts.

[![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)


## Block Diagram

<p align="center">
  <img src="https://i.postimg.cc/bJv5x0tK/x.png" alt="App Screenshot" width="800">
</p>  


## Features

- Binary classification of text (Human vs AI-generated)
- Zero-shot evaluation using RoBERTa, BART, GPT-2, and GPT-4o
- Parameter-efficient fine-tuning using LoRA
- Performance analysis across familiar and unfamiliar domains
- Balanced training using undersampling and structured preprocessing
- Domain generalization evaluation on OUTFOX dataset and GPT-4 generated content
- Results for the models using Adam Optimizer:
  <p align="center">
    <img src="https://i.postimg.cc/9Qr4PtFZ/x2.png" alt="App Screenshot" width="400">
  </p>  
- Results for the models using LoRA:
  <p align="center">
    <img src="https://i.postimg.cc/y6jWwrD0/x3.png" alt="App Screenshot" width="400">
  </p>  

## Dataset

The dataset used for this project is the official SemEval 2024 Task 8 Subtask A Monolingual dataset: https://drive.google.com/drive/folders/1CAbb3DjrOPBNm0ozVBfhvrEh9P9rAppc

## Tech Stack

- **Language**: Python 3.9+
- **Frameworks & Libraries**:
  - PyTorch
  - Hugging Face Transformers
  - PEFT (Parameter-Efficient Fine-Tuning)
  - Datasets (Hugging Face)
  - scikit-learn
  - Accelerate
- **Platform**: Google Colab Pro (with T4, L4, and A100 GPUs)
- **Hardware Requirements**:
  - Minimum 16 GB RAM
  - 5 GB disk space
  - At least 16 GB GPU memory for LoRA-based fine-tuning

## Running Tests

The models can be tested using historical Bitcoin price data to verify prediction accuracy.
