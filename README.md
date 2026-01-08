# 📈 TCS Stock Price Analysis & Dashboard

## Overview
This project analyzes **multi-year stock market data** using **EDA, feature engineering, and predictive modeling**, and presents insights through an interactive Power BI dashboard.

---

## Dataset
Daily stock data with key features:
- `Date`, `Open`, `High`, `Low`, `Close`, `Volume`

---

## Data Preparation & EDA
- Cleaned and validated daily stock data
- Explored price trends, volatility, and volume behavior
- Visualized Close price over time

---

## Feature Engineering
- Rolling Mean indicators (MA50, MA200)  
- Previous Day Close (`Prev_Close`) as a lag feature  
- Month and Day of Week extracted from Date  

These features capture temporal dependencies and trends for predictive modeling.

---

## Modeling
- **Time-based train–test split** was performed to preserve chronological order and avoid data leakage 
- Models explored: **Linear Regression, Ridge Regression, Random Forest, Gradient Boosting, ARIMA**   
- **Cross-validation** was used to assess model stability before final selection  

**Model Insights:**  
- Linear and Ridge Regression showed similar performance  
- Linear Regression was selected for its simplicity, interpretability, and competitive performance

---

## Dashboard
An interactive **Power BI dashboard** was created, featuring:

**Cards**
- Latest Close Price
- Highest Price (selected period)
- Lowest Price (selected period)
- Average Volume

**Charts**
- Line chart: Close Price with rolling means (MA50, MA200) over time  
- Column chart: Volume over time

**Interactivity**
- Year-based slicer  
- DAX measures for latest Close, month extraction, and slicer-aware card values

---

## Tools & Technologies
- **Python**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Statsmodels  
- **Power BI**: Data modeling, DAX measures, dashboard creation  

---

## Key Takeaways
- Feature engineering significantly improved predictive performance  
- Linear models performed as well as more complex models due to strong linearity  
- Time-aware splitting and cross-validation are critical in stock prediction tasks  
- Interactive dashboards enhance interpretability and stakeholder communication  

---

## Note on AI Assistance
> AI tools were used to assist in drafting this README.
