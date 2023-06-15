# Sarcasm-Detection-BERT
Final Project for COSC 480: Natural Language Processing at Colgate University

## Abstract
Sarcasm detection has crucial implications on sentimental analyses, which is prevalently applied to social media monitoring and customer support management. Recently, sarcasm detection studies have investigated how pre-trained transformers-based models achieve better prediction accuracies for in-distribution testing on a specific data genre in the sarcasm detection domain. To uncover the abstract-level elements of sarcasm across data types, we select Naive Bayes with Term Frequency - Inverse Document Frequency (TF-IDF) and DistilBERT as our models of interest and introduce a pipeline to test generalizability: a model will be trained on high-quality, large-scale dataset of news headlines, then its performances on in-distribution news headlines and on manually annotated out-of-distribution sarcastic datasets from Twitter and Reddit will be compared. We argue that while both models fail the test of generalizability, Naive Bayes is capable of learning something about sarcasm on an abstract level while DistilBERT is not. Our results make the case that a simpler model is probably more efficient and powerful for social-media sarcasm detection in real-world tasks.

## Research Questions
1. How generalizable are the performances of 5-gram Naive Bayesian model  with TF-IDF and DistilBERT trained on news headlines when performing sarcasm detection on Tweets and Reddit posts?
2. Based on the out-of-distribution performances of these 2 NLP models, what can we infer about a) what linguistic properties make a text sarcastic, b) whether trained LMs are able to capture these properties, and c) whether different data types share the same set of features that indicate sarcasm

## Methodology
We summarize our methodology and contributions in this work as follows:
- We first introduce a balanced, high-quality and large-scale news headline dataset, which is validated as superior in language and labeling. We also manually cleaned and selected two social media datasets from Twitter and Reddit from available benchmark datasets in this domain.
- Next, we create a pipeline for training, hyper-parameter tuning, and testing, which both Naive-Bayes with IF-IDF and DistilBERT will follow. We establish a baseline using a five-gram Naive Bayes model and conduct testing (both in-distribution and out-of-distribution), then evaluate using accuracy and F-1 scores. We discover obvious failure of generalizability in both cases.
- Lastly, we discovered a surprising finding when cross-examining Naive Bayes and DistilBERT model: TF-IDF generates higher accuracy than a fine-tuned DistilBERT on social media datasets. We then discuss its implications and future work.

## Paper 
The research paper writeup for this project follows the Instructions for ACL Proceedings 2023. 

## Poster

## Acknowledgements
We would like to thank Professor Grusha Prasad for the supportive guidance and insightful conversations.
