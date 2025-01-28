EVO Astra Internship Project
Overview
This repository contains the work done during the EVO Astra Internship, where I developed a predictive model to forecast term deposits for clients of Banco de Portugal. The dataset consists of client demographics and marketing campaign data, and the goal was to predict whether a client would subscribe to a term deposit.

Key Highlights
Predictive Model for forecasting term deposits using client demographics and campaign data.
Explored a dataset containing over 45,000 client records.
Achieved 90% accuracy using a Random Forest model.
Evaluated the model using metrics like accuracy, precision, recall, and F1-score, with scores reaching 70%.
Data preprocessing involved handling missing values and feature engineering to improve model performance.
Table of Contents
Project Description
Technologies Used
Data Analysis
Model Development
Results
Setup and Installation
Usage
Contributions
License
Project Description
The goal of this project was to predict whether a client would subscribe to a term deposit based on their demographics and interaction with the marketing campaign. The project involved extensive data exploration, feature engineering, model development, and performance evaluation.

Data Exploration and Preprocessing
Exploring the Dataset: We started by examining the dataset, which contains demographic and contact information about clients who were approached through a marketing campaign. The dataset included columns such as age, job type, marital status, education, and more.
Handling Missing Data: Missing values were identified and handled appropriately, either by filling or excluding them based on the data distribution.
Feature Selection: We assessed all features for relevance to the prediction task, excluding variables like contact duration, which did not significantly improve the model's performance.
Technologies Used
Python 3.8: Programming language used for data analysis and model development.
Pandas: Used for data manipulation and analysis.
NumPy: Used for numerical computations.
Scikit-Learn: Library used for building machine learning models.
Random Forest: The model chosen for classification due to its strong performance.
Matplotlib & Seaborn: For data visualization.
Data Analysis
1. Data Loading and Cleaning
We began by loading the data into a Pandas DataFrame, followed by a thorough examination of missing values, duplicate entries, and data types. Various techniques, including filling missing values and removing outliers, were applied to clean the data.

2. Feature Engineering
The most relevant features for prediction were selected. Data transformation techniques such as one-hot encoding were used to convert categorical variables into numeric representations.

3. Data Visualization
We utilized Seaborn and Matplotlib to visualize key relationships within the data. Heatmaps, pairplots, and bar plots helped us identify patterns and correlations.

Model Development
1. Choosing the Algorithm
We opted for the Random Forest Classifier, which is an ensemble model known for its robustness and high accuracy in classification tasks. It is capable of handling a large number of input variables without overfitting.

2. Training the Model
The model was trained on a train-test split of the dataset. Hyperparameters such as n_estimators and max_depth were tuned to improve performance.

3. Evaluation Metrics
The model was evaluated using the following metrics:

Accuracy: 90%
Precision: 70%
Recall: 70%
F1-score: 70%
These metrics were chosen to evaluate how well the model predicted the outcome of interest: term deposit subscription.

Results
1. Model Performance
The Random Forest model performed excellently with an accuracy of 90%.
The evaluation metrics for precision, recall, and F1-score reached around 70%, indicating balanced performance for both class prediction and classification accuracy.
2. Insights
Certain features such as job type and education had a significant impact on predicting whether a client subscribed to a term deposit.
Excluding the contact duration feature led to a cleaner model with reduced complexity without sacrificing performance.
Setup and Installation
Follow these steps to set up the project on your local machine:

1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/Sahilopl/EVOAstra-Internship-project.git
cd EVOAstra-Internship-project
2. Install Dependencies
Ensure you have Python 3.8 or higher installed. Then, create a virtual environment and install the required packages.

bash
Copy
Edit
python -m venv venv
source venv/bin/activate   # On Windows, use venv\Scripts\activate
pip install -r requirements.txt
3. Running the Code
Once the dependencies are installed, you can run the code for data analysis and model training.

bash
Copy
Edit
python model.py
Usage
This project provides functionality for:

Loading and preprocessing data.
Training a machine learning model on the given dataset.
Evaluating the model using multiple metrics.
Making predictions on new client data for term deposit subscription.
Contributions
If you'd like to contribute to this project, feel free to fork this repository and submit a pull request. Contributions are welcome to improve the model, add new features, or help with documentation.

Fork the repository.
Clone your fork to your local machine.
Create a new branch.
Make your changes and commit them.
Push your changes to your forked repository.
Submit a pull request.
License
This project is licensed under the MIT License. See the LICENSE file for more details.
