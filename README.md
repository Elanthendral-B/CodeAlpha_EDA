# CodeAlpha Web Scraping Project

## Task 1: Web Scraping

This project is created as part of the CodeAlpha Data Analytics Internship.

## Project Description

The purpose of this project is to extract book information from a public website using Python and BeautifulSoup.

The scraped information includes:

- Book Title
- Book Price
- Availability

## Technologies Used

- Python
- Requests
- BeautifulSoup
- Pandas
- VS Code

## Libraries Used

```python
requests
beautifulsoup4
pandas


# CodeAlpha - Exploratory Data Analysis

## Internship Task 2

This project performs Exploratory Data Analysis (EDA) on an Online Retail dataset.

## Objectives

- Understand the structure of the dataset
- Identify missing values
- Detect duplicate records
- Clean the dataset
- Analyze sales statistics
- Find the top-selling products
- Analyze country-wise sales
- Analyze monthly sales trends

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Dataset

Online Retail Sales Dataset.

## Key Analysis

### Data Cleaning
- Removed duplicate records
- Handled missing product descriptions
- Converted invoice dates into datetime format
- Removed invalid quantity values
- Removed invalid unit prices

### Sales Analysis
The project calculates total sales using:

`TotalSales = Quantity × UnitPrice`

### Key Findings

- Total cleaned records: 524,878
- Total revenue: 10,642,110.80
- Top-selling product by quantity: PAPER CRAFT, LITTLE BIRDIE
- Highest-sales country: United Kingdom
- Highest-sales month: November 2011

## Project Structure

CodeAlpha_EDA/
│
├── dataset/
│   └── online_retail.csv
│
├── eda_analysis.py
│
└── README.md

## How to Run

1. Install Python.
2. Install required libraries:

```bash
pip install pandas numpy matplotlib seaborn

# CodeAlpha Data Visualization



## Internship Task 3

## Project Overview

This project performs Exploratory Data Analysis and Data Visualization on an Online Retail dataset using Python.

The main objective is to analyze sales data and identify useful patterns, best-selling products, top-performing countries, and monthly sales trends.

## Technologies Used

- Python
- Pandas
- Matplotlib
- Seaborn

## Dataset

The project uses the Online Retail dataset containing the following columns:

- InvoiceNo
- StockCode
- Description
- Quantity
- InvoiceDate
- UnitPrice
- CustomerID
- Country

The original dataset contains 541,909 rows and 8 columns.

## Data Cleaning

The following data cleaning steps were performed:

- Removed duplicate rows
- Filled missing product descriptions
- Created a TotalSales column
- Prepared the data for analysis and visualization

After cleaning, the dataset contains 524,878 rows and 9 columns.

## Analysis Performed

### 1. Monthly Sales Trend

A line chart was created to analyze sales performance month by month.

### 2. Top 10 Best-Selling Products

A bar chart was created to identify the products with the highest quantity sold.

### 3. Top 10 Countries by Sales

Sales revenue was analyzed by country to identify the top-performing countries.

## Key Results

- Total Revenue: 10,642,110.804
- Highest-selling product by quantity: PAPER CRAFT , LITTLE BIRDIE
- United Kingdom generated the highest sales revenue.
- November 2011 recorded the highest monthly sales.

## Output

The project generates the following visualizations:

- `monthly_sales_trend.png`
- `top_10_products.png`

## How to Run

1. Install Python.
2. Install the required libraries:

```bash
pip install pandas matplotlib seaborn


# CodeAlpha Task 4 – Sentiment Analysis

## Project Overview

This project performs sentiment analysis on product descriptions from the Online Retail dataset.

The objective is to classify text data into three sentiment categories:

* Positive
* Negative
* Neutral

The project uses Python and Natural Language Processing (NLP) techniques to analyze the sentiment of product descriptions.

## Dataset

The dataset used in this project is `online_retail.csv`.

### Original Dataset

* Rows: 541,909
* Columns: 8

### Important Columns

* `InvoiceNo` – Invoice number
* `StockCode` – Product code
* `Description` – Product description
* `Quantity` – Quantity purchased
* `InvoiceDate` – Date and time of transaction
* `UnitPrice` – Unit price
* `CustomerID` – Customer identifier
* `Country` – Customer country

## Data Cleaning

The following preprocessing steps were performed:

1. Loaded the Online Retail CSV dataset.
2. Checked the dataset structure and missing values.
3. Removed rows with missing product descriptions.
4. Converted product descriptions to text format.
5. Converted text to lowercase.
6. Removed special characters and numbers.
7. Removed extra spaces.
8. Saved the cleaned dataset as `cleaned_online_retail.csv`.

After cleaning, the dataset contained:

**540,399 records and 9 columns.**

## Sentiment Analysis

VADER Sentiment Analysis was used to calculate sentiment scores for the product descriptions.

The sentiment classification rules were:

* Compound score >= 0.05 → Positive
* Compound score <= -0.05 → Negative
* Between -0.05 and 0.05 → Neutral

A sentiment score was also stored for each product description.

## Results

The sentiment analysis produced the following results:

| Sentiment | Number of Records | Percentage |
| --------- | ----------------: | ---------: |
| Neutral   |           417,487 |     77.26% |
| Positive  |           109,162 |     20.20% |
| Negative  |            13,750 |      2.54% |
| **Total** |       **540,399** |   **100%** |

## Key Insights

1. Neutral sentiment represents the majority of the product descriptions at 77.26%.
2. Positive sentiment accounts for 20.20% of the descriptions.
3. Negative sentiment represents only 2.54%.
4. The analysis shows that most product descriptions contain neutral or descriptive language rather than strongly emotional language.
5. Positive sentiment is considerably higher than negative sentiment in the analyzed text.

## Visualizations

The project generates three visualizations:

### 1. Sentiment Distribution

A bar chart showing the number of Positive, Negative, and Neutral records.

### 2. Sentiment Percentage Distribution

A pie chart showing the percentage contribution of each sentiment category.

### 3. Sentiment Score Distribution

A histogram showing the distribution of sentiment scores.

## Technologies Used

* Python
* Pandas
* NLTK concepts / Natural Language Processing
* VADER Sentiment Analysis
* Matplotlib
* Seaborn
* Visual Studio Code
* GitHub

## Project Files

```text
CodeAlpha_Sentiment_Analysis/
│
├── online_retail.csv
├── cleaned_online_retail.csv
├── sentiment_analysis_results.csv
├── sentiment_analysis.py
├── sentiment_distribution.png
├── sentiment_percentage.png
├── sentiment_score_distribution.png
└── README.md
```

## Conclusion

This project demonstrates how Natural Language Processing and sentiment analysis can be applied to text data.

The analyzed product descriptions were classified into Positive, Negative, and Neutral categories using VADER sentiment analysis. The results and visualizations provide an overview of sentiment patterns present in the dataset.

## Important Dataset Note

The Online Retail dataset contains product descriptions rather than customer review comments. Therefore, the sentiment analysis in this project represents sentiment detected in product-description text and should not be interpreted as direct customer-review sentiment.
