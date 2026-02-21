# 🐦 Twitter Sentiment Analysis

## 📌 Overview

This project builds an end-to-end Natural Language Processing (NLP) pipeline to classify tweets as **positive** or **negative** using supervised machine learning techniques. It demonstrates practical text preprocessing, feature engineering, model training, and evaluation on large-scale social media data.

---

## 📂 Dataset

The dataset used in this project is the **Sentiment140 dataset** from Kaggle:

🔗 https://www.kaggle.com/datasets/kazanova/sentiment140

The dataset contains 1.6 million labeled tweets.
Each record includes:

* **target** – Tweet polarity (`0 = Negative`, `4 = Positive`)
* **id** – Unique tweet identifier
* **date** – Timestamp of the tweet
* **flag** – Query associated with the tweet (`NO_QUERY` if none)
* **user** – Username of the tweet author
* **text** – The content of the tweet

---

## ⚙️ Methodology

### 🔹 Data Preprocessing

* Text cleaning (removing punctuation, URLs, special characters)
* Lowercasing
* Stopword removal
* Tokenization

### 🔹 Feature Engineering

* Text vectorization using CountVectorizer / TF-IDF
* Conversion of tweet text into numerical feature vectors

### 🔹 Model Training

* Supervised machine learning classifier trained on labeled tweet data

---

## 📊 Model Evaluation

### 🔹 Accuracy

* **Training Accuracy:** 79.87%
* **Test Accuracy:** 77.67%

The small gap (~2%) between training and test accuracy indicates good generalization with no significant overfitting.

---

### 🔹 Classification Report (Test Data)

| Class        | Precision | Recall | F1-Score | Support |
| ------------ | --------- | ------ | -------- | ------- |
| 0 (Negative) | 0.79      | 0.76   | 0.77     | 160,000 |
| 1 (Positive) | 0.77      | 0.80   | 0.78     | 160,000 |

* **Overall Accuracy:** 78%
* **Macro Average F1-Score:** 0.78
* **Weighted Average F1-Score:** 0.78

---

### 🔹 Interpretation

* The model achieves balanced performance across both sentiment classes.
* Precision and recall values are consistent, indicating stable classification behavior.
* Similar training and testing accuracy suggests the model is not overfitting.
* Performance is solid for a classical machine learning approach on noisy social media text.

---

## 🚀 Future Improvements

* Hyperparameter tuning
* Use of n-grams and advanced vectorization techniques
* Implementation of deep learning models (LSTM / GRU)
* Transformer-based models (BERT)
* Deployment as an API or web application

---

## 🛠 Tech Stack

* Python
* Pandas & NumPy
* Scikit-learn
* NLP preprocessing techniques
* Jupyter Notebook

---

## 💡 Key Takeaways

* Large-scale text classification implementation
* Practical NLP pipeline development
* Balanced sentiment prediction performance
* Strong baseline model with room for advanced improvements
* This implementation is based on a tutorial from GeeksforGeeks and was developed for practice purposes.

---
