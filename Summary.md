# Topic Modeling Stand Up Comedy
Jonathan Wyatt

## Abstract
The goal of this project was to use NLP to derive topics from Stand Up Comedy across various modern Comedians from the last few years.  The Data set was assembled using information [Scraps From The Loft](https://scrapsfromtheloft.com/stand-up-comedy-scripts/) and supplemented with reviews and ratings from [IMDB](https://www.imdb.com/?ref_=nv_home).  The goal of this work was really to explore general themes comedians touch on in their stand ups which figured to be challenging with invented words, sound effects, nuance and sarcasm. The exploration lead to about five major topics identified as love, religion, politics, race and home life. The data was also used to compare comedian and how they varied across time as well as recommending three comedians based on a particular stand up. 

## Design
This project was a pure passion project as I love Comedy.  It was also designed to examine male vs female comedian as the industry is heavily male dominated in terms of recognition and finances with only one female comedian ever breaking the top ten in annual revenues.  

The Project serves to look at what topics these mordern philosphers talk about and in the future could be the basis for ideas to think about when creating routing.  With more transcripts and artists, the goal would be to build a robust, content based recommended beyond the first pass in this project.

## Data
The main dataset contains 1400 documents assmebled from 31 stand ups by 18 comedians.  The distribution of gender (as identified by online sources) was split down the middle of 9 male and 9 female comedians.  The rating information for each special was broken down into average rating by user, rating by male and females, as well as total reviews by user and gender.  Each special was broken into about 40-50 documents at average word length of 190 words per document.  

We hope to add more comedy specials to the database in the future for deeper analysis and more robust analysis.


## Algorithms

*Pre-Processing*

A combination of Lemmatization, Stemming, NLTK and Spacy were used for preparing the text for model usage. 

*Models*
  
NMF, LSA and Corex were the primary models used in this analysis with Anchored Corex providing the most robust results.

*Model Evaluation and Selection*
  
The entire training dataset of 41,000 records was split into 80/20 train/validation vs. holdout.  The scores shown below reflect the AUC ROC for the train vs validation set and the test model based on a refit mode with train and validation together.

The focus of this Project was Topic Modeling with five main derived topics out of the 1400 documents

1) Love

2) Politics

3) Race

4) Religion

5) Homelife

The analysis also looked at Ali Wong's 2016 Baby Cobra stand up processed through a content based recommender using cosine similarity.

The top three most related artists were:
1) Amy Schumer
2) Louis CK
3) Bill Burr

## Tools
- Numpy and Pandas for data manipulation
- Scikit-learn for modeling
- Matplotlib, ScatterText, Seaborn for plotting


## Communication
The Slides for this analysis are included in this repo with further work to be done, so stay tuned. 
