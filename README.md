# Sales Analysis of AAL Company (4th Quarter 2020)

## Project Overview
AAL, established in 2000, is a well-known brand in Australia, especially recognized for its clothing business. The company operates in various states and caters to a wide demographic. Due to a surge in business, AAL is expanding and seeking data-driven insights for the 4th quarter of 2020 to aid in their decision-making process. The CEO has tasked the head of sales and marketing (S&M) with analyzing the sales data and making informed investment decisions.

### Objectives:
1. Identify states generating the highest and lowest revenues.
2. Provide insights and recommendations for improving sales in lower-performing states.
3. Provide weekly, monthly, and quarterly reports.
4. Develop a dashboard to visualize key sales metrics (state-wise, group-wise, and time-of-day sales analysis).
5. Use data wrangling, statistical analysis, and visualization to assist in sales strategy development.

## Steps Performed

### 1. Data Wrangling

Data wrangling is the process of cleaning and transforming the raw data into a usable format. In this project, the following steps were performed:
- **Missing Values Handling**: Identified and handled missing data using mean imputation for the 'Sales' column and standard methods for other columns where appropriate.
- **Date Parsing**: Standardized the `Date` column into the datetime format.
- **Normalization**: Applied Min-Max normalization to the `Sales` column to bring all data points into a uniform scale.
- **Duplicate Handling**: Removed any duplicate or null values that might interfere with analysis.

### 2. Data Analysis

Performed the following statistical analysis:
- **Descriptive Statistics**: Calculated mean, median, mode, and standard deviation for `Sales` and `Unit` columns.
- **Sales Grouping**: Grouped sales data by `State` and `Group` (e.g., kids, women, men, seniors) to identify trends.
- **Revenue Insights**: Analyzed which states have the highest and lowest revenues.
- **Sales by Group**: Identified which demographic group generated the highest and lowest sales.
- **Unit Analysis**: Conducted similar analysis for `Unit` to understand product sales patterns.

### 3. Data Visualization

Visualized the data to provide insights through the following charts and plots:
- **State-wise Sales Analysis by Group**: Used bar charts to show how sales vary by group across different states.
- **Group-wise Sales Across States**: Created a heatmap to display sales data for each group across all states.
- **Time-of-the-Day Sales**: Analyzed sales across different times of the day to identify peak and off-peak sales periods.
- **Sales Trends**: Generated line charts for daily, weekly, monthly, and quarterly sales trends.

#### Visualization Tools:
- **Seaborn**: Used for creating informative plots such as bar charts, heatmaps, and line charts.
- **Matplotlib**: Used to enhance visualizations and ensure clarity.

### 4. Report Generation

- **Jupyter Notebook**: The analysis was done in a Jupyter Notebook, where code and visualizations are integrated. This notebook also includes markdown cells with explanations of the steps and insights.
- **Markdown**: The report is structured with markdown to explain the purpose, methodology, and results clearly.

## Data File

The dataset used in this project is named `AusApparalSales4thQrt2020.csv`, and it contains the following key columns:
- `Date`: The date of the sale transaction.
- `State`: The state in which the sale occurred.
- `Group`: The demographic group (e.g., kids, women, men, seniors).
- `Sales`: The sales amount for that transaction.
- `Unit`: The number of units sold.

## Tools & Libraries Used

- **Python**: The programming language used for data analysis and visualization.
- **Pandas**: For data manipulation and analysis (e.g., handling missing values, grouping).
- **NumPy**: For numerical operations.
- **Matplotlib**: For creating static, animated, and interactive visualizations.
- **Seaborn**: For advanced visualizations like heatmaps and statistical plots.
- **JupyterLab**: Used for code execution and report generation.

## Installation and Setup

To replicate this project on your local machine, please follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/sdeepak001/sales-analysis-AAL.git
   cd sales-analysis-AAL
   ```
2. **Install dependency**:
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the Code**:
   ```bash
   jupyter notebook Sales_Analysis.ipynb
   ```

