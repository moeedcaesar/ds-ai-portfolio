# IMDB Movie Review Sentiment Analysis

This project builds a **Naive Bayes text classifier** to predict the sentiment of IMDB movie reviews as **positive** or **negative**. The workflow covers **data preprocessing, vectorization, model training, and prediction** using Python and scikit-learn.

---

## 🗂️ Project Overview

| Project | Description | Tools |
|---------|-------------|-------|
| IMDB Sentiment Analysis | Preprocessing IMDB reviews and training a Multinomial Naive Bayes model to classify reviews as positive or negative. | Python, Pandas, NLTK, Scikit-learn |

---

## 📊 Dataset

- **Source:** IMDB Dataset of 50,000 movie reviews  
- **Balanced Classes:** 25,000 positive, 25,000 negative  
- **Columns:**
  - `review`: Raw movie review text  
  - `sentiment`: Target label (`positive` / `negative`)  

---

## 🧹 Data Preprocessing

1. **Tokenization:** Split reviews into words using NLTK.  
2. **Stopword Removal:** Removed common English stopwords.  
3. **Lowercasing & Cleaning:** Keep only alphabetic words, convert to lowercase.  
4. **Example of a cleaned review:**

thought wonderful way spend time hot summer weekend sitting air conditioned theater watching comedy plot simplistic dialogue witty characters likable even well bread suspected serial killer may disappointed realize match point risk addiction thought proof woody allen still fully control style many us grown ...


- Applied preprocessing to all reviews and stored in a new column `clean_review`.

---

## 🛠️ Feature Extraction

- **Bag-of-Words (BoW)** model using `CountVectorizer` from scikit-learn.  
- Converts text into numerical feature vectors for model training.

---

## 🔍 Model

- **Algorithm:** Multinomial Naive Bayes (`MultinomialNB`)  
- **Train/Test Split:** 80% training, 20% testing  
- **Prediction Example:**

```python
clean_text = "This movie is my favourite movie"
count_vector = model.transform(pd.Series(clean_text))
model_nb.predict(count_vector)
# Output: ['positive']
