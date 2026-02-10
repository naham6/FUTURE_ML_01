# Retail Sales & Demand Forecasting Tool

Building a bridge between historical data and future inventory needs. This tool helps retail businesses optimize their stock levels by predicting daily sales, effectively balancing the risk of overstocking against the cost of lost sales.

---

## 📊 Project Overview

The core objective is to leverage transactional data to forecast demand. By identifying patterns in daily sales—especially during high-pressure periods like the holidays—this tool provides actionable insights for smarter inventory management.

## 📁 Dataset

We utilize the **Online Retail Dataset** from the UCI Machine Learning Repository.

* **Source:** [UCI Online Retail Dataset](https://archive.ics.uci.edu/dataset/352/online+retail)
* **Context:** A transnational dataset containing transactions from a UK-based non-store online retail firm.
* **Timeframe:** December 1, 2010 – December 9, 2011.
* **Scale:** Over 540,000 transaction records.

---

## 🛠 Technical Implementation

The project is built using **Python** within a **Jupyter Notebook** environment. The workflow is divided into three critical phases:

### 1. Data Cleaning

Raw retail data is often "noisy." We ensure accuracy by:

* Filtering out missing Customer IDs.
* Removing duplicate transaction entries.
* Rectifying negative quantity values (returns/adjustments) to ensure a clean baseline for forecasting.

### 2. Feature Engineering

We transform raw inputs into predictive signals, specifically by calculating **Total Purchase Amounts** per transaction to weigh the financial impact of different products and timeframes.

### 3. Exploratory Data Analysis (EDA)

Understanding the "who" and "where" before predicting the "when."

* **Geographic Spread:** Most transactions originate from the UK, with significant volume from Germany and France.
* **Customer Segmentation:** Identifying "Whale" customers (e.g., ID 15098) who drive high-volume individual purchases.

### 📚 Tech Stack

* **Core:** `pandas`, `numpy`
* **Visualization:** `matplotlib`, `seaborn`
* **Time Series:** `datetime`

---

## 💡 Key Insights

* **Volume:** The dataset's size (540k+ records) allows for robust statistical modeling.
* **Concentration:** A small percentage of high-value customers significantly influence total revenue.
* **Seasonality:** Clear trends emerge during the Q4 holiday season, necessitating higher safety stock levels.

---

## 🤖 Machine Learning Models
I mplemented and compared two regression models to determine the most accurate forecasting approach:

**Linear Regression:** Provides a baseline for sales trends.

**Random Forest Regressor:** Captures non-linear patterns and complex interactions in the data.

**Evaluation:**

**Metric:** Mean Absolute Error (MAE)

**Result:** The Random Forest model achieved a lower MAE, making it the preferred choice for this dataset.

## 🚀 How to Run

1. **Clone the Repository:**
```bash
git clone https://github.com/naham6/FUTURE_ML_01.git

```


2. **Install Dependencies:**
```bash
pip install -r requirements.txt

```


3. **Prepare the Data:**
Download the dataset from the UCI link and place the `.xlsx` or `.csv` file in the project root directory.
4. **Execute the Analysis:**
Open and run all cells in `Sales_Forecasting.ipynb`.

