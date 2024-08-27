# Heart Disease Prediction
This project involves predicting the likelihood of heart disease using a dataset of patient information. The dataset contains various features related to patient health, which are used to train and evaluate a Random Forest Classifier model.

## Dataset
The dataset used is heart.csv, which includes the following columns:

age: Age of the patient
sex: Gender of the patient (1 = male, 0 = female)
cp: Chest pain type
trtbps: Resting blood pressure (in mm Hg)
chol: Serum cholesterol level (in mg/dl)
fbs: Fasting blood sugar (1 = true, 0 = false)
restecg: Resting electrocardiographic results
thalachh: Maximum heart rate achieved
exng: Exercise induced angina (1 = yes, 0 = no)
oldpeak: Depression induced by exercise relative to rest
slp: Slope of the peak exercise ST segment
caa: Number of major vessels colored by fluoroscopy
thall: Thalassemia
output: Heart disease presence (1 = disease, 0 = no disease)

### Preprocessing
Binning: The age feature is converted into categorical bins: 0-20, 20-40, 40-60, 60-100.
Scaling: The features trtbps, chol, and thalachh are scaled to a range of [0, 1] using Min-Max Scaling.
Encoding: The age feature is label encoded for model compatibility.

### Data Splitting
The dataset is split into training, validation, and test sets as follows:
Training set: 60% of the data
Validation set: 20% of the training data
Test set: 20% of the original data

### Model
A Random Forest Classifier is used to predict the presence of heart disease. The model is trained on the training set and evaluated on the test set.

### Evaluation
The model's performance is evaluated using the following metrics:

Classification Report: Provides precision, recall, and F1-score for each class.
Confusion Matrix: Displays the true positives, false positives, true negatives, and false negatives.

Classification Report:

              precision    recall  f1-score   support

           0       0.86      0.83      0.84        29
           1       0.85      0.88      0.86        32

    accuracy                           0.85        61
    macro avg       0.85      0.85      0.85        61
    weighted avg       0.85      0.85      0.85        61
    
Confusion Matrix:
[[24  5]
 [ 4 28]]

### Contributing
Feel free to contribute to this project by submitting issues or pull requests.
