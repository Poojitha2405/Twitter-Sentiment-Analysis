Project Overview
This project focuses on real-time sentiment analysis of Twitter data, leveraging Big Data technologies and NLP. The goal is to analyze tweets and classify them as positive, negative, or neutral by implementing a data pipeline for ingestion, processing, and analysis.

Tech Stack & Tools Used 
Data Ingestion: Tweepy (Twitter API), Apache Kafka
Data Processing: Apache Spark, Pandas, NLTK, TextBlob
Data Storage: PostgreSQL, AWS S3, Snowflake
Machine Learning: Logistic Regression, Naïve Bayes, LSTM (Deep Learning)
Data Visualization: Matplotlib, Seaborn, Plotly

Project Workflow
1. Data Ingestion:
Collected tweets using Tweepy (Twitter API) based on specific keywords.
Streamed real-time tweets using Apache Kafka for scalable ingestion.
Stored raw data in AWS S3 for persistence.
2. Data Processing & Cleaning:
Removed special characters, emojis, URLs, and stopwords using NLTK.
Applied Tokenization, Lemmatization, and TF-IDF vectorization for feature extraction.
Filtered out noisy data and duplicates for better model performance.
3. Sentiment Classification:
Used TextBlob for initial sentiment polarity scoring.
Implemented ML models (Logistic Regression, Naïve Bayes) for improved accuracy.
Integrated LSTM (Deep Learning) for better contextual sentiment analysis.
Training Dataset: Used twitter_training.csv dataset for model training and evaluation.
Columns: Tweet ID, Category, Sentiment, Original Tweet, Processed Tweet
Usage: Helps in supervised learning to classify new tweets accurately.
4. Data Pipeline & Storage:
Processed real-time data using Apache Spark Streaming.
Stored structured data in PostgreSQL / Snowflake for querying and analytics.
Used Airflow for automated ETL scheduling and monitoring.
5. Data Visualization & Insights:
Created interactive sentiment trend graphs using Plotly & Seaborn.
Analyzed tweet sentiment distribution over time.
Derived insights on public opinion regarding various topics.

Project Outcomes & Learnings:

Built an end-to-end real-time data pipeline,
Integrated Big Data tools (Kafka, Spark, Snowflake, PostgreSQL),
Applied NLP & Machine Learning for text classification,
Automated ETL workflows with Airflow,
Created interactive dashboards for sentiment trends.

Dataset Details:

File: twitter_training.csv

Columns:
ID: Unique identifier for each tweet
Category: The topic or keyword related to the tweet
Sentiment: Sentiment classification (Positive, Negative, Neutral)
Tweet Text: The actual content of the tweet.

Usage: Used to train and validate the sentiment analysis model for better accuracy.
