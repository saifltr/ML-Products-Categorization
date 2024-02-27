<h2>Project Overview</h2>

<h4> Cleaning_and_Preprocessing.py </h4>
This project aims to collect product data from various CSV files, perform data cleaning and extraction of relevant information, and save the processed data into a single CSV file. The code is written in Python and utilizes the pandas library for data manipulation and BeautifulSoup for HTML parsing.

<h4>Model_Training.py</h4>
This Python script performs various tasks related to data preprocessing, machine learning model building, and evaluation on a dataset of product descriptions from multiple ecommerce websites.
# Code Overview

This Python script performs various tasks related to data preprocessing, machine learning model building, and evaluation on a dataset of product descriptions from multiple ecommerce websites.

## Model Building and different approaches for training the ML models

### 1. Data Loading and Filtering
- The script loads the dataset from a CSV file named "cleaned_products.csv".
- It filters the dataset based on the spider name to create separate dataframes for each website. This is done to analyze and model data from different sources individually.

### 2. Gender Categorization
- Two approaches are used for gender categorization:
  - The first approach utilizes TF-IDF Vectorizer and Support Vector Classifier (SVC) for gender classification based on product titles.
  - The second approach combines CountVectorizer and SVC for gender classification, considering both product titles and metadata.

### 3. Product Categorization
- Product categories are assigned using TF-IDF Vectorizer and Logistic Regression. 
- The code categorizes products into different categories such as Clothing, Accessories, Electronics, etc., based on their titles.

### 4. Product Categorization with Metadata
- This section incorporates metadata along with product titles for categorization.
- TF-IDF Vectorizer and Support Vector Classifier are employed to categorize products into various categories using both title and metadata information.

### 5. Model for Product Categorization
- A machine learning model is built using Logistic Regression to categorize products into different categories based solely on their titles.
- The model predicts the category of a product based on its title using TF-IDF Vectorizer for feature extraction and Logistic Regression for classification.

<h4>Dependencies</h4>
<p>pandas: For data manipulation and analysis.</p>
<p>BeautifulSoup (bs4): For parsing HTML data.</p>
<p>scikit-learn: For model training</p>
<p>nltk: For natural language processing</p>
