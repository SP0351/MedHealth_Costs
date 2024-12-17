# MedHealth_Costs
The project aims to investigate the quantitative relationship between multiple factors and the medical costs of individuals. It helps understand some of the factors that influence the medical costs and to assess the length to which they affect the individuals.

---
# Medical Cost Analysis Project
Exploring the Relationship Between Health & Personal Factors and Medical Charges

## Project Overview
This project investigates the quantitative relationship between medical costs and various demographic, lifestyle, and health factors such as:

- Age
- Gender
- BMI (Body Mass Index)
- Smoking habits
- Number of children
- Region of residence

The goal is to understand how these factors influence individual medical costs, which can help healthcare providers, insurers, and policymakers make informed decisions to manage costs effectively.

## Data Source
- Kaggle Insurance Dataset
- Per capita income data from World Population Review

## Data Cleaning and Preparation
### 1. Data Loading and Inspection
- The dataset was imported and inspected for structure, column names, and data types.
- Variables include both numerical (age, BMI, charges) and categorical (gender, smoker, region) data.

### 2. Handling Missing Values
- Missing data was identified and handled appropriately to ensure data integrity.
- Imputation techniques were applied where necessary.

### 3. Data Cleaning and Formatting
- Categorical variables (e.g., gender, smoker, and region) were converted into numerical values using dummy encoding:
  - Male: 0, Female: 1
  - Smoker: 0 (No), 1 (Yes)
- Outliers were checked for key numerical variables such as BMI and charges.
- Per capita income data was merged into the main dataset based on the region.

## Exploratory Data Analysis (EDA)
The EDA phase focused on understanding the relationships between key variables and answering the following questions:

- What factors have the most significant impact on medical charges?
- How do age, BMI, and smoking habits interact to influence costs?
- Are there regional or demographic trends in medical expenses?

## Key Visualizations and Insights
- **Distribution Charts**: Visualizations for age, BMI, smoker status, and region were created to analyze variable distributions.
- **Correlation Heatmap**: Highlighted strong correlations between charges and smoker status, BMI, and age.
- **Boxplots**: Compared medical charges across:
  - Regions
  - Gender
  - Smoking status
- **Scatter Plots and Regression**: Explored relationships between medical charges and numerical variables such as age, BMI, and number of children.

## Results and Findings
### Key Drivers of Medical Charges
- **Smoker Status**: Smokers incur significantly higher medical costs compared to non-smokers.
- **BMI**: Higher BMI values are associated with increased charges, especially for smokers.
- **Age**: Older individuals face higher medical costs, with notable increases observed for seniors.

### Interactions
- The interaction between BMI and smoking status revealed that smokers with high BMI incur the highest charges.
- Gender also influenced charges, particularly in older age groups where males had higher costs.

### Regional Differences
- Variations in charges were observed across regions, possibly reflecting differences in healthcare costs and regional incomes.

## Recommendations
- **Preventive Healthcare Initiatives**: Encourage healthy behaviors (e.g., smoking cessation, weight management) to reduce medical costs.
- **Targeted Interventions**: Policies and insurance strategies should focus on high-risk groups (e.g., smokers with high BMI).
- **Data-Driven Pricing Models**: Use findings to inform premium pricing based on demographic and health factors.

## Limitations
- The analysis relied on a limited set of factors. Other variables such as income, chronic diseases, or location-specific healthcare costs were not included.
- Per capita income data reflects regional averages, not individual earnings.

## Tools and Technologies
- **Python**: Data analysis and visualization
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- **Jupyter Notebook**: Code execution and reporting
- **Random Forest & ANOVA**: Statistical modeling and hypothesis testing

## Future Work
- Expand the analysis to include additional factors like chronic health conditions, healthcare access, and time-based trends.
- Incorporate machine learning techniques to predict medical costs with higher accuracy.
