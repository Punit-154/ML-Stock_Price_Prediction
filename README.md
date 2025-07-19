# ML-Stock_Price_Prediction
This is my first ML project,Predicting the stock prices,over a period of time
The goal of this Project is to understand and predict the stock prices of various companies using past data and visualizing the graphs in order to understand the market trend

**Technologies Used**
1)Python 
2)Pandas
3)Numpy
4)Matplotlib
5)Scikit-learn
6)Jupyter Notebook
**Dataset**
The dataset prices.csv contains data such as Date, symbol, Open, Close, Low, High, Volume.
The dataset securities.csv contains data such as Ticker Symbol, Security, SEC filings, GICS Sector, GICS Sub Industry, Address of Headquarters, Date first added, CIK
**Project Working**
Step-1:Data Preprocessing
    The data is first checked for presence of null values.In this data,no null values are present
Step-2:Model Building
    PCA(Principle Component Analysis) feature analysis is applied and we find that the "Open" columns explains about 99% of the data 
    Hence the "Open" columns has been used in order to save time and resources sent during computing
    A Linear regrssion model is applied in order to predict the price
Step-3:Evaluation & Visualization
  The accuracy of the model is predicted and is estimated to be around 99.98%
  A function was created which allowed the user to input company Ticker Symbols and pplot the graph between the predicted prices and actual prices
  Along with the graph,all the details of the company was added along wiht its accuracy,highest and lowest predicted price and actual price


**Future Improvements**
  Add support for time series forecasting (e.g., LSTM, ARIMA)
  Include more features like market indicators or sentiment analysis
  Host the notebook using Streamlit or Flask for an interactive UI
