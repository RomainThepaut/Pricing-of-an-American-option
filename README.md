# **American Option Pricing using Monte Carlo and Longstaff-Schwartz Regression**  

## 📌 **Project Overview**  
This project focuses on pricing American options (both call and put) using the **Monte Carlo simulation** combined with the **Longstaff-Schwartz regression method**. The underlying asset follows a **Black-Scholes dynamic**, and the pricer allows flexibility in configuration to analyze different scenarios.  

## 🛠 **Features**  
✅ **Customizable Regression Degree** – Users can select the polynomial degree for the regression step.  
✅ **Flexible Path Selection** – Choose to include all trajectories or only in-the-money trajectories.  
✅ **European vs. American Option Pricing** – Compare the calculated price of an American option with its European counterpart.  
✅ **Confidence Interval Analysis** – Assess the impact of the number of simulations on pricing accuracy.  

## 📊 **Mathematical Model**  
The underlying asset follows the Black-Scholes model:  
$dS_t = (r - q) S_t dt + \sigma S_t dW_t$
 
where:  
- $\( S_t \)$ is the asset price,  
- $\( r \)$ is the risk-free interest rate,  
- $\( q \)$ is the continuous dividend yield,  
- $\( \sigma \)$ is the volatility,  
- $\( dW_t \)$ is a Wiener process.  

## 🚀 **How It Works**  
1. Simulate multiple asset price paths using Monte Carlo.  
2. Apply **Least-Squares Monte Carlo (LSM)** with **Longstaff-Schwartz regression** to estimate the optimal exercise strategy.  
3. Compare American option values to European option prices.  
4. Analyze the impact of simulation count on pricing confidence.  

## 📂 **Project Structure**  
```
📁 AmericanOptionPricer  
 ┣ 📂 src              # Core implementation  
 ┣ 📂 notebooks        # Jupyter notebooks for visualization  
 ┣ 📂 data             # Sample simulation results  
 ┣ 📄 README.md        # Project documentation  
 ┣ 📄 requirements.txt # Dependencies  
 ┗ 📄 main.py          # Execution script  
```  

## ⚡ **Getting Started**  
1️⃣ **Clone the repository**  
```bash
git clone https://github.com/yourusername/AmericanOptionPricer.git
cd AmericanOptionPricer
```  
2️⃣ **Install dependencies**  
```bash
pip install -r requirements.txt
```  
3️⃣ **Run the pricing script**  
```bash
python main.py
```  

## 📈 **Results & Insights**  
The implementation provides a clear visualization of how different factors (regression degree, path selection, number of simulations) influence American option pricing.  

## 📬 **Contributions & Feedback**  
Feel free to contribute by submitting a pull request or opening an issue. Any feedback is highly appreciated! 🚀
