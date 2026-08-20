# Data Validation

## Dataset Overview

| Property | Value |
|----------|-------|
| Source | Customer Churn Dataset |
| Records | 3,333 |
| Features | 20 |
| Target | Churn (Binary) |

## Data Quality Checks

### Completeness
- All records have complete data for all 20 features
- No null values detected

### Accuracy
- Numerical ranges validated against business rules
- Categorical values verified for consistency

### Consistency
- State abbreviations standardized to 2-letter codes
- Plan types consistently labeled (Yes/No)

## Feature Validation

| Feature | Min | Max | Expected Range | Status |
|---------|-----|-----|----------------|--------|
| Account length | 1 | 243 | > 0 | Pass |
| Total day minutes | 0 | 351 | >= 0 | Pass |
| Total day calls | 0 | 165 | >= 0 | Pass |
| Customer service calls | 0 | 9 | >= 0 | Pass |

## Churn Distribution

| Churn | Count | Percentage |
|-------|-------|------------|
| False | 2,850 | 85.5% |
| True | 483 | 14.5% |

## Notes

- Dataset appears to be from a fictional telecom provider
- Geographic distribution covers multiple U.S. states
- Usage patterns show typical telecom customer behavior
