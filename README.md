# 🎭 Emotion Recognition in Text using BERT

> A high-performance NLP system for multiclass emotion classification using a fine-tuned BERT model.

---

## 📘 Overview
This project aims to build a reliable model for detecting human emotions from text. The model classifies input into six categories: **joy, sadness, anger, fear, love, and surprise**.

At its core, the system leverages a fine-tuned **BERT-base-uncased** model. By adapting a pre-trained transformer to a labeled emotion dataset, the model is able to capture subtle linguistic patterns and contextual cues that reflect emotional intent.

---

## 🚀 Key Features
- **Transformer-based model**  
  Uses `bert-base-uncased` to capture deep contextual relationships in text.

- **Six-class emotion classification**  
  Predicts one of six emotional states: joy, sadness, anger, fear, love, or surprise.

- **End-to-end pipeline**  
  Covers the full workflow: data preprocessing, tokenization, training, and evaluation.

- **Strong performance**  
  Achieves around **96% accuracy** on the test set.

---

## 📊 Dataset Information
The model was trained on a dataset with more than 20,000 labeled samples:
- **Train:** ~16,000  
- **Validation:** ~2,000  
- **Test:** ~2,000  

Each sample is labeled with one of the following emotions:
`joy`, `sadness`, `anger`, `fear`, `love`, `surprise`.

For preprocessing, the text is tokenized using `BertTokenizerFast` with a maximum sequence length of 128.

---

## 🛠️ Tech Stack
- **Language:** Python  
- **Frameworks:** TensorFlow, Keras  
- **Libraries:** Hugging Face Transformers, Datasets  
- **Tools:** Scikit-learn, Pandas, Matplotlib, Seaborn  

---

## 📈 Model Performance
The model shows consistent performance across all emotion classes, indicating good generalization.

| Metric | Score |
| :--- | :--- |
| **Accuracy** | **96.4%** |
| **Macro F1-Score** | **0.96** |
| **Training Time** | ~3–5 epochs (T4 GPU) |

### Sample Classification Report

    precision    recall  f1-score   support

    anger       0.93      0.96      0.95       215
    fear        0.97      0.96      0.96       224
    joy         0.98      0.98      0.98       250
    sadness     0.98      0.95      0.97       250
    ...

---

## 🏗️ Project Structure
- `emotionanalysis-nlp.ipynb` → Main notebook for training and experimentation  
- `dataset/` → Contains raw text files for training, validation, and testing  

---

## ⚙️ How to Run

1. Clone the repository:
   git clone https://github.com/Frazanhibriz/EmotionAnalysis-NLP.git

2. Install the required dependencies:
   pip install transformers datasets tensorflow pandas scikit-learn

3. Open `emotionanalysis-nlp.ipynb` using Jupyter Notebook or Google Colab, then run all cells.

---

**Focus:** NLP & Machine Learning Engineering
