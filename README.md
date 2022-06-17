# finding-frauds-while-tracking-imbalanced-data
Repository for the course project of Artificial Inteligence

This repository contains the following files:
Data_cleaning.ipynb
Cleaned_data.csv
Feature_engineering_and_modeling.ipynb
Encoded_data.csv

In case .ipynb files are too large to be rendered, online tool, [nbviewer](https://nbviewer.org/) can be used for the rendering.

In the Data_cleaning.ipinb notebook, I removed the features (columns) and reduced the feature space from 151 to 24. For each feature considered, there is a graph / histogram display. The initial dataset, Lending_club_loan_data.csv (downloaded from this link https://www.kaggle.com/datasets/wordsforthewise/lending-club) contained 2260701 rows. The cleaned data is saved in the file Cleaned_data.csv and has 1270217 rows.


In Feature_engineering_and_modeling.ipynb notebook, missing values have been filled. Also, categorical features have been encoded.
Models XGBClassifier, RandomForestClassifier and DecisionTreeClassifier have been trained on the encoded data.

Encoded_data.csv contains cleaned, imputed and encoded data.
