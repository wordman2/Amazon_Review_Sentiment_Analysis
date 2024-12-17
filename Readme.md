# **Amazon Reviews Sentiment Analysis**

This repository explores and classifies **Amazon reviews** based on their sentiment. The analysis includes **visualization of BERT embeddings**, fine-tuning sentiment classification models, and performing topic extraction. This project was eloborated as part of the Data Mining lecture at TU Dublin. Below is an overview of the key tasks and techniques implemented in this project.

---

## **Key Highlights**

1. **Sentiment Classification**:
   - One transformer-based models are fine-tuned and evaluated on the Amazon reviews dataset:
     - **DistilBERT**: A faster, lightweight version of BERT.

2. **Embedding Visualization**:
   - BERT embeddings of reviews are projected into **2D space** using **t-SNE** for better visualization and interpretation.

3. **Topic Extraction**:
   - Unsupervised learning techniques are applied to identify themes and similarities within the reviews:
     - **Latent Dirichlet Allocation (LDA)**: For topic modeling.
     - **k-Means Clustering**: For clustering similar reviews.

---

## **Project Workflow and Repo Structure**

1. **Data Understanding and Preparation**:
   - Load and preprocess Amazon reviews dataset.

2. **Data Visualisation and Exploration**:
    - Generate 768 dimensional BERT embeddings for reviews.
    - Use **t-SNE** to reduce embedding dimensions to 2D for visualization.
   
3. **Model Building and Evaluation**
    - Fine-tune DistilBERT on the review data.
   - Evaluate models for accuracy and performance.
   
4. **Advanced Techniques and Analysis**:
   - Apply LDA to extract topics from the reviews.
   - Use k-Means clustering to group similar reviews based on BERT embeddings.

---

## **Technologies Used**

- **Python**: For scripting and model training.
- **Transformers**: Hugging Face library for BERT-based models.
- **scikit-learn**: For k-Means clustering.
- **Gensim**: For LDA topic modeling.

---

## **Installation**

To reproduce the analysis, clone this repository and install the required libraries:

```bash
git clone https://github.com/wordman2/amazon-reviews-sentiment.git
cd amazon-reviews-sentiment
conda env create --file environment.yml