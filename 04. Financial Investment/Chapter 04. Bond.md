# 1. Overview
# 2. Valuation
### 2.1. Coupon Bond
- Trái phiếu **trả lãi định kỳ mỗi năm**
$$
\begin{align}
P_0 = \sum_{t=1}^n \frac{C}{(1+k_d)^t} + \frac{F}{(1+k_d)^n}\\\\
\end{align}
$$
- Trái phiếu **trả lãi định kì nửa năm**
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
\text{Coupon Rate} = \frac{\text{Annual Coupon}}{\text{Face Value}} \tag{2.1}\\\\
\end{align}
$$
- Lợi suất danh nghĩa 
	- Chỉ đo phần lợi tức / trái tức được trả hàng năm
	- Không đo phần lợi tức hưởng từ chênh lệch giá
### 3.2. Current Yield
$$
\begin{align}
\text{Current Yield} = \frac{\text{Annual Coupon}}{\text{Market Price}} \tag{2.2}\\\\
\end{align}
$$
- Lợi suất hiện hành
	- Chỉ đo phần lợi tức / trái tức được trả hàng năm dưới dạng % của giá thị trường trái phiếu
	- Không đo phần lợi tức hưởng từ chênh lệch giá
### 3.3. Yield to Maturity (YTM)
$$
\begin{align}
P_0 = \sum_{t=1}^n \frac{C}{(1 + YTM)^t} + \frac{F}{(1 + YTM)^n} \tag{2.3}\\\\
\end{align}
$$
- Lợi suất khi đáo hạn
	- Lợi suất thực tế thu được từ trái phiếu nếu mua bây giờ và nắm giữ đến khi đáo hạn
	- Phản ánh chính xác tổng lợi tức thực sự (trái tức và mệnh giá)
### 3.4. Yield to Call (YTC)
$$
\begin{align}
P_0 = \sum_{t=1}^n \frac{C}{(1 + YTC)^t} + \frac{P_c}{(1 + YTC)^n} \tag{2.4}\\\\
\end{align}
$$
- Nhà phát hành có thể phát hành ***trái phiếu kèm theo điều khoản mua lại / gọi lại - Callable Bond***. Công ty sẽ gọi lại với giá ***thu hồi khi lãi suất thị trường r giảm*** (thường khi r < YTM), tức là công ty đang phải trả lãi cao hơn so với thị trường. Sau đó, công ty phát hành trái phiếu mới với lãi suất thấp hơn để thay thế
- **Giá thu hồi (Call Price)** thường:
	- Cao hơn mệnh giá để bù đắp rủi ro cho nhà đầu tư `<< giá thu hồi = mệnh giá + phí gọi lại (call premium) >>`
	- Thấp hơn giá thị trường `<< lãi suất khi giảm khiến giá tăng, Call Price đặt ra mức giá trần >>`
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
# 4. Risk
### 4.1. Credit Risk / Default Risk
- Rủi ro tín dụng, hay rủi ro vỡ nợ là khi tổ chức phát hành trái phiếu không có đủ khả năng tài chính để thanh toán khoản tiền phải trả 
- **Bảng xếp hạng tín dụng:**
	![[credit_rating_scale.png#center|720]]
- **Tiêu chuẩn xếp hạng:**
	![[credit_rating_criteria.png#center|560]]
	- Các tổ chức tín nhiệm như S&P tính giá trị trung vị (median) của những tỷ số đã chọn
	- Các tỷ số
		- Phải được đánh giá trong phạm vi ngành
		- Tỷ trọng khác nhau tùy nhà phân tích
### 4.2. Reinvestment Risk
- Rủi ro tái đầu tư là khi trái chủ đã nhận được tiền nhưng không có cơ hội tái đầu tư lại với mức lãi suất tương đương
- Nhà đầu tư sẽ lựa chọn trái phiếu không có điều khoản thu hồi để nhận mức lãi suất cao khi giá trái phiếu giảm  --> giảm thiểu rủi ro tái đầu tư
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
- Rủi ro tỷ giá xảy ra **khi đầu tư trái phiếu nước ngoài**, và nhận được tiền lãi và gốc bằng tiền nước ngoài
- Nếu **tỷ giá tăng**, USD tăng so với VND, thì khi quy đổi tiền từ USD sang VND sẽ được **ít tiền hơn**
# 5. Term Structure of Interest Rates
### 5.1. The Yield Curve
- **Cấu trúc kỳ hạn của lợi suất** là ảnh hưởng của thời gian đáo hạn lên lợi suất
- Đường cong lợi suất: 
	- Là đồ thị phản ánh mối quan hệ đó
	- Thường dùng cho trái phiếu chính phủ do rủi ro thấp và nhiều kỳ hạn
	- Có 3 dạng:
		![[the_yield_curve.webp#center|360x]]
		- **Đường cong lợi suất bình thường (Normal)**
			- Lãi suất trái phiếu ngắn hạn *thấp hơn* dài hạn
			- Phổ biến nhất vì thông thường trái phiếu dài hạn có rủi ro cao hơn ngắn hạn
		- **Đường cong lợi suất đảo ngược (Inverted)**
			- Lãi suất trái phiếu ngắn hạn *cao hơn* dài hạn
			- Trong TH này, nhà đầu tư cho rằng nền kinh tế trong tương lai gần sẽ gặp khó khăn nhưng vẫn hoạt động tốt trong dài hạn --> rủi ro ngắn hạn lớn hơn
			- Khá hiếm xuất hiện, nó được coi như dấu hiệu dự báo suy thoái kinh tế
		- **Đường cong lợi suất phẳng (Flat)**
			- Lãi suất trái phiếu ngắn hạn *bằng* dài hạn
			- Xảy ra trong giai đoạn chuyển giao chu kỳ kinh tế. Nhà đầu tư không chắc chắn về triển vọng tương lai `-- VD: tăng trưởng có thể chững lãi, suy thoái có thể bỗng phục hồi --`
### 5.2. Sensitivity of the Bond Price to the Interest Rate
- Trong một thị trường cạnh trang, tất cả chứng khoán phải cung cấp cho các nhà đầu tư một tỷ suất sinh lời kỳ vọng hợp lý như nhau. Xét ví dụ như sau:
	- Nếu *1 trái phiếu có coupon 8%*, và các trái phiếu tương đồng cũng 8%, thì trái phiếu đó sẽ được bán bằng mệnh giá
	- Tuy nhiên, *nếu lãi suất thị trường tăng lên 9%*, liệu có ai mua một trái phiếu với coupon 8% bằng mệnh giá? Giá trái phiếu sẽ phải giảm cho tới khi lợi suất kỳ vọng (YTM) của trái phiếu tăng lên bằng lãi suất thị trường
	- Ngược lại, *nếu lãi suất thị trường xuống 7%*, trái phiếu coupon 8% trở nên hấp dẫn khiến các nhà đầu tư trả giá cao hơn cho tới khi lợi suất kỳ vọng (YTM) của trái phiếu không còn cao hơn lãi suất thị trường
- **Các ý chính tóm tắt như sau:**
	- Giá trái phiếu tỷ lệ nghịch với YTM
	- Với cùng một lượng tăng/giảm của YTM, giá sẽ giảm nhiều (khi YTM tăng) ít so với khi giá tăng (khi YTM giảm)
	- Giá của trái phiếu dài hạn nhạy cảm với lãi suất hơn so với trái phiếu ngắn hạn
	- Khi thời gian đáo hạn gia tăng, độ nhạy cảm của giá với lãi suất tăng với tỷ lệ giảm dần
	- Trái phiếu có lãi suất coupon thấp hơn sẽ nhạy cảm hơn
	- Trái phiếu có YTM thấp hơn sẽ nhạy cảm hơn
### 5.3. Theory
- Lý thuyết kì vọng (Expectations Theory)
- Lý thuyết ưu tiên thanh khoản (Liquidity Preference Theory)
- Lý thuyết phân đoạn thị trường (Segmented Markets Theory)
### 5.4. Duration
##### 5.4.1 Macaulay Duration
- **Duration:**
	- Là thời gian đáo hạn trung bình cho tới thời điểm nhận dòng tiền của trái phiếu
	- Duration sẽ thấp khi dòng tiền thu về sớm hơn (vd: coupon cao, kỳ hạn ngắn...)
	- Duration càng cao thì rủi ro lãi suất càng lớn – tức là giá trái phiếu sẽ biến động mạnh hơn khi lãi suất thay đổi
-  **Công thức Macaulay Duration:**
	$$
	\begin{flalign*}
	D &: \text{thời gian đáo hạn trung bình} \\
	t &: \text{năm nhận dòng tiền} \\
	T &: \text{năm đáo hạn} \\
	CF &: \text{dòng tiền nhận được chưa chiết khấu} && \\
	DCF &: \text{dòng tiền sau chiết khấu} && \\
	\end{flalign*}
	$$
	$$
	\begin{align}
	DCF_t &= \frac{CF_t}{(1+YTM)^t}\\\\
	P = \text{Total DCF} &= \sum_{t= 1}^T \ \frac{CF_t}{(1+YTM)^t}\\\\
	D_{macaulay} &= \sum_{t= 1}^T \ t \cdot \frac{DCF_t}{P} \tag{3.1}\\
	\end{align}
	$$
---

- **Ví dụ:** Biết tỷ suất chiết khấu là 10%. Xét 3 trái phiếu có cùng mệnh giá 1000 VNĐ
	- ***Trái phiếu A:*** Coupon 10%, kỳ hạn 3 năm
	- ***Trái phiếu B:*** Coupon 10%, kỳ hạn 5 năm
	- ***Trái phiếu C:*** Zero-coupon, kỳ hạn 5 năm

| Trái phiếu   | Năm (t) | Dòng tiền (CF) | Hệ số chiết khấu (1 / (1 + r)^t) |       PV(CF) |     t × PV(CF) |
| ------------ | ------: | -------------: | :------------------------------: | -----------: | -------------: |
| A            |       1 |            100 |              0.9091              |        90.91 |          90.91 |
| A            |       2 |            100 |              0.8264              |        82.64 |         165.28 |
| A            |       3 |          1,100 |              0.7513              |       826.43 |      2,47x9.28 |
| ***Tổng A*** |         |                |                                  | ***999.98*** | ***2,735.47*** |
| B            |       1 |            100 |              0.9091              |        90.91 |          90.91 |
| B            |       2 |            100 |              0.8264              |        82.64 |         165.28 |
| B            |       3 |            100 |              0.7513              |        75.13 |         225.38 |
| B            |       4 |            100 |              0.6830              |        68.30 |         273.20 |
| B            |       5 |          1,100 |              0.6209              |       682.96 |       3,414.80 |
| ***Tổng B*** |         |                |                                  | ***999.94*** | ***4,169.57*** |
| C            |       1 |              0 |              0.9091              |         0.00 |           0.00 |
| C            |       2 |              0 |              0.8264              |         0.00 |           0.00 |
| C            |       3 |              0 |              0.7513              |         0.00 |           0.00 |
| C            |       4 |              0 |              0.6830              |         0.00 |           0.00 |
| C            |       5 |          1,000 |              0.6209              |       620.92 |       3,104.60 |
| ***Tổng C*** |         |                |                                  | ***620.92*** | ***3,104.60*** |

$$
\begin{align}
D_{A} &= \frac{2,735.47}{999.98} \approx 2.74 \text{ năm}\\\\
D_{B} &= \frac{4,169.57}{\text{999.94}} \approx 4.17 \text{ năm}\\\\
D_{C} &= \frac{3,104.60 }{\text{620.92}} \approx 5 \text{ năm}\\
\end{align}
$$

- **Kết luận:**
	- Với trái phiếu zero-coupon, duration = thời gian đáo hạn
	- Giữ nguyên thời gian đáo hạn, ***coupon càng cao thì duration càng thấp*** `<< coupon càng cao thì dòng tiền càng sớm hơn >>`
	- Giữ lãi suất coupon không đổi, ***thời gian đáo hạn càng dài thì duration càng cao*** `<< thời gian càng dài thì dòng tiền càng muộn >>`
	- Giữ các nhân tố khác không đổi, ***YTM càng cao thì duration càng thấp*** `<< giống coupon, dòng tiền thu về sớm hơn >>`
##### 5.4.2. Modified Duration
|                         | Công thức                                                                                                                                      | Ý nghĩa                                                                                            |
| ----------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| ***Macaulay Duration*** | $$D_{macaulay} = \sum_{t= 1}^T \ t \cdot \frac{DCF_t}{P} \tag{3.1}$$                                                                           | Tính thời gian trung bình hoàn vốn                                                                 |
| ***Modified Duration*** | $$D_{modified}= \frac{D_{macaulay}}{1 + YTM_{periodic}} \tag{3.2}$$<br>$$\text{hoặc:} \quad D_{modified}= -\frac{1}{P} \cdot \frac{dP}{dYTM}$$ | Đo độ nhạy giá trái phiếu với lãi suất. Cho biết giá thay đổi bao nhiêu % khi lãi suất thay đổi 1% |

- **Công thức tính % thay đổi giá dựa trên Duration:**
	$$
	\begin{align}
	\frac{\Delta P}{P} = - D_{modified} \cdot \Delta YTM \tag{3.3}\\\\
	\end{align}
	$$
- **Chứng minh công thức:** `<< đạo hàm 1 lần của P theo YTM>>`
	$$
	\begin{align}
	&P = \sum_{t=1}^T \ \frac{CF_t}{(1 + YTM)^t} \\\\
	&\Rightarrow \frac{dP}{dYTM} = \sum_{t=1}^T \ \frac{CF_t}{(1+YTM)^t} \\\\
	&\Leftrightarrow\ ...\ = \sum_{t=1}^T \ \frac{-t \cdot CF_t}{(1+YTM)^{t+1}} \\\\
	&\Leftrightarrow\ ...\ = -P \cdot \left( \frac{1}{P} \cdot \sum_{t=1}^T \frac{t \cdot CF_t}{(1+YTM)^t} \right) \cdot \frac{1}{1+YTM} \\\\
	\text{Thay (3.1) và (3.2)} \quad
	&\Leftrightarrow\ ...\ = -P \cdot \frac{D_{macaulay}}{1+YTM} = -P \cdot D_{modified} \\\\
	&\Rightarrow \frac{dP}{dYTM} \cdot \Delta YTM = -P \cdot D_{modified} \cdot \Delta YTM\\\\
	&\Leftrightarrow \Delta P = -P \cdot D_{modified} \cdot \Delta YTM\\\\
	&\Leftrightarrow \frac{\Delta P}{P} = -D_{modified} \cdot \Delta YTM\\\\
	\end{align}
	$$
### 5.5. Convexity
- ***Duration chỉ đo được sự thay đổi tuyến tính***. Qui tắc duration là một ước tính tương đối tốt nếu lãi suất thay đổi nhỏ, và sai số sẽ càng cao khi biến động lãi suất càng mạnh
- ***Độ lồi (Convexity)*** ***đo được sự thay đổi phi tuyến tính (bậc 2)***, điều chỉnh sai số của Duration giúp ước lượng chính xác hơn
- **Đặc điểm Convexity:**
	- Lãi suất coupon càng thấp thì độ lồi càng cao
	- Thời hạn càng dài thì độ lồi càng cao
	- Khi lợi suất tăng thì độ lồi giảm. Đường cong giá lồi hơn ở mức lợi suất thấp và ít lồi hơn ở mức lợi suất cao
	- Khi lợi suất giảm, giá trái phiếu tăng lên nhiều hơn so với việc giá trái phiếu giảm khi lợi suất tăng cùng một lượng
	- Giả sử 2 trái phiếu cùng Duration, trái phiếu A có đường cong giá lồi hơn trái phiếu B
		- Khi lợi suất giảm, giá A tăng nhiều hơn B
		- Khi lợi suất tăng, giá A giảm ít hơn B
- ![[convexity.png#center|480x]]
- **Công thức Convexity:**
	$$
	\begin{align}
	\text{Convexity} &= \frac{1}{P} \cdot \frac{d^2P}{d{YTM}^2} = \frac{1}{P} \cdot \left[ \frac{dP}{dYTM} \right]'_{YTM} \\\\
	&= \frac{1}{P} \cdot \left[ \sum_{t=1}^T \ \frac{-t \cdot CF_t}{(1+YTM)^{t+1}} \right]'_{YTM} \\\\
	&= \frac{1}{P} \cdot \sum_{t=1}^T \ \frac{t \cdot (t+1) \cdot CF_t}{(1+YTM)^{t+2}} \tag{4.1}\\\\
	\end{align}
	$$
- **Công thức % thay đổi giá dựa trên Convexity:** `<< chứng minh bằng cách lấy đạo hàm 2 lần của P theo YTM>>`
	$$
	\begin{align}
	\frac{\Delta P}{P} = - D_{modified} \cdot \Delta YTM + \frac{1}{2} \cdot \text{Convexity} \cdot \Delta YTM^2\tag{4.2}\\\\
	\end{align}
	$$
---
- **Đối với trái phiếu có quyền chọn lại (Callable Bond):** `<< không thể dùng YTM do có thể bị thu hồi sớm, dùng r >>`
	$$
	\begin{align}
	P_r = min(P_{non-callable},\  C)\\
	\end{align}
	$$
	- Khi ***lãi suất r cao***, trái phiếu vẫn sẽ hoạt động như trái phiếu bình thường
		$$
		\begin{align}
		P_r &= P_{non-callable}\\\\
		\Rightarrow \frac{dP_r}{dr} &< 0\\\\
		\text{và:}\quad \frac{d^2P_r}{dr^2} &> 0 
		\end{align}
		$$
	- Tại ***vùng r mà giá trái phiếu sắp bị Call***, khi r giảm, giá sẽ không còn ***tăng với tốc độ tăng dần*** như trước (Positive Convexity), mà giá sẽ ***tăng với tốc độ giảm dần*** (Negative Convexity) `<< đạo hàm bậc 2 để nói về tốc độ thay đổi của độ dốc, convexity âm vì đồ thị đang cong lên bỗng cong xuống >>`
		$$
		\begin{align}
		P_r &= P_{non-callable}\\\\
		\Rightarrow \frac{dP_r}{dr} &\rightarrow 0\\\\
		\text{và:}\quad \frac{d^2P_r}{dr^2} &< 0 
		\end{align}
		$$
	- Khi ***lãi suất r giảm tới một ngưỡng nào đó***, nhà phát hành quyết định thu hồi ở mức giá Call. Lúc này, ***giá không còn phụ thuộc vào lãi suất r nữa*** (Convexity phẳng)
		$$
		\begin{align}
		P_r &= C\\\\
		\Rightarrow \frac{dP_r}{dr} &= 0\\\\
		\text{và:}\quad \frac{d^2P_r}{dr^2} &= 0 
		\end{align}
		$$