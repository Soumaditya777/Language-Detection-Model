# 🌐 Language Detection Model (Multilingual NLP)

A Machine Learning project that detects the language of a given text using Natural Language Processing (NLP) techniques. The model is trained on multilingual data using a Naive Bayes classifier and CountVectorizer.

---

## 📁 Dataset Overview

- **Source**: `language.csv`
- **Records**: 22,000
- **Languages Covered**: 22
  - English, French, Spanish, German, Hindi, Chinese, Japanese, Korean, Tamil, Arabic, Persian, Thai, Dutch, Turkish, Russian, Latin, Swedish, Estonian, Indonesian, Romanian, Pushto, Urdu

---

## 🔍 Objective

Build a classification model that takes in any short text and correctly predicts its language.

---

## 🧪 Libraries Used

- `pandas`  
- `numpy`  
- `scikit-learn` (`CountVectorizer`, `MultinomialNB`, `train_test_split`)

---

## 🔧 Process

### ✅ 1. Data Preprocessing
- No missing values
- Verified language distribution (1000 samples per language)

### 🧠 2. Feature Extraction
- Used **CountVectorizer** to convert text into numerical features (Bag-of-Words)

### 🧪 3. Model Training
- Split dataset into train/test (67%/33%)
- Trained a **Multinomial Naive Bayes** classifier

---

## 📈 Model Performance

- **Train/Test Split**: 14,740 train / 7,260 test
- **Accuracy**: `95.3%`

```python
model.score(X_test, y_test)
# Output: 0.953
