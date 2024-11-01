# Salary Prediction using Linear Regression

Welcome to the **Salary Predictor**! This project leverages Linear Regression to predict salaries based on an employee's age, gender, degree, job title, and years of experience. With well-structured data exploration, visualization, feature engineering, and model evaluation, this repository provides a comprehensive look at building a regression model for real-world salary predictions.

## Project Overview
This project uses a dataset of employee salaries to:
- Clean and preprocess the data
- Engineer relevant features for model training
- Train and evaluate a Linear Regression model
- Predict an employee's salary based on specific features

## Key Features
- **Data Preprocessing**: Renaming columns, handling duplicates, and dealing with missing values.
- **Exploratory Data Analysis (EDA)**: Visualization of feature distributions and correlation between variables.
- **Feature Engineering**: Scaling numerical values and encoding categorical variables to optimize model performance.
- **Model Training and Evaluation**: Linear Regression model training with accuracy evaluation metrics, including Mean Absolute Error and R² score.

## Table of Contents
1. [Installation](#installation)
2. [Project Structure](#project-structure)
3. [Data Preprocessing](#data-preprocessing)
4. [Exploratory Data Analysis](#exploratory-data-analysis)
5. [Feature Engineering](#feature-engineering)
6. [Model Development](#model-development)
7. [Future Enhancements](#future-enhancements)

## Installation

Clone this repository:
```bash
git clone https://github.com/yourusername/salary_predictor.git
```

## Project Structure

```markdown
salary_predictor/
└── Employee_salaries.csv      # Dataset used for training the model
├── salary_predictor.ipynb          # Jupyter notebook with data processing and model
├── README.md                       # Project documentation
```

## Data Preprocessing
The initial steps involve:
- Importing libraries such as `pandas`, `numpy`, and `seaborn`
- Reading the dataset
- Renaming columns and handling duplicate records to maintain data integrity

## Exploratory Data Analysis
Through visualizations like histograms, bar charts, and heatmaps, the project investigates relationships between features:
- Distribution of features such as age and salary
- Correlation matrix to understand relationships between numeric variables

## Feature Engineering
The project uses several preprocessing techniques to make the data more suitable for model training:
- **Encoding**: Categorical columns like Gender, Degree, and Job Title are converted to numeric codes.
- **Scaling**: Standardization of numerical features (Age, Experience) to improve model accuracy.

## Model Development
The Linear Regression model is trained using the processed features:
1. Splitting the data into training and testing sets
2. Training the model on training data
3. Predicting salaries for test data
4. Evaluating the model using R² score and Mean Absolute Error

### Model Accuracy
The model achieved an R² score of approximately **(Enter score here)%**, indicating the proportion of variance explained by the model.

### Making Predictions
The model can predict salary based on:
```python
Age = 49
Gender = 0 # Female
Degree = 2 # Ph.D.
Job_title = 22 # Director
Experience = 15

# Input values are scaled before prediction
Emp_salary = model.predict([[Age, Gender, Degree, Job_title, Experience]])
print(f"Predicted Salary: ${Emp_salary[0]:.2f}")
```

## Future Enhancements
Some potential enhancements include:
- Exploring additional machine learning models like Random Forest or Gradient Boosting
- Using hyperparameter tuning for model optimization
- Expanding the dataset to include more demographic or job-related features

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request with any improvements.
