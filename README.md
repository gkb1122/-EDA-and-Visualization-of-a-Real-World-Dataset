Titanic Dataset Cleaning and Analysis
This repository contains a Python-based data analysis project where we clean and explore the Titanic dataset. The dataset is typically used for demonstrating data cleaning techniques, basic statistical analysis, and visualization. This project uses various libraries like Pandas, NumPy, Matplotlib, Seaborn, and Scipy to perform the necessary operations.

Project Overview
The code performs the following operations on the Titanic dataset (test.csv):

Loading and Inspecting Data:

The dataset is uploaded via Google Colab's files.upload() method.
The first few rows are displayed to understand the dataset structure.
Data Cleaning:

Missing Values Handling:
Imputes missing values in the 'Age' and 'Fare' columns with the mean.
Optionally removes rows with missing data (df.dropna()).
Duplicate Data Removal:
Identifies and removes duplicate rows from the dataset.
Outlier Detection:
Identifies outliers in the 'Age' column using the Z-score method.
Specific Row Removal:
Removes a specific row where the PassengerId equals 988.
Exploratory Data Analysis (EDA):

Visualization:
Boxplot: Identifies outliers in the 'Age' column.
Bar Plots: Visualizes the distribution of categorical features (Pclass, Sex, Embarked).
Histograms: Displays the distribution of numerical features (Age, Fare, SibSp, Parch).
Correlation Analysis:
A heatmap visualizes the correlation between numeric variables such as 'Age', 'Fare', 'SibSp', and 'Parch'.
Data Optimization:

Converts categorical columns (Pclass, Sex, Embarked, Cabin, Ticket) into category type for memory efficiency.
Summary of Cleaned Data:

Provides descriptive statistics of the cleaned dataset.
Lists the number of unique values in each categorical column.
Dataset
This project uses the Titanic dataset file, test.csv, which contains information about passengers aboard the Titanic, including features such as Age, Fare, Pclass, Sex, Embarked, and more.

To upload the test.csv dataset in Google Colab, the code uses the following:

python
Copy
uploaded = files.upload()
df = pd.read_csv(next(iter(uploaded)))
You can upload your own version of the Titanic dataset (in CSV format) by using the files.upload() method in Google Colab.

Libraries Used
This project requires the following libraries:

Pandas: For data manipulation and analysis.
NumPy: For numerical operations.
Matplotlib: For visualizations and plotting.
Seaborn: For advanced visualizations.
SciPy: For statistical calculations (Z-score for outlier detection).
Google Colab: For file uploads in Google Colab environment.
To install the necessary libraries (if running locally):
bash
Copy
pip install pandas numpy matplotlib seaborn scipy
Code Overview
Step 1: Data Upload and Inspection
The dataset (test.csv) is uploaded, and the first few rows are printed to inspect the structure.

python
Copy
uploaded = files.upload()
df = pd.read_csv(next(iter(uploaded)))
print(df.head())
Step 2: Data Cleaning
Missing values in the Age and Fare columns are imputed with the mean.
Duplicates are removed.
Outliers in the Age column are detected using the Z-score method.
Step 3: Exploratory Data Analysis (EDA)
Visualizations include:

Boxplot for detecting outliers in the Age column.
Bar plots to visualize the distribution of categorical variables (Pclass, Sex, Embarked).
Histograms for numerical variables (Age, Fare, SibSp, Parch).
A correlation heatmap to analyze the relationships between numerical variables.
Step 4: Data Optimization
Categorical variables (Pclass, Sex, Embarked, Cabin, Ticket) are converted to category type for memory optimization.
Step 5: Summary of Cleaned Data
Descriptive statistics are provided for the cleaned dataset.
The number of unique values for each categorical column is displayed.

