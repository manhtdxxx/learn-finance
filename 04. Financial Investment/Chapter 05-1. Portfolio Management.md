# 1. Portfolio Theory
### 1.1. Risk & Return
##### 1.1.1. One Risky Asset
- `r_i: lợi nhuận ứng với khả năng i`
- `p_i: xác suất xảy ra khả năng i`
- `n: số khả năng có thể xảy ra`
$$
\begin{align}
E(r) = \sum_{i=1}^n p_i \cdot r_i\\\\
\sigma= \sqrt{\sum_{i=1}^n\ [\ r_i - E(r)\ ]^2}\\\\
\end{align}
$$
##### 1.1.2. One Risky Asset + One Risk-free Asset
- **Lợi nhuận kỳ vọng & Rủi ro**
	$$
	\begin{align}
	E(r_p) &= w_a \cdot E(r_a) + (1- w_a) \cdot r_f\\
	&= r_f + w_a \cdot [\ E(r_a) - r_f\ ]\\\\
	\sigma_p &= w_a \cdot \sigma_a + (1-w_a) \cdot 0 \\
	&=w_a \cdot \sigma_a\\\\
	\end{align}
	$$
- **Đường phân bổ vốn CAL (Capital Allocation Line)**
	$$
	\begin{align}
	E(r_p) &= r_f + \frac{[\ E(r_a) - r_f\ ]}{\sigma_a} \cdot \sigma_p\\\\
	\end{align}
	$$
### 1.2. Mức ngại rủi ro (Risk Aversion)
- Danh mục đầu tư sẽ càng hấp dẫn khi tỷ suất sinh lời càng cao và rủi ro càng thấp
- Thực tế, tỷ suất sinh lời tỷ lệ thuận với rủi ro, danh mục đầu tư nào hấp dẫn hơn sẽ trở nên không rõ ràng
- **Giá trị hữu dụng (Utility)** giúp lượng hóa các quyết định đầu tư cảm tính
	$$
	\begin{align}
	U &= E(r) - 0.5 \cdot A \cdot \sigma^2
	\end{align}
	$$
	- Hệ số 0.5 là một quy ước tỉ lệ
	- Utility tăng khi tỷ suất sinh lợi kỳ vọng tăng 
	- Utility giảm khi rủi ro cao; giảm tới mức nào còn phụ thuộc vào A
- **Tỷ suất lợi nhuận tương đương chắc chắn (Certainty Equivalent - CE)** là mức *tỷ suất lợi nhuận chắc chắn* mà nhà đầu tư sẵn sàng chấp nhận *thay cho* một *khoản đầu tư rủi ro*, vì nhà đầu tư đánh giá *hai lựa chọn* này có mức *hấp dẫn tương đương nhau* `<< ý nghĩa: tuy tỷ suất lợi nhuận chắc chắn < tỷ suất lợi nhuận rủi ro, nhưng mà lại bằng về utility >>`