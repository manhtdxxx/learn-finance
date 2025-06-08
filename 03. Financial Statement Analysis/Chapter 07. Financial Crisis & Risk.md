# 1. Financial Crisis
- Đặc điểm khủng hoảng tài chính là sự mất cân đối giữa khả năng và nhu cầu thanh toán nợ ngắn hạn của DN.
- DN lâm vào khủng hoảng tài chính → giá trị giảm sút, rủi ro tăng cao.
### 1.1. Đánh giá từng chỉ số (William Beaver)
- **Objective:**  
	- To identify financial ratios that can predict a company’s failure (bankruptcy) in advance.
- **Approach:**
	- ***Univariate analysis*** of financial ratios.
	- Evaluated each ratio ***independently*** to see how well it could differentiate between failed and non-failed firms.
	- Introduced the concept of a ***cut-off point*** (threshold) for each ratio to classify firms as healthy or distressed.
- **Result:**
	- Found that some ratios were good predictors of bankruptcy ***several years (up to 5) in advance***.
	- Established that ***financial distress is a process***, not a one-time event.
- **Key Financial Ratios:**

| Ratio                             | Interpretation                                                          |
| --------------------------------- | ----------------------------------------------------------------------- |
| *Net Income / Total Assets (ROA)* | Profitability – earning power relative to assets                        |
| *Debt / Total Assets*             | Leverage – how much of the firm is financed by debt                     |
| *Cash Flow / Total Debt*          | Liquidity – ability to cover debt with internal funds                   |
| *Current Ratio*                   | Ability to pay short-term obligations                                   |
| *Working Capital / Total Assets*  | Short-term financial health (WC = Current Assets - Current Liabilities) |

---
### 1.2. Kết hợp các chỉ số (Edward Altman)
- **Objective:**  
	- To develop a ***multivariate model*** that combines several financial ratios into a single score to predict corporate bankruptcy.
- **Approach:**
	- ***Multivariate Discriminant Analysis (MDA)*** to find a linear combination of variables that best separates bankrupt from non-bankrupt firms.
	- More comprehensive than Beaver’s univariate method.
- **Result:**
	- High predictive accuracy (~70-80%) for bankruptcy within 1-2 years.
	- Used ***mainly for manufacturing firms***, but there are variations for private firms, non-manufacturers, and emerging markets.
- **Altman Z-score:**

| Variable | Definition                                        |
| -------- | ------------------------------------------------- |
| X1       | *Working Capital / Total Assets*              |
| X2       | *Cumulative Retained Earnings / Total Assets* |
| X3       | *EBIT / Total Assets*                         |
| X4       | *Market Capitalization / Total Liabilities*   |
| X5       | *Sales / Total Assets*                        

$$
\begin{align}
Z &= 1.2 X_1 + 1.4 X_2 + 3.3 X_3 + 0.6 X_4 + 0.999 X_5\\\\
\end{align}
$$
- **Z-score Range:**
	- ***Z < 1.81:***  Distress Zone - High risk of bankruptcy
	-  ***Z > 2.99:***  Safe Zone - Low risk of bankruptcy
	- ***1.81 < Z < 2.99:***  Grey Zone - Some risk, caution 
# 2. Risk
### 2.1. Business Risk
### 2.2. Financial Risk