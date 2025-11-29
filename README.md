# Sentiment Analysis on Book Reviews (VADER + Transformers)

This project demonstrates practical sentiment analysis using two approaches:

1. **VADER (Rule-based sentiment analysis)**  
2. **Hugging Face Transformer Models (Pre-trained deep learning models)**

The goal is to compare how classical rule-based NLP and modern transformer-based models interpret sentiment in a small dataset of book reviews.

---

## 📌 Project Summary

- Loads a dataset of 100 book reviews  
- Cleans text (lowercasing + punctuation removal)  
- Applies **VADER** to generate compound scores  
- Converts scores into **negative / neutral / positive** categories  
- Uses a **Transformer pipeline** (`pipeline("sentiment-analysis")`) to classify reviews  
- Visualizes sentiment distribution for both models  

This project gives a clear, practical understanding of sentiment analysis workflows in Python.

---

## 📂 Dataset

`book_reviews_sample.csv`

Columns include:

| Column | Description |
|--------|-------------|
| index | Unique ID |
| reviewText | Original review text |
| rating | Rating given by reviewer |
| reviewText_clean | Processed, cleaned text |

---

## 🧹 Text Preprocessing

- Convert all text to lowercase  
- Remove punctuation using regex  
- Avoid removing stopwords, lemmatization, or stemming because small words (e.g., *not*) affect sentiment

## 📊 Results

- VADER provides nuanced scores and supports negative, neutral, positive.

- Transformers return binary results (POSITIVE or NEGATIVE).

- Visualizations clearly highlight differences in how each model interprets the same text.

## 🛠 Dependencies

- Install required libraries:

pip install pandas numpy nltk transformers vaderSentiment scikit-learn

## ▶️ How to Run

- Place the dataset file in the project directory

- Run the script or the Jupyter Notebook

- View printed outputs and sentiment distribution plots
