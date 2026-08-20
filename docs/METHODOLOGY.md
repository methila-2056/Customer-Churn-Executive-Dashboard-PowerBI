# Methodology

## Data Analysis Approach

This project follows a structured approach to analyze customer churn:

### 1. Data Understanding
- Dataset: Telecom customer records (3,333 records, 20 features)
- Target variable: Churn (binary: True/False)
- Key predictors: Service calls, plan types, usage patterns

### 2. Data Preparation
- **Missing Values**: No significant missing values in the dataset
- **Data Types**: Appropriate type conversions applied
- **Feature Engineering**: Created calculated columns for analysis

### 3. Exploratory Data Analysis
- Distribution analysis for numerical features
- Correlation analysis between features and churn
- Segment analysis by plan types and geography

### 4. Visualization Design
- KPI cards for at-a-glance metrics
- Geographic heatmap for state-wise analysis
- Bar charts for categorical comparisons
- Scatter plots for correlation analysis

### 5. Insight Generation
- Statistical significance testing
- Pattern identification
- Actionable recommendations

## DAX Measures

Key DAX measures used in the dashboard:

```dax
Total Customers = COUNTROWS(table)
Active Customers = CALCULATE(COUNTROWS(table), table[Churn] = "False")
Churned Customers = CALCULATE(COUNTROWS(table), table[Churn] = "True")
Churn Rate = DIVIDE([Churned Customers], [Total Customers])
Average Monthly Charge = AVERAGE(table[Total day charge])
```
