# 📚 Book Review Sentiment Analysis

This project performs **sentiment analysis** on book reviews to classify them as **positive** or **negative** using **Natural Language Processing (NLP)** and **Machine Learning (ML)** techniques.

---

## 🔍 Project Overview

Using the `bookReviewsData.csv` dataset, this project builds a classification pipeline that:
- Cleans and preprocesses text reviews
- Transforms the text into numerical features using **TF-IDF**
- Trains and evaluates models using **Logistic Regression** and **Random Forest**
- Tunes hyperparameters using **GridSearchCV**
- Evaluates models using:
  - AUC-ROC Score
  - Confusion Matrix
  - Precision / Recall / F1 Score
  - ROC Curve Visualization

---

## 🧠 Machine Learning Pipeline

### ✅ 1. Data Preparation
- Dataset: `bookReviewsData.csv`
- Target: `Positive Review` (binary classification: True/False)
- Preprocessing:
  - Convert text to lowercase
  - Remove punctuation and stopwords
  - Vectorize using **TF-IDF** with `ngram_range=(1, 2)` and `max_features=5000`
  - Split into training and test sets (80/20)

### 🤖 2. Models Used
- **Logistic Regression** with hyperparameter tuning (`C`) via GridSearchCV
- **Random Forest** with 100 estimators and `entropy` criterion

### 🧪 3. Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1 Score
- AUC-ROC Score
- Confusion Matrix
- ROC Curve

### 🔧 4. Model Optimization
- Logistic Regression:
  - Tuned regularization strength `C` using GridSearchCV
  - Best `C`: **2.23**
- Random Forest:
  - Used 100 estimators
  - No further tuning (for comparison only)

---

## 📊 Results Summary

| Model                | Accuracy | Precision | Recall | F1 Score | AUC   |
|---------------------|----------|-----------|--------|----------|-------|
| Logistic Regression | 0.83     | 0.83      | 0.84   | 0.83     | 0.91  |
| Random Forest       | 0.81     | 0.82      | 0.81   | 0.81     | 0.89  |

✅ **Selected Model:** **Logistic Regression**  
✔ Slightly higher AUC  
✔ Easier to interpret  
✔ More stable on TF-IDF data

---

## 📁 Dataset Details

- **File**: `bookReviewsData.csv`
- **Columns**:
  - `Review`: Text of the book review
  - `Positive Review`: Label (`True` for positive, `False` for negative)
- **Class Distribution**: Balanced (~50/50)

---

## 📈 Visualizations

- **Word Cloud** of most common terms
- **ROC Curve** to visualize classifier performance
- **Confusion Matrix** to show classification results

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/book-review-sentiment-analysis.git
