# 1. Concept
| **Tiêu chí**          | **Tài sản thực**                                                                    | **Tài sản tài chính**                                   |
| --------------------- | ----------------------------------------------------------------------------------- | ------------------------------------------------------- |
| 1. Loại tài sản       | Bao gồm cả tài sản hữu hình và tài sản vô hình                                      | Là các tài sản tài chính                                |
| 2. Chuyển đổi sở hữu  | Việc thay đổi lĩnh vực đầu tư và chủ sở hữu rất khó khăn                            | Việc thay đổi lĩnh vực đầu tư và chủ sở hữu rất dễ dàng |
| 3. Lợi ích đầu tư     | Lợi ích đầu tư có thể là lợi nhuận hoặc phi lợi nhuận tùy thuộc vào mục đích đầu tư | Lợi ích đầu tư chủ yếu là lợi nhuận                     |
| 4. Phân phối thu nhập | Phân phối lần đầu                                                                   | Phân phối lại thu nhập                                  |
| 5. Thuế               | Đánh thuế một lần                                                                   | Chịu thuế hai lần                                       |
| 6. Hình thức đầu tư   | Đầu tư trực tiếp                                                                    | Đầu tư gián tiếp                                        |
| 7. Tính thanh khoản   | Thanh khoản thấp                                                                    | Thanh khoản cao                                         |
# 2. Financial Instrument
[[Chapter 03-1. Financial Instrument]]

# 3. Return & Risk
### 3.1. Return
- **Thu nhập từ đầu tư tài chính:**
	- Cổ tức, trái tức, ...
	- Chênh lệch giá bán - giá mua
- **Tỷ suất sinh lời theo kỳ / Holding Period Yield - HPY:**
$$
\begin{align}
\text{HPY} = \frac{\text{Ending Value} - \text{Initial Value} + \text{Income Generated}}{\text{Initial Value}}\\\\
\end{align}
$$
- **Tỷ suất sinh lời trung bình hàng năm:**
	- Phương pháp trung bình cộng (Arithmetic Mean)  `-- bỏ qua hiệu ứng lãi kép --`
		$$
		\begin{align}
		R_{arithmetic} = \frac{1}{n} \cdot \sum_{i=1}^n HPY_{annual}\\
		\end{align}
		$$
	- Phương pháp trung bình nhân (Geometric Mean)
		$$
		\begin{align}
		R_{geometric} = \sqrt{\prod_{i=1}^n\  (1 + HPY_{annual})}\ -\ 1\\\\
		\end{align}
		$$
- **Tỷ suất sinh lời kì vọng:**
	$$
	\begin{align}
	E(R) = \sum_{i=1}^n p_i \cdot R_i\\\\
	\end{align}
	$$
- **Tỷ suất sinh lời thực tế:**
	$$
	\begin{align}
	\text{Nominal Return} &= (1 + \text{Real Return}) \cdot (1 + \text{Inflation Rate}) - 1\\\\
	\Leftrightarrow \text{Real Return} &= \frac{1 + \text{Nominal Return}}{1 + \text{Inflation Rate}} - 1\\\\
	\end{align}
	$$
### 3.2. Risk
- Rủi ro tài chính phản ánh sự sai biệt giữa tỷ suất lợi nhuận thực tế với tỷ suất lợi nhuận kỳ vọng
	$$
	\begin{align}
	\sigma= \sqrt{\sum_{i=1}^n\ p_i \cdot [\ R_i - E(R)\ ]^2}\\
	\end{align}
	$$
- **Các loại rủi ro:**
	- Rủi ro phi hệ thống ***(Unsystematic Risk / Firm-specific Risk / Diversifiable Risk)***
		- Tác động đến một công ty hoặc một nhóm nhỏ các công ty
		- Nguyên nhân: các yếu tố nội tại của công ty gây ra và nó có thể kiểm soát được
		- VD: rủi ro kinh doanh, rủi ro tài chính, rủi ro quản lý...
		- Giảm đến loại bỏ hoàn toàn khi dang mục đầu tư càng đa dạng hóa
	- Rủi ro hệ thống ***(Systematic Risk / Market Risk / Non-diversifiable Risk)***
		- Tác động đến toàn bộ thị trường hoặc phân khúc thị trường
		- Nguyên nhân: các yếu tố vĩ mô như lạm phát, chính sách vĩ mô, thay đổi công nghệ, tỷ giá....
		- Không thể loại bỏ nhờ đa dạng hóa danh mục. Có thể giảm thông qua phân bổ vốn đầu tư
### 3.3. Risk Premium
- Phần bù rủi ro thể hiện mối quan hệ giữa rủi ro và lợi tức kỳ vọng: với rủi ro càng cao, lợi tức mà nhà đầu tư kỳ vọng nhận được cũng càng cao
	$$
	\begin{align}
	\text{Risk Premium} = \text{Required Rate of Return} - \text{Risk-free Rate}
	\end{align}
	$$
	