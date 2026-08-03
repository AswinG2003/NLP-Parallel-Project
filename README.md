# NLP-Based Twitter Sentiment Analysis

## 📌 Project Overview

This project focuses on **Twitter sentiment analysis using Natural Language Processing (NLP), Classical Machine Learning, and Deep Learning techniques**.

The objective is to classify tweets into four sentiment categories:

* **Positive**
* **Negative**
* **Neutral**
* **Irrelevant**

The project compares the performance of classical machine learning models using **TF-IDF features** with a **Deep Learning model using Word2Vec document embeddings**. Multiple evaluation metrics, including Accuracy, Precision, Recall, F1-Score, ROC-AUC, and PR-AUC, are used for comprehensive model comparison.

---

## 📊 Dataset

The project uses the **Twitter Entity Sentiment Analysis** dataset from Kaggle.

**Dataset:** Twitter Entity Sentiment Analysis
**Source:** Kaggle

**Dataset Link:**
https://www.kaggle.com/datasets/jp797498e/twitter-entity-sentiment-analysis
              |
---

## 🎯 Objective

The main objectives of this project are:

1. Perform exploratory data analysis on Twitter data.
2. Clean and preprocess tweet text.
3. Convert textual data into numerical representations.
4. Train classical machine learning models.
5. Build a Deep Learning sentiment classification model.
6. Evaluate all models using multiple performance metrics.
7. Compare classical ML and Deep Learning approaches.
8. Identify the best-performing model based on evaluation results.

---
## Project workflow

### 🧹 Data Preprocessing

### 1. Missing Value Handling

### 2. Duplicate Removal

### 3. URL Removal

### 4. Number Removal

### 5. Text Cleaning

---

## 🧠 Feature Extraction

Two different text representation approaches are used.

### TF-IDF

**TF-IDF (Term Frequency–Inverse Document Frequency)** is used to convert tweets into numerical feature vectors for the classical machine learning models.

TF-IDF helps represent the importance of words within individual tweets while reducing the influence of very common words.

### Word2Vec

**Word2Vec** is used to create word embeddings for the Deep Learning model.

The project creates **100-dimensional Word2Vec document embeddings** and uses these representations as input to the neural network.

---

## 🤖 Machine Learning Models

### 1. Logistic Regression

Logistic Regression is used as one of the baseline classical machine learning models.

The model uses **TF-IDF features** to classify tweets into the four sentiment categories.

### 2. Linear SVM

A **Linear Support Vector Machine (LinearSVC)** is trained using TF-IDF features.

The model achieved an accuracy of approximately **70.03%** in the evaluated test set.

### 3. Deep Learning

A feed-forward Deep Learning neural network is developed using **Word2Vec document embeddings**.

The model includes:

* Input layer
* Dense hidden layers
* ReLU activation
* Dropout regularization
* Early stopping
* Learning-rate reduction

---

## 📈 Model Evaluation

The models are evaluated using several classification metrics:

### Accuracy

Measures the overall percentage of correctly classified tweets.

### Precision

Measures how many of the tweets predicted as a particular sentiment actually belong to that sentiment.

### Recall

Measures how many tweets belonging to a sentiment class are correctly identified.

### F1-Score

Provides a balance between Precision and Recall.

### ROC-AUC

ROC curves and AUC are used to evaluate the classification performance across sentiment classes.

### Precision-Recall AUC

Precision-Recall curves and PR-AUC provide an additional evaluation of model performance.

The project compares ROC-AUC and PR-AUC along with the standard classification metrics.

---

## 📊 Model Comparison

The following models are compared:

| Model               | Feature Representation |
| ------------------- | ---------------------- |
| Logistic Regression | TF-IDF                 |
| Linear SVM          | TF-IDF                 |
| Deep Learning       | Word2Vec               |

The models are compared using:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC
* PR-AUC

The final comparison table is sorted according to **weighted F1-Score** to identify the best-performing model.

---

## 📉 Visualizations

The project includes several visualizations for analyzing model performance:

* Confusion Matrix
* ROC Curve
* Precision-Recall Curve
* Model Performance Comparison
* Classification Reports

The ROC and Precision-Recall curves are generated for Logistic Regression, Linear SVM, and Deep Learning models.

---

## 🏆 Results

The evaluated models demonstrate different performance levels.

The **Linear SVM** achieved approximately **70.03% accuracy** and performed better than Logistic Regression among the classical machine learning models.

The final model comparison considers weighted F1-Score along with Accuracy, Precision, Recall, ROC-AUC, and PR-AUC to determine the overall best model.

---

## 🔍 Conclusion

This project demonstrates how NLP techniques can be combined with both classical machine learning and Deep Learning for Twitter sentiment classification.

Logistic Regression and Linear SVM use **TF-IDF features**, while the Deep Learning model uses **100-dimensional Word2Vec document embeddings**.

The Deep Learning architecture uses dense layers, ReLU activation, dropout regularization, early stopping, and learning-rate reduction. Model performance is evaluated beyond simple accuracy using ROC-AUC and Precision-Recall AUC.

The final comparison helps identify the model with the highest weighted F1-Score and provides a broader understanding of the strengths of each approach.

---

## 🛠️ Technologies Used

### Programming Language

* Python

### NLP

* NLTK
* Word2Vec
* TF-IDF

### Machine Learning

* Scikit-learn
* Logistic Regression
* Linear SVM

### Deep Learning

* TensorFlow
* Keras

### Data Processing

* Pandas
* NumPy

### Visualization

* Matplotlib
* Seaborn
* WordCloud

### Development Environment

* Google Colab
* GitHub

---

## 📦 Libraries Used

```text
pandas
numpy
matplotlib
seaborn
nltk
scikit-learn
gensim
tensorflow
```

---

## 👥 Team Project

This project was developed as a collaborative NLP and Machine Learning project.

### Contributions

* Data Loading & Exploratory Data Analysis          -- Aswin G
* Data Cleaning & NLP Preprocessing                 -- Aswin G
* Classical Machine Learning                        -- Aswin G
* Deep Learning                                     -- Midhula M S
* Model Evaluation                                  -- Midhula M S
* ROC & Precision-Recall Analysis                   -- Midhula M S
* Model Comparison                                  -- Midhula M S
* Conclusion                                        -- Midhula M S

---

## 📚 Dataset Reference

**Twitter Entity Sentiment Analysis Dataset – Kaggle**

https://www.kaggle.com/datasets/jp797498e/twitter-entity-sentiment-analysis

---

## ⭐ Key Highlights

* Twitter sentiment classification
* NLP preprocessing
* TF-IDF feature extraction
* Word2Vec embeddings
* Logistic Regression
* Linear SVM
* Deep Learning
* Confusion Matrix
* ROC-AUC analysis
* Precision-Recall AUC analysis
* Comparative model evaluation
* End-to-end NLP pipeline

