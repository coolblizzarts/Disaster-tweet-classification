# Disaster Tweet Classification

This project was developed as part of **EE599 - Machine Learning**.  
The goal is to build a classifier that predicts whether a given tweet is about a real disaster or not.

## 📌 Project Overview
- Dataset: 10,000 hand-labeled tweets with fields:
  - `id`, `keyword`, `location`, `text`, `target`
- Task: Binary classification (`target=1` → disaster, `target=0` → not disaster)
- Models: Naive Bayes, Logistic Regression, and Random Forest were tested
- Evaluation Metrics: Accuracy and F1-score

## 🛠️ Tech Stack
- Python 3.x
- Pandas, NumPy for preprocessing
- Scikit-learn for ML models
- NLTK / SpaCy for text preprocessing
- Jupyter Notebook for experimentation

## 🚀 Results
- Naive Bayes baseline achieved **~78% accuracy**
- Logistic Regression with TF-IDF improved performance
- Random Forest with tuned hyperparameters gave the best results
- LIME analysis provided **human-understandable explanations** of why a model classified a tweet as disaster or not

## 🔍 Interpretability with LIME
To ensure transparency and trust in the models, **LIME** was applied:
- LIME explains predictions by perturbing input text and observing model behavior.
- It highlights **important words/phrases** that contributed to a tweet being classified as a disaster.
- Example: For the tweet *"Forest fire near Los Angeles, thousands evacuated"*, LIME highlighted *"fire"* and *"evacuated"* as key features influencing a *disaster* prediction.
- This step demonstrates that the model aligns with human intuition, increasing reliability in real-world use.

## 📂 Files
- `EE599 Project_Disaster tweet classification.ipynb`: Main notebook with preprocessing, training, and evaluation.
- `Dataset/`: Train, test, and sample submission files.
- `requirements.txt`: Dependencies.

## 🧑‍💻 How to Run
1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/disaster-tweet-classification.git
   cd disaster-tweet-classification
