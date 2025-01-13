# Sentiment-Analysis

## Overview
This project performs **sentiment analysis** on a dataset of text samples labeled with emotions. The goal is to classify text into emotional categories using machine learning techniques.

---

## Dataset
- **Source**: [Emotions Dataset for NLP](https://www.kaggle.com/datasets/praveengovi/emotions-dataset-for-nlp)
- **Format**: `Text;Emotion`  
- **Emotions**: sadness, joy, love, anger, fear, surprise  

---

## Methodology

### 1. Data Preparation
- Combined the `train` and `validation` datasets into a single DataFrame for consistent preprocessing and model training.

### 2. Text Preprocessing
- **Lowercase Conversion**: Converted all text to lowercase for uniformity.
- **Special Character Removal**: Stripped unwanted characters and symbols.
- **Tokenization**: Split text into individual words.
- **Stopword Removal**: Eliminated common words that do not carry significant meaning.
- **Lemmatization**: Reduced words to their base forms for consistency.

### 3. Feature Engineering
- Transformed text data into numerical vectors using **CountVectorizer**.

### 4. Model Training
- Employed a **Random Forest Classifier**.
- Tuned hyperparameters using **GridSearchCV** for optimal performance.

### 5. Evaluation
- Measured model performance using:
  - **Accuracy**
  - **Precision**
  - **Recall**
  - **F1-score**

---

## Results

### Performance on the Test Set
- **Accuracy**: 96.1%  
- **Precision**: 96.16%  
- **Recall**: 95.33%  
- **F1-score**: 0.96 (weighted average)

---

## Key Insights
1. The model demonstrates **high accuracy** across all emotion categories.
2. **Precision and recall** are well-balanced, indicating good overall performance.
3. The classifier effectively distinguishes between different emotions, showcasing its robustness.
