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
