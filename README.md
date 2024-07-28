
# Conversational AI with DialoGPT

Welcome to the Conversational AI with DialoGPT project! This project focuses on building a chatbot using the DialoGPT model.

## Introduction

Conversational AI involves creating systems that can engage in dialogue with humans. In this project, we leverage the power of DialoGPT to build a chatbot that can handle various conversational contexts.

## Dataset

For this project, we will use a custom dataset of conversational data. You can create your own conversational data and place them in the `data/conversational_data.csv` file.

## Project Overview

### Prerequisites

- Python 3.6 or higher
- PyTorch
- Hugging Face Transformers
- Datasets
- Flask

### Installation

To set up the project, follow these steps:

```bash
# Clone this repository and navigate to the project directory:
git clone https://github.com/your-username/dialogpt_chatbot.git
cd dialogpt_chatbot

# Install the required packages:
pip install -r requirements.txt

# Ensure your data includes conversational data. Place these files in the data/ directory.
# The data should be in a CSV file with one column: text.

# To fine-tune the DialoGPT model for conversational AI, run the following command:
python scripts/train.py --data_path data/conversational_data.csv

# To evaluate the performance of the fine-tuned model, run:
python scripts/evaluate.py --model_path models/ --data_path data/conversational_data.csv
