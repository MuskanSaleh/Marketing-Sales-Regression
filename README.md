# Marketing-Sales-Regression

A linear regression analysis on marketing sales data, exploring the impact of radio promotion budgets on sales. Implemented Ordinary Least Squares (OLS) and checked model assumptions, including linearity, normality, independent observations, and homoscedasticity. Visualizations are included to support insights and findings.

***Project Findings:***

Model Summary: Simple Linear Regression on marketing sales data.

Y-intercept: 41.5326, Slope: 8.1733.

Interpretation: A $1 million increase in radio promotion budget leads to an average sales increase of $8.1733 million.

Statistical Significance: p-value = 0.000 (significant at 0.05 level).

Hypothesis Testing: Reject the null hypothesis (no relationship between radio budget and sales).

Confidence Interval: 95% CI for the slope: [7.791, 8.555], meaning the true slope likely falls in this range.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Data Exploration](#data-exploration)
- [Model Building](#model-building)
- [Results](#results)
- [Assumption Checks](#assumption-checks)
- [Conclusion](#conclusion)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)

## Project Overview

The goal of this analysis is to examine the impact of the radio advertising budget on sales using ordinary least squares (OLS) linear regression. The analysis provides insights into the relationship between marketing spend and sales performance.

## Dataset

The dataset used in this analysis is named `_marketing_sales_data.csv`, which includes the following columns:

- **TV**: Category of TV advertising spend (Low, Medium, High)
- **Radio**: Amount spent on radio advertising (in millions)
- **Social Media**: Amount spent on social media advertising (in millions)
- **Influencer**: Type of influencer marketing (Micro, Macro, Mega, Nano)
- **Sales**: Total sales generated (in millions)

## Data Exploration

The initial exploration of the dataset includes:

- Displaying the first 10 rows of data
- Checking for null values
- Dropping rows with null values

A pairwise relationship plot was created to visualize the correlations among the variables.

## Model Building

The following steps were taken to build the linear regression model:

1. **OLS Data Preparation**: Selected `Radio` and `Sales` columns for the analysis.
2. **Linear Regression Formula**: Defined the formula as `Sales ~ Radio`.
3. **Model Fitting**: Implemented the OLS approach and fit the model to the data.

## Results

The regression model summary provides key insights:

- **Model Equation**:
  \[
  y{Sales} = 8.1733 * x{Radio} + 41.5326
  \]
- **Y-intercept**: 41.5326
- **Slope**: 8.1733 (indicates sales increase by 8.1733 million dollars for every 1 million dollar increase in radio budget)
- **R-squared**: 0.757 (75.7% of sales variability explained by radio budget)
- **p-value**: 0.000 (statistically significant relationship)

## Assumption Checks

To ensure the validity of the linear regression model, the following assumptions were checked:

- **Linearity**: Confirmed through scatterplots and regression plots.
- **Normality of Residuals**: Visualized using histograms and Q-Q plots.
- **Independence of Observations**: Residuals vs. fitted values showed no patterns.
- **Homoscedasticity**: Residuals appeared randomly spaced.

## Conclusion

The analysis demonstrates a significant positive relationship between radio advertising budgets and sales. The results indicate that increasing radio budget leads to higher sales, providing a data-driven foundation for marketing decisions.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Statsmodels

## Getting Started

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```
