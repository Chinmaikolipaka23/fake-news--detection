# Fake News Detection System

A Machine Learning–based Fake News Detection system that classifies news articles as **Fake** or **Real** using NLP techniques and multiple classification algorithms.

---

##  Overview
This project uses **Natural Language Processing (NLP)** and **Machine Learning models** to detect fake news.  
Text data is converted into numerical features using **TF-IDF Vectorization**, and three different models are trained and evaluated:

- Logistic Regression
- Naive Bayes
- Random Forest

The best-performing model is used to predict whether a given news article is fake or real.

---

##  Features
- Text preprocessing and feature extraction using **TF-IDF**
- Comparison of multiple ML models
- Model evaluation using accuracy, confusion matrix, and classification report
- Predicts fake or real news for **custom user input**

---

## Technologies Used
- **Python**
- **Machine Learning**
- **Natural Language Processing (NLP)**
- **TF-IDF Vectorizer**
- **Logistic Regression**
- **Naive Bayes**
- **Random Forest**
- **Scikit-learn**
- **Pandas, NumPy**
- **Jupyter Notebook**

---

##  Dataset
- Dataset: `train1.csv`
- Columns used:
  - `title`
  - `author`
  - `text`
  - `label` (0 = Real, 1 = Fake)

Missing values are handled and important text columns are combined before training.

---

##  Model Pipeline
1. Load and clean dataset  
2. Combine text fields (`title + author + text`)
3. Split data into training and testing sets  
4. Convert text data to numerical features using **TF-IDF**
5. Train and evaluate:
   - Logistic Regression
   - Naive Bayes
   - Random Forest
6. Compare model accuracies
7. Predict fake or real news for new inputs

---

##  Model Evaluation
Each model is evaluated using:
- Accuracy Score
- Confusion Matrix
- Classification Report (Precision, Recall, F1-score)

Final predictions are made using **Logistic Regression**.

---

##  Example Prediction
```text
Input: "Government secretly planning to control weather through satellites"
Output: Fake News
