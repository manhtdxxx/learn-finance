# 1. Valuation of Debt Securities
### 1.1. Treasury Bill
- **Trên Primary Market:**
	- `Lãi suất tín phiếu trúng thầu (%/năm)`
	- `Kỳ hạn của tín phiếu`
	$$Giá\ bán\ ban\ đầu = \frac{Mệnh\ giá}{1 + \dfrac{Lãi\ suất\ trúng\ thầu\ \cdot \ Kỳ\ hạn}{365}}$$
- **Trên Secondary Market:**
	- `Lãi suất tín phiếu hiện hành trên thị trường (%/năm)`
	- `Kỳ hạn còn lại của tín phiếu cho đến ngày đáo hạn`
	$$Giá\ bán\ lại = \frac{Mệnh\ giá}{1 + \dfrac{Lãi\ suất\ thị\ trường\ \cdot \ Kỳ\ hạn\ còn\ lại}{365}}$$
### 1.2 Bond
##### Valuation
- ...
	- `P: giá trị của trái phiếu tại thời điểm phát hành`
	- `F: giá trị của trái phiếu tại thời điểm đáo hạn`
	- `C: lãi thanh toán hằng năm` 
	- `k_d: tỷ suất chiết khấu/tỷ suất sinh lời cần thiết theo thị trường (%/năm)`
	- `n: số năm còn lại cho đến khi đáo hạn`
1. **Discount Bond**
$$P = \frac{F}{(1 + k_d)^n}$$
2. **Coupon Bond (Trả lãi theo năm)**
	$$P = \sum_{t=1}^n \frac{C}{(1+k_d)^t} + \frac{F}{(1+k_d)^n}$$
3. **Coupon Bond (Trả lãi nửa năm 1 lần)**
	$$P = \sum_{t=1}^{2n} \frac{C/2}{(1+k_d/2)^{t}} + \frac{F}{(1+k_d/2)^{2n}}$$
##### Sensitivity of the Bond Price to the Interest Rate
- ***Giá trái phiếu*** với ***lãi Coupon khác nhau*** biến động khi ***lãi suất thị trường*** thay đổi
	- Lãi suất thị trường tăng → giá trái phiếu giảm
	- Lãi suất thị trường giảm → giá trái phiếu tăng
	- Lãi suất thị trường = lãi suất trái phiếu → giá trái phiếu = mệnh giá
	- Lãi suất thị trường < lãi suất trái phiếu → giá trái phiếu > mệnh giá
	- Lãi suất thị trường > lãi suất trái phiếu → giá trái phiếu < mệnh giá
![[bond_price_to_interest_rate.png|center|560]]
- Trục
	- X: số kỳ còn lại tới ngày đáo hạn
	- Y: giá thị trường của trái phiếu
- ***Lãi suất thị trường = 8%*** `<< cũng có thể hiểu là YTM yêu cầu của nhà đầu tư lúc đó >>`
- Đường
	- ***Coupon Rate = 8%***
		- Giá trái phiếu bằng mệnh giá dù bất cứ kỳ hạn nào
	- ***Coupon Rate = 10% và 12%***
		- Lãi suất thị trường thấp hơn lãi coupon
		- Giá trái phiếu bán cao hơn mệnh giá do trả lãi coupon cao
		- Giá sẽ giảm dần về bằng mệnh giá khi tới ngày đáo hạn
	-  ***Coupon Rate = 4% và 12%***
		- Lãi suất thị trường cao hơn lãi coupon
		- Giá trái phiếu bán thấp hơn mệnh giá do trả lãi coupon thấp
		- Giá sẽ tăng dần về bằng mệnh giá khi tới ngày đáo hạn
# 2. Valuation of Equity Securities
### 2.1. Preferred Stock
- Khi cổ phiếu ưu đãi là cổ phiếu không có quyền mua lại, không chuyển đổi được với kỳ hạn không xác định và trả cổ tức với tỷ suất cố định
	- `P: giá trị của cổ phiếu ưu đãi cổ tức`
	- `D: cổ tức ưu đãi`
	- `k_p: tỷ suất chiết khấu/tỷ suất sinh lời cần thiết theo thị trường (%/năm)`
	$$P = \frac{D}{k_{p}}$$
---
### 2.2. Common Stock
1. Do cổ phiếu không có kỳ đáo hạn ***(n --> +∞)***
	- `P: giá trị của cổ phiếu thường tại thời điểm phát hành`
	- `D_t: cổ tức thường tại thời điểm kết thúc kỳ hạn t`
	- `k_e: tỷ suất chiết khấu/tỷ suất sinh lời cần thiết theo thị trường (%/năm)`
	$$P = \sum_{t=1}^n \frac{D_t}{(1+k_e)^{t}}$$
2. Tuy nhiên các nhà đầu tư có thể sẽ không đầu tư mãi và mong muốn *bán cổ phiếu tại một thời điểm* kì vọng thì dòng thu nhập của họ thay vì chỉ là cổ tức mãi mãi thì sẽ gồm cổ tức và giá bán ***(n hữu hạn)***
	- `P_n: giá bán của cổ phiếu tại thời điểm cuối kì n`
	$$P = \sum_{t=1}^n \frac{D_t}{(1+k_e)^{t}} + \frac{P_n}{(1+k_e)^n}$$
##### 2.2.1 Dividend Discount Model - DDM
1. **Khi tốc độ tăng trưởng cổ tức không đổi (Gordon growth model)**
	- ***Cổ tức gia tăng hằng năm với tỉ lệ g***
	$$
	\begin{align}
	D_0 &: \text{cổ tức vừa chia tại cuối kì thứ 0} \\
	D_1 &= D_0 \cdot (1+g)\\
	D_2 &= D_0 \cdot (1+g)^2\\
	D_3 &= D_0 \cdot (1+g)^3\\
	&...\\
	D_{n-1} &= D_0 \cdot (1+g)^{n-1}\\
	D_{n} &= D_0 \cdot (1+g)^{n}
	\end{align}
	$$
	- ***Định giá***
	$$
	\begin{align}
	P &= \frac{D_1}{1+k_e} + \frac{D_2}{(1+k_e)^2} + \frac{D_3}{(1+k_e)^3} +\ ...\ + \frac{D_n}{(1+k_e)^n}\\\\
	&= \frac{D_0 \cdot(1+g)}{1+k_e} + \frac{D_0 \cdot(1+g)^2}{(1+k_e)^2} +\frac{D_0 \cdot(1+g)^3}{(1+k_e)^3} +\ ...\ + \frac{D_0 \cdot(1+g)^n}{(1+k_e)^n}\\\\
	&= \ ............ \ \text{(Sum of a finite Geometric Series)}\\\\
	&= \frac{D_0 \cdot (1+g)}{k_e - g} \qquad (*)
	\end{align}
	$$
	---
2. **Khi tốc độ tăng trưởng cổ tức thay đổi**
	- Giả sử một cổ phiếu có lợi tức cổ phần được chia lần đầu là 1,50 USD, lợi tức cổ phần gia tăng mỗi năm 20% trong 4 năm kế tiếp. Từ năm thứ 5 trở đi, tỷ lệ này giảm xuống chỉ còn 6% mỗi năm. Tỷ lệ sinh lời cần thiết của cổ phiếu theo thị trường là 16%.
		- ***Giá trị hiện tại của lợi tức cổ phần tương lai trong 4 năm*** như sau
		$$ \begin{align*}
		D_1 &= 1.50 \cdot (1 + 0.2) = 1.8000 \\
		D_2 &= 1.50 \cdot (1 + 0.2)^2 = 2.1600 \\ 
		D_3 &= 1.50 \cdot (1 + 0.2)^3 = 2.5920 \\ 
		D_4 &= 1.50 \cdot (1 + 0.2)^4 = 3.1104 \\ 
		D_5 &= D_4 \cdot (1 + 0.06) = 3.2970
		\end{align*} 
		$$
		- ***Định giá bán của cổ phiếu tại thời điểm cuối năm 4*** bằng cách chiết khấu dòng cổ tức cuối năm thứ 5 trở đi
		$$P_4 = \frac{D_5}{k_e - g_2} = \frac{3.2970}{0.16 - 0.06} = 32.97$$
		- ***Định giá bán của cổ phiếu hiện tại cuối năm 0***
			- Coi rằng các nhà đầu tư sẽ muốn bán cổ phiếu đó tại thời điểm cuối năm 4
			$$P_0 = \sum_{t=1}^4 \frac{D_t}{(1+k_e)^{t}} + \frac{P_4}{(1+k_e)^4} = 6.535+18.21 = 24.745$$
			- Coi rằng các nhà đầu tư sẽ đầu tư vào cổ phiếu đó mãi mãi
			$$
			\begin{align}
			P_0 &= \sum_{t=1}^4 \frac{D_t}{(1+k_e)^{t}} + (\frac{D_4\cdot(1+g_2)}{(1+k_e)^5} + \frac{D_4\cdot(1+g_2)^2}{(1+k_e)^6}+\ ...\ +\frac{D_4\cdot(1+g_2)^{n-4}}{(1+k_e)^n})\\
			&= \sum_{t=1}^4 \frac{D_t}{(1+k_e)^{t}} + \sum_{t=5}^n \frac{D_4 \cdot (1+g_2)^{n-4}}{(1+k_e)^{n}} = 6.535 + 18.21 = 24.745
			\end{align}
			$$
---
##### 2.2.2. Discounted Cash Flow - DCF
- Mô hình chiết khấu dòng tiền tự do cho doanh nghiệp - FCFF
- Mô hình chiết khấu dòng tiền tự do cho vốn chủ sở hữu - FCFE
---

##### 2.2.3. Based on P/E
- Chỉ số P/E thể hiện số tiền mà nhà đầu tư sẵn sàng chi trả cho một đồng lợi nhuận
$$
\begin{align}
P/E &= \frac{Market\ Price}{EPS}\\\\
<< EPS &= \frac{Net\ Income - Preferred\ Equity}{Shares\ outstanding} >> \\\\
\end{align}
$$
- **Ý nghĩa :**
	- ***Khi P/E thấp :***
		- Các cổ đông hiện hữu không còn thấy khả năng phát triển của DN, nên quyết định bán chốt lời, khiến giá thị trường giảm --> P/E thấp
		- Hoặc có thể DN hoạt động hiệu quả hơn so với thời gian trước, khiến EPS tăng --> P/E thấp. Trong TH này có thể nói cổ phiếu đang bị định giá thấp và là cơ hội để mua
	- ***Khi P/E cao :***
		- Thông thường, chỉ số P/E cao thể hiện sự kỳ vọng của nhà đầu tư về việc tăng trưởng thu nhập từ cổ phiếu đó sẽ cao hơn trong tương lai
		- Tuy nhiên, chỉ số P/E cao đôi khi là biểu hiện việc doanh nghiệp kinh doanh kém hiệu quả, khiến EPS thấp --> P/E mới cao
	---
- **Định giá :** 
	- ***Dựa theo P/E trung bình ngành :*** 
		$$P = EPS_{\ kì\ vọng}\ \cdot\ P/E_{\ trung\ bình\ ngành}$$
	- ***Dựa theo P/E kết hợp với mô hình Gordon tăng trưởng cố định với tỷ lệ `g` :***
$$
\begin{align}
P = \frac{D_1}{k_e - g} &= \frac{Dividend\ Payout\ Ratio \cdot EPS_1}{k_e - g}\\\\
\Rightarrow P &= EPS_{\ kì\ vọng}\ \cdot\ \frac{Dividend\ Payout\ Ratio}{k_e - g}
\end{align}
$$