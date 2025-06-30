# Supervised Machine Learning Project (Car Sales Mathematical Modelling)
## Project Objective
The main objective of this project is to build a supervised machine learning model (specifically linear regression) to predict the price of used cars based on various features such as mileage, engine volume, and year of manufacture. The goal includes data cleaning, exploration, visualization, and transformation to meet the assumptions of linear regression and ultimately derive insights about car pricing.

## Data used
- <a href = "https://github.com/pagonzales/Supervised_Machine_Learning_Project_Car_Sales/blob/main/dataset.csv">Dataset</a>
## Questions
- What features significantly influence the price of a used car?
- How well can a linear regression model predict the car price?
- Are there any outliers or anomalies in the dataset that affect prediction accuracy?
- Can the assumptions of linear regression (e.g., linearity, normality, no multicollinearity) be satisfied with this dataset?

## Process
- Starting with Data cleaning, Data Loading and Initial Inspection.
  - Load raw CSV data using pandas.
  - Inspect the first few rows and generate descriptive statistics.
- Data Preprocessing
  - Drop irrelevant columns like "Model" of cars.
  - Handle missing values by removing incomplete rows.
  - Visualize distributions of numerical variables (Price, Mileage, EngineV, Year).
- Outlier Removal
  - Use quantile thresholds to eliminate extreme outliers in features.
  - Filter values based on visual inspection of distribution plots.
- Assumption Checks for Linear Regression
  - Visualize scatter plots between Price and independent variables to assess linearity.
  - Apply a log transformation to the Price variable to achieve a more linear relationship with predictors.
- Model Preparation (continuation in further cells)
   - Use train/test split, fitting the model, evaluating metrics such as R², residual analysis to know if the mathematical model is a good a approximation.
## Image

## Project insights
- Newer Cars Are Worth the Investment
  - We found a strong relationship between a car’s year of manufacture and its price. Simply put, the newer the car, the more money it brings in. This isn’t surprising—but it confirms that investing more in newer vehicles (even if they cost a bit more upfront) will likely yield better returns.
- Mileage Tells the Real Story
  - Mileage had one of the biggest impacts on price. Cars with high mileage lose a lot of their value, even if they’re otherwise in good condition.
- Bigger Engine ≠ Bigger Profit
  - Cars with larger engines do tend to cost more, but only up to a point. Once the engine volume gets too high, the price doesn’t always scale—maybe because buyers don’t want to pay extra for gas-guzzlers or luxury taxes.
- Outliers Throw Off the Whole Picture
  - Some vehicles had extremely high or low prices that didn’t match the rest. These outliers can skew our analysis and confuse customers who see inconsistent pricing.
- Clean Data = Better Decisions
  - A lot of our early data had missing values or inconsistent entries. Once we cleaned it up, everything made more sense—and the model gave much more accurate predictions.

## Final conclusion
This project showed us that with the right data and a bit of cleaning, we can actually predict used car prices pretty accurately using just a few key features like the car’s age, mileage, and engine size.
What’s more important is that the model isn’t just good at math—it gives us real, useful insights we can act on. For example, newer cars and those with lower mileage clearly hold more value, so we should focus on getting more of those in our inventory. We also saw how messy data and outlier prices can throw everything off, which tells us that keeping the records (data) clean is just as important as the model itself.

