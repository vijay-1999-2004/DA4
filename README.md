Page View Time Series Visualizer

This project is part of the Data Analysis with Python certification from freeCodeCamp.

In this project, time series data is visualized using line charts, bar charts, and box plots. The dataset contains the daily page views on the freeCodeCamp.org forum from 2016-05-09 to 2019-12-03. These visualizations help analyze growth trends and seasonal patterns in site traffic over time.

📌 Dataset Overview

The dataset (fcc-forum-pageviews.csv) contains:

date: The date of observation (YYYY-MM-DD format).

value: Total page views recorded on that date.

🛠️ Data Cleaning & Preparation

Date Parsing: Loaded dataset into Pandas with date set as the index and parsed into datetime format.

Outlier Removal: Cleaned dataset by removing data points where page views fell:

Below the 2.5th percentile

Above the 97.5th percentile

📊 Visualizations Generated

Daily Line Plot (line_plot.png):

Title: Daily freeCodeCamp Forum Page Views 5/2016-12/2019

X-Axis: Date

Y-Axis: Page Views

Purpose: Displays daily page view trends over time.

Monthly Bar Plot (bar_plot.png):

Title Legend: Months (sorted January–December)

X-Axis: Years

Y-Axis: Average Page Views

Purpose: Compares average daily page views for each month grouped by year.

Box Plots (box_plot.png):

Plot 1: Year-wise Box Plot (Trend) — Displays overall yearly distribution and growth trend.

Plot 2: Month-wise Box Plot (Seasonality) — Displays monthly distribution from Jan–Dec across all years to identify seasonal traffic peaks.

🚀 Setup & Execution

1. Install Dependencies

Ensure you have Python installed along with the required libraries:

pip install pandas matplotlib seaborn


2. Run Main Script

Make sure fcc-forum-pageviews.csv, time_series_visualizer.py, and main.py are in the same directory, then run:

python main.py


📁 File Structure

├── fcc-forum-pageviews.csv    # Forum traffic dataset
├── time_series_visualizer.py  # Data processing and plotting functions
├── main.py                    # Entry point to execute plots and tests
├── test_module.py             # Unit tests provided by freeCodeCamp
└── README.md                  # Project documentation
