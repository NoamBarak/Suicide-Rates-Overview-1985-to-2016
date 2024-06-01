# Suicide Risk Prediction System for Psychiatrists 👩🏻‍⚕️

![Alt Text](picture.png)


## Introduction
In psychiatry, patients may resist collaboration, leading to potential misdiagnoses.  
Our goal is to aid psychiatrists in assessing suicide risk, utilizing a comprehensive database.  
We offer tools to identify subtle indicators, aiming for improved patient care outcomes.

## Solution
### General Approach
We utilized a dataset from Kaggle containing information about suicides based on objective parameters.   
We omitted certain columns during data processing to avoid bias and excessive computational load.  
Additionally, we experimented with various machine learning models to determine the most effective one for our system.

### Technical Challenges
1. **Data Encoding**: Initially, we performed one-hot encoding, but due to the dataset's diversity, this led to a large number of columns and memory issues. We later adopted a different encoding method to mitigate this problem.
2. **Model Selection**: We initially built neural networks but found them less satisfactory. After consulting with our course instructor, we incorporated external tools like sklearn libraries, which significantly improved our models' success rates.

### Model Comparison
We experimented with several models:
- Linear Regression
- Decision Tree Regression
- Random Forest Regression
- Multilayer Perceptron
- XGBoost Regression

Our results showed that Random Forest Regression performed the best, with XGBoost Regression closely behind.  
However, Random Forest Regression was chosen to avoid overfitting due to a larger disparity between training and test scores.

### Process Description
When a new patient visits a psychiatrist, they input information such as country, year, gender, and age.  
The system then provides objective information, allowing the psychiatrist to assess the patient's risk without relying solely on conversation. The system evaluates all data in the database and assigns a score to each population segment. When a new patient arrives, the system predicts their risk, and the psychiatrist receives an appropriate notification based on the patient's score.

### Additional Evaluation Measures
To enhance usability, we included visual aids such as tables and graphs for psychiatrists, providing additional insights beyond the selected model. These visual aids offer supplementary information about suicide trends across different demographics.

## Summary and Conclusions
Through this project, we explored various relevant models and compared their performance. We aim to assist psychiatrists in diagnosing suicidal tendencies based on statistical data rather than relying solely on verbal communication. Despite challenges, including potential errors in conversation-based assessments, our system provides an additional objective tool for psychiatrists to minimize future suicides and save lives.

