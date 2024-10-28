# Lung Cancer Prediction using CSV Data

This project was developed for the **CSE422 (Artificial Intelligence)** course at **BRAC University**. The aim is to predict the likelihood of lung cancer using various health and lifestyle indicators.

Check out the project on my [GitHub Repository](https://github.com/ShakeefAhmedRakin/LungCancerPrediction).

## Dataset Overview

The lung cancer dataset comprises 1,000 patient records, each containing various health and lifestyle indicators relevant to lung cancer diagnosis.

### Lung Cancer Dataset Structure:
- **Patient Id**: Unique identifier for each patient.
- **Age**: Age of the patient (in years).
- **Gender**: Gender of the patient.
- **Air Pollution**: Level of air pollution exposure.
- **Alcohol use**: Frequency of alcohol consumption.
- **Dust Allergy**: Presence of dust allergy.
- **Occupational Hazards**: Exposure to workplace hazards.
- **Genetic Risk**: Genetic predisposition to lung cancer.
- **Chronic Lung Disease**: History of chronic lung disease.
- **Balanced Diet**: Indicator of diet quality.
- **Obesity**: Body mass index.
- **Smoking**: Smoking status.
- **Passive Smoker**: Exposure to secondhand smoke.
- **Chest Pain**: Indicator of chest pain.
- **Coughing of Blood**: Indicator of coughing blood.
- **Fatigue**: Indicator of fatigue.
- **Weight Loss**: Significant weight loss history.
- **Shortness of Breath**: Indicator of shortness of breath.
- **Wheezing**: Indicator of wheezing.
- **Clubbing of Finger Nails**: Indicator of nail clubbing.
- **Frequent Cold**: Indicator of frequent colds.
- **Dry Cough**: Indicator of a dry cough.
- **Snoring**: Indicator of snoring.
- **Level**: Class of lung cancer risk.
- **Result**: Outcome of the diagnosis.

### Script For Introducing NULL Values

Initially, the dataset had no null values or repeating columns. A Python script was created to introduce null values and add two repeating columns for learning data preprocessing techniques.

![Script for Introducing NULL Values](https://raw.githubusercontent.com/ShakeefAhmedRakin/LungCancerPrediction/refs/heads/main/script%20for%20inserting%20null%20values.PNG)

## Data Preprocessing

After loading the dataset, the following steps were taken:
- Introduced artificial null values and two repeating columns for learning preprocessing techniques.
- Utilized imputation (strategy = mean) from sklearn to handle null values.
- Mapped categorical features like Gender and Level to numerical values for analysis.
- Dropped less impactful features, including Genetic Risk and Occupational Hazards, based on correlation analysis.
- Scaled the dataset using MinMaxScaler from sklearn and split it into 75% training and 25% testing sets while keeping both the unscaled and scaled variants.

## Model Training and Evaluation

Various models were trained and evaluated based on their performance on both the scaled and unscaled data:
- Decision Tree
- Naive Bayes
- Random Forest
- Support Vector Machine
- Grid Search

### Evaluation Metrics:
Models were evaluated based on precision, recall, F1-score, support, and accuracy, with confusion matrices visualized using seaborn heatmaps.

## Things I Learned

Throughout this project, I gained valuable insights into:
- Data preprocessing techniques for handling missing values.
- Feature selection and its impact on model performance.
- Implementing various machine learning algorithms for classification tasks.
- Evaluating model performance using different metrics.
- Visualizing data and model results for better understanding.

## Citations

The dataset collected from the following works:
- [Lung Cancer Dataset on Kaggle](https://www.kaggle.com/datasets/thedevastator/cancer-patients-and-air-pollution-a-new-link)
