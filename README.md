<div align="center">

# Social Risk Sentinel

## Suicidal Ideation Detection In Online Social Content

<img src="Assets/web.gif" > 
</div>

## Introduction

Social media and online communities provide people with safe and anonymous places to talk about their mental health and share their emotions. To help prevent suicide, it's important to identify posts and messages online that may indicate someone is thinking about suicide. I used advanced technology called natural language processing (NLP) to do this. Specifically, I looked at two popular websites, Reddit and Twitter. By analyzing the words people use in their posts, and using techniques like machine learning and deep learning, I can determine if someone might be at risk of suicide or not.

## DataSet

I gathered data from two different sources: Reddit and Twitter. In the Reddit dataset, there were 2958 instances of posts suggesting suicidal thoughts, alongside 5381 posts that did not indicate suicidal intentions. These posts were collected from various subreddits such as 'suicide watch', 'depression', and 'anxiety'. On Twitter, I collected a total of 3000 tweets that contained phrases like 'end my life' or 'die'.

## Feature Processing and Training

- Conducted text cleaning and eliminated certain stopwords specific to the corpus. Additionally, generated a word cloud to visually represent the most commonly used words in the corpus.
- Utilized both Bag of Words and TFIDF Vectorizer for vectorization.
- Employed grid search CV to identify optimal parameters for training the model with Random Forest Classifier, achieving an accuracy of 96%.
- Trained the model using Multilayer Bidirectional LSTM with GLOBE embedding, resulting in an accuracy of 97%.

## Results

Results of different methods applied

## Usage

- `Dataset` : All the collected and cleaned dataset
- `Data_Collection` : Code for scraping data from reddit and twitter
- `Src` : All The source code for text preprocessing and building ml models
- `Pretrained_Models` : All the Pretrained Models and tokenizers
- `Flask`: Code for server and model deployment

### How to Run Server

- `cd Flask`
- `python app.py`
