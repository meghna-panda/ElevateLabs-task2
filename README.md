# ElevateLabs-task2
# Titanic Dataset - Exploratory Data Analysis (EDA)

## Objective
The goal of this project is to perform **Exploratory Data Analysis (EDA)** on the Titanic dataset to understand data distributions, feature relationships, and uncover patterns that could be helpful for machine learning models.

## Tools & Libraries Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Dataset Info
- Dataset: [Titanic Dataset from Kaggle](https://www.kaggle.com/datasets/yasserh/titanic-dataset)
- Rows: 891
- Columns: 12
- Target variable: `Survived` (0 = No, 1 = Yes)

## Tasks Performed
### 1. Data Inspection
- Loaded the dataset using `pandas`
- Viewed basic info using `.info()` and `.describe()`
- Identified missing values using `.isnull().sum()`

### 2. Data Cleaning
- Filled missing `Age` values with mean
- Filled missing `Embarked` values with mode
- Dropped `Cabin` column due to excessive missing data

### 3. Data Visualization
- **Histograms**: To understand distributions of numerical features
- **Boxplot**: To check for outliers in `Age`
- **Correlation Heatmap**: To check feature relationships
- **Pairplot**: To visualize feature interactions
- **Countplots**:
  - `Survived` counts
  - `Pclass` vs `Survived`

### 4. Export
- Saved the cleaned dataset as `cleaned_titanic.csv` for further analysis or ML tasks

## Insights Observed
- Passengers in 1st class had a higher survival rate
- Females had a higher chance of survival than males
- Younger passengers were more likely to survive
- `Pclass`, `Fare`, and `Age` showed correlation with survival

## Files Included
- `Titanic-Dataset.csv` – original dataset
- `eda.ipynb` – Jupyter notebook with EDA
- `cleaned_titanic.csv` – preprocessed dataset
- `README.md` – project description
