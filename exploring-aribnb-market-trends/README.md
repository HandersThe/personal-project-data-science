# New York Airbnb Data Analysis

This project analyzes Airbnb listing data in New York to provide insights on private rooms for a real estate start-up.

## Project Overview

As a consultant for a real estate start-up, we're investigating the short-term rental market in New York using Airbnb data. The analysis focuses on private room listings, pricing, and review dates.

## Data Sources

The project uses three data files located in the `data` folder:

1. `airbnb_price.csv`
2. `airbnb_room_type.xlsx`
3. `airbnb_last_review.tsv`

## Project Objectives

1. Determine the earliest and most recent review dates.
2. Count the number of private room listings.
3. Calculate the average listing price.
4. Combine the results into a single DataFrame.

## Key Outputs

The analysis produces the following key outputs:

1. Two variables storing the earliest and most recent review dates.
2. A variable containing the count of private room listings.
3. A variable with the average listing price, rounded to two decimal places.
4. A DataFrame called `review_dates` with the following columns:
   - `first_reviewed`
   - `last_reviewed`
   - `nb_private_rooms`
   - `avg_price`

## Getting Started

### Prerequisites

- Python enviroment
- pandas
- openpyxl

Or just use Google colab for ease of use.

## Results

After running the analysis, you'll have:
- Variables containing the earliest and most recent review dates.
- A count of private room listings.
- The average listing price.
- A `review_dates` DataFrame summarizing the findings.

## Data Dictionary

- `first_reviewed`: Date of the earliest review
- `last_reviewed`: Date of the most recent review
- `nb_private_rooms`: Number of private room listings
- `avg_price`: Average price of listings (rounded to 2 decimal places)