# Heart Disease Prediction Model

A machine learning project that predicts whether a patient has a healthy or defective heart based on medical attributes.

## Overview

This project uses patient medical data to implement a logistic regression model to predict heart condition. It achieves approximately 82% accuracy on test dataset, making it a reliable tool for preliminary heart health assessment.

## Dataset

The model uses a dataset with the following features:
 
1. **age**: Age of the patient (Numeric).  
2. **sex**: Gender of the patient. Values: 1 = male, 0 = female.  
3. **cp**: Chest pain type. Values: 0 = Typical angina, 1 = Atypical angina, 2 = Non-anginal pain, 3 = Asymptomatic.  
4. **trestbps**: Resting Blood Pressure (in mm Hg) (Numeric).  
5. **chol**: Serum Cholesterol level (in mg/dl) (Numeric).  
6. **fbs**: Fasting blood sugar > 120 mg/dl. Values: 1 = true, 0 = false.  
7. **restecg**: Resting electrocardiographic results. Values: 0 = Normal, 1 = ST-T wave abnormality, 2 = Left ventricular hypertrophy.  
8. **thalach**: Maximum heart rate achieved (Numeric).  
9. **exang**: Exercise-induced angina. Values: 1 = yes, 0 = no.  
10. **oldpeak**: ST depression induced by exercise relative to rest (Numeric).  
11. **slope**: Slope of the peak exercise ST segment. Values: 0 = Upsloping, 1 = Flat, 2 = Downsloping.  
12. **ca**: Number of major vessels (0-3) colored by fluoroscopy. Values: 0, 1, 2, 3.  
13. **thal**: Thalassemia types. Values: 1 = Normal, 2 = Fixed defect, 3 = Reversible defect.  
14. **target**: Outcome variable (presence of heart disease). Values: 1 = Defective heart, 0 = Healthy heart.  


## Project Structure

- `myfirstproject_heart_disease_prediction.ipynb`: Jupyter Notebook file containing the entire workflow
- `data.csv`: Dataset with medical attributes

## Technical Implementation

1. **Data Processing**
   - Loading data from CSV
   - Exploratory data analysis
   - Checking for missing values
   - Statistical description of the dataset

2. **Model Development**
   - Feature and target separation
   - Train-test split (80% training, 20% testing)
   - Logistic regression model training

3. **Evaluation**
   - Accuracy measurement on training and test data
   - Prediction system for individual patient data

## Usage

1. **Clone the repository**
   ```
   git clone https://github.com/Killua2026/machineLearningprojects/disease-prediction.git
   cd heart-disease-prediction
   ```

2. **Install dependencies**
   ```
   pip install -r requirements.txt
   ```

3. **Change the file path in Jupyter Notebook according to suit the name and location of the dataset**
   ```
   heart_data = pd.read_csv(r\"disease-prediction/data/raw/data.csv\")
   ```

4. **Run all the cells in the jupyter notebook**
   
5. **Making predictions for new patients using input data**
   
   You can predict heart health status for a new patient using either a pandas DataFrame:
   ```python
   input_data = (41,0,1,130,204,0,0,172,0,1.4,2,0,2)
   feature_names = X_train.columns
   input_data_df = pd.DataFrame([input_data], columns=feature_names)
   prediction = model.predict(input_data_df)
   ```
   
   Or using a numpy array:
   ```python
   input_data = (58,1,0,114,318,0,2,140,0,4.4,0,3,1)
   input_data_as_numpy_array = np.asarray(input_data)
   input_data_reshaped = input_data_as_numpy_array.reshape(1,-1)
   prediction = model.predict(input_data_reshaped)
   ```

## Model Performance

- Training data accuracy: ~ approximately 85%
- Test data accuracy: ~ approximately 82%



## Contact
iobi.2301688.stu.cu.edu.ng
