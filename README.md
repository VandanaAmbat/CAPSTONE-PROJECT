# Liver-Disease-Prediction

## OBJECTIVE

Statistical Analysis of Liver Disease data for accurately Diagnosing if a person has liver disease or not.

## About the Data set:
This is a machine learning project where we will predict whether a person is suffering from Liver Disease or not. The data set was downloaded from Kaggle. This data set contains 936 liver patient records and 764 non liver patient records. The "Dataset" column is a class label used to divide groups into liver patient (liver disease) or not (no disease). This data set contains 843 male patient records and 857 female patient records.

## Columns:

1. Age
2. Gender
3. BMI
4. AlcoholConsumption
5. Smoking
6. GeneticRisk
7. PhysicalActivity
8. Diabetes
9. Hypertension
10. LiverFunctionTest
11. Diagnosis
    
A binary classification problem statement.

# Project Description:
After loading the dataset the first step was to perform an extensive Exploratory Data Analysis(EDA). Count plot for the target was made to check whether the dataset is balanced or not. It was a balanced dataset. Histograms and scatter plots were were made tp understand the distribution of the data and the correlation distribution. Then a correlation heatmap was plotted to check the correlation between all the independent features. Skweness and Kurtosis were conducted and found out that features like Diabetes and Hypertesnion tends to deviate more from the required values.

The second step was to perform Feature Engneering. Label Encoding was performed on "Gender", where 1 denotes Female and 0 denotes Male. The dataset was divided into independent(X) and dependent(y) features.

The Third step was Model Selection without Hyperparameter Tuning. The dataset was divided into indepenent and dependent features. Train test split was performed for getting the train and test datasets. Logistic Regression, Decision tree, Adaboost,Random Forest Classifier,Gradient Boosting was applied on the training data after testing and Predicton and validaion was performed on the test dataset.

The Fourth step was Feature Selection. Features were studied using different methods like SelectK best, Lasso and RFE. The best results were obtained from SelectKbest and the corresponding features got selected.

The fifth step was to perform Hyperparameter Optimization on our model. GridSearchCV was used after setting a list of parameters. The model with the best parameters was then fitted on the train and test data. Best model was validated using accuracy score.
The final step was to save the model as a pickle file to reuse it again for the Deployment purpose. pickle was used to dump the model at the desired location.

The "Liver Disease Prediction.ipynb" file contains all these informations.
