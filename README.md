# 📊 Social Media Sentiment Analysis

![Python](https://img.shields.io/badge/Python-3.9-blue)
![ML](https://img.shields.io/badge/Machine%20Learning-Project-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## Overview

This project focuses on analyzing user-generated tweets and comments and classifying them into four sentiment categories:
Positive, Negative, Neutral, and Irrelevant.

The objective is to build a high-accuracy sentiment classification model that can be used for real-time tweet sentiment prediction.

👥 Team Members

This project was developed as a group effort:

Lipika Maji 

Urmi Kanrar 

Samayita Mohanta 

📂 Dataset

Source: Kaggle

Dataset: Twitter Entity Sentiment Analysis
🔗 https://www.kaggle.com/datasets/jp797498e/twitter-entity-sentiment-analysis

Dataset Features:
id → Tweet ID
game → Associated entity/game
response → Sentiment label
comments → Tweet text

🛠️ Technologies Used

Python

Pandas

NumPy

Scikit-learn

Matplotlib

Seaborn

WordCloud

XGBoost

Joblib

⚙️ Project Workflow

🔹 1. Data Cleaning & EDA
Converted text to lowercase

Removed:

URLs,
Punctuation,
Special characters,

Checked:

Missing values,
Duplicate data,

Visualizations:

Tweet length distribution (Boxplot)
Top 20 entities
Sentiment distribution

WordClouds

🔹 2. Feature Engineering

Train-test split
Text converted using TF-IDF Vectorization

🔹 3. Model Building

Models used:


Logistic Regression

Naive Bayes

Decision Tree

Linear SVM

Random Forest

🔹 Ensemble Learning:

XGBoost

Stacking Model


🔹 Validation:
K-Fold Cross Validation used to avoid overfitting

📈 Key Insights

Dataset is imbalanced (Irrelevant class has fewer samples)
Negative tweets show slightly higher variability
Decision Tree showed overfitting (~97% train vs ~72% test accuracy)
TF-IDF high dimensionality affected tree-based models
💾 Model Saving

The final model was saved using Joblib for reuse:

joblib.dump(model, "Stacking_model.joblib")

This allows:

Reloading the model without retraining
Real-time prediction on user input

🚀 How to Run
# Clone repository
git clone https://github.com/your-username/your-repo-name.git

# Open project
cd your-repo-name

# Run notebook
jupyter notebook

🔮 Future Improvements
Improve class balance using SMOTE
Deploy as a web application (Streamlit / Flask)
Use Deep Learning (LSTM / BERT)
Real-time Twitter API integration
🤝 Contribution

This was a collaborative academic project. All team members contributed to data preprocessing, model building, and evaluation.

📄 License

This project is for academic and learning purposes.
