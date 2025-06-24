# Stand-Up Comedy NLP Analysis 🎤

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![NLP](https://img.shields.io/badge/NLP-TextBlob%2FNLTK%2BGensim-green)
![Data Science](https://img.shields.io/badge/Analysis-Sentiment%2BTopic%20Modeling-orange)

A comprehensive NLP analysis of 12 top stand-up comedy specials, with special focus on Ali Wong's comedic style.

## 📌 Project Overview

This project explores:
- Linguistic patterns across top comedians
- Sentiment analysis of routines
- Topic modeling to identify common themes
- Text generation in Ali Wong's style

## 🎭 Featured Comedians
| Comedian | Special | Year |
|----------|---------|------|
| Ali Wong | Baby Cobra | 2016 |
| Dave Chappelle | The Age of Spin | 2017 |
| John Mulaney | Comeback Kid | 2015 |
| Louis C.K. | Oh My God | 2013 |
| Bill Burr | I'm Sorry You Feel That Way | 2014 |
| ...and 7 others | | |

## 🛠️ Technologies Used
```python
# Core Libraries
import pandas as pd
import numpy as np
from sklearn.feature_extraction.text import CountVectorizer
from textblob import TextBlob
from gensim import models
```
## Analysis Techniques
- Document-Term Matrix creation with custom stop words
- Sentiment Analysis using TextBlob
- LDA Topic Modeling (4 identified topics)
- Markov Chain Text Generation

## Visualizations
- Word clouds for each comedian
- Sentiment trend lines
- Profanity scatter plots
- Vocabulary comparison charts

  ## 📂 Project Structure
  ├── notebooks/
│   ├── 1_Data_Cleaning.ipynb       # Web scraping & text preprocessing
│   ├── 2_EDA.ipynb                 # Exploratory analysis & word clouds
│   ├── 3_Sentiment_Analysis.ipynb  # Polarity & subjectivity analysis
│   ├── 4_Topic_Modeling.ipynb      # LDA topic modeling
│   └── 5_Text_Generation.ipynb     # Markov chain text generation
├── data/
│   ├── transcripts/                # Raw transcript files
│   ├── corpus.pkl                  # Processed text corpus  
│   └── dtm.pkl                     # Document-term matrix
└── utils/                          # Helper functions

🔍 Key Findings
- Word Frequency Analysis
- https://i.imgur.com/wordcloud.png

## Sample sentiment calculation
```
pol = lambda x: TextBlob(x).sentiment.polarity
data['polarity'] = data['transcript'].apply(pol)
```
## Topic Modeling Results
- Identified 4 key topics:
- Family (mom, parents)
- Relationships (husband, wife)
- Controversial issues (guns)
- Observational humor

## Generated Comedy
- Example Markov chain output:
- "My husband does know what delivery means. Asian girls have to be pregnant again because white people love dogs."
## 🚀 Installation
- Clone repository:
 ```
  git clone (https://github.com/Abdallah1Atef/Brainwave_Matrix_Intern/edit/Task-2/nlp-in-python-tutorial-master).git
  cd standup-analysis
  ```
  
