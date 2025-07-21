# PubMed-NLP-Classifier

A lightweight end-to-end ML pipeline that classifies biomedical abstracts from PubMed into disease categories using TF-IDF and Logistic Regression.

## Project Overview

This project retrieves real-world abstracts from PubMed based on multiple disease keywords and trains a multiclass text classifier to categorize them automatically. It's designed as a proof-of-concept for biomedical text classification tasks in noisy and unstructured environments.

- Language: Python
- Libraries: `Biopython`, `scikit-learn`, `pandas`
- Dataset: Ffetched abstracts using the Entrez API (Biopython)
- Model: TF-IDF + Logistic Regression
- Classes: `["cancer", "diabetes", "stroke", "asthma", "hypertension"]`

## Features

- Programmatic access to PubMed abstracts using the Entrez API
- Automated corpus creation and labeling
- Preprocessing pipeline using `TfidfVectorizer`
- Multiclass classifier with `LogisticRegression`
- Achieved ~61% accuracy on test set across 5 disease classes

## Installation

```bash
git clone https://github.com/yourusername/pubmed-nlp-classifier.git
cd pubmed-nlp-classifier
pip install -r requirements.txt
