# 1. Cost of Capital
- Chi phí sử dụng vốn là cái giá mà doanh nghiệp phải trả cho việc sử dụng nguồn tài trợ (bao gồm cả chi phí cơ hội). 
- Chi phí sử dụng vốn cũng có thể được xem là **tỷ suất sinh lời mà các nhà cung ứng vốn trên thị trường yêu cầu doanh nghiệp phải trả** nhằm đảm bảo sự tài trợ vốn của họ đối với DN
---
### 1.1. Cost of Debt
- Khi đi vay, phần lợi nhuận khi tính thuế TNDN sẽ không tính phần lãi vay
- Chi phí sử dụng vốn vay là tỷ lệ chiết khấu `(i)` làm cân bằng dòng tiền `(CF)` mà DN phải thanh toán cho chủ nợ trong tương lai và khoản nợ vay `(P)` mà DN vay hiện tại
##### Before Tax
- Hàng năm, sẽ trả dần khoản vay gồm tiền gốc lẫn tiền lãi
$$ P = \sum_{t=1}^n \frac{CF_t}{(1+i)^t}$$

- Khi các khoản phải trả hằng năm không đổi:
$$P = CF \cdot \frac{1-(\frac{1}{1+i})^n}{i}$$
##### After Tax
- Do Cost of Equity vẫn bị tính thuế TNDN nên để có thể so sánh được chi phí sử dụng từ các nguồn vốn khác nhau thì cần có cơ sở đồng nhất
 `-- Nếu DN làm ăn thua lỗ thì sẽ không phải nộp thuế ==> CIT rate = 0% --`
$$i\ \ AFTER\ \ tax \ =\  i\ \ BEFORE\ \ tax \cdot (1 - CIT\ rate)$$
 
---
### 1.2. Cost of Equity
##### 1.2.1. Common Share
1. **Cổ phiếu thường**
	- ***Theo mô hình tăng trưởng không đổi (Gordon growth model):***
	$$P = \frac{D_0 \cdot (1+g)}{i - g} \  \ => \ \ i  = \frac{D_1}{P} + g$$
	- ***Theo mô hình CAPM (Capital Asset Pricing Model)***
		- ***Rf :*** Lãi suất phi rủi ro (Risk-Free Rate)
			- Là loại lãi suất mà tại đó, tỷ lệ rủi ro của tài sản gần bằng 0
			- Thường thì sẽ được lấy bằng lãi suất trái phiếu chính phủ kỳ hạn 10 năm
		- ***Beta*** là đại được đo lường mức độ biến động của cổ phiếu so với thị trường chung
			- Nếu một tài sản có beta = 1, nó sẽ biến động theo thị trường
			- Nếu beta > 1, nó biến động mạnh hơn so với thị trường
			- Nếu beta < 1, nó biến động yếu hơn so với thị trường
		- ***Risk Premium*** là khoản thưởng khi bạn đầu tư vào cổ phiếu (rủi ro cao), so với cầm giữ các tài sản khác (có rủi ro thấp)
		- ***Rm:***  Tỷ suất sinh lời kỳ vọng của thị trường (Required Market Return)
		$$
		\begin{align}
		k_e &= r_f + Beta \cdot Risk\ Premium\\
		&= r_f + Beta \cdot (r_m - r_f)
		\end{align}
		$$
	---
2. **Cổ phiếu thường mới phát hành**
	- Khi phát hành một cổ phiếu mới thì sẽ phát sinh thêm chi phí mới: in ấn, bảo lãnh phát hành, môi giới, ... Vì vậy cần phải tính giá ròng cho cổ phiếu đó
	$$Giá\ ròng = Giá\ phát\ hành \cdot (1- Tỷ\ lệ\ chi\ phí\ phát\ hành)$$
	- ***Theo mô hình tăng trưởng không đổi (Gordon growth model):***
	$$i = \frac{D_1}{Giá\ ròng} + g$$
---
##### 1.2.2. Preferred Share
- Người sở hữu cổ phiếu ưu đãi chỉ nhận được cổ tức ưu đãi cố định hằng năm
$$P = \frac{D}{i} \ \ =>\ \ i  = \frac{D}{P}$$
---
##### 1.2.3. Retained Earnings
- Đo lường bằng chi phí cơ hội, thể hiện rằng lợi nhuận nếu được chia cho các cổ đông thì họ có thể dùng số tiền đó để đầu tư nơi khác và thu lợi nhuận. Như vậy, **chi phí sử dụng lợi nhuận để lại chính là chi phí sử dụng cổ phần thường**
-  ***Theo mô hình tăng trưởng không đổi (Gordon growth model):***

$$i  = \frac{D_1}{P} + g$$

---
### 1.3. Weighted Average Cost of Capital (WACC)
 - Để đủ vốn kinh doanh thì DN cần phải huy động từ nhiều nguồn vốn khác nhau và mỗi nguồn sẽ có chi phí sử dụng khác nhau. Do đó ta cần xác định chi phí sử dụng bình quân của các nguồn đó
 - ***Công thức:***
	 - `w(i): tỉ trọng của nguồn vốn thứ i`
	 - `k(i): chi phí sử dụng nguồn vốn thứ i`
	 - `t(i): vốn của nguồn i được sử dụng`
	 - `T: tổng số vốn từ các nguồn`
	 $$WACC = \sum_{i=1}^n w_i \cdot k_i \  = \  \sum_{i=1}^n \frac{t_i}{T} \cdot k_i$$
---
### 1.4. Marginal Cost of Capital (MCC)
- Chi phí sử dụng vốn cận biên là **chi phí cho đồng vốn mới nhất tăng thêm** khi doanh nghiệp huy động đầu tư cho hoạt động kinh doanh `-- WACC đạo hàm theo t(i), T --`
- DN sẽ huy động vốn có *chi phí thấp trước* (lợi nhuận giữ lại, nợ lãi suất thấp, ...). Tuy nhiên, khi DN *đạt đến giới hạn* của những nguồn giá rẻ này (hết lợi nhuận giữ lại, nợ thêm sẽ tăng lãi, ...) và *cần phát hành cổ phiếu mới*, *chi phí sẽ tăng vọt* vì vốn chủ sở hữu thường có chi phí cao hơn nợ --> Bước nhảy này sẽ phản ánh được mối quan hệ phi tuyến tính
![[marginal_WACC.png#center|480]]
- **Điểm gãy** - **Break Point** là điểm mà số vốn mới có thể huy động được trước khi MCC nhảy vọt
$$Break\ Point\ i = \frac{Tổng\ giá\ trị\ của\ nguồn\ vốn\ i}{Tỷ\ trọng\ của\  nguồn\ vốn\ i}$$
**==>** DN có thể huy động vốn tới Break-Point (Tổng số vốn mới) mà không thay đổi WACC, sau đó nếu muốn tăng vốn, thì WACC sẽ nhảy vọt

---
# 2. Capital Structure
##### 2.1. Overview
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
- ***Some theories :***
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
- ***Nguyên tắc đảm bảo tính tương thích - Timing Principle*** 
	- Thời gian của tài sản được đầu tư < thời gian đáo hạn của nguồn vốn huy động
	`VD: Nguồn vốn ngắn hạn nên được đầu tư vào tài sản ngắn hạn`
	- Để đảm bảo, thì Net Working Capital > 0
- ***Nguyên tắc cân bằng giữa lợi nhuận và rủi ro - Risk Principle***
	- Khi đầu tư nhiều vào TSCĐ, thì nên đảm bảo sản lượng dự kiến > sản lượng hòa vốn
	- Khi huy động vốn bằng vay nợ, thì nên đảm bảo OROA > i
- ***Nguyên tắc đảm bảo quyền kiểm soát doanh nghiệp - Control Principle***
	- Khi huy động vốn bằng cổ phiếu, cần đảm bảo quyền kiểm soát DN cho những cổ đông quan trọng để quyền điều hành DN không bị xáo trộn
- ***Nguyên tắc tài trợ linh hoạt - Flexibility Principle***
	- Điều chỉnh nhu cầu vốn tăng giảm, hay thay đổi cơ cấu vốn một cách linh hoạt trong từng thời kỳ cụ thể
- ***Nguyên tắc tối thiểu hoá chi phí sử dụng vốn - Cost Principle***
	- Lựa chọn nguồn vốn có chi phí thấp
	- Đánh giá xu hướng biến động chi phí của từng nguồn để xác định vốn huy động và thời gian huy động thích hợp