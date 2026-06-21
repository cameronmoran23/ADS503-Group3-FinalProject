# Predictive Modeling for Bank Transaction Fraud Detection

**ADS503: Applied Predictive Modeling - Group 3**

## Team Members/Contributors
- Cameron Moran
- Brandon Rodriguez-Andrade
- Jacob Moore

### Downloading the Dataset
The dataset is too large to be stored directly on GitHub, so it is not included in the repository. Each team member needs to download it locally before running the notebook:

1. Go to the dataset page on Kaggle: https://www.kaggle.com/datasets/nafiulislam490/bank-transaction-fraud-detection-dataset
2. Sign in (or create a free Kaggle account if you don't have one).
3. Click the "Download" button to download the dataset as a '.zip' file.
4. Unzip the downloaded file.
5. Rename the extracted '.csv' file to 'bank_fraud.csv' and place it directly in the root of the project folder (the same folder as Final_Project_Notebook-Team3.rmd):
6. Make sure the file is named exactly 'bank_fraud.csv'

## Installation
To use this project, first clone the repository on your device using the command below:

```bash
git init
git clone https://github.com/cameronmoran23/ADS503-Group3-FinalProject
```

## Project Objective/Goals:
This project applies predictive modeling techniques to detect fraudulent bank transactions using a large-scale synthetic data set of one million transactions. The team conducts exploratory data analysis, addresses significant class imbalance using re sampling techniques, and builds and compares multiple classification models. Model performance is evaluated using AUC-ROC, precision, recall, and F1-score.

### Methods Used (Will add later)
- Exploratory Data Analysis: distributions, correlations, and relationship between predictors and the target variables
-Data pre-processing and cleaning
- Resampling Techniques to address class imbalance
- Building and comparing multiple classification models
- Model evaluation using AUC-ROC, precision, recall, and F1-score

### Technologies
- R
- R Studio
- Visual Studio Code

## Project Description
The dataset is sourced from kaggle (Bank Transaction Fraud Detection Dataest), containing 1,000,000 transaction records. There are 26 variables, with the target variable being a binary attribute 'is_fraud', indicating whether a transaction is fraudulent.

### Pre-processing
- No missing values were found in the dataset, since it is synthetic — no imputation or row dropping was needed.
- Dropped the 'fraud_type column, keeping 'is_fraud' as the sole target variable.
- Converted 'is_fraud' to a factor for classification.
- Subsetted the data into 1%, 5%, 10%, 25%, and 50% samples to manage long training times on the full dataset (see Challenges Faced below).
- For modeling, predictors were centered and scaled; PCA may also be applied.


### Modeling (ADD LATER)

### Challenges faced:
- The dataset is 1 million rows by 26 columns. Since the dataset is so large, we ran into long wait times when training models. To address this, we created smaller subsets of the data (1%, 5%, 10%, 25%, 50%) to train and compare models on before scaling up.

## Acknowledgements
- Professor: Dr. Ebrahim Tarshizi, University of San Diego
- ADS-503: Applied Predictive Modeling, University of San Diego
- Kaggle - Bank Transaction Fraud Detection Dataset