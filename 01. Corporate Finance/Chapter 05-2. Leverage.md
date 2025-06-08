
# 1. Operating Leverage
- OL thể hiện cách thức sử dụng chi phí cố định (FC) để tác động đến sản lượng (Q) nhằm thay đổi lợi nhuận (EBIT) hoạt động sản xuất kinh doanh của DN
### 1.1. Degree of Operating Leverage (DOL)
- **Công thức 1:**
	- `DOL(Q(0)): mức độ ảnh hưởng của đòn bẩy kinh doanh tại sản lượng Q(0)`
	- `EBIT(Q(0)): lợi nhuận trước thuế và lãi vay tại mức sản lượng Q(0)`
	- `% ΔEBIT: % thay đổi về EBIT`
	- `% ΔSales: % thay đổi về sản lượng (hay doanh thu)`
	$$
	\begin{align} 
	DOL_{Q_0} = \frac{\% \ \Delta EBIT}{\% \ \Delta Sales} = \frac{\Delta EBIT / EBIT_{Q_0}}{\Delta Q / Q_0} = \frac{\Delta EBIT / EBIT_{Q_0}}{(p\cdot \Delta Q) / (p \cdot Q_0)}\\
	\end{align}
	$$
- **Ý nghĩa:** Tại mức sản lượng Q(0) hay mức doanh thu P * Q(0), khi sản lượng / doanh thu tăng 1% thì EBIT sẽ tăng DOL (%)
- **Công thức 2:**
	- `p x Q : Doanh thu`
	- `FC hoặc F : chi phí cố định (không gồm I vì I thuộc hđ tài chính)`
	- `VC : chi phí biến đổi`
	- `v : chi phí biến đổi trên 1 sản phẩm`
	- `Q(BEP): sản lượng hòa vốn (khi doanh thu = chi phí)`
	$$
	\begin{align}
	EBIT &= p \cdot Q - (FC + VC)\\
	&= p \cdot Q - (F + v \cdot Q)\\
	&= Q \cdot (p - v) - F\\
	=> \Delta EBIT &= \Delta Q \cdot (p - v)\\\\
	==> DOL_{Q_0} &= \frac{Q_0 \cdot (p - v)}{Q_0 \cdot (p - v)  - F} = \frac{EBIT_{Q_0} + F}{EBIT_{Q_0}}\\\\
	\end{align}
	$$

### 1.2. Mối quan hệ giữa DOL và BEP
- **Câu hỏi đặt ra:** Ta thấy FC càng lớn thì DOL càng lớn, vậy FC càng cao thì EBIT càng tốt?
$$
\begin{align}
Break\ Even\ Point &:\ p \cdot Q_{BEP} = v \cdot Q_{BEP} + F\\\\
==> DOL_{Q_0}&= \frac{Q_0}{Q_0 - \frac{F}{p-v}} = \frac{Q_0}{Q_0 - Q_{BEP}}
\end{align}
$$
![[break_even_point.png#center|480]]
- Khi ***Q(0) < Q(BEP)*** hay ***EBIT(Q(0)) < 0***   ==> DOL < 0 :
	- DN càng sản xuất thêm càng lỗ nhiều hơn
	- DN nào có FC cao hơn thì DN đó có mức giảm lỗ nhanh hơn
- Khi ***Q(0) > Q(BEP)*** hay ***EBIT(Q(0)) > 0***   ==> DOL > 0 :
	- DN càng sản xuất thêm càng lãi ít đi
	- DN nào có FC cao hơn thì DN đó có mức tăng trưởng lợi nhuận nhanh hơn
---
# 2. Financial Leverage
- FL thể hiện ở việc doanh nghiệp sử dụng vốn vay (Debt) nhằm gia tăng tỉ suất lợi nhuận trên vốn chủ sở hữu (ROE) hay thu nhập trên mỗi cổ phiếu (EPS) của DN
### 2.1. Degree of Financial Leverage (DFL):
- **Công thức 1:**
	$$
	\begin{align}
	DFL_{EBIT_0} &= \frac{\% \ \Delta ROE}{\% \ \Delta EBIT} = \frac{\Delta ROE / ROE_{EBIT_0}}{\Delta EBIT / EBIT_0}\\\\
	\text{(or)} &= \frac{\% \ \Delta EPS}{\% \ \Delta EBIT} = \frac{\Delta EPS / EPS_{EBIT_0}}{\Delta EBIT / EBIT_0}
	\end{align}
	$$
- **Ý nghĩa:** Tại mức EBIT(0), khi EBIT tăng 1% thì EPS hay ROE sẽ tăng DFL (%)
- **Công thức 2:**
	- `NI : Net Income (after Interest and Tax)`
	- `A = E + D (Assets = Equity + Debt)`
	- `I = D . i (Interest = Debt . interest_rate)` 
	- `t : CIT rate`
	- `PD: Preferred Dividends`
	- `NS : Number of Outstanding Common Shares`
	$$
	\begin{align}
	 EPS &= \frac{NI - PD}{NS} = \frac{(EBIT - I) \cdot (1-t) - PD}{NS}\\\\
	=> \Delta EPS &= \frac{\Delta EBIT \cdot (1-t)}{NS}\\\\\\
	==> DFL_{EBIT_0} &= \frac{EBIT_0 \cdot (1-t)}{(EBIT_0 - I) \cdot (1-t) - PD}
	\end{align}
	$$
---
### 2.2. Mối quan hệ giữa DFL và ROE
- **Return on Assets - ROA:** tỉ suất lợi nhuận ròng trên tổng tài sản (Equity + Debt)
	`--> cứ 1 đồng tài sản (VCSH + NPT) sẽ có ROA đồng lợi nhuận ròng`
- **Return on Equity - ROE:** tỉ suất lợi nhuận ròng trên vốn chủ sở hữu là chỉ số quan trọng nhất đối với các cổ đông 
	`--> cứ 1 đồng VCSH sẽ có ROE đồng lợi nhuận ròng`
- **Operating ROA - OROA:** tỉ suất EBIT trên tổng tài sản
$$
\begin{align}
ROA &= \frac{NI}{A} = \frac{NI}{E + D} = \frac{ROE}{1 + D/E}\\\\
ROE &= \frac{NI}{E} = \frac{NI}{A - D} = \frac{ROA}{1 - D/A}\\\\
OROA &= \frac{EBIT}{A}
\end{align}
$$
---
- **Mối quan hệ giữa OROA và ROE:**
	$$
	\begin{align}
	ROE &= \frac{NI}{E} = \frac{(EBIT - D \cdot i) \cdot (1-t)}{E}\\\\
	&= \frac{(OROA \cdot A - D \cdot i) \cdot (1-t)}{E}\\\\
	&= (OROA + \frac{OROA \cdot D - D \cdot i}{E}) \cdot (1-t)\\\\
	&= [\ OROA + \frac{D}{E} \cdot(OROA - i)\ ] \cdot (1-t)
	\end{align}
	$$
	- ***Khi OROA > i :*** 
		`<< OROA (đồng lợi nhuận trước lãi vay sinh ra từ 1 đồng tài sản) > i (đồng chi phí lãi vay sinh ra từ 1 đồng vay nợ) >>`
		- Khi vay càng nhiều thì lợi nhuận sau lãi vay càng tăng -> ROE càng tăng -> DFL có lợi
	- ***Khi OROA < i :*** 
		`<< OROA (đồng lợi nhuận trước lãi vay sinh ra từ 1 đồng tài sản) < i (đồng chi phí lãi vay sinh ra từ 1 đồng vay nợ) >>`
		- Khi vay càng nhiều thì lợi nhuận sau lãi vay càng giảm -> ROE càng giảm -> DFL có hại
	- ***Khi OROA = i :*** 
		`<< OROA (đồng lợi nhuận trước lãi vay sinh ra từ 1 đồng tài sản) = i (đồng chi phí lãi vay sinh ra từ 1 đồng vay nợ) >>`
		- Dù vay như thế nào thì lợi nhuận trước và sau lãi vay như nhau
---
### 2.3. Mối quan hệ giữa DFL và EBIT
- **Câu hỏi đặt ra:** Ta thấy vay càng nhiều thì DFL càng lớn, vậy vay càng nhiều thì EPS sẽ càng cao?
$$
\begin{align}
Indifference\ Point:\quad EPS_1 &= EPS_2\\\\
<=> \frac{(EBIT' - I_1)\cdot(1-t) - PD_1}{NS_1} &= \frac{(EBIT' - I_2)\cdot(1-t) - PD_2}{NS_2}
\end{align}
$$
![[indifference_point.jpg#center|480]]
- Nếu ***EBIT < EBIT'*** thì nên phát hành **cổ phiếu** `<< nếu vay càng nhiều mà EBIT không đủ lớn để bù đắp chi phí lãi vay, thì EPS phải càng giảm để bù đắp >>`
- Nếu ***EBIT > EBIT'*** thì nên phát hành **trái phiếu**
---
# 3. Total Leverage
### 3.1. Degree of Total Leverage (DTL)
- **Công thức:**
	$$ 
	\begin{align}
	DTL &= DOL \cdot DFL \\\\
	&= \frac{\% \ \Delta EBIT}{\% \ \Delta Sales} \cdot \frac{\% \ \Delta EPS}{\% \ \Delta EBIT}\\\\
	&= \frac{EBIT_{Q_0} + F}{EBIT_{Q_0}} \cdot \frac{EBIT_{Q_0} \cdot (1-t)}{(EBIT_{Q_0} - I) \cdot (1-t) - PD}\\\\
	&= \frac{(EBIT_{Q_0} + F) \cdot (1-t)}{(EBIT_{Q_0} - I) \cdot (1-t) - PD}
	\end{align}
	$$
- **Ý nghĩa:** Tại mức sản lượng Q(0) hay doanh thu p * Q(0), khi sản lượng/doanh thu tăng 1% thì EPS sẽ tăng DTL (%)

