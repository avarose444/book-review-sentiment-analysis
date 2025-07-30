📚 Book Review Sentiment Analysis
This project performs sentiment analysis on book reviews to classify them as positive or negative using Natural Language Processing (NLP) and Machine Learning (ML) techniques.

🔍 Project Overview
Using the bookReviewsData.csv dataset, this project builds a classification pipeline that:

Cleans and preprocesses text reviews

Transforms the text into numerical features using TF-IDF

Trains and evaluates models using Logistic Regression and Random Forest

Tunes hyperparameters using GridSearchCV

Evaluates models using AUC, Confusion Matrix, Precision, Recall, F1 Score, and ROC Curve

🧠 Machine Learning Pipeline
✅ 1. Data Preparation
Loaded and inspected the dataset

Preprocessed text:

Lowercasing

Stopword removal

TF-IDF vectorization

🤖 2. Models Used
Logistic Regression

Random Forest Classifier

🧪 3. Evaluation Metrics
Accuracy

Precision / Recall / F1 Score

AUC-ROC Score

Confusion Matrix

ROC Curve Plot

🔧 4. Model Optimization
Used GridSearchCV to tune:

C for Logistic Regression

n_estimators for Random Forest

📊 Results Summary
Model	Accuracy	Precision	Recall	F1 Score	AUC
Logistic Regression	0.83	0.83	0.84	0.83	0.91
Random Forest	0.81	0.82	0.81	0.81	0.89

✔️ Final model selected: Logistic Regression – slightly higher AUC and more interpretable.

📁 Dataset
Source: bookReviewsData.csv

Columns:

Review: Free-text review

Positive Review: Boolean label (True/False)

🚀 How to Run
Clone the repo:

bash
Copy
Edit
git clone https://github.com/your-username/book-review-sentiment-analysis.git
Open the Jupyter Notebook:

bash
Copy
Edit
jupyter notebook DefineAndSolveMLProblem.ipynb
Run all cells to reproduce the pipeline and results.

🛠️ Technologies Used
Python

Pandas / NumPy

Scikit-learn

Matplotlib / Seaborn

TF-IDF Vectorizer

GridSearchCV

📌 Key Takeaway
This project demonstrates how a simple NLP pipeline can effectively analyze sentiment in text data, helping companies automate review moderation, improve recommendation systems, and better understand customer feedback.
