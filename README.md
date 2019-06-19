# Fake-news-prediction

The aim of this project is to identify that particular article if fake or not based on the text of the article.

To prepare a dataset for this, I scraped data from this [website](https://mediabiasfactcheck.com). This website contains the list of news websites and also mentioned that a news website produce high, low or mixed factual data. 

I used WebhoseIO API to scrape these articles along with other meta information about these articles like author, country of the publication, date of publication, is it from news site or bolg etc.

The link of the notebook for scraping data is given below.

[Notebook to scrape data](https://github.com/krutika731/Fake-news-prediction/blob/master/scraping_data_using_API.ipynb)

### EDA:-
After scraping I did some data cleaning and EDA for the articles meta data information.
I removed all the duplicate articles scraped from different website. And also removed all non-English articles from my dataset.

After cleaning the data, I did EDA on article meta data and link for notebook with the code of EDA is given below.

[EDA notebook](https://github.com/krutika731/Fake-news-prediction/blob/master/fake_news_identification_EDA.ipynb)

### Modeling:-

- With Doc2vec:-

    For modeling, I used Doc2vec to generated the vector from trained article text. Doc2vec create the word embedding that can help to   
    retain the meaning of the text in your document.

    After getting the vecotrs from Doc2Vec I tried diffrent classification models like Logistic Regression and Random forest.
    The link of that jupyter notebook given below.

[Doc2vec model](https://github.com/krutika731/Fake-news-prediction/blob/master/Doc2vec_model.ipynb)

- With neural network:-

     I used Keras LSTM model to improve the accuracy in classification. I used Bidirectional LSTM with Conv1D layer to improve the 
     result.The link for this jupyter notebook is given below.

[Deep learning model](https://github.com/krutika731/Fake-news-prediction/blob/master/with_LSTM.ipynb)
