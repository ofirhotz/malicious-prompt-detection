# 🛡️ Malicious Prompt Detection in LLMs

  
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ofirhotz/malicious-prompt-detection/blob/main/Malicious_Prompt_Detection.ipynb)

An end-to-end Machine Learning and Natural Language Processing (NLP) pipeline designed to detect malicious prompts and prompt-injection attacks targeting Large Language Models (LLMs).

---

## 📌 Project Overview
As Large Language Models (LLMs) are widely integrated into autonomous workflows, securing them against adversarial inputs—such as prompt injections, jailbreaks, and system override attempts—has become critical.

This project analyzes adversarial and benign inputs from the **MPDD (Malicious Prompt Detection Dataset)**, extracts linguistic and statistical feature representations, and trains classification models to reliably filter malicious prompts.

---

## ⚙️ Pipeline Architecture

1. **Exploratory Data Analysis (EDA):**
   * Class balance inspection across training and test splits.
   * Token length and lexical diversity distributions for benign vs. adversarial samples.

2. **Feature Engineering & Preprocessing:**
   * Text sanitization and token normalization.
   * Extraction of statistical indicators (punctuation ratio, casing anomalies, entropy metrics).
   * N-gram extraction and TF-IDF vectorization.

3. **Model Training & Evaluation:**
   * Benchmark classification models (Logistic Regression, Random Forest, Naive Bayes / SVM).
   * Cross-validation and hyperparameter optimization.
   * Evaluation using Precision, Recall, F1-Score, and ROC-AUC curves.

---

## 📂 Repository Structure

```text
├── Malicious_Prompt_Detection.ipynb   # Main Jupyter notebook with pipeline and analysis
├── MPDD_trainset.csv                  # Training dataset
├── MPDD_testset.csv                   # Holdout test dataset
└── README.md                          # Project documentation
```

## 🚀 Getting Started

### Option 1: Run in Google Colab (Recommended)
Click the badge below to run the complete pipeline interactively:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ofirhotz/malicious-prompt-detection/blob/main/Malicious_Prompt_Detection.ipynb)

### Option 2: Run Locally
1. Clone the repository:
   ```bash
   git clone [https://github.com/ofirhotz/malicious-prompt-detection.git](https://github.com/ofirhotz/malicious-prompt-detection.git)
   cd malicious-prompt-detection

2. Install dependencies:

    ```text
    pip install notebook pandas numpy scikit-learn matplotlib seaborn
    ```

3. Launch Jupyter Notebook:

   ```text
   jupyter notebook Malicious_Prompt_Detection.ipynb
   ```
