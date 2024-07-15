# CodeAlpha_Project_TitanicClassification
This project concerns with the classification of the survived and unsurvived poeple in Tianic incident
# Project Structure
Titanic_data.ipynb: The main Jupyter Notebook containing data loading, preprocessing, model training, and prediction.

# Model and Preprocessing Details
Preprocessing Pipeline

# The preprocessing pipeline includes the following steps:
AgeImputer: Fills missing values in the 'Age' column with the median age.

FeatureEncoder: Encodes categorical features 'Embarked' and 'Sex' using OneHotEncoder.

FeatureDropper: Drops irrelevant features such as 'Embarked', 'Name', 'Ticket', 'Sex', 'Cabin', and any temporary columns.
# Model
The model used is a RandomForestClassifier, tuned using GridSearchCV to find the best hyperparameters.

# Input Features
Pclass: Passenger class (1, 2, or 3)

Sex: Gender of the passenger (male or female)

Age: Age of the passenger

SibSp: Number of siblings/spouses aboard

Parch: Number of parents/children aboard

Fare: Fare paid by the passenger

Embarked: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

# To predict survival for a hypothetical passenger:

Run the get_user_input() function to enter the passenger's details.
Pass the input data to predict_survival() to get the prediction.
The function will return 1 if the passenger would survive, and 0 otherwise.
