# Insurance Risk Analysis

This notebook focuses on analyzing risk differences in insurance claims based on various demographic and geographical factors. It includes multiple analyses to assess the impact of province, postal code, gender, and their associated claims data.

## Contents

### 1. Risk Analysis Across Provinces
- **Objective**: Compare claims frequency between two groups based on provinces.
- **Methodology**:
  - Load dataset into a Pandas DataFrame.
  - Define control (Gauteng) and test (Western Cape) groups.
  - Verify group sizes and check for null values.
  - Calculate claims frequency.
  - Perform a t-test for statistical comparison.
  - Visualize claims distribution using histograms.

### 2. Analysis of TotalPremium and TotalClaims by Postal Code Group
- **Objective**: Examine significant differences in TotalPremium and TotalClaims between two groups derived from the top 50 most frequent postal codes.
- **Methodology**:
  - Identify the top 50 postal codes by frequency.
  - Split into two groups: odd indexed and even indexed.
  - Conduct independent t-tests on TotalPremium and TotalClaims.
  - Evaluate significance with α = 0.05.

### 3. ANOVA Test for Profit Margin Differences Across Zip Codes
- **Objective**: Test for significant differences in profit margins across different zip codes.
- **Methodology**:
  - Calculate profit margin as TotalPremium minus TotalClaims.
  - Group data by postal code.
  - Perform ANOVA test to assess differences in average profit margins.
  - Interpret p-values to accept or reject the null hypothesis.

### 4. Hypothesis Testing: Risk Difference between Men and Women
- **Objective**: Evaluate risk differences based on gender.
- **Methodology**:
  - Conduct a t-test comparing average TotalClaims.
  - Perform a Chi-squared test for claim occurrence.
  - Formulate null and alternative hypotheses and interpret results.

## Results and Interpretation
- Each section concludes with statistical outcomes, indicating whether to reject or fail to reject the null hypothesis based on p-values.

## Usage
- Ensure you have the necessary Python libraries installed (`pandas`, `scipy`, `matplotlib`, etc.).
- Run each section sequentially to perform the analyses as described.

## Contributions
- Contributions are welcome! Please follow standard practices for issue reporting and pull requests.

## License
- This project is licensed under the MIT License.