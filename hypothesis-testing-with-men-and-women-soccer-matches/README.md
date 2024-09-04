# Soccer Goals Hypothesis Test: Women's vs Men's World Cup Matches

This project performs a hypothesis test to compare the mean number of goals scored in women's and men's international soccer matches, specifically in Official FIFA World Cup matches since January 1, 2002.

## Project Overview

The analysis aims to determine whether there is a significant difference in the average number of goals scored in women's international soccer matches compared to men's matches. This is done through a hypothesis test using data from Official FIFA World Cup matches.

## Hypothesis

- Null Hypothesis (H0): The mean number of goals scored in women's international soccer matches is the same as in men's matches.
- Alternative Hypothesis (H1): The mean number of goals scored in women's international soccer matches is greater than men's matches.

## Key Parameters

- Significance Level: 10% (α = 0.10)
- Time Period: Matches since January 1, 2002
- Assumption: Each match is fully independent (team form is ignored)

## Key Output

The analysis produces a dictionary called `result_dict` with the following structure:

```python
result_dict = {
    "p_val": p_val,
    "result": result
}
```

Where:
- `p_val` is the calculated p-value from the hypothesis test
- `result` is either "fail to reject" or "reject", depending on the outcome of the test

## Getting Started

### Prerequisites

- Python enviroment
- pandas
- scipy

Or just use Googel colab for ease of use.

## Methodology

1. **Data Loading and Preparation**: 
   - Load the FIFA World Cup match data.
   - Filter for matches since January 1, 2002.

2. **Normality**:
   - Determine normality using histograms.

3. **Hypothesis Testing**:
   - Perform an appropriate two-sample test (Mann-Whitney U t-test in this case).
   - Calculate the p-value.

4. **Decision Making**:
   - Compare the p-value to the significance level (α = 0.10).
   - Determine whether to reject or fail to reject the null hypothesis.

5. **Result Storage**:
   - Store the p-value and the test result in the `result_dict` dictionary.

## Results Interpretation

- If p-value ≤ 0.10: Reject the null hypothesis. This suggests the mean number of goals scored by women's is significantly greater than the mean number of goals scored by men's.
- If p-value > 0.10: Fail to reject the null hypothesis. This suggests there is not enough evidence to conclude a significant difference in the mean number of goals scored.

## Limitations and Assumptions

- The analysis assumes each match is independent, ignoring potential effects of team form or other factors.
- The test only considers Official FIFA World Cup matches, which may not be representative of all international soccer matches.
- The analysis does not account for potential confounding variables such as tournament structure, team rankings, or environmental factors (no causality).

## Potential Extensions

- Extend the analysis to include other international tournaments or friendly matches.
- Investigate trends in goal scoring over time for both women's and men's matches.
- Analyze the impact of factors such as home advantage, team rankings, or tournament stages on goal scoring.