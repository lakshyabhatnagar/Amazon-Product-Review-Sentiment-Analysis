# 🛍️ Amazon Reviews Sentiment Analysis

This project performs sentiment analysis on Amazon product reviews using NLP techniques such as tokenization, lemmatization, POS tagging, and Word2Vec embedding. The objective is to classify product reviews based on their associated ratings, using machine learning models.

---

## 📁 Dataset

**File:** `amazon_reviews.csv`  
**Columns:**
- `reviewText`: The text content of the Amazon product review.
- `rating`: An integer score (typically 1 to 5) representing the sentiment of the review.

---

## 🚀 Project Workflow

### 1. Data Preprocessing
- Lowercasing, punctuation removal using regex
- Tokenization with `nltk.word_tokenize`
- POS tagging with `nltk.pos_tag`
- Lemmatization using WordNet Lemmatizer with POS mapping
- Stopword removal

### 2. Word2Vec Embedding
- Trained a Gensim `Word2Vec` model on the entire corpus
- Each sentence is converted into a single fixed-size vector by averaging the word vectors

### 3. Train-Test Split
- Data is split into training and test sets (e.g., 80-20 split)
- Features: Word2Vec-based sentence vectors
- Labels: Review ratings

### 4. Classification
- You can use any ML model (e.g., Logistic Regression, SVM, Random Forest)
- Evaluate with metrics like accuracy, precision, recall, F1-score

---

## 📚 Technologies Used

- **Python**
- **Google Colab**
- **pandas, NumPy**
- **nltk**
- **gensim**
- **scikit-learn**

---

## 🧠 How to Use

1. Upload `amazon_reviews.csv` into your Google Colab environment.
2. Run `Amazon_Reviews_Sentiment_Analysis.ipynb`.
3. The notebook handles preprocessing, vectorization, and classification.
4. Use the final outputs to evaluate model performance or try other ML algorithms.

---

## 📌 License

This project is open for educational and personal use. Attribution appreciated.
