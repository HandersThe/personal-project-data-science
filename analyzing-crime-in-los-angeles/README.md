# Crime Data Analysis Project

This project analyzes the `crimes.csv` dataset to extract insights about crime patterns in a specific area.

## Project Objectives

The main objectives of this analysis are:

1. Identify the hour with the highest frequency of crimes.
2. Determine the area with the largest frequency of night crimes (between 10pm and 3:59am).
3. Analyze the distribution of crimes across different victim age groups.

## Key Variables

- `peak_crime_hour`: An integer representing the hour with the highest crime frequency.
- `peak_night_crime_location`: A string indicating the area with the most night crimes.
- `victim_ages`: A pandas Series containing the frequency of crimes for different age groups.

## Age Group Categories

The victim age groups are categorized as follows:

- "0-17"
- "18-25"
- "26-34"
- "35-44"
- "45-54"
- "55-64"
- "65+"

## Getting Started

### Prerequisites

- Python enviroment
- pandas
- matplotlib
- Seaborn

Or just use Google colab for ease of use.

## Results

After running the analysis, you'll find:

- The hour with the highest crime frequency (`peak_crime_hour`)
- The area with the most night crimes (`peak_night_crime_location`)
- A breakdown of crimes by victim age groups (`victim_ages`)