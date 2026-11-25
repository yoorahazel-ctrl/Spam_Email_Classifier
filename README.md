# Spam_Email_Classifier
# 📧 End-to-End Spam Email Classifier

A beginner-friendly Natural Language Processing (NLP) and Machine Learning pipeline that classifies text messages into **Ham** (legitimate) or **Spam** using Python and Scikit-Learn.

## 📌 Overview
This project demonstrates the foundational workflow of supervised text classification. It ingests raw text data, normalizes it to reduce vocabulary noise, converts words into numerical vectors, and trains a probabilistic classifier to identify unwanted messages with over **90% accuracy**.

## 🛠️ Tech Stack & Tools
* **Language:** Python 3
* **Environment:** Google Colab / Jupyter Notebook
* **Data Handling:** Pandas
* **Machine Learning & NLP:** Scikit-Learn (`CountVectorizer`, `MultinomialNB`, `train_test_split`)

## ⚙️ Project Workflow
1. **Data Sourcing & Balancing:** Loaded text data from Scikit-Learn's built-in repositories and verified class distribution to ensure a balanced binary dataset (`ham` vs. `spam`).
2. **Text Preprocessing:** Built a custom Python normalization function to convert text to lowercase, strip punctuation, and remove extra whitespace.
3. **Feature Engineering (Vectorization):** Used `CountVectorizer` (Bag-of-Words) to transform cleaned text into a numerical frequency matrix. Fitted strictly on the training set to prevent data leakage.
4. **Model Training:** Split the data (80% training / 20% testing) and trained a **Multinomial Naive Bayes** classifier—chosen for its speed and high performance on word-frequency features.
5. **Evaluation & Live Inference:** Evaluated the model on unseen test data focusing on **Precision** (to minimize false positives) and built an interactive function to classify custom user-input sentences in real time.

## 🚀 How to Run This Project

### Option 1: Run in Google Colab (Recommended)
1. Click the badge below to open the notebook directly in Google Colab:
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](YOUR_COLAB_LINK_HERE)
2. Go to **Runtime > Run all** to execute the pipeline and test custom sentences at the bottom.

### Option 2: Run Locally
1. Clone this repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
   cd YOUR_REPO_NAME

