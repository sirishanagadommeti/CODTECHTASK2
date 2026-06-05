# CODTECHTASK2
Project Overview
Name: Dommeti Naga Sirisha
Company: CodTech IT Solutions
ID: CT12AI26
Domain: Artificial Intelligence
Duration: May to July 2024
Mentor: G. Sravani

Project overview:sentenetal analysis
objective:
The objective of this project is to develop a sentiment analysis model that can accurately classify and predict the sentiment of a given text. Sentiment analysis, also known as opinion mining, is a crucial aspect of natural language processing (NLP) that aims to identify and extract subjective information from textual data. This project involves data collection, preprocessing, feature extraction, model training, and evaluation. By leveraging various machine learning algorithms and techniques, this project aims to provide valuable insights into public opinion and sentiment trends across different domains, such as social media, customer reviews, and news articles.

Key Activities :
Data Collection: Gathered textual data from various sources.
Data Preprocessing: Cleaned and tokenized text data.
Exploratory Data Analysis: Analyzed data patterns and visualized sentiment distribution.
Feature Extraction: Extracted relevant features using techniques like TF-IDF and word embeddings.
Model Training: Trained machine learning models to classify sentiments.
Model Evaluation: Evaluated model performance using metrics such as accuracy, precision, recall, and F1-score.
Deployment: Deployed the model for real-time sentiment analysis.

Order Date =
DATE(
    LEFT(Sales[Order Date Key],4),
    MID(Sales[Order Date Key],5,2),
    RIGHT(Sales[Order Date Key],2)
)


Order Date =
DATE(
    VALUE(LEFT(FORMAT(Sales[Order Date Key], "00000000"), 4)),
    VALUE(MID(FORMAT(Sales[Order Date Key], "00000000"), 5, 2)),
    VALUE(RIGHT(FORMAT(Sales[Order Date Key], "00000000"), 2))
)

Order Date =
DATE(
    INT(Sales[Order Date Key] / 10000),
    INT(MOD(Sales[Order Date Key] / 100, 100)),
    MOD(Sales[Order Date Key], 100)
)

