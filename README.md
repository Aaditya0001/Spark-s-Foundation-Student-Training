# Sparks-Foundation-Student-Training

## Introduction
This session provided a rigorous, experiential learning framework aimed at equipping participants with advanced competencies in data science and machine learning. This training module emphasized foundational proficiencies in leveraging Jupyter Notebook and deploying supervised learning methodologies. The curriculum was meticulously designed to synthesize theoretical constructs with applied problem-solving, demonstrated through a focused case study employing linear regression as an analytic tool.

## Dependencies
- `numpy`: For numerical computations and array manipulations.
- `pandas`: For data manipulation and analysis.
- `scikit-learn`: For machine learning algorithms and evaluation metrics.
- `Matplotlib`: For data visualization.

```python
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_absolute_error
from sklearn.metrics import mean_squared_error
from sklearn.metrics import r2_score
from sklearn.model_selection import train_test_split
import matplotlib.pyplot as plt
```

## DataPreProcessing and EDA

The dataset contains two columns:
- **Hours**: The number of hours a student studied per day (independent variable).
- **Scores**: The percentage score achieved by the student (dependent variable).
The dataset is small and simple, making it ideal for demonstrating the fundamentals of linear regression. The primary goal is to establish a linear relationship between the Hours and   Scores to predict outcomes based on input values.

EDA: It's is an essential step to understand the dataset and uncover patterns, relationships, and anomalies. The following steps were performed during the analysis:
Following EDA was conducted:
- **Data Inspection**: The dataset was loaded into a Pandas DataFrame. The structure of the dataset (rows, columns, and types) was examined using functions like head(), info(), and describe().
- **Missing Values Check**: Checked for null or missing values using isnull().sum(). he dataset had no missing values, ensuring a clean input for the model.
- **Descriptive Statistics**: Used describe() to calculate key statistics such as mean, median, min, max, and standard deviation for the columns. Observed the range of Hours and Scores to ensure the data is in a reasonable scale.
- **Data Visualization**: Plotted a scatter plot of Hours vs. Scores using Matplotlib to visually examine the relationship. Observed a positive correlation between the two variables, indicating that as study hours increase, the scores also tend to improve.

## Results
The performance of the linear regression model was evaluated using various metrics, yielding the following results:
-**Mean Absolute Error (MAE)**: This metric reflects the average magnitude of errors in the model's predictions, with an average absolute deviation of 0.854 percentage points from the actual scores.
-**Mean Squared Error**: Its value is 0.748. The MSE quantifies the average squared difference between predicted and actual values, indicating a relatively low overall error.
-**R-squared (R²)**: This metric demonstrates that approximately 95.4% of the variance in student scores is explained by the number of study hours, highlighting the model's strong predictive performance.

