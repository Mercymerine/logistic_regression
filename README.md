# Logistic Regression
# Titanic Survival Analysis
This project analyzes the Titanic dataset to predict passenger survival using logistic regression. The analysis explores various factors that influenced the likelihood of survival during the tragic sinking of the Titanic.

### Table of Contents
Overview

Dataset

Data Preprocessing

Data Analysis

Modeling

Technologies Used

### Overview
The Titanic was a British passenger liner that sank after hitting an iceberg during its maiden voyage in April 1912. This project aims to analyze the factors affecting survival rates among the passengers. The dataset includes various attributes such as passenger class, gender, age, and fare paid, which are used to build a predictive model.

### Dataset
The dataset used in this project contains the following columns:

PassengerId: Unique ID number assigned to each passenger.
Survived: Survival status (1 = survived, 0 = did not survive).
Pclass: Ticket class (1 = First Class, 2 = Second Class, 3 = Third Class).
Name: Full name of the passenger.
Sex: Gender of the passenger (male or female).
Age: Age of the passenger (some values may be missing).
SibSp: Number of siblings/spouses aboard.
Parch: Number of parents/children aboard.
Ticket: Ticket number assigned to the passenger.
Fare: Amount paid for the ticket.
Cabin: Cabin number assigned to the passenger (may be missing).
Embarked: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).

### Data Preprocessing
Loading the Data: The dataset is loaded into a pandas DataFrame.
Handling Missing Values: Missing values are identified and handled appropriately:
The 'Age' column is filled with the mean age.
The 'Embarked' column is filled with the mode.
Data Cleaning: Unnecessary columns such as 'PassengerId', 'Name', 'Cabin', and 'Ticket' are dropped for analysis.
Encoding Categorical Variables: The 'Survived', 'Sex', and 'Embarked' columns are encoded to facilitate modeling.

### Data Analysis
Histograms are plotted to visualize the distribution of age and fare.
Count plots are generated to compare survival rates and embarkation points.
A correlation heatmap is created to identify relationships between variables.
Boxplots and scatterplots are used to explore the influence of passenger class and age on survival.

### Modeling
Logistic regression is used to predict survival based on the features available in the dataset. The following steps are performed:

Data Splitting: The dataset is split into training and testing sets (80% training, 20% testing).
Model Training: A logistic regression model is trained on the training set.
Model Evaluation: Cross-validation is employed to evaluate the model's performance using log-loss as the scoring metric.

##### Results
The mean log-likelihood (log-loss) of the logistic regression model is calculated to assess its predictive performance.

### Technologies Used
Programming Language: Python
Libraries:
pandas for data manipulation
numpy for numerical operations
seaborn and matplotlib for data visualization
scikit-learn for machine learning

Recommendations for Im
