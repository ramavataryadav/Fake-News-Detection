# Fake-News-Detection

## 1. Introduction

In an era where misinformation spreads rapidly online, detecting fake news is more critical than ever. This project leverages deep learning, specifically Long Short-Term Memory (LSTM) networks, to classify news articles as **real** or **fake** based on their textual content.

## 2. Project Overview

We implement a text classification pipeline that includes:
- Data preprocessing
- Text vectorization using Tokenizer + Embedding Layer
- LSTM model for sequence classification
- Evaluation using standard metrics
- Flask web interface for real-time predictions
Import Libraries
1. Load and Check Data
2. Visualization
3. Data Cleaning
    * Removal of HTML Contents
    * Removal of Punctuation Marks and Special Characters
    * Removal of Stopwords
    * Lemmatization
    * Perform it for all the examples 
4. N-Gram Analysis
    * Unigram Analysis
    * Bigram Analysis
    * Trigram Analysis
5. Modeling
    * Train - Test Split
    * Tokenizing
    * Training LSTM Model
    * Analysis After Training 

## 3. Dataset

We use the "Fake and Real News Dataset" from Kaggle:
- URL: https://www.kaggle.com/clmentbisaillon/fake-and-real-news-dataset

Each sample includes:
- Title
- Text/body
- Label (`REAL` or `FAKE`)

## 4. Data Preprocessing

Steps include:
- Lowercasing
- Removing punctuation and stopwords
- Tokenization
- Sequence padding for consistent input size

## 5. Model Architecture

The model consists of:
- Embedding Layer
- LSTM Layer
- Dense Layers
- Sigmoid Output Layer (binary classification)

## 6. Directory Structure

```
Fake_News_Detection_LSTM/
│
├── Dataset/                # Dataset CSV files
├── Model Building/              # Saved models
└── README.md
```

## 7. How to Run

### Training the Model
```bash
python Fake_News_Detection_with_LSTM.py
```

## 8. Evaluation Metrics

We use the following metrics to evaluate model performance:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

## 9. Technologies Used

- Python
- NumPy / Pandas / Matplotlib
- TensorFlow / Keras
- NLTK / SpaCy
- Flask
- Jupyter Notebook

## 10. Results

| Metric      | Value    |
|-------------|----------|
| Accuracy    | 94.7%    |
| Precision   | 93.2%    |
| Recall      | 95.1%    |
| F1 Score    | 94.1%    |

*(Note: Results may vary depending on data splits and training epochs.)*

## 11. Future Work

- Incorporate BERT and transformer-based models
- Add support for multilingual fake news detection
- Use metadata (author, source, date) for richer context
- Browser plugin for live fact-checking

## 12. Acknowledgements

- Kaggle and dataset contributors
- TensorFlow and Keras community
- Open-source NLP libraries (NLTK, SpaCy)
