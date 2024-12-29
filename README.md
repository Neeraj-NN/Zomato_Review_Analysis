# Restaurant Data Analysis

This Python script performs analysis and visualization of restaurant review data. It processes a CSV file containing restaurant information, including ratings and prices, to generate insights and visualizations.

## Prerequisites

- Python 3.x
- Required libraries:
  - pandas
  - matplotlib
  - seaborn

Install required libraries using:
```bash
pip install pandas matplotlib seaborn
```

## Input Data Format

The script expects a CSV file named `reviews.csv` with the following columns:
- Restaurant Name
- Overall_Rating
- Rate for two (cost for two people)

Additional columns may be present but are not used in the analysis.

## Features

1. **Data Preprocessing**
   - Handles numeric conversion of 'Rate for two' column
   - Removes commas from price values
   - Performs data cleaning and null value handling

2. **Basic Data Inspection**
   - Displays dataset information using `df.info()`
   - Shows the first few rows of data using `df.head()`

3. **Visualization**
   - Creates a histogram of restaurant ratings distribution
   - Generates a scatter plot showing the relationship between ratings and cost
   - Annotates top-rated restaurants on the scatter plot

4. **Analysis**
   - Identifies and displays the top 5 restaurants by rating

## Usage

1. Place your `reviews.csv` file in the same directory as the script
2. Run the script:
```bash
python restaurant_analysis.py
```

## Output

The script generates:
1. A histogram showing the distribution of overall ratings
2. A scatter plot displaying the relationship between restaurant ratings and cost for two
3. Console output showing:
   - Dataset information
   - Sample of the data
   - Top 5 highest-rated restaurants

## Error Handling

The script includes error handling for:
- Missing input file
- Missing required columns
- Invalid data formats

## Notes

- Missing values in 'Overall_Rating' are filled with 0
- The script automatically generates restaurant names if not provided in the dataset
- The scatter plot is configured for optimal visualization of large datasets

## Contributing

Feel free to submit issues and enhancement requests.
