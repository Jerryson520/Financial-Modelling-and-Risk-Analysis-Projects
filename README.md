# Financial-Modelling-and-Risk-Analysis-Projects
## 1. SOFR Futures Pricing and Swap Rate Calculation
### Task Summary:

1. **Objective:**
   - Calculate the market forecast of the 3-month SOFR rate using SOFR futures prices for the first 12 contracts (with maturities in March, June, September, and December).
   - Use linear interpolation to estimate the 3-year fixed-floating swap rate starting on the spot date (February 28, 2024).
   - Compute the DV01 (Dollar Value of 1 basis point) of the swap for different payment conventions.

2. **Steps:**
   - **Market Forecast of SOFR Rate:**
     - Identify the maturity dates of the first 12 SOFR futures contracts, which mature on the third Wednesday of March, June, September, and December.
     - Use the last quoted prices of the SOFR futures contracts to estimate the market's forecast of the 3-month SOFR rate on those maturity dates.

   - **Linear Interpolation:**
     - Apply linear interpolation to forecast the 3-year fixed-floating swap rate based on the quarterly 3-month SOFR rates.

   - **Swap Rate Calculation and DV01 Determination:**
     - **Case 1: Quarterly Fixed/Quarterly Floating (Money Market Basis):** 
       - Calculate the fixed rate and DV01 assuming both the floating rate (3-month SOFR) and the fixed rate are paid quarterly, using the money market convention.
     - **Case 2: Semi-Annual Fixed/Quarterly Floating (Bond Basis Actual/365):**
       - Calculate the fixed rate and DV01 when the floating rate is paid quarterly, but the fixed rate is paid semi-annually on an Actual/365 bond basis.
     - **Case 3: Semi-Annual Fixed/Quarterly Floating (Bond Basis 30/360):**
       - Calculate the fixed rate and DV01 when the floating rate is paid quarterly, but the fixed rate is paid semi-annually on a 30/360 bond basis.

3. **Key Outputs:**
   - **Market Forecast of SOFR Rates:** Estimated 3-month SOFR rates on the maturity dates of the first 12 SOFR futures contracts.
   - **3-Year Swap Rates:** Fixed swap rates under different payment conventions (Quarterly/Money Market, Semi/Bond Actual/365, and Semi/Bond 30/360).
   - **DV01 of the Swap:** The sensitivity of the swap value to a 1 basis point change in interest rates for each payment convention.

This task involves both forecasting interest rates from futures contracts and determining the fixed rates and sensitivities for various types of interest rate swaps.

## 2. Discriminant Analysis of Energy vs. Tech Companies using SVM
**Objective:**

- Perform a discriminant analysis to identify which financial ratios can best differentiate between companies in the energy and technology sectors.
- Apply linear discriminant function or Support Vector Machines (SVM) to determine which pair of financial ratios has the best discriminating power.
- Compute the confusion matrix for evaluating the classification performance.

**Steps:**

1. **Company Groups:**
   - **Energy Sector:**  
     Occidental Petroleum (OXY), Exxon-Mobil (XOM), British Petroleum (BP), China Petroleum and Chemical (SNP), ConocoPhillips (COP), Eni (E), Total (TTE), Chevron (CVX)

   - **Technology Sector:**  
     Meta, formerly Facebook (FB), Apple (AAPL), Amazon (AMZN), Microsoft (MSFT), Alphabet (GOOG), Netflix (NFLX), International Business Machines (IBM)

2. **Accounting Ratios Considered:**
   - Current Ratio
   - Long-term debt to Total Assets
   - Return on Assets (ROA)
   - Return on Equity (ROE)

3. **Discriminant Analysis:**
   - Determine which of the accounting ratios has the strongest discriminating power between the two industry sectors.
   - Use linear discriminant function or SVM to assess the discriminating power of each ratio.
   - Compute the confusion matrix to evaluate the classification performance of the chosen models.

**Key Outputs:**

- **Best Discriminating Factor:**  
  Identify which financial ratio provides the best classification between energy and technology companies.

- **Confusion Matrix:**  
  Assess classification performance using the confusion matrix to understand prediction accuracy for the selected model.


## 3. Efficient Frontier Simulation and Portfolio Optimization in Python
**Objective:**

- Analyze the daily closing prices of specific stocks to calculate key financial metrics and construct efficient frontiers.
- Apply regression analysis to determine the Capital Asset Pricing Model (CAPM) factors α and β for each stock relative to the S&P 500 (SPY).

**Steps:**

1. **Stocks Considered:**
   - Apple Computers (AAPL)
   - Pfizer (PFE)
   - Consolidated Edison (ED)
   - ExxonMobil (XOM)
   - American Water Works (AWK)
   - S&P 500 (SPY) as the market index

2. **Analysis Tasks:**
   - Calculate the average daily return and annual volatility for each of the selected stocks.
   - Determine the covariance and correlation matrix of the daily returns for the stocks.
   - Perform regression analysis of the daily return of each stock against the S&P 500 (SPY) to compute the α (alpha) and β (beta) values.
   - Draw the efficient frontier for the following portfolios:
     - Portfolio 1: AAPL and PFE (only long positions)
     - Portfolio 2: ED, XOM, and AWK (only long positions)
     - Portfolio 3: AAPL, PFE, ED, XOM, and AWK (only long positions)
   - Combine and draw all three efficient frontiers on one graph for comparison.

**Key Outputs:**

- **Financial Metrics:**
  - Average daily return and annual volatility of each stock.
  - Covariance and correlation matrix of daily returns.
  - Regression results for α and β values of each stock relative to the S&P 500.

- **Efficient Frontiers:**  
  Three efficient frontiers, showing the risk-return trade-off for different portfolio combinations of the selected stocks.
