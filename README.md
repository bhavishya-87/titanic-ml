# Titanic Survival Prediction
![Running GIF](https://camo.githubusercontent.com/1140a4f2ffe1d7d5432df78421909e56c97909423568e609983ec3d4fbcb0b22/68747470733a2f2f726561646d652d747970696e672d7376672e6865726f6b756170702e636f6d3f666f6e743d4f72626974726f6e2673697a653d343026636f6c6f723d253233373941353030266865696768743d3637266475726174696f6e3d333030302663656e7465723d74727565266c696e65733d254630253946253835254236254630253946253836253831254630253946253835254234254630253946253835254234254630253946253836253833254630253946253835254238254630253946253835254244254630253946253835254236254630253946253836253832)
## Overview
This project aims to predict the survival of passengers aboard the Titanic using machine learning techniques. The dataset used in this project is named "titanic_train.csv" and contains various attributes of passengers, including whether they survived or not. We will employ the Logistic Regression algorithm to create a predictive model for passenger survival.

## Libraries Used
The code utilizes the following Python libraries:
- Pandas: For data manipulation and analysis.
- Seaborn: For data visualization.
- Scikit-Learn (sklearn): For machine learning tools and evaluation metrics.
- NumPy: For numerical operations.

## Code Workflow
The code performs the following steps:

1. **Data Loading:** Loads the Titanic dataset from the "titanic_train.csv" file using Pandas.

2. **Data Exploration:** Displays information about the dataset using `data.info()`, showing the data types and missing values.

3. **Data Preprocessing:**
   - Selects relevant features ('Pclass', 'Sex', 'Age', 'SibSp', 'Parch', 'Embarked') and the target variable ('Survived').
   - Visualizes data using Seaborn countplots for categorical features like 'Sex', 'Pclass', 'SibSp', 'Parch', and their relationship with survival.

4. **Data Cleaning:** Removes unnecessary columns ('PassengerId', 'Ticket', 'Fare', 'Parch', 'Name', 'Cabin').

5. **Missing Age Imputation:**
   - Calculates the mean age for passengers in each Pclass (1st, 2nd, and 3rd).
   - Fills missing age values with the corresponding class's mean age.

6. **One-Hot Encoding:**
   - Converts categorical variables ('Pclass', 'Sex', 'SibSp', 'Embarked') into binary (dummy) variables using Pandas' `pd.get_dummies`.

7. **Model Training:**
   - Splits the data into training and testing sets using `train_test_split`.
   - Initializes a Logistic Regression model and trains it on the training data.

8. **Model Evaluation:**
   - Calculates the coefficients and intercept of the trained Logistic Regression model.
   - Uses a confusion matrix from Scikit-Learn to evaluate the model's performance.

## Usage
To use this code for Titanic survival prediction, follow these steps:

1. Ensure you have the required libraries installed: Pandas, Seaborn, Scikit-Learn, and NumPy.

2. Place the "titanic_train.csv" dataset file in the same directory as the code.

3. Run the code step by step or in its entirety.

4. Review the confusion matrix and model evaluation results to assess the predictive performance of the Logistic Regression model.

5. Modify the code as needed for further analysis or to apply different machine learning algorithms.

Feel free to explore and adapt this code for your specific needs in Titanic survival prediction.
![Running GIF](  https://raw.githubusercontent.com/trinib/trinib/82213791fa9ff58d3ca768ddd6de2489ec23ffca/images/footer.svg)
