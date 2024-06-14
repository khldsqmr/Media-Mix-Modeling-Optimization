# Marketing Mix Modeling Optimization (MMM) Project

This project uses Marketing Mix Modeling (MMM) to optimize marketing budget allocation across various channels, aiming to maximize sales and understand the impact of each channel.

## Objective
Optimize marketing budget allocation across various channels to maximize sales and understand the impact of each channel.

## Key Concepts
1. **Ad Stock**: Measures the impact of past advertisements on current sales using a decay factor.
2. **Diminishing Returns**: Describes how returns on investments decrease as more is spent. Modeled using the formula: 
   Response(X) = (a * X^α) / (X^α + c^α)

## Formulas and Concepts

### Response Curve Formula
Response(X) = (a * X^α) / (X^α + c^α)

Where:
- X is the ad stock (transformed marketing spend).
- a is the scale parameter, indicating the maximum potential impact on sales.
- α is the shape parameter, indicating how quickly diminishing returns set in.
- c is the saturation parameter, indicating the spend level where returns start to diminish significantly.

### Diminishing Returns
- Additional spending yields decreasing marginal returns beyond a certain point (threshold).

### Optimization Objective
- Maximize total sales by reallocating the budget to channels with the highest incremental returns.

## Methodology

1. **Data Preparation**:
    - Loaded historical spend and sales data.
    - Calculated ad stock for each channel.

2. **Model Fitting**:
    - Fitted the sales response model to each channel to determine optimal coefficients.

3. **Budget Allocation**:
    - Optimized the budget using the fitted model to maximize total sales.
    - Compared optimized allocations with actual spends.
    - ## Budget Allocation

      | Channel       | Optimized Budget |
      |---------------|------------------|
      | Search_Ads    | $49,889.02       |
      | Social_Media  | $924,352.37      |
      | TV_Ads        | $0.00            |
      | Radio_Ads     | $18,954.22       |
      | Billboards    | $6,804.39        |

4. **Visualization**:
    - Scatter plots to explore initial correlations.
    - Diminishing returns plots to identify optimal spend thresholds.
    - Comparison of optimized and actual budget allocations.

5. **Ad-hoc Analysis**:
    - Detailed comparison table with percentage differences.
    - Examination of predicted vs. actual sales to validate model accuracy.

## Explanation of Response Curve and Diminishing Returns

### Response Curve
The response curve captures the relationship between marketing spend and sales. The formula used is:

Response(X) = (a * X^α) / (X^α + c^α)

Where:
- X is the ad stock (transformed marketing spend).
- a is the scale parameter, indicating the maximum potential impact on sales.
- α is the shape parameter, indicating how quickly diminishing returns set in.
- c is the saturation parameter, indicating the spend level where returns start to diminish significantly.

### Diminishing Returns
Diminishing returns describe how the incremental benefit (sales) decreases as more is spent on a channel. This is illustrated in the response curve, where initial increases in spend yield significant sales gains, but beyond a certain point, additional spend results in smaller sales increments.

### Correctness of the Formula
The formula used in the analysis is a common representation of diminishing returns in marketing models. It correctly captures the key aspects:
- Initial high returns on investment.
- Gradual reduction in incremental gains as spend increases.
- A saturation point beyond which additional spend yields minimal returns.

## Results

- **Optimized Budget Allocation**:
    - Reallocated funds to channels with higher marginal returns.
    - Showed significant improvements in total profit compared to actual allocations.

- **Diminishing Returns Visualization**:
    - Highlighted the optimal spending thresholds for each channel.

- **Comparison of Allocated Budgets**:
    - Illustrated differences between optimized and actual spends using percentage differences.

- **Total Profit Calculation**:
    - Demonstrated overall improvement in returns from optimized budget allocation.

This project demonstrated the use of Marketing Mix Modeling (MMM) to optimize budget allocations across various marketing channels, with the aim of maximizing sales. The analysis provided clear insights into the efficiency of each channel's spend, helping to make informed decisions on budget distribution.
