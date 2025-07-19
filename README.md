# ML Stock Price Prediction

The goal of this project is to analyze historical stock data, build a prediction model using ML techniques, and visualize trends to understand market behavior.



## Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn  
- Jupyter Notebook  


## Dataset

Two datasets were used:

1. **`prices.csv`** – Contains:
   - `date`, `symbol`, `open`, `close`, `low`, `high`, `volume`

2. **`securities.csv`** – Contains:
   - `Ticker Symbol`, `Security`, `SEC filings`, `GICS Sector`, `GICS Sub Industry`, `Headquarters Address`, `Date First Added`, `CIK`

---

## Project Workflow

### Step 1: Data Preprocessing
- Checked for null values — none found.

### Step 2: Model Building
- Applied PCA (Principal Component Analysis).
- Found that the `open` column explains ~99% of the variance.
- Used `open` column to build a **Linear Regression** model.

### Step 3: Evaluation & Visualization
- Model accuracy ≈ **99.98%**.
- A function allows users to enter a ticker symbol and view:
  - Actual vs Predicted price graph
  - Company info (sector, address, etc.)
  - Summary: accuracy, highest/lowest actual and predicted prices

---

## Future Improvements

- Add time series forecasting (e.g., LSTM, ARIMA)
- Use additional features (market indicators, sentiment analysis)
- Deploy using Streamlit or Flask for interactivity

---

## Colab Link to See the Output:
[Open in Google Colab](https://colab.research.google.com/drive/1N1rxdrQQhEmqUUTZldCHxMJuDnjfvY-y?usp=sharing)
