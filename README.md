Retail Sales & Demand Forecasting Tool
Project Overview
The goal of this project is to build a forecasting tool to help retail businesses plan inventory more effectively. By predicting daily sales, we aim to reduce the risks of overstocking while ensuring sufficient supply for high-demand periods, such as the holidays.

Dataset
The project utilizes the Online Retail dataset from the UCI Machine Learning Repository.

Data Source: UCI Online Retail Dataset

Description: This is a transnational dataset which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail.

Technical Implementation
The analysis is performed using Python in a Jupyter Notebook environment. Key steps include:

Data Cleaning: Handling missing customer IDs, removing duplicate entries, and correcting negative quantity values.

Feature Engineering: Calculating total purchase amounts per transaction.

Exploratory Data Analysis (EDA): Visualizing top customers by total purchase amount and identifying sales trends.

Libraries Used: pandas, numpy, matplotlib, and datetime.

Key Insights
The dataset contains over 540,000 transaction records.

The analysis identifies high-value customers, such as Customer ID 15098, who made significant individual purchases.

Most transactions originate from the United Kingdom, followed by Germany and France.

How to Run
Clone this repository.

Install dependencies: pip install -r requirements.txt.

Download the dataset from the link above and place it in the project directory.

Run the Retail_Sales_Forecasting.ipynb notebook.
