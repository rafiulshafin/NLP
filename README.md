# Title: Sentiment Analysis using BERT and ELECTRA


This project implements Sentiment Analysis on Social Media Text Data using two state-of-the-art transformer models: BERT (Bidirectional Encoder Representations from Transformers) and ELECTRA (Efficiently Learning an Encoder that Classifies Token Replacements Accurately).

The goal of the project is to fine-tune these pre-trained models on labeled sentiment datasets and evaluate their performance in text classification tasks.

# Datasets
1.Social Media Sentiment Analysis Dataset 1 = https://www.kaggle.com/datasets/kashishparmar02/social-media-sentiments-analysis-dataset


2.Social Media Sentiment Analysis Dataset 2 = https://www.kaggle.com/datasets/abdullah0a/social-media-sentiment-analysis-dataset

# Models Implemented
1. BERT
   
a.Pre-trained Model: bert-base-uncased

b.Tokenization: WordPiece using BertTokenizer

c.Fine-tuning: Classification head on [CLS] token

d.Loss: Cross-Entropy

e.Optimizer: AdamW with scheduler

f.Epochs: 5

g.Batch Size: 16


2. ELECTRA
   
a.Pre-trained Model: google/electra-small-discriminator

b.Tokenization: Subword tokenization using ElectraTokenizer

c.Fine-tuning: Classification layer on discriminator output

d.Loss: Cross-Entropy

e.Optimizer: AdamW with scheduler

f.Epochs: 5

g.Batch Size: 16

# Results:
| Model       | Dataset 1 Accuracy | Dataset 1 F1-Score | Dataset 2 Accuracy | Dataset 2 F1-Score |
| ----------- | ------------------ | ------------------ | ------------------ | ------------------ |
| **BERT**    | 97.85%             | 0.9787             | 34.00%             | 0.3223             |
| **ELECTRA** | **100.00%**        | **1.0000**         | **51.01%**         | **0.3446**         |

# Technologies Used
1.Python

2.PyTorch

3.Hugging Face Transformers

4.Scikit-learn

5.Pandas, NumPy
