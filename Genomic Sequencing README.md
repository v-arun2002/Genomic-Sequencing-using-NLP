# 🧬 Genome Sequencing Using NLP  
*A Machine Learning & Deep Learning Project for Promoter Region Classification*

This project applies **Natural Language Processing (NLP)** techniques to **genomic DNA sequences** to classify promoter vs. non-promoter regions.  
By treating DNA sequences as biological text, we unlock new pathways for scalable and accurate genomic analysis.

---

## ⭐ Overview

- **Goal:** Predict whether a genomic DNA sequence is a **promoter** or **non-promoter** region  
- **Dataset:** 22,598 labeled FASTA sequences from *Drosophila Melanogaster*  
- **Approach:** NLP tokenization (k-mers), ML & DL models, ensemble learning  
- **Best Model:** **CNN with one-hot encoded k-mers (k=6)**  
- **Best Accuracy:** **91.3%**

---

## 📌 Project Highlights

- 🔍 **Problem:** Promoter region classification in genomic DNA  
- 📚 **Dataset:** Drosophila Melanogaster genome (22,598 FASTA sequences)  
- 🧪 **Techniques Used:**
  - k-mer tokenization (analogous to NLP n-grams)
  - TF-IDF vectorization  
  - One-hot encoding for DL models  
- 🤖 **Models:**
  - Classical ML: Random Forest, LightGBM, Naive Bayes, Logistic Regression  
  - Deep Learning: LSTM, BiLSTM, CNN  
  - Ensemble: Voting Classifier, Stacking Classifier  
- 🏆 **Top Performance:**  
  CNN + one-hot encoded 6-mers → **91.3% accuracy**

---

## 🧠 Motivation

Promoter regions control gene expression and are essential to understanding biological regulation.  
Traditional lab-based methods (DNase footprinting, ChIP-seq) are **accurate but expensive and slow**.

Using **NLP + ML**, we create an **automated, scalable, cost-effective** system that analyzes DNA sequences as text patterns, enabling rapid genomic discovery and computational biology research.

---

## 📊 Dataset Overview

| Attribute        | Details                                                                 |
|------------------|-------------------------------------------------------------------------|
| **Source**       | [IEEE DataPort – Drosophila Melanogaster](https://dx.doi.org/10.5072/FK2GT5M94X) |
| **Format**       | FASTA                                                                  |
| **Total Sequences** | 22,598                                                              |
| **Classes**      | Promoter (1), Non-Promoter (0)                                         |
| **Class Balance**| Balanced                                                               |

---

## 🧭 Project Architecture  
<img width="1632" height="947" alt="PROJECT_ARCHITECTURE" src="https://github.com/user-attachments/assets/7ec4dfe8-a9f3-4228-9e16-1f0b1c136b4c" />

---


## 🧪 Preprocessing Pipeline

- Convert sequences to uppercase  
- Remove unknown nucleotides  
- Standardize sequence length  
- Generate **k-mers (k = 5–6)**  
- Map labels (Promoter / Non-Promoter)  
- Remove duplicate sequences  

---

## 🔍 Feature Engineering

- **TF-IDF Vectorization** on k-mers for classical ML models  
- **One-Hot Encoding** for CNN, LSTM, and BiLSTM models  

---

## 🤖 Model Performance Summary

| Model                       | Accuracy (%) |
|----------------------------|--------------|
| Random Forest + TF-IDF     | 72.2         |
| LightGBM + TF-IDF          | 78.4         |
| Naive Bayes + TF-IDF       | 74.3         |
| Logistic Regression        | 78.2         |
| LSTM                       | 69.1         |
| BiLSTM                     | 67.3         |
| **CNN**                    | **91.3**     |

---

## 🔮 Future Enhancements

- 🔬 Integrate genomic transformer models such as **DNABERT**  
- 🧩 Include biological metadata such as gene location and conservation scores  
- 🧬 Expand to **multi-class classification** (enhancers, silencers, exons, etc.)  
- 🚀 Explore attention-based and transformer-based deep learning architectures  

---

## 🤝 Acknowledgements

This work is inspired by state-of-the-art genomic classification models and was supported by coursework at **Northeastern University**.
