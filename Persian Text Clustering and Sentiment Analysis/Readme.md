Persian Text Clustering and Sentiment Analysis

This project focuses on clustering and sentiment analysis of Persian texts using two public datasets: Persian-Text-Sentiment and Persian News Dataset. It combines natural language preprocessing with vectorization and clustering techniques (KMeans) to group semantically similar documents and evaluate cluster quality.

📂 Datasets

Persian-Text-Sentiment

Source: SeyedAli/Persian-Text-Sentiment

Description: A labeled collection of Persian text samples categorized by sentiment polarity.

Purpose: Used for clustering and sentiment-based document grouping.

Persian News Dataset

Source: saied/persian_news_dataset

Description: A large corpus of Persian news articles categorized by topic.

Purpose: Used for topic clustering and linguistic preprocessing.

🧪 Pipeline Overview

Install Dependencies

Required libraries:

datasets

scikit-learn

stanza

pandas

Installation:

bash
Copy
Edit
pip install datasets stanza scikit-learn pandas
Load and Explore Data

Load both datasets using Hugging Face’s datasets library

Display text samples and associated labels

Count sentiment label ranges and categories

Feature Extraction using TF-IDF

Use TfidfVectorizer with min_df set to 50 or 2

Unicode normalization and stopword filtering

Extract token-document matrix for clustering

Clustering with KMeans

Number of clusters:

2 for Persian-Text-Sentiment

6 for Persian News Dataset

Evaluate clustering using Calinski-Harabasz Index

Store cluster assignments in DataFrames

Output and Visualization

Save each cluster’s documents into separate CSV files
(e.g. cluster0.csv, cluster1.csv, ...)

Print top 10 keywords (terms) for each cluster

Advanced Preprocessing with Stanza

POS tagging using stanza’s Persian language models

Filter tokens based on syntactic roles: NOUN, VERB, ADJ, etc.

Re-vectorize preprocessed texts and recluster

📈 Evaluation

Calinski-Harabasz Index used for unsupervised cluster quality

Keyword extraction helped interpret the cluster meanings

Different min_df and cluster count parameters were tested

📁 Outputs

The following files are generated:

cluster0.csv

cluster1.csv

...

Keyword lists per cluster printed to console

⚙️ Configuration Parameters

min_df values tested: [2, 10, 50]

number of clusters: [2, 6]

sample sizes: [500, 1000]

🧠 Project Goals

This project aims to:

Introduce Persian text preprocessing using Stanza

Perform unsupervised learning on Persian documents

Explore how clustering can reveal document structure in the absence of labels

🚀 How to Run

Clone this repository

Open Code.ipynb in Jupyter or Google Colab

Run all cells step by step

📬 Contact

If you have suggestions, questions, or improvements, feel free to open an issue in this repository.

Let me know if you'd like me to generate a minimal version or format it for GitHub with Markdown styling.