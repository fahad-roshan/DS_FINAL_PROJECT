*Analysis of Reviews on E-Commerce for Women's Apparel

**Project Overview

The project is based on a Women's Clothing E-commerce dataset. Our main goal is to determine the sentiment of reviews and find out if a reviewer like it or not which will be told by reviewing text.

Dataset

The dataset has the following columns.
Unnamed: 0: Index
Image ID: id for image Image URL - URL of the Product
Age: Age of the reviewer
Title: Review title
Review Text: Full review text
Rating: Product rating
Recommended IND: (Rating) 1 if reviewer recommends the product else Writing Mode promptindrical components with homogeneous materials(error probability.toFixed(2));
Positive Feedback Count : Number of positive feedback
Division Name: Product Division
Department Name :Product Department
Type Entity: Class of the product

***Cleaning/Pre-Processing of Data

Dealing with missing values : we have removed all rows containing null values.

Text Preprocessing:

Contractions Fixing : expanded contrations in review texts.
Spelling Correction : Made changes in the spellings.
Tokenization - Split the text into words
Remove Stop Words: Swapped out very common English stop words.
Lemmatization - Words brought into base or root form

Data Analysis

Word Clouds
We created two word clouds to visualize the dominant sentiment words in both positive and negative comments.

Data Splitting
The data was dividied in this ratio -- 90% train,10% test. The split was stratified to keep up the same class ratio in both sets.

Vectorization
Review texts were converted to a document-term matrix with CountVectorizer and min_df = 3.

Data Preprocessing:

Cleaned review text and other features such as Age, Rating, and Positive Feedback Count are used.
Text data is vectorized using CountVectorizer and TfidfVectorizer.
Numerical and categorical features are preprocessed using pipelines.

Model Training & Evaluation:

Models used include Naive Bayes, Linear SVM, k-Nearest Neighbors, and Logistic Regression.
Performance metrics like accuracy, precision, recall, and F1-score are calculated for each model.
Confusion matrices and learning curves are plotted for a visual understanding of the models' performances.
Feature Engineering:

Text data is transformed using CountVectorizer and TfidfVectorizer.
Numerical and categorical features are processed using StandardScaler and OneHotEncoder.
Prediction:

After training, the models predict the sentiment of new reviews.
The results are used to identify which department has the most and least positive reviews.
Installation Instructions
Dependencies

pip install pandas numpy matplotlib seaborn scikit-learn wordcloud
Running the Code
Data Preparation:

The dataset should be loaded into a DataFrame named clothing_data.
Additional features such as 'Cleaned Review Text' and 'Recommended IND' should be present.
Model Training and Evaluation:

Run the code to train models, evaluate their performance, and generate learning curves and confusion matrices.
Predictions:

Input new review text to predict whether it would recommend the product or not.
Department Analysis:

After prediction, the code identifies the departments with the most and least positive reviews.

Files
clothing_data.csv: Input dataset containing reviews and features.
model_training.py: Python script for training, evaluating, and comparing models.
preprocessing.py: Script for preprocessing the dataset.
prediction.py: Script for making predictions on new data.
department_analysis.py: Script to analyze department-wise positive reviews.

Results
The Logistic Regression model showed promising results with the following evaluation metrics:

Accuracy: 0.87
Precision: 0.88
Recall: 0.87
F1-Score: 0.87
Most Positive Department: Dresses

Least Positive Department: Intimate



