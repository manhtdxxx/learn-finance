# 1. Overview of Credit Risk
### 1.1. Concept
- Tín dụng là sự chuyển quyền sử dụng vốn dưới hình thức tiền tệ hoặc hàng hóa từ chủ sở hữu sang người sử dụng trong một thời gian nhất định với một chi phí nhất định
- Rủi ro tín dụng là loại rủi ro phát sinh do khách nợ không còn khả năng chi trả. Rủi ro tín dụng là tính không chắc chắn và tiềm ẩn về khoản lỗ do không có khả năng thanh toán của bên đối tác
### 1.2. Classification
- Rủi ro vỡ nợ - Default Risk
	- Khi người đi vay không có khả năng trả gốc hoặc lãi
- Rủi ro hạ cấp - Downgrading Risk
	- Liên quan đến chứng khoán nợ. VD trái phiếu là 1 hình thức tín dụng
	- Doanh nghiệp phát hành có kết quả kinh doanh kém đi → trái phiếu bị hạ mức xếp hạng tín nhiệm → giá trái phiếu giảm khi lãi suất yêu cầu từ nhà đầu tư cao hơn → nhà đầu tư đang nắm giữ sẽ lỗ vốn nếu bán ra
# 2. Credit Risk Management according to Basel
### 2.1. Basel 1
- Hiệp định Basel 1 cung cấp định nghĩa về vốn ngân hàng C và tài sản rủi ro RWA:
	- **Vốn cấp 1 - Tier 1**
		- Vốn điều lệ
		- Thặng dư vốn cổ phần
		- Lợi nhuận giữ lại
		- ...
	- **Vốn cấp 2 - Tier 2**
		- Chênh lệch đánh giá lại tài sản
		- Các khoản dự phòng tổn thất chung
		- Công cụ lai giữa nợ và vốn. VD cổ phiếu ưu đãi
		- Nợ thứ cấp có kì hạn. VD ngân hàng phát hành trái phiếu trên 5 năm
	- **Tài sản rủi ro có trọng số - RWA**
		- Cách tính:
			$$\text{RWA} = \text{Giá trị} \cdot \text{Hệ số rủi ro}$$
		- Hệ số rủi ro được xác định dựa theo nhóm tài sản. VD như sau:
			- Chính phủ: 0%
			- Ngân hàng: 20%
			- Vay có đảm bảo: 50%
			- Doanh nghiệp: 100%
- ***Yêu cầu tối thiểu của Basel 1:*** 
$$
\begin{align}
\text{Tỷ lệ vốn cấp 1} &= \frac{\text{Tier 1}}{\text{RWA}} \ge 4\% \\\\
\text{Tỷ lệ vốn cấp 1 và cấp 2} &= \frac{\text{Tier 1} + \text{Tier 2}}{\text{RWA}} \ge 8\%
\end{align}
$$
### 2.2. Basel 2
#### 2.2.1. Standardized Approach (SA)
- Dựa vào xếp hạng tín nhiệm của các tổ chức uy tín (S&P, Moody’s, Fitch) để xác định hệ số rủi ro