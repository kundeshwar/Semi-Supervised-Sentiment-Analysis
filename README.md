# Semi-Supervised-Sentiment-Analysis
This code uses semi-supervised learning to perform sentiment analysis on a dataset of movie reviews from IMDB. 
 Semi-supervised learning is used to classify the reviews as either positive or negative based on their text content. The dataset is pre-processed and cleaned using NLTK library and pre-trained models.

## Prerequisites
- Python 3.x
- Jupyter Notebook
- pandas
- matplotlib
- seaborn
- NLTK
- scikit-learn
## Installation
**Install** 
```
Python 3.x
```
**Install** Jupyter Notebook:
``` 
pip install jupyter
```
**Install** pandas: 
``` 
pip install pandas 
```
**Install** matplotlib: 
``` 
pip install matplotlib 
```
**Install** seaborn: 
``` 
pip install seaborn 
```
**Install** NLTK: 
``` 
pip install nltk 
```
**Install** scikit-learn: 
``` 
pip install -U scikit-learn 
```
## Dataset
The dataset used in this code is the IMDB dataset. It contains 50,000 movie reviews labeled as positive or negative.

## Running the Code
- Open Semi-Supervised Sentiment Analysis.ipynb in Jupyter Notebook.
- Run each cell to execute the code step by step.
- The final output of the code is the accuracy score of the trained model on the test data.
## Preprocessing
1. The data is preprocessed to remove noise such as URLs, special characters, and HTML tags.
2. The text is converted to lowercase to make it easier to work with.
3. Stopwords are removed from the text, as they do not add much meaning to the sentiment of the review.
4. The Porter stemming algorithm is used to convert words to their base form, to reduce the number of unique words in the dataset and improve the model's accuracy.
## Model
- The dataset is split into a training set and a test set.
- The training set is further split into a labeled set and an unlabeled set.
- A logistic regression model is trained on the labeled data.
- The model is used to predict labels for the unlabeled data.
- The predicted labels are combined with the labeled data to create a new, larger labeled dataset.
- A Multinomial Naive Bayes model is trained on the new labeled dataset.
- The accuracy of the trained model is evaluated on the test set.
## Conclusion
Semi-supervised learning can be an effective approach to sentiment analysis, especially when labeled data is scarce. This code demonstrates how to use semi-supervised learning to classify movie reviews as either positive or negative with high accuracy.
