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

The goal of this project is to help a car company understand what affects the price of a car. They want to know things like:

- Does more horsepower mean a higher price?
- Which brands give better value for the money?
- Does the type of car (like SUV or sedan) change how much it costs?

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

Since this is my first data analysis project, I broke it into a few simple steps:

1. **Explore the dataset**  
   ➤ Load the CSV file and look at the data with `.head()`, `.info()`, and `.describe()`.

2. **Clean the data**  
   ➤ I fixed text formatting, dropped unnecessary columns, and removed outliers.

3. **Feature engineering**  
   ➤ I created new columns like `price_per_hp` and `power_to_weight` to help with analysis.

4. **Save the cleaned data**  
   ➤ I saved a clean version of the dataset to use later.

5. **Next steps**  
   ➤ I plan to group data, find patterns, and eventually create some tables or simple charts (only with Pandas).

## The rationale to map the business requirements to the Data Visualisations

## Analysis techniques used

## Ethical considerations

## Unfixed Bugs

## Development Roadmap

## Main Data Analysis Libraries

## Credits
