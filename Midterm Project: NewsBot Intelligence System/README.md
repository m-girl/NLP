Project Overview
The NewsBot Intelligence System is an end to end Natural Language Processing (NLP) pipeline designed to analyze, classify, and extract insights from news articles.

Built entirely in a Jupyter Notebook, the system combines:

•	Text preprocessing
•	TF IDF vectorization
•	Machine learning classification
•	Sentiment analysis
•	Named Entity Recognition (NER)
•	Entity analytics
•	Comprehensive dataset insights
•	A full NewsBot inference engine

This project demonstrates how modern NLP techniques can transform raw text into structured intelligence suitable for:

•	Automated content routing
•	Editorial decision support
•	Trend monitoring
•	Entity tracking
•	Sentiment aware analysis
•	Knowledge extraction

Features

News Classification

Classifies articles into 5 categories:

business, entertainment, politics, sport, tech

Sentiment Analysis

Uses VADER to compute:

•	compound
•	positive
•	neutral
•	negative

Named Entity Recognition

Extracts entities such as:

PERSON, ORG, GPE, MONEY, DATE, PRODUCT, EVENT, and more.

Entity Analytics

•	Entity frequency
•	Entity type distribution
•	Category specific entity patterns
•	Heatmaps and visualizations

Comprehensive Insights Dashboard

Combines classification, sentiment, entities, and dataset statistics into a single intelligence report.

NewsBot Intelligence System

A fully integrated class that processes new articles and returns:
•	predicted category
•	confidence scores
•	sentiment
•	extracted entities
•	actionable insights

Project Structure

├── data/
│   └── bbc-news-data.csv
├── notebook/
│   └── newsbot_intelligence_system.ipynb
├── README.md
└── requirements.txt  (optional)

Setup Instructions

Follow these steps to run the project in Jupyter Notebook.

1. Install Python 3.9+
   
Recommended:

•	Anaconda
•	Miniconda
•	pyenv

2. Install Dependencies
   
Inside your environment:
pip install numpy pandas matplotlib seaborn scikit-learn nltk spacy

3. Download spaCy Model

python -m spacy download en_core_web_sm

4. Download NLTK Resources

Inside a Python shell or notebook:

import nltk
nltk.download('vader_lexicon')

5. Launch Jupyter Notebook
   
jupyter notebook

Open:

newsbot_intelligence_system.ipynb

 How to Use the Notebook
 
The notebook is organized into modules:

Module 1 — Load & Explore Dataset

Load the BBC news dataset and inspect categories.

Module 2 — Preprocessing

Clean text, remove noise, and prepare for vectorization.

Module 3 — Feature Engineering

Generate TF IDF vectors, sentiment scores, and length features.

Module 4 — Model Training

Train and evaluate:

•	Naive Bayes
•	Logistic Regression
•	SVM

Module 5 — Model Comparison

Compare accuracy, CV scores, and select the best model.

Module 6 — NER Pipeline

Extract entities using spaCy.

Module 7 — Entity Analytics

Visualize entity patterns and distributions.

Module 8 — Comprehensive Insights

Generate a full intelligence dashboard.

Module 9 — NewsBot Intelligence System

Run the final integrated system on new articles.

Testing the System

At the end of the notebook, you can test NewsBot with:

newsbot.process_article(title, content)

This returns:

•	predicted category
•	confidence
•	sentiment
•	entities
•	insights

Example Output

Predicted Category: tech (43.22% confidence)

Sentiment: positive (0.660)

Entities Found: Microsoft Corporation, Satya Nadella, $2 billion

Insights:

 - High confidence classification
 - Positive sentiment detected
 - Key entities identified
 - 
Requirements (Optional)

If you want a requirements.txt:

numpy
pandas
matplotlib
seaborn
scikit-learn
nltk
spacy
en-core-web-sm @ https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.7.1/en_core_web_sm-3.7.1.tar.gz

License

This project is for educational and research purposes.

Acknowledgements

•	BBC News Dataset
•	spaCy NLP
•	NLTK VADER
•	Scikit Learn

