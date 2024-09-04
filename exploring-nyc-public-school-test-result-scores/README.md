# NYC Schools SAT Analysis

This project analyzes SAT scores from New York City schools, focusing on math performance, overall SAT performance, and borough-level statistics.

## Project Objectives

1. Identify schools with the best math results.
2. Determine the top 10 performing schools based on combined SAT scores.
3. Find the borough with the largest standard deviation in combined SAT scores.

## Key Outputs

The analysis produces the following key outputs:

1. `best_math_schools`: A DataFrame of schools with top math performance.
2. `top_10_schools`: A DataFrame of the 10 best-performing schools based on total SAT scores.
3. `largest_std_dev`: A DataFrame with statistics for the borough showing the largest standard deviation in SAT scores.

## Getting Started

### Prerequisites

- Python enviroment
- pandas

Or just use Google colab for ease of use.

## Methodology

1. **Data Loading**: 
   - Read the NYC schools SAT data file using pandas.

2. **Best Math Schools Analysis**:
   - Filter schools with math scores at least 80% of the maximum (800).
   - Create `best_math_schools` DataFrame with "school_name" and "average_math" columns.
   - Sort results by "average_math" in descending order.

3. **Top 10 Schools Analysis**:
   - Calculate total SAT score for each school.
   - Create `top_10_schools` DataFrame with "school_name" and "total_SAT" columns.
   - Sort by "total_SAT" in descending order and select top 10.

4. **Borough Standard Deviation Analysis**:
   - Group data by borough and calculate standard deviation of total SAT scores.
   - Identify borough with largest standard deviation.
   - Create `largest_std_dev` DataFrame with borough name, number of schools, average SAT score, and standard deviation.
   - Round numeric values to two decimal places.

## Results

After running the analysis, you'll have:
- `best_math_schools`: DataFrame of top-performing schools in math.
- `top_10_schools`: DataFrame of the 10 best schools by total SAT score.
- `largest_std_dev`: DataFrame with statistics for the borough showing the most variation in SAT scores.

## Data Dictionary

### best_math_schools
- `school_name`: Name of the school
- `average_math`: Average math SAT score

### top_10_schools
- `school_name`: Name of the school
- `total_SAT`: Combined SAT score (sum of math, reading, and writing scores)

### largest_std_dev
- `borough`: Name of the NYC borough
- `num_schools`: Number of schools in the borough
- `average_SAT`: Mean of total SAT scores in the borough
- `std_SAT`: Standard deviation of total SAT scores in the borough

## Potential Extensions

- Visualize the distribution of SAT scores across boroughs.
- Analyze trends in SAT performance over time (if historical data is available).
- Investigate correlations between SAT scores and other factors (e.g., school size, funding).