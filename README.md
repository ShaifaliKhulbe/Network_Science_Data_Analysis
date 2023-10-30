# Twitter Data Analysis: Hyderabad Blast

This project involves the analysis of tweets related to the "Hyderabad blast" topic. The objective is to gain insights from the dataset by performing various text processing and network science techniques.

## Pre-processing

1. **Remove Stop-Words**: We use the Natural Language Toolkit (NLTK) library to remove common stop-words from the text, improving the quality of the data.

2. **Remove Hashtags and User Accounts**: Any hashtags and user account mentions are removed to focus on the content of the tweets.

3. **Remove Noise**: Words with less than three letters, considered as noise, are eliminated.

## Text Processing

1. **Top Keywords by TF-IDF**: The top 50 keywords from the dataset are identified using the Term Frequency-Inverse Document Frequency (TF-IDF) method.

2. **Top Nouns by TF-IDF**: Only nouns from tweet text are retained, and then the top 50 nouns are extracted using TF-IDF.

## Network Science and Pretrained Language Model

1. **Graph Creation**: A graph (G) is created where nodes represent tweets, and edges are established based on cosine similarity between the tweet texts.

2. **Graph Analysis**:
   - **Degree Distribution**: The degree distribution of the graph is calculated.
   - **Degree Centrality**: Degree centrality of all tweets is calculated, and the top 10 tweets are identified.
   - **PageRank Centrality**: PageRank centrality of all tweets is calculated, and the top 10 tweets are identified.
   - **Clustering Coefficients**: Clustering coefficients are calculated for the entire graph, top 10 tweets, and bottom 10 tweets.

3. **BERT Embedding-Based Graph (G1)**: A similar graph (G1) is created, but cosine similarity is calculated based on pre-trained BERT uncased embeddings.

4. **Comparison of Centrality Measures**:
   - A comparison is made between G (text-based) and G1 (BERT-based) in terms of degree centrality, PageRank centrality, and clustering coefficients.

## Sentiment Calculation

1. **Sentiment Analysis**: The sentiment of each tweet is determined using both the Vader sentiment analyzer and SentiWordNet.

For a detailed analysis of the questions and the project's findings, please refer to the provided Colab notebook.

## Python Libraries Used

- NLTK (Natural Language Toolkit)
- Scikit-learn
- NetworkX
- Transformers (for BERT embeddings)
- VaderSentiment
- Matplotlib


## Repository Contents

- `Data/hblast_input_data`: This directory contains the dataset of tweets related to the topic "Hyderabad blast."

- `Computational_Social_Science_Questions.pdf`: The PDF file with the questions for this analysis.

- `Hyderabad_Blast_Analysis.ipynb`: The Colab notebook with the responses to the questions and the analysis.

- `README.md`: The README file you are currently reading.
---
