# ☕ Coffee Shop Sales Analysis

## Project Overview

This project explores historical coffee shop sales data using Python and exploratory data analysis (EDA).

The objective is to understand product performance, identify customer purchasing patterns, investigate sales and revenue trends, and examine how historical selling prices relate to sales performance.

The analysis aims to translate raw sales data into meaningful business insights and practical recommendations that could support better operational and commercial decisions.

## Business Problem

The coffee shop collects sales data but lacks a clear understanding of its product performance, purchasing patterns and revenue trends.

Without analysing this information, it can be difficult to identify the most important products, understand periods of high demand, recognise changes in customer preferences and make informed decisions about stock planning and pricing.

This project addresses the following business questions:

1. Which products perform best in terms of sales volume and revenue?
2. When does the coffee shop experience the highest demand?
3. How do sales and revenue change over time?
4. How have historical selling prices related to sales volume and revenue?
5. What opportunities can be identified to improve business performance?

## Dataset

The dataset was obtained from Kaggle:

**Source:** [Coffee Revenue Dataset – Kaggle](https://www.kaggle.com/datasets/rifatalam3/coffee-revenue-dataset)

The dataset contains **3,547 individual drink sales**, covering the period from March 2024 to March 2025.

Each row represents an individual drink sold.

The dataset includes information such as:

- Date and time of sale
- Drink type
- Selling price
- Payment method
- Weekday and month information

*Note: The currency associated with the recorded selling prices is not specified in the dataset. Financial figures are therefore presented using the original recorded values.*

## Tools and Technologies

- **Python** – Data analysis and manipulation
- **Pandas** – Data cleaning, transformation and analysis
- **NumPy** – Numerical operations
- **Matplotlib** – Data visualisation
- **Seaborn** – Statistical data visualisation
- **Jupyter Notebook** – Interactive analysis and documentation

## Project Workflow

### 1. Data Understanding and Cleaning

- Inspected the dataset structure and data types.
- Checked for missing values and duplicate records.
- Standardised column names using snake_case.
- Converted date and time columns into appropriate formats.
- Created additional variables to support the analysis, including weekend indicators.

### 2. Exploratory Data Analysis

**Product Performance**

Analysed sales volume, revenue contribution and average selling prices across different drinks to identify the strongest and weakest performers.

**Hourly and Weekday Demand**

Investigated sales distribution by hour and day of the week to identify periods of higher and lower demand.

**Monthly Sales and Revenue Trends**

Examined changes in monthly sales and revenue to identify fluctuations and potential trends over the observation period.

**Product Sales Mix**

Analysed the percentage contribution of individual drinks to total monthly sales to identify changes in product popularity.

**Historical Pricing Analysis**

Investigated recorded selling prices alongside average daily sales and revenue to explore how product performance varied across historical price periods.

## Key Findings

The analysis revealed several interesting insights:

- **Product performance:** Americano with Milk was the most frequently purchased drink, while Latte generated the highest total revenue.
- **Peak demand:** 10:00 was the busiest hour, with a secondary increase in sales around 16:00.
- **Weekday performance:** Tuesday recorded the highest sales volume, while Sunday recorded the lowest.
- **Monthly trends:** October 2024 recorded the highest monthly sales, followed by a significant decline towards January 2025. February 2025 experienced a strong recovery.
- **Changing product preferences:** Americano and Cocoa experienced substantial increases in sales contribution during February 2025.
- **Pricing patterns:** Different products displayed different sales patterns across recorded price periods, demonstrating that sales performance cannot be explained by selling price alone.

## Business Recommendations

Based on the findings, the following recommendations were identified:

1. **Improve stock planning:** Prioritise stock availability for high-performing products, particularly Americano with Milk, Latte and Cappuccino.
2. **Review staffing requirements:** Investigate staffing levels during peak demand periods, particularly around 10:00 and 16:00.
3. **Investigate changing demand:** Explore the factors behind the significant increase in Americano and Cocoa sales during February 2025.
4. **Review lower-performing products:** Investigate the demand and positioning of Espresso and Cortado before considering changes to the product range.
5. **Monitor pricing performance:** Track selling prices alongside sales volume and revenue. Incorporating product costs would allow future analysis of profitability.

## Limitations

- The dataset does not specify the currency associated with selling prices.
- Product costs and operating expenses are unavailable, preventing profitability analysis.
- Customer identifiers are not available, so individual purchasing behaviour and customer retention cannot be investigated.
- Confirmed opening days are unavailable. Daily averages are based on dates with recorded transactions.
- Historical price changes overlap with changes in time and potentially seasonal demand. The analysis cannot establish a causal relationship between price changes and sales.
- March 2025 contains incomplete data, ending on March 23.

## Repository Structure


Coffee_Shop_Sales_Analysis/
|
├──src/
|    ├── data/
|    │   └── coffee_sales.csv
|    │
|    ├── notebooks/
|    |    └── coffee_sales_analysis.ipynb
|    |
|    ├── utils
|          └── bootcampviztools.py
|
├── README.md
├── requirements.txt
└── .gitignore


## How to Run the Project

1. Clone the repository:

```bash
git clone <repository-url>
```

2. Navigate to the project directory:

```bash
cd Coffee_Sales_Analysis
```

3. Create a virtual environment:

```bash
python -m venv venv
```

4. Activate the environment.

Windows (Git Bash):

```bash
source venv/Scripts/activate
```

5. Install the required libraries:

```bash
pip install -r requirements.txt
```

6. Launch Jupyter Notebook:

```bash
jupyter notebook
```

7. Open `notebooks/coffee_sales_analysis.ipynb` and run the analysis.

## Conclusion

This project demonstrates how exploratory data analysis can help transform raw sales records into meaningful business insights.

By examining product performance, purchasing patterns, monthly trends and historical pricing, the analysis identifies opportunities for improved stock planning, operational efficiency and business decision-making.

The project also highlights the importance of recognising data limitations and avoiding unsupported conclusions when interpreting business data.