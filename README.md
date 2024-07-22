# Student Performance Predictor
The main objective of this project is to develop a predictive model that can forecast the performance of students in their mathematics exam. This project is solely for the purpose of learning.

## Problem Statement
This end to end Machine Learning project helps in predicting the Maths Score of a student using the following 7 parameters:-

1. Gender
2. Race or Ethnicity
3. Parental level of Education
4. Lunch Type
5. Test Preparation Course
6. Writing score (Out of 100)
7. Reading Score (Out of 100)

## Steps to followed for this ML project
- Understand the problem statement
- Dataset
- Perform data checks
- Exploratory Data Analysis
- Data Pre-Processing
- Model Training
- Selecting the best model

## Steps to be followed until Deployment
- Setup a github Repository and a local environment
- Setup a Project Structure
- Setup Logging and Exception handling files
- Understand the problem statement
- Perform Exploratory Data Analysis and Model Training
- Perform Data Ingestion
- Perform Data Transformation using Pipelines
- Perform Model Training and Model Evaluating Component
- Undergo Model Hyper Parameter Training
- Create Prediction Pipeline using Flask Webapp

## Dataset Details
- Source:- https://www.kaggle.com/datasets/spscientist/students-performance-in-exams?datasetId=74977

## Dataset Information
- gender : sex of students -> (Male/female)
- race/ethnicity : ethnicity of students -> (Group A, B,C, D,E)
- parental level of education : parents' final education ->(bachelor's degree, some college, master's degree, associate's degree, high school)
- lunch : having lunch before test (standard or free/reduced)
- test preparation course : complete or not complete before test
- math score (To be predicted)
- reading score (out of 100)
- writing score (out of 100)

## Data Checks Performed
- Missing values
- Duplicates
- data type
- the number of unique values of each column
- statistics of data set
- various categories present in the different categorical column

## Exploratory Data Analysis (EDA)
- Find more details in the [EDA](notebook/EDA.ipynb) and [Model Training](notebook/Model_Training.ipynb)

## Conclusions from EDA
- Student's Performance is related with lunch, race, parental level education
- Females lead in pass percentage and also are top-scorers
- Student's Performance is not much related with test preparation course
- Finishing preparation course is benefitial.

## Models used for Training
- Linear Regression
- Lasso
- Ridge
- K-Neighbours Regressor
- Decision Tree
- Random Forest Regressor
- XGB Regressor
- CatBoosting Regressor
- AdaBoost Regressor

## Run this project locally on your computer
Clone this project 

```bash
git clone https://github.com/SwarnavaBanerjee24/student-performance-predictor.git
```

After setting up environment and installing packages Run

```bash
  python application.py
```
## Screenshots
### Home page
![Screenshot 2024-07-06 203324](https://github.com/SwarnavaBanerjee24/ml-projects/blob/main/templates/Screenshot%202024-07-06%20203324.png)

### Before Prediction
![Screenshot 2024-07-06 211422](https://github.com/SwarnavaBanerjee24/ml-projects/blob/main/templates/Screenshot%202024-07-06%20211422.png)

### After Prediction
![Screenshot 2024-07-06 211430](https://github.com/SwarnavaBanerjee24/ml-projects/blob/main/templates/Screenshot%202024-07-06%20211430.png)

## Deployment using CI-CD pipeline using Amazon EC2 Instance
1. Setup Docker build
2. Setup Github workflow
3. Setup IAM user in AWS
