# 1. Overview
# 2. Valuation
### 2.1. Coupon Bond
- Trái phiếu trả lãi định kỳ **mỗi năm**
$$
\begin{align}
P_0 = \sum_{t=1}^n \frac{C}{(1+k_d)^t} + \frac{F}{(1+k_d)^n}\\\\
\end{align}
$$
- Trái phiếu trả lãi định kì **nửa năm**
$$
\begin{align}
P_0 = \sum_{t=1}^{2n} \frac{C/2}{(1+k_d/2)^t} + \frac{F}{(1+k_d/2)^{2n}}\\\\
\end{align}
$$
### 2.2. Zero-coupon Bond
- Với **trái phiếu không trả lãi** , doanh nghiệp phát hành sẽ bán với giá thấp hơn mệnh giá và mua lại với giá bằng mệnh giá khi đáo hạn
$$
\begin{align}
P_0 = \frac{F}{(1 + k_d)^n}\\\\
\end{align}
$$
- Với **trái phiếu trả lãi 1 lần vào thời điểm đáo hạn**, tổ chức phát hành sẽ trả cho chủ sở hữu trái phiếu với toàn bộ tiền lãi và mệnh giá
$$
\begin{align}
P_0 = \frac{F + I}{(1 + k_d)^n}\\\\
\end{align}
$$
# 3. Yield
### 3.1. Coupon Rate / Nominal Yield
$$
\begin{align}
\text{Coupon Rate} = \frac{\text{Annual Coupon}}{\text{Face Value}}\\\\
\end{align}
$$
- Lợi suất danh nghĩa 
	- Chỉ đo phần lợi tức / trái tức được trả hàng năm
	- Không đo phần lợi tức hưởng từ chênh lệch giá
### 3.2. Current Yield
$$
\begin{align}
\text{Current Yield} = \frac{\text{Annual Coupon}}{\text{Market Price}}\\\\
\end{align}
$$
- Lợi suất hiện hành
	- Chỉ đo phần lợi tức / trái tức được trả hàng năm dưới dạng % của giá thị trường trái phiếu
	- Không đo phần lợi tức hưởng từ chênh lệch giá
### 3.3. Yield to Maturity (YTM)
$$
\begin{align}
P_0 = \sum_{t=1}^n \frac{C}{(1 + YTM)^t} + \frac{F}{(1 + YTM)^n}\\\\
\end{align}
$$
- Lợi suất khi đáo hạn
	- Lợi suất thực tế thu được từ trái phiếu nếu mua bây giờ và nắm giữ đến khi đáo hạn
	- Phản ánh chính xác tổng lợi tức thực sự (trái tức và mệnh giá)
### 3.4. Yield to Call (YTC)
$$
\begin{align}
P_0 = \sum_{t=1}^n \frac{C}{(1 + YTC)^t} + \frac{P_c}{(1 + YTC)^n}\\\\
\end{align}
$$
- Nhà phát hành có thể phát hành **trái phiếu kèm theo điều khoản mua lại / gọi lại - Callable Bond**. Công ty sẽ gọi lại với giá thu hồi khi lãi suất thị trường giảm (thường thấp hơn YTM), tức là công ty đang phải trả lãi cao hơn so với thị trường. Sau đó, công ty phát hành trái phiếu mới với lãi suất thấp hơn để thay thế
- **Giá thu hồi (Call Price)** thường:
	- Cao hơn mệnh giá để bù đắp rủi ro cho nhà đầu tư `<< giá thu hồi = mệnh giá + phí gọi lại (call premium) >>`
	- Thấp hơn giá thị trường do lãi suất thị trường giảm
- **Lợi suất thu hồi (YTC)** mà nhà đầu tư thực sự nhận được **thường thấp hơn YTM** do:
	- Thời gian đầu tư ngắn đi do bị thu hồi sớm
	- Tổng lợi tức nhận được ít hơn, không nhận đủ lợi tức cho tới lúc đáo hạn mà chỉ nhận cho tới lúc bị thu hồi
 - Ngoài ra, lãi suất tái đầu tư thấp hơn khi phải đầu tư lại trong môi trường lãi suất thấp `<< lãi suất tái đầu tư là lãi suất khi nhà đầu tư dùng lợi tức nhận được từ một khoản đầu tư để đầu tư tiếp >>`
---
![[callable_bond.jpg#center|360x]]
- Trục
	- X - Giá trái phiếu
	- Y - lãi suất thị trường
- Đường
	- Option-free Bond Value
		- Giá trái phiếu không có quyền gọi lại theo lãi suất thị trường
	- Callable Bond Value
		- Giá trái phiếu có quyền gọi lại theo lãi suất thị trường
	- Call Price
		- Mức giá công ty trả nếu gọi lại trái phiếu
		- Khi lãi suất thị trường giảm, giá trái phiếu tăng. Nhưng do có khả năng bị gọi lại, giá trái phiếu bị giới hạn
	- ***Call Option Value*** `<< Call Option Value = Option-free Bond Value - Callable Bond Value >>`
		- Giá trị của quyền gọi lại mà công ty nắm giữ. Tức là phần thiệt hại của nhà đầu tư
# 4. Risks
### 4.1. Credit Risk / Default Risk
- Rủi ro tín dụng, hay rủi ro vỡ nợ là khi tổ chức phát hành trái phiếu không có đủ khả năng tài chính để thanh toán khoản tiền phải trả 
- ***Bảng xếp hạng tín dụng:***
	![[credit-ratings.png#center|720x]]
- ***Tiêu chuẩn xếp hạng:***
	![[credit-rating-criteria.png#center|560]]
	- Các tổ chức tín nhiệm như S&P định kì tính giá trị trung vị của những tỷ số đã chọn
	- Các tỷ số
		- Phải được đánh giá trong phạm vi ngành
		- Tỷ trọng khác nhau tùy nhà phân tích
### 4.2. Reinvestment Risk
- Rủi ro tái đầu tư là khi trái chủ đã nhận được tiền nhưng không có cơ hội tái đầu tư lại với mức lãi suất tương đương
- Nhà đầu tư sẽ lựa chọn trái phiếu không có điều khoản thu hồi để nhận mức lãi suất cao hơn --> giảm thiểu rủi ro tái đầu tư
### 4.3. Interest Risk
- Thông thường, lãi suất và giá trái phiếu sẽ có quan hệ ngược chiều
- Trái phiếu dài hạn có rủi ro lãi suất cao hơn ngắn hạn vì giá sẽ biến động mạnh hơn khi lãi suất thay đổi `-- dựa vào công thức --`
- Khi **lãi suất trái phiếu tăng**, giá trái phiếu giảm
	- Khi cần bán trái phiếu trước đáo hạn thì sẽ phải bán với giá thấp
	- Nếu tiếp tục giữ thì lợi suất hiện tại của trái phiếu không còn hấp dẫn vì có thể mua trái phiếu mới rẻ hơn mà lãi suất cao hơn
- Đối với **trái phiếu có quyền chọn bán - Put Bond**
	- Khi lãi suất thị trường tiếp tục tăng khiến giá trái phiếu tiếp tục giảm, nhà đầu tư có quyền bán lại trái phiếu cho công ty để tránh được khoản lỗ tiềm tàng --> giảm thiểu rủi ro lãi suất
	- Khi tình hình tài chính công ty phát hành xấu đi, nhà đầu tư có thể bán ngay --> giảm thiểu rủi ro tín dụng / vỡ nợ
### 4.4. Inflation Risk
- Giá trị dòng tiền thực tế giảm khi lạm phát tăng cao
- Dù nhận đủ tiền danh nghĩa, nhưng khả năng mua sắm thực tế bị giảm
### 4.5. Liquidity Risk
- Rủi ro thanh khoản sẽ cao đối với các doanh nghiệp nhỏ, lạ, chưa niêm yết, hoặc xếp hạng tín dụng thấp
- Khi nhà đầu tư khẩn cấp cần tiền, có thể sẽ không tìm được người mua, hoặc phải bán với giá thấp hơn
### 4.6. Exchange Rate Risk / Currency Risk
- Rủi ro tỷ giá xảy ra khi đầu tư trái phiếu nước ngoài, và nhận được tiền lãi và gốc bằng tiền nước ngoài
- Nếu **tỷ giá tăng**, USD tăng so với VND, thì khi quy đổi tiền từ USD sang VND sẽ được ít tiền hơn
# 5. Term Structure of Interest Rates
- Cấu trúc kỳ hạn của lợi suất là ảnh hưởng của thời gian đáo hạn lên lợi suất
### 5.1. The Yield Curve
- Đường cong lợi suất là đồ thị phản ánh mối quan hệ đó
![[the-yield-curves.webp#center|360x]]
- Có 3 dạng:
	- Đường cong lợi suất bình thường (normal)
	- Đường cong lợi suất phẳng (flat)
	- Đường cong lợi suất đảo ngược (inverted)