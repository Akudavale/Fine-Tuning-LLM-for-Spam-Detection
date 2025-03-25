# Fine-Tuning LLM for Spam Detection

This repository contains code for fine-tuning a language model (LLM) for spam detection using the GPT-2 model architecture. The notebook demonstrates downloading a pre-trained GPT-2 model, fine-tuning it on a spam classification dataset, and generating text samples.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Dataset](#dataset)
- [Model Configuration](#model-configuration)
- [Training](#training)
- [Inference](#inference)
- [License](#license)

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/Akudavale/Fine-Tuning-LLM-for-Spam-Detection.git
   cd Fine-Tuning-LLM-for-Spam-Detection
2. Create a virtual environment and activate it:
   python -m venv env
source env/bin/activate  # On Windows use `env\Scripts\activate`
3. Install the required packages:
  pip install -r requirements.txt

## Usage
jupyter notebook Fine-Tuning LLM for spam classification model.ipynb

## Project Structure
Fine-Tuning LLM for spam classification model.ipynb: Jupyter notebook containing the code for fine-tuning the GPT-2 model and performing spam classification.
requirements.txt: List of required Python packages.

## Model Configuration
The GPT-2 model is configured with the following settings:

Vocabulary size: 50257
Context length: 1024
Embedding dimension: 768
Number of attention heads: 12
Number of layers: 12
Dropout rate: 0.1
Query-key-value bias: False

## Training
The notebook includes code for loading the dataset, preprocessing the data, and fine-tuning the GPT-2 model on the spam classification task. The training process involves:

1. Loading the pre-trained GPT-2 model.
2. Preparing the dataset by tokenizing and encoding text data.
3. Fine-tuning the model on the balanced dataset.

## Inference
The notebook demonstrates how to generate text samples using the fine-tuned model. The following functions are provided for inference:
1. **generate_text_simple**: Generates text by predicting the next token based on the context.
2. **generate**: Generates text with additional options for top-k sampling and temperature scaling.
