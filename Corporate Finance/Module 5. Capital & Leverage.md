# 1. Cost of Capital
- Chi phí sử dụng vốn là cái giá mà doanh nghiệp phải trả cho việc sử dụng nguồn tài trợ (bao gồm cả chi phí cơ hội). 
- Chi phí sử dụng vốn cũng có thể được xem là **tỷ suất sinh lời mà các nhà cung ứng vốn trên thị trường yêu cầu doanh nghiệp phải trả** nhằm đảm bảo sự tài trợ vốn của họ đối với DN
---
### 1.1. Cost of Debt
- Khi đi vay, phần lợi nhuận khi tính thuế TNDN sẽ không tính phần lãi vay
- Chi phí sử dụng vốn vay là *tỷ lệ chiết khấu (i)* làm cân bằng *dòng tiền (CF) mà DN phải thanh toán cho chủ nợ* trong tương lai và *khoản nợ vay (P)* mà DN vay hiện tại
##### 1.1.1. Before Tax
- Hàng năm, sẽ trả dần khoản vay gồm tiền gốc lẫn tiền lãi
$$ P = \sum_{t=1}^n \frac{CF_t}{(1+i)^t}$$

- Khi các khoản phải trả hằng năm không đổi:
$$P = CF \cdot \frac{1-(\frac{1}{1+i})^n}{i}$$
##### 1.1.2. After Tax
- Do Cost of Equity vẫn bị tính thuế TNDN nên để có thể so sánh được chi phí sử dụng từ các nguồn vốn khác nhau thì cần có cơ sở đồng nhất
$$i\ \ AFTER\ \ tax \ =\  i\ \ BEFORE\ \ tax \cdot (1 - CIT\ rate)$$
 `Nếu DN làm ăn thua lỗ thì sẽ không phải nộp thuế ==> CIT rate = 0%`
 
---
### 1.2. Cost of Equity
##### 1.2.1. Common Share
1. **Cổ phiếu thường**
	$$P =\sum_{t=1}^n \frac{D_t}{(1+i)^t}$$
	- *Theo mô hình tăng trưởng không đổi (Gordon growth model):*
	$$P = \frac{D_0 \cdot (1+g)}{i - g} \  \ => \ \ i  = \frac{D_1}{P} + g$$
	- *Theo mô hình CAPM (Capital Asset Pricing Model)*
		- **Rf** : Lãi suất phi rủi ro (Risk Free Rate)
			- Là loại lãi suất mà tại đó, tỷ lệ rủi ro của tài sản gần bằng 0
			- Thường thì sẽ được lấy bằng lãi suất trái phiếu chính phủ kỳ hạn 10 năm
		- **Beta** là đại được đo lường mức độ biến động của cổ phiếu so với thị trường chung
			- Nếu một tài sản có beta = 1, nó sẽ biến động theo thị trường
			- Nếu beta > 1, nó biến động mạnh hơn so với thị trường
			- Nếu beta < 1, nó biến động yếu hơn so với thị trường
		- **Risk Premium** là khoản thưởng khi bạn đầu tư vào cổ phiếu (rủi ro cao), so với cầm giữ các tài sản khác (có rủi ro thấp)
		- **Rm** : Tỷ suất sinh lời kỳ vọng của thị trường (Required Market Return)
		$$
		\begin{align}
		k_e &= r_f + Beta \cdot Risk\ Premium\\
		&= r_f + Beta \cdot (r_m - r_f)
		\end{align}
		$$
	---
1. **Cổ phiếu thường mới phát hành**
	- Khi phát hành một cổ phiếu mới thì sẽ phát sinh thêm chi phí mới: in ấn, bảo lãnh phát hành, môi giới, ... Vì vậy cần phải tính giá ròng cho cổ phiếu đó
	$$Giá\ ròng = Giá\ phát\ hành \cdot (1- Tỷ\ lệ\ chi\ phí\ phát\ hành)$$
	- Theo mô hình tăng trưởng không đổi (Gordon growth model):
	$$i = \frac{D_1}{Giá\ ròng} + g$$
---
##### 1.2.2. Preferred Share
- Người sở hữu cổ phiếu ưu đãi chỉ nhận được cổ tức ưu đãi cố định hằng năm
$$P = \frac{D}{i} \ \ =>\ \ i  = \frac{D}{P}$$
---
##### 1.2.3. Retained Earnings
- Đo lường bằng chi phí cơ hội, thể hiện rằng lợi nhuận nếu được chia cho các cổ đông thì họ có thể dùng số tiền đó để đầu tư nơi khác và thu lợi nhuận
**==>** Chi phí sử dụng lợi nhuận để lại chính là chi phí sử dụng cổ phần thường
$$i  = \frac{D_1}{P} + g$$

---
### 1.3. Weighted Average Cost of Capital (WACC)
 - Để đủ vốn kinh doanh thì DN cần phải huy động từ nhiều nguồn vốn khác nhau và mỗi nguồn sẽ có chi phí sử dụng khác nhau. Do đó ta cần xác định chi phí sử dụng bình quân của các nguồn đó
 - **Công thức :**
	 - `w(i): tỉ trọng của nguồn vốn thứ i`
	 - `k(i): chi phí sử dụng nguồn vốn thứ i`
	 - `t(i): vốn của nguồn i được sử dụng`
	 - `T: tổng số vốn từ các nguồn`
	 $$WACC = \sum_{i=1}^n w_i \cdot k_i \  = \  \sum_{i=1}^n \frac{t_i}{T} \cdot k_i$$
---
### 1.4. Marginal Cost of Capital (MCC)
- Chi phí sử dụng vốn cận biên là chi phí cho đồng vốn mới nhất tăng thêm khi doanh nghiệp huy động đầu tư cho hoạt động kinh doanh (**WACC đạo hàm theo t(i), T**)
- DN sẽ huy động vốn có chi phí thấp trước (lợi nhuận giữ lại, nợ lãi suất thấp, ...). Tuy nhiên, khi DN đạt đến giới hạn của những nguồn giá rẻ này (hết lợi nhuận giữ lại, nợ thêm sẽ tăng lãi, ...) và cần phát hành cổ phiếu mới, chi phí sẽ tăng vọt vì vốn chủ sở hữu thường có chi phí cao hơn nợ. Bước nhảy này sẽ phản ánh được mối quan hệ phi tuyến tính
- **Điểm gãy** - **Break Point** là điểm mà số vốn mới có thể huy động được trước khi MCC nhảy vọt
$$Break\ Point\ i = \frac{Tổng\ giá\ trị\ của\ nguồn\ vốn\ i}{Tỷ\ trọng\ của\  nguồn\ vốn\ i}$$
**==>** DN có thể huy động vốn tới Break-Point (Tổng số vốn mới) mà không thay đổi WACC, sau đó nếu muốn tăng vốn, thì WACC sẽ nhảy vọt
![[MCC.png#center|480]]

---
# 2. Capital Structure
##### 2.1. Concepts
- Vốn kinh doanh của DN được hình thành từ 2 nguồn:
	- Vốn chủ sở hữu
	- Nợ phải trả
$$
\begin{align}
Hệ\ số\ VCSH &= \frac{VCSH}{Tổng\ nguồn\ vốn} =\ \ 1 - Hệ\ số\ nợ\\\\
Hệ\ số\ nợ &= \frac{NPT}{Tổng\ nguồn\ vốn} = \ \ 1 - Hệ\ số\ VCSH\\\\
Hệ\ số\ đảm\ bảo\ nợ &= \frac{VCSH}{NPT}
\end{align}
$$
##### 2.2. Some theories of capital structure
- Khi huy động vốn kinh doanh, DN luôn cố gắng tối thiểu chi phí sử dụng vốn (WACC min) bằng cách thay đổi cấu trúc vốn
- Some theories :
	1. **Traditional Theory**
		- Chi phí VCSH cao hơn chi phí NPT
		- Khi vay nợ tăng lên tới một ngưỡng nhất định mà chi phí nợ không đổi, phần nợ trong cấu trúc vốn cao hơn, có nghĩa là phần có chi phí thấp hơn đã cao hơn, phần có chi phí cao hơn giảm đi => WACC giảm
		- Tuy nhiên, khi mức nợ tăng cao, chi phí VCSH cũng phải tăng lên để đảm bảo bù đắp rủi ro cho chủ nợ
			- Khi nợ tăng thì cần phải có 1 lượng VCSH tăng để đảm bảo khả năng thanh toán nợ cho chủ nợ
			- DN phải trả nợ trước rồi mới đến việc chia cổ tức. Với phần nợ > phần VCSH, các nhà đầu tư cổ phiếu sẽ nhận thấy rủi ro, và DN phải tăng chi phí sử dụng vốn (tỷ suất sinh lời của cổ phiếu) lên để hấp dẫn họ
		- Khi vay nợ tăng lên, phần nợ có chi phí thấp hơn tăng lên, nhưng chi phí VCSH cũng tăng => WACC tăng
	2. **Modigliani-Miller Approach**
	3. **Trade-off Theory**
	4. **Pecking Order Theory**
### 2.3. #Principles of Capital Structure Management
- *Nguyên tắc đảm bảo tính tương thích - Timing Principle* : 
	- Thời gian của tài sản được đầu tư < thời gian đáo hạn của nguồn vốn huy động
	`VD: Nguồn vốn ngắn hạn nên được đầu tư vào tài sản ngắn hạn`
	- Để đảm bảo, thì Net Working Capital > 0
- *Nguyên tắc cân bằng giữa lợi nhuận và rủi ro - Risk Principle* :
	- Khi đầu tư nhiều vào TSCĐ, thì nên đảm bảo sản lượng dự kiến > sản lượng hòa vốn
	- Khi huy động vốn bằng vay nợ, thì nên đảm bảo OROA > i
- *Nguyên tắc đảm bảo quyền kiểm soát doanh nghiệp - Control Principle*
	- Khi huy động vốn bằng cổ phiếu, cần đảm bảo quyền kiểm soát DN cho những cổ đông quan trọng để quyền điều hành DN không bị xáo trộn
- *Nguyên tắc tài trợ linh hoạt - Flexibility Principle*
	- Điều chỉnh nhu cầu vốn tăng giảm, hay thay đổi cơ cấu vốn một cách linh hoạt trong từng thời kỳ cụ thể
- *Nguyên tắc tối thiểu hoá chi phí sử dụng vốn - Cost Principle*
	- Lựa chọn nguồn vốn có chi phí thấp
	- Đánh giá xu hướng biến động chi phí của từng nguồn để xác định vốn huy động và thời gian huy động thích hợp
---
# 3. Leverage
### 3.1. Operating Leverage
- OL thể hiện cách thức sử dụng **chi phí cố định** (FC) để tác động đến sản lượng (Q) nhằm thay đổi lợi nhuận (EBIT) hoạt động sản xuất kinh doanh của DN
- **Degree of Operating Leverage (DOL)** :
	- `DOL(Q(0)): mức độ ảnh hưởng của đòn bẩy kinh doanh tại sản lượng Q(0)`
	- `EBIT(Q(0)): lợi nhuận trước thuế và lãi vay tại mức sản lượng Q(0)`
	- `% ΔEBIT: % thay đổi về EBIT`
	- `% ΔSales: % thay đổi về sản lượng (hay doanh thu)`
	$$DOL_{Q_0} = \frac{\% \ \Delta EBIT}{\% \ \Delta Sales} = \frac{\Delta EBIT / EBIT_{Q_0}}{\Delta Q / Q_0} = \frac{\Delta EBIT / EBIT_{Q_0}}{(p\cdot \Delta Q) / (p \cdot Q_0)}$$
	**==>** Tại mức sản lượng Q(0) hay mức doanh thu P * Q(0), khi sản lượng/doanh thu tăng 1% thì EBIT sẽ tăng DOL (%)
	$$
	\begin{align}
	EBIT &= p \cdot Q - (FC + VC)\\
	&= p \cdot Q - (F + v \cdot Q)\\
	&= Q \cdot (p - v) - F\\
	=> \Delta EBIT &= \Delta Q \cdot (p - v)\\\\
	==> DOL_{Q_0} &= \frac{Q_0 \cdot (p - v)}{Q_0 \cdot (p - v)  - F} = \frac{EBIT_{Q_0} + F}{EBIT_{Q_0}}
	\end{align}
	$$
- ...
	- `p x Q : Doanh thu`
	- `FC hoặc F : chi phí cố định (không gồm I vì I thuộc hđ tài chính)`
	- `VC : chi phí biến đổi`
	- `v : chi phí biến đổi trên 1 sản phẩm`
	- `Q(BEP): sản lượng hòa vốn (doanh thu = chi phí)`
	---
- **Quan hệ giữa DOL và BEP:**
	- Ta thấy FC càng lớn thì DOL càng lớn, vậy FC càng cao thì EBIT càng tốt?
	$$
	\begin{align}
	Break\ Even\ Point &:\ p \cdot Q_{BEP} = v \cdot Q_{BEP} + F\\\\
	==> DOL_{Q_0}&= \frac{Q_0}{Q_0 - \frac{F}{p-v}} = \frac{Q_0}{Q_0 - Q_{BEP}}
	\end{align}
	$$
	![[break even point.png#center|480]]
	1. *Khi Q(0) < Q(BEP) <=> EBIT(Q(0)) < 0   ==> DOL < 0 :*
		- DN càng sản xuất thêm càng lỗ nhiều hơn
		- DN nào có FC cao hơn thì DN đó có mức giảm lỗ nhanh hơn
	2. *Khi Q(0) > Q(BEP) <=> EBIT(Q(0)) > 0   ==> DOL > 0 :*
		- DN càng sản xuất thêm càng lãi ít đi
		- DN nào có FC cao hơn thì DN đó có mức tăng trưởng lợi nhuận nhanh hơn
### 3.2. Financial Leverage
- FL thể hiện ở việc doanh nghiệp sử dụng **vốn vay** (Debt) nhằm gia tăng tỉ suất lợi nhuận trên vốn chủ sở hữu (ROE) hay thu nhập trên mỗi cổ phiếu (EPS) của DN
- **Một vài chỉ số đánh giá:** 
	- *Return on Assets - ROA* : tỉ suất lợi nhuận ròng trên tổng tài sản (Equity + Debt)
		`--> cứ 1 đồng tài sản (VCSH + NPT) sẽ có ROA đồng lợi nhuận ròng`
	- *Return on Equity - ROE* : tỉ suất lợi nhuận ròng trên vốn chủ sở hữu là chỉ số quan trọng nhất đối với các cổ đông 
		`--> cứ 1 đồng VCSH sẽ có ROE đồng lợi nhuận ròng`
	- *Operating ROA - OROA* :  tỉ suất EBIT trên tổng tài sản
	$$
	\begin{align}
	ROA &= \frac{NI}{A} = \frac{NI}{E + D} = \frac{ROE}{1 + D/E}\\\\
	ROE &= \frac{NI}{E} = \frac{NI}{A - D} = \frac{ROA}{1 - D/A}\\\\
	OROA &= \frac{EBIT}{A}
	\end{align}
	$$
- **Mối quan hệ giữa OROA và ROE:**
	$$
	\begin{align}
	ROE &= \frac{NI}{E} = \frac{(EBIT - D \cdot i) \cdot (1-t)}{E}\\\\
	&= \frac{(OROA \cdot A - D \cdot i) \cdot (1-t)}{E}\\\\
	&= (OROA + \frac{OROA \cdot (D + E) - D \cdot i}{E}) \cdot (1-t)\\\\
	&= [\ OROA + \frac{D}{E} \cdot(OROA - i)\ ] \cdot (1-t)
	\end{align}
	$$
	- *Khi OROA > i :*
		`OROA (đồng lợi nhuận trước lãi vay sinh ra từ 1 đồng tài sản) > i (đồng chi phí lãi vay sinh ra từ 1 đồng vay nợ)`
		- Khi vay càng nhiều thì lợi nhuận sau lãi vay càng tăng => DFL dương và tăng => ROE/EPS dương và tăng 
	- *Khi OROA < i :*
		`OROA (đồng lợi nhuận trước lãi vay sinh ra từ 1 đồng tài sản) < i (đồng chi phí lãi vay sinh ra từ 1 đồng vay nợ)`
		- Khi vay càng nhiều thì càng lỗ => DFL âm và giảm => ROE/EPS âm và giảm 
	- *Khi OROA = i :* 
		`OROA (đồng lợi nhuận trước lãi vay sinh ra từ 1 đồng tài sản) = i (đồng chi phí lãi vay sinh ra từ 1 đồng vay nợ)`
		- Dù vay như thế nào thì lợi nhuận trước và sau lãi vay như nhau
	---
- **Degree of Financial Leverage (DFL)** :
	$$
	\begin{align}
	DFL_{EBIT_0} &= \frac{\% \ \Delta ROE}{\% \ \Delta EBIT} = \frac{\Delta ROE / ROE_{EBIT_0}}{\Delta EBIT / EBIT_0}
	\end{align}
	$$
	**==>** Tại mức EBIT(0), khi EBIT tăng 1% thì EPS hay ROE sẽ tăng DFL (%)
	$$
	\begin{align}
	 EPS &= \frac{NI - PD}{NS} = \frac{(EBIT - I) \cdot (1-t) - PD}{NS}\\\\
	=> \Delta EPS &= \frac{\Delta EBIT \cdot (1-t)}{NS}\\\\\\
	==> DFL_{EBIT_0} &= \frac{EBIT_0 \cdot (1-t)}{(EBIT_0 - I) \cdot (1-t) - PD}
	\end{align}
	$$
- ...
	- `NI : Net Income (after Interest and Tax)`
	- `A = E + D (Assets = Equity + Debt)`
	- `I = D . i (Interest = Debt . interest_rate)` 
	- `t : CIT rate`
	- `PD: Preferred Dividends`
	- `NS : Number of Outstanding Common Shares`
	---
- **Mối quan hệ giữa EBIT và EPS:**
	- Ta thấy vay càng nhiều thì DFL càng lớn, vậy vay càng nhiều thì EPS sẽ càng cao?
	$$
	\begin{align}
	Indifference\ Point:\quad EPS_1 &= EPS_2\\\\
	<=> \frac{(EBIT' - I_1)\cdot(1-t) - PD_1}{NS_1} &= \frac{(EBIT' - I_2)\cdot(1-t) - PD_2}{NS_2}
	\end{align}
	$$
	![[indifference point.jpg#center|480]]
	- Nếu EBIT < EBIT' thì nên phát hành cổ phiếu
		`Nếu vay càng nhiều mà EBIT không đủ lớn để bù đắp chi phí lãi vay, thì EPS phải càng giảm để bù đắp`
	- Nếu EBIT > EBIT' thì nên phát hành trái phiếu
### 3.3. Total Leverage
- **Degree of Total Leverage (DTL):**
	$$ 
	\begin{align}
	DTL &= DOL \cdot DFL \\\\
	&= \frac{\% \ \Delta EBIT}{\% \ \Delta Sales} \cdot \frac{\% \ \Delta EPS}{\% \ \Delta EBIT}\\\\
	&= \frac{EBIT_{Q_0} + F}{EBIT_{Q_0}} \cdot \frac{EBIT_{Q_0} \cdot (1-t)}{(EBIT_{Q_0} - I) \cdot (1-t) - PD}\\\\
	&= \frac{(EBIT_{Q_0} + F) \cdot (1-t)}{(EBIT_{Q_0} - I) \cdot (1-t) - PD}
	\end{align}
	$$
	**==>** Tại mức sản lượng Q(0) hay doanh thu p * Q(0), khi sản lượng/doanh thu tăng 1% thì EPS sẽ tăng DTL (%)

