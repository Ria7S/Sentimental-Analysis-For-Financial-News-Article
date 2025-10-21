# 📰 Sentiment Analysis of Financial News Using NLTK & SpaCy

Predict and analyze sentiment in financial news articles using Natural Language Processing (NLP).
This project combines **data cleaning, preprocessing, and machine learning models** to classify financial news headlines and descriptions as **Positive, Negative, or Neutral**.

---

## 📊 Overview

Financial markets are heavily influenced by news sentiment.
This project aims to build an **AI-driven sentiment analysis system** that interprets the tone of financial news and helps in understanding market sentiment.

Using datasets from **CNBC** and **Reuters**, the project performs:

* Text preprocessing with **NLTK & SpaCy**
* Sentiment scoring using **VADER**
* Model building using **Linear SVM, Logistic Regression, and Naive Bayes**
* Real-time prediction on live scraped articles from the web

---

## 🧠 Key Features

* **Data Cleaning & Preprocessing:** Handling missing values, duplicates, tokenization, stopword removal, stemming, and lemmatization.
* **Sentiment Classification:** Labeling news as *Positive*, *Negative*, or *Neutral* using NLTK’s VADER sentiment analyzer.
* **Model Comparison:** Evaluating models such as:

  * Linear Support Vector Machine (SVM)
  * Logistic Regression
  * Multinomial & Bernoulli Naive Bayes
* **Visualization:** Count plots, pie charts, confusion matrices, and ROC curves for performance insights.
* **Real-time Prediction:** Sentiment detection for live financial news scraped using **BeautifulSoup**.

---

## 📁 Dataset

**Source:** [Kaggle - Financial News Headlines](https://www.kaggle.com/datasets/notlucasp/financial-news-headlines)

The dataset contains:

* **CNBC Headlines:** ~3,000 articles
* **Reuters Headlines:** ~32,000 articles

Each includes:

```
time | headline | description
```

---

## ⚙️ Tech Stack

* **Programming Language:** Python
* **Libraries Used:**

  * `NLTK`, `SpaCy`, `Pandas`, `NumPy`
  * `Scikit-learn`, `Matplotlib`, `Seaborn`
  * `BeautifulSoup`, `Requests`
* **Models Implemented:**

  * LinearSVC – *Best model with ~83.8% accuracy*
  * Logistic Regression
  * Multinomial Naive Bayes
  * Bernoulli Naive Bayes

---

## 📈 Model Performance

| Model                   | Accuracy  | Highlights                          |
| ----------------------- | --------- | ----------------------------------- |
| **Linear SVM**          | **83.8%** | Best performer                      |
| Logistic Regression     | 80.7%     | Balanced performance                |
| Multinomial Naive Bayes | 70.7%     | Fast but less accurate              |
| Bernoulli Naive Bayes   | 71.8%     | Works well for binary text features |

**Distribution of Sentiments:**

* Positive: 48.4%
* Negative: 39.8%
* Neutral: 11.3%

---

## 🌐 Real-time Sentiment Example

| Headline                                                           | Predicted Sentiment |
| ------------------------------------------------------------------ | ------------------- |
| “Rape survivor sustains fatal injuries in Kolkata”                 | Negative            |
| “We’ll pay more for non-Covid companies if vaccine trial succeeds” | Positive            |

---

## 📚 Learnings

* Text preprocessing significantly affects sentiment accuracy.
* Combining **headlines + descriptions** provides more robust sentiment signals.
* Real-time web scraping integrated with NLP offers dynamic market analysis capabilities.
