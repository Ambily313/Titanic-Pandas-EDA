# Titanic Dataset: EDA and Data Cleaning with Pandas


This project performs a complete exploratory data analysis (EDA) and data cleaning pipeline on the classic **Titanic dataset** using **pandas**. The dataset contains demographic and travel information for passengers on the Titanic, and the goal is to explore patterns related to survival, fare, class, and more.

---

##  Project Objectives

- Explore the structure and summary of the dataset.
- Identify and handle missing values.
- Apply filtering, sorting, and ranking operations.
- Perform group-wise aggregation and analysis.
- Engineer new features (e.g., Family Size, Age Group).
- Prepare data for further analysis or modeling.

---

## 📂 Dataset

- **Source**: [Titanic-data-github](https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv)


---

##  Features Overview

| Column        | Description                               |
|---------------|-------------------------------------------|
| PassengerId   | Unique ID for each passenger              |
| Survived      | 0 = No, 1 = Yes                           |
| Pclass        | Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd)|
| Name          | Name of the passenger                     |
| Sex           | Gender                                    |
| Age           | Age in years                              |
| SibSp         | Siblings/spouses aboard                   |
| Parch         | Parents/children aboard                   |
| Ticket        | Ticket number                             |
| Fare          | Ticket fare                               |
| Cabin         | Cabin number                              |
| Embarked      | Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton) |

---

## ✅ Tasks Performed

### 1.  Data Loading & Inspection
- Loaded CSV using pandas
- Viewed top and bottom rows
- Checked shape, column names, data types
- Identified missing values

### 2.  Filtering & Selection
- Selected subsets of passengers (e.g., by age, gender, fare)
- Used `loc`, `iloc`, and boolean masking
- Filtered passengers by port, cabin availability, etc.

### 3.  Sorting & Ranking
- Sorted by age, fare, and class
- Ranked top-paying passengers

### 4.  Aggregation & Statistics
- Used `.groupby()` to analyze survival rate by gender and class
- Explored fare, age distributions
- Counted unique tickets and embarkations

### 5.  Data Cleaning
- Filled missing age with median
- Imputed most common embarked value
- Dropped `Cabin` due to heavy missingness
- Cleaned column names and standardized text case
- Renamed columns for clarity

### 6. Feature Engineering
- `FamilySize = SibSp + Parch + 1`
- `IsMinor` based on age
- Encoded `Sex` to numeric
- Normalized fare column
- Binned age into child/teen/adult/senior groups

### 7.  Advanced Filtering
- Passengers with names containing "Smith"
- Ticket prefixes, age ranges, embark locations
- Checked for outliers (age > 80)

---

### 8. Visualizations 
- Survival Count by Gender
- Age Distribution of Passengers
- Survival Count by Passenger Class
- Fare Distribution by Class
- Survival by Embarkation Port (Heatmap)
- Age vs Fare by Survival (Scatterplot)

---

##  Tools & Libraries

- `pandas`
- `numpy`
- `matplotlib` / `seaborn` 
- Jupyter Notebook

---




