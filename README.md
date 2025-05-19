# Project Car Price Analysis

## Dataset Content

This dataset contains information about 205 cars, including technical specifications and prices. Each row is a different car, and each column is a feature like engine size, horsepower, fuel type, and so on.

Some of the key columns are:

- `carname`: brand and model
- `price`: the car's price in USD
- `horsepower`, `enginesize`, `curbweight`: these help describe performance
- `carbody`, `fueltype`: describe the type of car

I downloaded the dataset from [Kaggle](https://www.kaggle.com/datasets/hellbuoy/car-price-prediction).

## Business Requirements

The goal is to help a car company understand:

- What features affect car prices
- Which car types are cheaper or more expensive
- Which brands give good value for money (performance vs. cost)

This can help the company make better decisions about pricing and design.

As a student, I’m using this project to practice cleaning data and finding answers to simple questions using Python, Pandas, and NumPy.

## Hypothesis and how to validate?

Here are some ideas (hypotheses) I want to test in this project:

1. **More horsepower = more expensive car**  
   ➤ I’ll compare the `horsepower` and `price` columns and check if there’s a pattern.

2. **Some brands are better value than others**  
   ➤ I’ll create a new column that shows the price per horsepower and compare it between brands.

3. **Car type affects price**  
   ➤ I’ll group cars by `carbody` and see the average price for each one.

All of this will be done using simple Pandas and NumPy functions — no machine learning or advanced tools.

## Project Plan

I followed this plan:

1. **ETL**

   - Loaded the dataset
   - Cleaned column names and values
   - Removed outliers
   - Created new columns (`carbrand`, `price_per_hp`)
   - Saved cleaned data

2. **Data Analysis**

   - Grouped data by brand, car body, fuel type
   - Calculated average prices and MPG

3. **Visualisations**

   - Created charts using Matplotlib, Seaborn, and Plotly

4. **Documentation**
   - Wrote this README and added comments to my notebook

## The rationale to map the business requirements to the Data Visualisations

| Business Question                      | Visualisation Used                       |
| -------------------------------------- | ---------------------------------------- |
| Which brands are most expensive?       | Bar chart (avg. price by brand)          |
| Which brands give best value?          | Bar chart (price per horsepower)         |
| Does car type affect price/efficiency? | Bar charts (city MPG & price by carbody) |
| Does more power = higher price?        | Scatter plot (horsepower vs price)       |

## Analysis techniques used

- Used `.groupby()` and `.mean()` to compare brands and car types
- Created new columns like `price_per_hp` and `power_to_weight`
- Visualised results with:
  - **Matplotlib** (basic plots)
  - **Seaborn** (grouped bar charts)
  - **Plotly** (interactive scatter plots)

## Ethical considerations

- The data is public and contains no personal information
- No machine learning or predictions were used
- This project was done for learning purposes only

## Unfixed Bugs

- Some Matplotlib and Seaborn plots saved as blank images in VSCode
- Fixed this by switching to Plotly or using `fig.savefig()` correctly

## Development Roadmap

If I continue this project, I would like to:

- Add more data (like car year or location)

## Main Data Analysis Libraries

- **Pandas** – for loading, cleaning, and analysing the data
- **NumPy** – for basic math and logic
- **Matplotlib** – for basic plots
- **Seaborn** – for nicer grouped charts
- **Plotly** – for interactive plots

## Credits

- Dataset: [Kaggle - Car Price Prediction](https://www.kaggle.com/datasets/hellbuoy/car-price-prediction)
- Help: Project supported by class, internet guides, and [ChatGPT]
- Inspiring: Alex the Analyst: [Pandas for Beginners](https://www.youtube.com/playlist?list=PLUaB-1hjhk8GZOuylZqLz-Qt9RIdZZMBE)
- Markdown: (https://www.markdownguide.org/basic-syntax/)
- Pandas: [CheatSheet](https://www.datacamp.com/cheat-sheet/pandas-cheat-sheet-for-data-science-in-python)
- Plotly: [CheatSheet](https://www.datacamp.com/cheat-sheet/plotly-express-cheat-sheet)
