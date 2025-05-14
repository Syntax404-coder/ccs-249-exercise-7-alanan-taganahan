# 🧠 tc_ner_model

CCS-249-Exercise-7-alanan-taganahan's **Trigram Language Model** and a **Hidden Markov Model for Named Entity Recognition (NER)**. This project dives into understanding how different models perform in tagging named entities using the CoNLL-2003 dataset.

---

## 📌 Objective

I wanted to compare two types of models:
- A **Trigram Language Model**, designed to predict the next word in a sequence.
- A **Hidden Markov Model (HMM)**, specifically trained for **Named Entity Recognition (NER)**.

My goal? To see how well each performs and to get hands-on experience with sequence modeling.

---

## 📂 Dataset

I'm using the [CoNLL-2003 dataset](https://www.clips.uantwerpen.be/conll2003/ner/), which contains English sentences annotated with:
- Named entities like **Persons (PER)**, **Organizations (ORG)**, **Locations (LOC)**, and **Miscellaneous (MISC)**.

> 📍 File used: `conll2003/eng.train`

---

## 🚀 Models Implemented

### 1. Trigram Language Model
- Predicts the next word given a bigram context.
- Useful for understanding sentence structure.
- **Not designed** for NER.
- **Accuracy:** ~12.66%
- Generated sentences were often incoherent or generic.

```python
context = ['capital', 'of']
model.predict_next(context)
