# Titanic Dataset - Exploratory Data Analysis

## Project Overview

This project performs Exploratory Data Analysis (EDA) on the Titanic dataset.

The goal of this project is to understand the dataset, identify patterns, analyze relationships between variables, and explore factors associated with passenger survival.

## Dataset

The dataset contains information about 891 Titanic passengers and includes 12 columns.

Some important columns are:

- `Survived` - Whether the passenger survived (0 = No, 1 = Yes)
- `Pclass` - Passenger class (1st, 2nd, or 3rd)
- `Name` - Passenger name
- `Sex` - Passenger gender
- `Age` - Passenger age
- `SibSp` - Number of siblings/spouses aboard
- `Parch` - Number of parents/children aboard
- `Fare` - Ticket fare
- `Cabin` - Cabin information
- `Embarked` - Port of embarkation

## Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## EDA Process

The following analyses were performed:

1. Dataset overview
2. Missing value analysis
3. Data type analysis
4. Overall survival analysis
5. Survival by gender
6. Survival by passenger class
7. Age distribution
8. Age vs survival
9. Age group analysis
10. Fare distribution and outlier analysis
11. Family size feature creation
12. Family size vs survival
13. Gender and passenger class analysis
14. Correlation analysis

## Key Findings

### Survival

Out of 891 passengers:

- 342 passengers survived.
- 549 passengers did not survive.

### Gender

The survival rate was:

- Female: 74.20%
- Male: 18.89%

### Passenger Class

The survival rate by passenger class was:

- 1st Class: 62.96%
- 2nd Class: 47.28%
- 3rd Class: 24.24%

### Age

Most passengers with recorded ages were approximately between 20 and 35 years old.

There were 177 missing values in the `Age` column.

### Fare

The fare distribution was strongly right-skewed.

- Mean fare: 32.20
- Median fare: 14.45
- Maximum fare: 512.33

The dataset contains several high-fare observations.

### Family Size

A new `FamilySize` feature was created using:

`FamilySize = SibSp + Parch + 1`

Most passengers were traveling alone.

### Gender and Passenger Class

Survival rates varied considerably across combinations of gender and passenger class.

For example:

- Female, 1st Class: 96.81%
- Female, 2nd Class: 92.11%
- Female, 3rd Class: 50.00%
- Male, 1st Class: 36.89%
- Male, 2nd Class: 15.74%
- Male, 3rd Class: 13.54%

## Missing Values

The dataset contains missing values in:

| Column | Missing Values |
|---|---:|
| Age | 177 |
| Cabin | 687 |
| Embarked | 2 |

## Project Structure

```text
Titanic_EDA/
│
├── Titanic_EDA.ipynb
├── train.csv
└── README.md