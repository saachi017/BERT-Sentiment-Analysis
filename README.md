# BERT-Sentiment-Analysis
Sentiment analysis and text classification using a pre-trained BERT model on the SMILE Twitter Emotion Dataset.

The objective is to fine-tune `bert-base-uncased` on the dataset and classify tweets into seven emotion/relevance categories.

---

## 🎯 Project Overview

Sentiment analysis is the task of identifying the emotional meaning expressed in text.

Traditional approaches often struggle when the meaning of a word changes depending on context. BERT addresses this by using contextual language representations learned from large-scale text.

In this project, BERT is fine-tuned for a 7-class text classification task.

---

## 📊 Dataset

**Dataset:** SMILE Twitter Emotion Dataset

The dataset contains tweets annotated with emotion/relevance labels.

### Dataset Statistics

- Original samples: **3,085**
- Samples after preprocessing: **3,011**
- Number of classes: **7**

### Classes

- Happy
- Angry
- Sad
- Surprise
- Disgust
- Nocode
- Not-relevant

---

## 🧠 Model

**Pre-trained model:** `bert-base-uncased`

The model follows this workflow:

Dataset  
↓  
Preprocessing  
↓  
Tokenization  
↓  
BERT  
↓  
Classification Head  
↓  
7-Class Prediction

The pre-trained BERT model is fine-tuned on the SMILE dataset for the classification task.

---

## ⚙️ Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- BERT
- Pandas
- Scikit-learn
- Google Colab / Jupyter Notebook

---

## 📈 Results

The model was evaluated using:

- Test Accuracy
- Macro-F1
- Weighted-F1

> Final performance metrics are documented in the presentation and notebook.

---

## 📁 Repository Structure

```text
BERT-Sentiment-Analysis/
│
├── dataset/
│   └── smile-annotations-final.csv
│
├── notebook/
│   └── BERT_Text_Classification_SMILE.ipynb
│
├── README.md
│
└── presentation/
    └── BERT_Sentiment_Analysis.pptx
