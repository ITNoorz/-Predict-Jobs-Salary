Project: Salary Prediction using Machine Learning
Overview
In this project, we will use a dataset of job listings to predict the salary for a given job. The dataset contains information such as the job title, description, required skills, and experience, as well as the location of the job and the company that is hiring.

We will use a combination of data preprocessing, feature engineering, and machine learning algorithms to build a model that can accurately predict the salary for a given job.

Dataset
The dataset for this project is called "jobs_train.csv" and is stored in a Google Drive folder. We will use the pandas library to read the dataset into a DataFrame.
VIP Note:

The visualization details and images for this project can be found in the Jupyter notebook notebook.ipynb.

The dataset used in this project, jobs_train.csv, can be found in my Google Drive at the following link:

https://drive.google.com/drive/folders/19EowB2aNrpUPf3rJ5zdSZnw_CZXXGz6z


Please make sure to mount your Google Drive and navigate to the correct folder to access the dataset.
The dataset contains the following columns:

jobId: a unique identifier for each job listing
companyId: a unique identifier for the company that is hiring
jobTitle: the title of the job
jobType: the type of job (e.g. full-time, part-time, internship)
degree: the level of education required for the job (e.g. bachelor's, master's, PhD)
major: the field of study required for the job (e.g. computer science, business)
industry: the industry that the job is in (e.g. technology, finance)
yearsExperience: the number of years of experience required for the job
milesFromMetropolis: the distance from the job location to the nearest metropolitan area
salary: the salary for the job (in USD)
Data Preprocessing
We will perform the following data preprocessing steps:

Remove unwanted characters from the jobId column to convert it from object to float datatype.
Convert the jobId, yearsExperience, salary, and milesFromMetropolis columns from object to float datatype.
Check for duplicate and null values in the dataset.
Remove any duplicate or null values from the dataset.
Use the LabelEncoder class from the scikit-learn library to encode the jobType, degree, major, and industry columns as numerical values.
Data Visualization
We will perform the following data visualization:

Job Types Count
Top Ten Highest Salaries by jobType
Mean Salary Grouped by jobType
Major Count
Top Ten Highest Salaries by Major
Mean Salary Grouped by Major
Degree Count
Top Ten Highest Salaries by Degree
Mean Salary Grouped by Degree
Industry Count
Top Ten Highest Salaries by Industry
Mean Salary Grouped by Industry
Scatter plot between yearsExperience and salary
Box plot for salary, yearsExperience and milesFromMetropolis
Correlation heatmap to show the correlation between columns
Modeling
We will use the following machine learning algorithms to build our model:

XGBoost
LightGBM
Linear Regression
We will split the dataset into training and testing sets, with 80% of the data used for training and 20% used for testing. We will use the mean squared error (MSE) metric to evaluate the performance of our model.

We will also save the best model using pickle.

Feature Importance
We will also plot feature importance for each model.

Deep Learning Model
We will also build deep learning model and plot feature importance.

Second Section
In the second section, we will use the trained model to make predictions on a new dataset. We will load the saved model from disk, preprocess the new dataset in the same way as the training data, and then use the model to make predictions. We will then print the predictions to the console.

We will use the following function to make predictions on a new dataset:

predict_from_csv(csv_path, model_path)

where csv_path is the path to the new dataset (in CSV format) and model_path is the path to the saved model (in pickle format).

The function will load the saved model from disk, preprocess the new dataset in the same way as the training data, and then use the model to make predictions. The function will then print the predictions to the console.
