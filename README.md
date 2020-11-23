# fake-news

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

Our final model performed extremely well, achieving an accuracy of 99.5% on the test set. We evaluated the model and confirmed that it is not overfitted to the training data and has reached convergence. See below visualisations of the accuracy and loss values for both train and test sets over the epochs.

<img src="/Images/accuracy.png" alt="Accuracy over epochs" width = "500" >
<img src="/Images/loss.png" alt="Loss over epochs" width = "500" >

Based on the results, we would recommend the social media platform implement our model to detect fake news.


## Contact

* If you have any questions, you can contact me at nzamersi@gmail.com