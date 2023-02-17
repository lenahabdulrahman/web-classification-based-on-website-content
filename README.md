# web-classification-based-on-website-content
A real-time website classifier was developed for page content-based filtering using machine learning techniques (ML) and Natural language processing (NLP).

## Table of contents
- [Web classification based on website content](#web-classification-based-on-website-content)
  - [Table of contents](#table-of-contents)
  - [Dataset](#dataset)
  - [Experimental setup](#Experimental-setup)
  - [Status](#status)


## Dataset
A public dataset available on Kaggle was used:[ click here](https://www.kaggle.com/datasets/hetulmehta/website-classification).
The dataset was compiled by scraping URLs and categorized into different categories based on the content of the extracted text. The dataset contains 1408 records and 3 attributes, including the target category. In addition, the target class contains 16 different classes, while the other attributes are purely text variables.

## Experimental-setup
* A Python programming language was used in this experiment to classify the webpages using a Jupyter notebook to perform the development. 
* Several text preprocessing techniques were employed to preprocess the dataset, including Lowercase conversion, removing characters that are not letters and punctuation, removing non-English words from NLTK corpus, word toknizing, removing stopwords and word lemmatization, and labeling the categorical target class with the Label Encoder.
*The dataset does not contain any missing values that need to be imputed.
* To train LSVM, SGD, and LR algorithms, direct partitioning of (75:25) with 123 random states was used. 
* A training pipeline was created to fit unigram vectorization with TfidfVectorizer, followed by GridSearchCV with stratified 10-fold cross-validation to determine the optimal hyperparameters.

## Status
Project is: _completed_.
