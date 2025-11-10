<h1 align="center">🎬 Movie Review Sentiment Analysis using NLTK</h1>

<p align="center">
  <em>A Natural Language Processing (NLP) project that classifies movie reviews as <b>Positive</b> or <b>Negative</b> using the NLTK library and Naive Bayes classifier.</em>
</p>

---

## 📘 Project Overview
This project demonstrates how to perform **Sentiment Analysis** using the **Natural Language Toolkit (NLTK)**.  
It utilizes the built-in `movie_reviews` dataset, which contains pre-labeled movie reviews categorized as *positive* or *negative*.  

The goal is to clean and preprocess textual data, extract linguistic features, and train a machine learning model that can automatically predict sentiment from text.

---

## 🧠 Problem Statement
Given a movie review, the model predicts whether the sentiment expressed in the text is **positive** or **negative**.  
This helps automate the understanding of audience emotions and opinions towards movies, products, or any text-based data.

---

## 🧩 Dataset
- **Source:** NLTK’s `movie_reviews` corpus  
- **Number of Reviews:** 2000 total  
  - 1000 Positive Reviews  
  - 1000 Negative Reviews  

Each review is stored as a list of words, and each is labeled with a sentiment category.

---

## 🧹 Data Preprocessing Workflow

1. **Load Dataset**
   - Imported `movie_reviews` from `nltk.corpus`.
   - Combined words and categories into a `documents` list of tuples → `(words, category)`.

2. **Shuffle Data**
   - Randomized document order to avoid bias during training.

3. **Text Cleaning**
   - Removed punctuation and stopwords.
   - Applied **lemmatization** using `WordNetLemmatizer`.
   - Used **Part-of-Speech (POS)** tagging to ensure accurate lemmatization.

4. **Feature Extraction**
   - Extracted the most frequent words to create a vocabulary.
   - Converted text into a **bag-of-words** representation for model input.

---

## ⚙️ Model Building

| Step | Description |
|:----:|:-------------|
| **Algorithm** | Naive Bayes Classifier (from NLTK) |
| **Feature Representation** | Bag of Words |
| **Training Data** | 80% of the dataset |
| **Testing Data** | 20% of the dataset |
| **Evaluation Metric** | Accuracy |

### 🧱 Model Pipeline
Text → Tokenization → Stopword Removal → Lemmatization → POS Tagging → Bag-of-Words → Naive Bayes Classifier


---

## 📈 Results

| Metric | Value |
|:-------:|:------:|
| Accuracy | ~85–90% |
| Dataset | NLTK Movie Reviews |
| Model | Naive Bayes |
| Type | Binary Classification |



---

## 🛠️ Tech Stack

| Category | Tools / Libraries |
|:----------|:-----------------|
| Language | Python |
| NLP Toolkit | NLTK |
| Data Processing | random, string |
| Feature Engineering | POS Tagging, Lemmatization |
| Classifier | Naive Bayes |
| Environment | Jupyter Notebook |

---



