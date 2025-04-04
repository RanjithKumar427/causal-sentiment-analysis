# ✨ Causal Sentiment Analysis: How Posting Time Affects Tweet Sentiment

---

## 🚀 Project Overview
This project investigates whether the **time a tweet is posted** causally affects its **sentiment positivity**, using a combination of **NLP** and **Causal Inference** techniques.

---

## 🔥 Approach

1. **Sentiment Prediction**  
   - Used HuggingFace Transformers to predict each tweet as **POSITIVE** or **NEGATIVE**.

2. **Feature Engineering**  
   - Extracted Posting Hour, Time of Day, Hashtag Count, Post Length.

3. **Causal Modeling**  
   - Built a Causal DAG using DoWhy to define treatment, outcome, and confounders.
   - Adjusted for confounders using backdoor adjustment.
   - Estimated causal effect using linear regression.

---

## 📈 Key Finding
- **Posting tweets in the Afternoon** increases the probability of positive sentiment by approximately **+1.67%** compared to Morning tweets.

---

## 🛠 Tools Used
- Python
- Huggingface Transformers
- pandas
- dowhy
- matplotlib

---

## 📢 Why This Project?
Understanding causal relationships (not just correlation) is critical for **actionable decision-making** in real-world scenarios like marketing campaigns, social media optimization, and content strategy.

---

## 📂 Repository Structure

```bash
causal-sentiment-analysis/
│
├── data/
│   ├── raw/          # Original dataset
│   └── processed/    # Cleaned, feature-engineered datasets
│
├── notebooks/
│   ├── 1_sentiment_modeling.ipynb
│   ├── 2_feature_engineering.ipynb
│   └── 3_causal_analysis.ipynb
│
├── src/
│   ├── data_processing.py
│   ├── sentiment_model.py
│   └── causal_model.py
│
├── outputs/
│   └── figures/       # DAG graphs and result visualizations
│
├── README.md
└── requirements.txt
