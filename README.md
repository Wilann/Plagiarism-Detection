# SageMaker Machine Learning

## Project: Plagiarism Detection 

### Source 

Project 6 from Udacity's [Machine Learning Engineer Nanodegree](https://www.udacity.com/course/machine-learning-engineer-nanodegree--nd009t)

### Overview

Built a plagiarism detector, using AWS SageMaker, that examines a text file and performs binary classification; labeling that file as either *plagiarized* or *not*, depending on how similar that text file is to a provided source text 

**Notebook 1: Data Exploration**
- Loaded in plagiarism text data
- Explored existing data features and data distribution (types of plagiarism/tasks)

**Notebook 2: Feature Engineering**
- Cleaned and pre-process the text data (convert categorical to numerical data) 
- Defined features (Containment with an n-gram range and Longest Common Subsequence) for comparing the similarity of an answer text and a source text, and extract similarity features 
- Selected "good" features, by analyzing the correlations between different features 
- Created train/test `.csv` files that hold relevant features and class labels for train/test data points 

**Notebook 3: Train and Deploy Your Model in SageMaker**
- Uploaded train/test feature data to S3 
- Defined a binary classification model and training script via Scikit-Learn
- Trained model and deployed it using SageMaker 
- Evaluate deployed classifier using accuracy (Result: 1.0)
