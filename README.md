# Financial-Training-for-Deep-Neural-Networks

## 📈 Description

This project explores various Neural Network (NN) architectures with the goal of **maximising the Sharpe Ratio (SR)**—a key financial performance metric—rather than minimising traditional loss functions like Mean Squared Error (MSE). Through empirical research, it's evident that directly optimising a financial objective leads to better trading performance than simply forecasting prices.

The NNs are trained to output **asset allocation values**, where:
- `0.1` indicates investing 10% of the portfolio
- `-0.1` indicates selling or shorting 10%

The models are benchmarked against the **S&P 500 index (^GSPC)**, aiming to outperform it in both return and risk-adjusted performance.

Using historical financial data, a carefully engineered set of input features, and backtesting, this project assesses how well deep learning models can learn trading strategies that beat market performance while maintaining a strong SR.

---

## 🚀 Features

- Custom cost function to optimise **Sharpe Ratio directly**
- Allocation-based output (continuous value from -1 to 1)
- Models include:
  - Single-layer Perceptron (SLP)
  - Multi-layer Perceptron (MLP)
  - Deep Learning Model (DLM)
- Feature engineering based on:
  - Returns
  - Volatility
  - Simple Moving Average (SMA)
  - Exponential Moving Average (EMA)
  - Smoothing factor
- Full backtesting and evaluation

---

## 🛠️ Tech Stack

- Python  
- NumPy, Pandas, Matplotlib  
- Financial data APIs (Yahoo Finance via `yfinance`)

---

## 📄 Project Paper

You can read the full research paper describing the methodology, experiments, and results: [Google Drive Link] (https://drive.google.com/file/d/1zZjJt8Cyc4BDlycIQg1VkMKlk4_8XJg6/view?usp=sharing)

---

## 📥 Installation

```bash
git clone https://github.com/CanGuv/Financial-Training-for-Deep-Neural-Networks.git
cd Financial-Training-for-Deep-Neural-Networks
pip install -r requirements.txt
