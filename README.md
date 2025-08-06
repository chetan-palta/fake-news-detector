# 📰 Fake News Detector

This project aims to detect fake news articles using Natural Language Processing (NLP) and Machine Learning techniques. The dataset includes real and fake news headlines/articles, and we build a pipeline to preprocess, clean, and classify the text using various models.

> ⚠️ Work-in-progress. Current version includes preprocessing and model training using TF-IDF and Logistic Regression.

---

## 📁 Project Structure

```

fake-news-detector/
├── data/
│   ├── raw/                      # Raw datasets (not committed)
│   └── cleaned\_df.pkl            # Preprocessed data (ignored in Git)
├── notebooks/
│   ├── 01\_explore\_dataset.ipynb         # Initial exploration
│   ├── 02\_text\_preprocessing.ipynb      # Text cleaning and preprocessing
│   └── 03\_model\_training.ipynb          # TF-IDF + Logistic Regression
├── .gitignore
├── README.md
└── requirements.txt (upcoming)

````

---

## 📌 Notebooks Overview

### 📓 01_explore_dataset.ipynb
- Loaded and inspected the raw dataset
- Checked for class distribution and null values
- Basic visualization and exploration

### 🧹 02_text_preprocessing.ipynb
- Performed text cleaning: lowercasing, punctuation removal, stopword removal, etc.
- Created a reusable cleaning function
- Saved the cleaned DataFrame as `cleaned_df.pkl` using `pickle`

### 🤖 03_model_training.ipynb
- Loaded preprocessed data from `.pkl`
- Vectorized text using **TF-IDF**
- Trained a **Logistic Regression** model
- Evaluated using accuracy, precision, recall, and confusion matrix

---

## ⚙️ Installation & Setup

1. Clone the repo:
```bash
git clone https://github.com/chetan-palta/fake-news-detector.git
cd fake-news-detector
````

2. Create and activate a virtual environment (optional but recommended):

```bash
python -m venv venv
venv\Scripts\activate  # For Windows
```

3. Install dependencies:

```bash
pip install -r requirements.txt  
```

4. Run the notebooks in order (recommended via Jupyter or VSCode).

---

## 🛑 Note on Large Files

* The `cleaned_df.pkl` file is over 280 MB and is not tracked via GitHub due to size limits.
* Re-run the preprocessing notebook (`02_text_preprocessing.ipynb`) locally to regenerate it.

---

## ✅ Next Steps

* Add more ML models (Naive Bayes, SVM)
* Implement GridSearchCV for hyperparameter tuning
* Add Streamlit or Gradio app for live demo
* Export final model for deployment

---

## 💡 Fun Fact

My favorite queue is the **coffee queue** ☕😉

---

## 🧠 Author

**Chetan Palta**
Aspiring AI/ML Engineer | DSA Explorer | Web Dev Learner 🚀
GitHub: [@chetan-palta](https://github.com/chetan-palta)

---

## 📜 License

MIT License. See `LICENSE` file for details.



