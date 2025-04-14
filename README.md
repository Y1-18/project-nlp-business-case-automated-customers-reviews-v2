
# Automated Customer Reviews - NLP Project

##  Project Overview

This project leverages state-of-the-art Natural Language Processing (NLP) techniques to automate the analysis of customer reviews from e-commerce platforms such as Amazon. The key goals are:

- **Sentiment Classification**: Automatically label reviews as positive, neutral, or negative.
- **Product Clustering**: Group product categories into broader meta-categories using embeddings and clustering.
- **Review Summarization**: Generate article-like summaries to help users make informed product decisions.

---

##  Business Objective

Manually analyzing thousands of customer reviews is inefficient and time-consuming. This system uses machine learning to extract insights from large volumes of text, helping companies improve products and enabling consumers to make smarter purchase decisions.

---

##  Tasks Breakdown

### 1. Review Classification

- **Model**: Fine-tuned `bert-base-uncased` using Hugging Face Transformers.
- **Labels**:
  - 1–2 stars → Negative
  - 3 stars → Neutral
  - 4–5 stars → Positive
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-score, Confusion Matrix.

### 2. Product Category Clustering

- **Technique**: Sentence-BERT for encoding product categories.
- **Algorithm**: KMeans clustering (n_clusters = 5).
- **Visualization**: PCA for 2D plotting of clusters.

### 3. Review Summarization

- **Model**: `T5-small` or `BART` for generating blog-style summaries.
- **Includes**:
  - Top 3 recommended products
  - Key differences
  - Top complaints
  - Worst product in the category

---

## Web App Features

Built using **Gradio**, the interactive web application allows users to:

- **Classify reviews** by entering custom text.
- **Explore clusters** of product categories visually.
- **Generate summaries** for selected categories.

---

##  Tech Stack

- Python
- Hugging Face Transformers
- Sentence Transformers
- Scikit-learn (KMeans, PCA)
- Gradio (Web UI)
- PyTorch
- Pandas, NumPy
- Matplotlib

---

##  How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/automated-customer-reviews-nlp.git
   cd automated-customer-reviews-nlp
   ```

2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch the app:
   ```bash
   python app.py
   ```

4. Or open and run the notebook in Google Colab.

---

##  Folder Structure

```
├── data/                    # Cleaned & raw datasets
├── models/                  # Fine-tuned transformer models
├── notebooks/               # Jupyter notebooks for experiments
├── app.py                   # Gradio interface
├── requirements.txt         # Python dependencies
├── README.md                # Project documentation
```

---

##  Sample Results

- Classification Accuracy: **87.4%**
- F1-score (Positive): **0.91**
- 5 Product Clusters (e.g., Accessories, Batteries, E-readers)
- Auto-generated summaries for each cluster category

---

##  Deployment

- The app is deployable via:
  - Hugging Face Spaces
  - AWS EC2 / Lambda
  - Streamlit Cloud
- Currently hosted at: [Insert Link Here]

---

## Deliverables

- ✅ Review Classifier (BERT)
- ✅ Product Category Clustering (KMeans)
- ✅ Summarizer (T5 or BART)
- ✅ Web App with user interaction
- ✅ PDF Report & PPT Presentation

---

## By Albandari Altalhi
---
