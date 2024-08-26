### This dataset is taken from Kaggle.
### This project is made with Python

### Imports
Before you start you should install these requirements on your environment
- pandas
- numpy
- scikit-learn(sklearn)
## Aim of this project:
We have a dataset that includes various tests that are made on a patient and as a result of these test we have our output that shows if the patient has a heart disease or not. This project aims to use machine learning algorithms to give us that output.

## Preprocessing
- MinMaxScaler()
- LabelEncoding(You can use One-hot encoding too. Code contains it.)
 
## Algorithms used
- RandomForestClassifier

# Sonuçlar

                    precision    recall  f1-score   support

               0       0.86      0.83      0.84        29
               1       0.85      0.88      0.86        32

    accuracy                               0.85        61
    macro avg          0.85      0.85      0.85        61
    weighted avg       0.85      0.85      0.85        61
