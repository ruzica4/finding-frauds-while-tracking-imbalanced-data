# finding-frauds-while-tracking-imbalanced-data
## Repository for the course project of Artificial Inteligence

This project uses Lending_club_loan_data.csv data to predict whether a loan will be paid or charged-off. 

LendingClub is a peer-to-peer lending company, meaning that it allows individuals or businesses to lend money through online services that match them with borrowers. More information on the LendingClub can be found [here](https://en.wikipedia.org/wiki/LendingClub#Overview).

This repository contains the following files:
* Data_cleaning.ipynb
* Feature_engineering_and_modeling.ipynb

In case .ipynb files are too large to be rendered, online tool, [nbviewer](https://nbviewer.org/) can be used.  
I have used Azure Synapse Analytics for this project, because the Lending_club_loan_data.csv file was very large in size (1.7GB).  
Lending_club_loan_data.csv dataset can be downloaded from [this](https://www.kaggle.com/datasets/wordsforthewise/lending-club) link.

## Short description

#### Data_cleaning.ipynb notebook
* Unnecessary features (columns) have been removed and the feature space has been reduced from 151 to 24
* There is a graph/histogram representation for each considered feature
* Cleaned data is stored in the Cleaned_data.csv file and contains 1270217 rows (dropped down from 2260701 rows)

#### Feature_engineering_and_modeling.ipynb
* The mean -strategy imputer was used to fill in the missing values
* Features were scaled using MinMaxScaler
* Categorical features were encoded
* Encoded, scaled and imputed data was stored in the Encoded_data.csv file
* For prediction, I used the following classifiers: XGBClassifier, RandomForestClassifier and DecisionTreeClassifier
