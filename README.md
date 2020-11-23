# Detecting Fake News

<img src="/Images/header.png" alt="Image of phone in front of buildings" >

*By Nadine Amersi-Belton*

## Problem statement

In this project we will look to to build a model to classify news as fake or true. As a hypothetical business scenario, we are working on a consulting assignment for a social media platform who has reported an influx of fake news. 

The rise of fake news is causing the company signficant concern as it could lead to a decline in user engagement not to mention the potential reputational damage for any entity targetted by the fake news, which the platform could be seen as facilitating.

By using machine learning to detect fake news, new stories posted on the platform could be systematically checked and should the model predict them to be fake, they would be initially rejected.

## Components

* **Jupyter Notebooks**

The Jupyter Notebook is our key deliverable and details data preprocessing, exploration, modelling and evaluation.


* **Data**

The data was obtained from [Kaggle](https://www.kaggle.com/clmentbisaillon/fake-and-real-news-dataset).


## Main technologies and packages used

* Python version 3.6.9 
* Nltk version 3.4.5
* Pandas version 0.25.1 
* Beautifulsoup4 version 4.8.0 
* Seaborn version 0.9.0
* Keras version 2.2.4 
* Tensorflow version 2.2.0 
* Wordcloud version 1.6.0

## Results and recommendations

From initial data exploration, we saw that the number of capitals in the title is a key distinguisher between true and fake news, with fake news stories having a significantly higher number, as per the below visualiastion.

<img src="/Images/capitals.png" alt="Distribution of Capitals in Title" width = "500" >

We analyzed n-grams in t, in particular unigrams, bigrams and trigrams. See below for the top 10 bigrams.

<img src="/Images/bigrams.png" alt="Bigrams" width = "500" >

We used GloVe embeddings to capture the global relationship between words. The algorithm works by building a word-word co-occurence matrix. We used a set of pre-trained word vectors from twitter data. Our final model performed extremely well, achieving an accuracy of 99.5% on the test set. We evaluated the model and confirmed that it is not overfitted to the training data and has reached convergence. See below visualisations of the accuracy and loss values for both train and test sets over the epochs.

<img src="/Images/accuracy.png" alt="Accuracy over epochs" width = "500" >
<img src="/Images/loss.png" alt="Loss over epochs" width = "500" >

The confusion matrix for the test set is shown below. We see overall that the False Positives (i.e. where the model predicted true news but actually the news was fake) are higher than the False Negatives, which is a shame as these are more detrimental. However the missclassification numbers are very low overall.

<img src="/Images/cnf.png" alt="Confusion Matrix" width = "500" >

Based on the results, we would recommend the social media platform implement our model to detect fake news.


## Contact

* If you have any questions, you can contact me at nzamersi@gmail.com

Header image: <span>Photo by <a href="https://unsplash.com/@jakobowens1?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">Jakob Owens</a> on <a href="https://unsplash.com/s/photos/social-media-news?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">Unsplash</a></span>