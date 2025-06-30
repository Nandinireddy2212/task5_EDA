# EDA Task 5: Titanic Dataset Analysis

The objective of this task is to perform comprehensive Exploratory Data Analysis (EDA) on the Titanic dataset to uncover meaningful insights and understand the factors that influenced passenger survival. The analysis uses Python-based tools to examine variable distributions, identify missing values and outliers, and explore relationships between features.

## Files Included

- `titanic.csv` → The dataset used for analysis, containing details about Titanic passengers.

- `task5 EDA colab notebook.ipynb` → The Colab notebook containing detailed Python code using Pandas, Matplotlib, and Seaborn for statistical and visual exploration.

- `EDA task5 Report.pdf` → A PDF report summarizing key findings, observations and insights

## Tools and Libraries Used

- **Colab Notebook**
- **Python**
- **Pandas** – For data manipulation and analysis
- **Matplotlib** – For basic plotting and customization
- **Seaborn** – For statistical visualizations

## Summary of Findings

- **Gender** was a key factor in survival. Female passengers had a significantly higher survival rate than males, reflecting evacuation practices that prioritized women and children.

- **Passenger Class (`Pclass`)** played a crucial role. First-class passengers had the highest survival rates, while third-class passengers had the lowest. This indicates socio-economic disparities in safety and access to lifeboats.

- **Fare** was positively correlated with survival. Higher-paying passengers (often in first class) had a better chance of surviving, suggesting that fare acted as a proxy for wealth and cabin location.

- **Age** influenced survival to some extent. Younger passengers, especially children, had better survival odds. Elderly passengers were less likely to survive.

- **Port of Embarkation (`Embarked`)** had an impact. Passengers boarding from Cherbourg (C) had higher survival rates compared to those from Southampton (S) or Queenstown (Q), likely due to a greater proportion of first-class travelers.

- **Family size** (captured through `SibSp` and `Parch`) affected survival. Passengers with small families (1–2 relatives aboard) had better survival outcomes than solo travelers or those with large families.

- **Missing values** were present mainly in the `Cabin` and `Age` columns. While `Cabin` had many missing entries and limited analytical value, missing `Age` values should be imputed to retain this important variable.

- **Outliers** were identified, particularly in the `Fare` column. A few passengers paid extremely high fares (above 500), which could skew the analysis or models without transformation.

- **Correlation analysis** revealed:
  - `Pclass` had a **strong negative correlation** with `Survived`
  - `Fare` showed a **positive correlation** with `Survived`
  - `SibSp` and `Parch` were moderately correlated with each other

- **Visualizations (pairplots, scatter plots)** showed clear clustering:
  - Survivors often belonged to first class, paid higher fares, and were younger or female
  - Non-survivors were primarily males from third class with low fares
