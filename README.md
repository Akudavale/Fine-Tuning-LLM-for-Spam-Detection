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
- [Acknowledgements](#Acknowledgements)

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

## Dataset
Almeida, T. & Hidalgo, J. (2011). SMS Spam Collection [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5CC84.

## Model Configuration
The GPT-2 model is configured with the following settings:

1. **Vocabulary size**: 50257
2. **Context length**: 1024
3. **Embedding dimension**: 768
4. **Number of attention heads**: 12
5. **Number of layers**: 12
6. **Dropout rate**: 0.1
7. **Query-key-value bias**: False

## Training
The notebook includes code for loading the dataset, preprocessing the data, and fine-tuning the GPT-2 model on the spam classification task. The training process involves:

1. Loading the pre-trained GPT-2 model.
2. Preparing the dataset by tokenizing and encoding text data.
3. Fine-tuning the model on the balanced dataset.

## Inference
The notebook demonstrates how to generate text samples using the fine-tuned model. The following functions are provided for inference:
1. **generate_text_simple**: Generates text by predicting the next token based on the context.
2. **generate**: Generates text with additional options for top-k sampling and temperature scaling.

## Acknowledgements 

This project would not have been possible without the following resources:
- **GPT-2 Model**: I used the GPT-2 model architecture provided by OpenAI. You can learn more about GPT-2 and access the models at [OpenAI's GPT-2 page](https://openai.com/research/gpt-2).
- **YouTube Tutorials**: The concepts and implementation strategies for this project were inspired by tutorials from the [Vizuara](https://www.youtube.com/@vizuara).

