# Liver-Disease-Prediction

## OBJECTIVE

Statistical Analysis of Liver Disease data for accurately Diagnosing if a person has liver disease or not.

## About the Data set:
This is a machine learning project where we will predict whether a person is suffering from Liver Disease or not. The data set was downloaded from Kaggle. This data set contains 416 liver patient records and 167 non liver patient records collected from North East of Andhra Pradesh, India. The "Dataset" column is a class label used to divide groups into liver patient (liver disease) or not (no disease). This data set contains 441 male patient records and 142 female patient records.

## Columns:

Age of the patient
Gender of the patient
Total Bilirubin
Direct Bilirubin
Alkaline Phosphotase
Alamine Aminotransferase
Aspartate Aminotransferase
Total Protiens
Albumin
Albumin and Globulin Ratio
Dataset: field used to split the data into two sets (patient with liver disease, or no disease)
A binary classification problem statement.

# Project Description:
After loading the dataset("indian_liver_patient.csv") the first step was to perform an extensive Exploratory Data Analysis(EDA). Count plos for the target was made to check whether the dataset is balanced or not. It was a balanced dataset. Factor plots were created for the features "Age , "Gender", "Dataset"(target). Histograms and scatter plots were were made tp understand the distribution of the data and the correlation distribution. Then a correlation heatmap was plotted to check the correlation between all the independent features. Jointplot was made for "Total_Protiens" and "Albumin".

The second step was to perform Feature Engneering. Missing values of the feature "Albumin_and_Globulin_Ratio" was handled by replacing it by its mean. Label Encoding was performed on "Gender", where 1 denotes male and 0 denotes female. Any other nan values was replaced with 0.94 (from domain knowledge). The dataset was divided into independent(X) and dependent(y) features.

The third step was Feature Selection. Features were selected manually based on domain knowledge. 'Total_Bilirubin', 'Direct_Bilirubin', 'Alkaline_Phosphotase', 'Alamine_Aminotransferase', 'Total_Protiens', 'Albumin', 'Albumin_and_Globulin_Ratio' were the features that got selected.

The Forth step was Model Building. The dataset was divided into indepenent and dependent features. Train test split was performed for getting the train and test datasets. Random Forest Classifier was applied on the training data after testing with other Machine Learning algorithmns. Predicton and validaion was performed on the test dataset.

The fifth step was to perform Hyperparameter Optimization on our model. RandomizedSearchCV was used after setting a list of parameters. The model with the best parameters was then fitted on the train and test data. Best model was validated using accuracy score, confusion matrix and classification report. False positives and false negaives were reduced.

The final step was to save the model as a pickle file to reuse it again for the Deployment purpose. Joblib was used to dump the model at the desired location.

The "Liver Disease Prediction.ipynb" file contains all these informations.

# Limitations

# Conclusions

# future Work
