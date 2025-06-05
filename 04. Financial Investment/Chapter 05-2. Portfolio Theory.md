# 1. Overview
### 1.1. Expected Return & Risk
- **Đối với 1 tài sản:**
$$
\begin{flalign*}
E(r) &: \text{lợi suất kì vọng của tài sản}\\
 r_i &: \text{lợi suất của tài sản ứng với khả năng i} && \\
 p_i &: \text{xác suất xảy ra khả năng i} && \\
n &: \text{số khả năng có thể xảy ra} &&  \\
\end{flalign*}
$$
$$
\begin{align}
E(r) = \sum_{i=1}^n p_i \cdot r_i\\\\
\sigma= \sqrt{\sum_{i=1}^n\ p_i \cdot [\ r_i - E(r)\ ]^2}\\\\
\end{align}
$$
- **Đối với danh mục đầu tư bất kì:**
$$
\begin{flalign*}
E(r_P) &: \text{lợi suất kì vọng của danh mục P}\\
E(r_i) &: \text{lợi suất kì vọng của tài sản i}\\
 w_i &: \text{tỷ trọng của tài sản i trong danh mục} && \\
  w_j &: \text{tỷ trọng của tài sản j trong danh mục} && \\
n &: \text{số tài sản trong danh mục} &&  \\
\end{flalign*}
$$
$$
\begin{align}
E(r_P) &= \sum_{i=1}^n w_i \cdot E(r_i)\\\\
\sigma_P = Var[\ E(r_p)\ ] &= \sum_{i=1}^n \sum_{j=1}^n w_i w_j \, \text{Cov}(r_i, r_j)\\\\
\end{align}
$$
### 1.2. Risk Aversion
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
	- Utility giảm khi rủi ro cao; giảm tới mức nào còn phụ thuộc vào **mức ngại rủi ro A**
		- A > 0 ***(Risk Averse)*** -  yêu cầu phần bù rủi ro cao hơn
		- A = 0 ***(Risk Neutral)*** - chỉ quan tâm tới lợi nhuận kì vọng
		- A < 0 ***(Risk Seeking)*** - sẵn sàng chấp nhận rủi ro cao để thu lợi lớn
# 2. Modern Portfolio Theory