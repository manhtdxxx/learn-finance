> [!NOTE] *Công thức tổng quát tính lợi suất kì vọng và rủi ro cho danh mục bất kì*
> $$
> \begin{aligned}
> E(r_P) &= \sum_{i=1}^n w_i \cdot E(r_i)\\\\
> \sigma_P^2 &= \sum_{i=1}^n \sum_{j=1}^n w_i w_j \, \text{Cov}(r_i, r_j) \\
> \end{aligned}
> $$

---
# 1. Between Risky Assets and Risk-Free Assets

> [!NOTE]
> Để đơn giản hóa, danh mục đầu tư sẽ chỉ gồm 1 tài sản rủi ro và 1 tài sản phi rủi ro
### 1.1. Expected Return and Risk

$$
\begin{flalign*}
C &: \text{danh mục C gồm 1 tài sản rủi ro và 1 tài sản phi rủi ro} \\
E(r_C) &: \text{tỷ suất sinh lời kì vọng của danh mục C} && \\
y &: \text{tỷ trọng tài sản rủi ro trong danh mục} && \\
E(r_p) &: \text{tỷ suất sinh lời kì vọng của tài sản rủi ro P} && \\
r_f &: \text{tỷ suất sinh lời của tài sản phi rủi ro} &&  \\
\end{flalign*}
$$
$$
\begin{align}
E(r_C) &= y \cdot E(r_p) + (1-y) \cdot r_f\\
&= r_f + y \cdot [\ E(r_p) - r_f\ ] \tag{1.1}\\\\
\sigma_C &= y \cdot \sigma_p + (1-y) \cdot 0 \\
&=y \cdot \sigma_p \tag{2.1}\\\\
\end{align}
$$
### 1.2. Capital Allocation Line (CAL)
- Thay công thức `(2.1)` vào `(1.1)`, ta có:
$$
\begin{align}
E(r_C) &= r_f + \frac{[\ E(r_p) - r_f\ ]}{\sigma_p} \cdot \sigma_C \tag{1.2}\\
\end{align}
$$
![[MPT_1.jpg#center|480x]]

- **Đường phân bổ vốn (CAL)** là tập hợp các điểm thể hiện sự kết hợp giữa lợi nhận và rủi ro của các danh mục đầu tư bao gồm tài sản rủi ro và phi rủi ro (y là tỷ trọng tài sản rủi ro). Gồm các thành phần:
	- ***Điểm R(f)***, tại đó nhà đầu tư nắm giữ tài sản phi rủi ro (y=0)
	- ***Điểm P***, danh mục chỉ bao gồm tài sản rủi ro (y=1)
	- ***Đoạn từ R(f) tới P***, tập hợp tất cả tài sản trong danh mục đầu tư, bao gồm rủi ro và phi rủi ro (0 < y < 1)
	- ***Đoạn từ P trở lên***, tài sản rủi ro vượt quá vốn đầu tư của danh mục (y > 1), lúc này nhà đầu tư đi vay thêm với lãi suất phi rủi ro để đầu tư vào tài sản rủi ro
- **Độ dốc của đường CAL** còn gọi là *tỷ lệ phần bù rủi ro*, hoặc *hệ số Sharpe*
$$
\begin{align}
Sharpe\ Ratio &= \frac{E(r_C) - r_f}{\sigma_C} \tag{3}\\
\end{align}
$$
---
![[CAL_with_leveraging.png#center|480]]
- Giả sử một nhà đầu tư có ngân sách đầu tư 300 triệu VNĐ và muốn vay thêm 120 triệu VNĐ để đầu tư vào tài sản rủi ro. Đây là một vị thế đòn bẩy ***(Leveraging)*** trong tài sản rủi ro (sử dụng vốn vay để mở rộng quy mô đầu tư vào tài sản rủi ro nhằm tăng lợi nhuận kì vọng, đi kèm với đó là rủi ro tăng theo). Khi đó, tỷ trọng đầu tư vào tài sản rủi ro là:
	$$
	\begin{align}
	y = \frac{300 + 120}{300} = 1.4
	\end{align}
	$$
- Khi đó, lợi suất kì vọng và rủi ro của danh mục mới như sau:
	$$
	\begin{align}
	E(r_C) &= r_f + y \cdot [\ E(r_p) - r_f\ ] = 7\% + 1.4 \cdot (15\% - 7\%) = 18.2\%\\\\
	\sigma_C &= y \cdot \sigma_p = 1.4 \cdot 22\% = 30.8\% \\\\
	Sharpe\ Ratio &= \frac{E(r_C) - r_f}{\sigma_C} = \frac{18.2\% - 7\%}{30.8\%} = 0.36\\
	\end{align}
	$$
- Tuy nhiên, các nhà đầu tư không thể vay với mức lãi suất phi rủi ro. Người cho vay sẽ yêu cầu lãi suất cao hơn đối với nhà đầu tư. Giả sử lãi suất vay = 9%. Khi đó, độ dốc của CAL sẽ gấp khúc tại điểm P (y>1)
	$$
	\begin{align}
	Sharpe\ Ratio &= \frac{E(r_p) - r_{f'}}{\sigma_p} = \frac{15\% - 9\%}{22\%} = 0.27\\
	\end{align}
	$$
- Như vậy, độ dốc của CAL sẽ giảm khi sử dụng đòn bẩy. Nói cách khác, nếu nhà đầu tư đi vay để đầu tư vào tài sản rủi ro, lợi nhuận tăng thêm sẽ giảm khi độ lệch chuẩn tăng thêm 1 đơn vị
# 2. Among Risky Assets
> [!NOTE]
> Để đơn giản hóa, danh mục đầu tư sẽ chỉ gồm 2 tài sản rủi ro
### 2.1. Expected Return and Risk
$$
\begin{flalign*}
P &: \text{danh mục P gồm 2 tài sản rủi ro: 1 trái phiếu và 1 cổ phiếu} \\
E(r_P) &: \text{tỷ suất sinh lời kì vọng của danh mục P} && \\
 w_D &: \text{tỷ trọng của trái phiếu trong danh mục} && \\
 E(r_D) &: \text{tỷ suất sinh lời kì vọng của trái phiếu} && \\
 w_E &: \text{tỷ trọng của cổ phiếu trong danh mục} && \\
 E(r_E) &: \text{tỷ suất sinh lời kì vọng của cổ phiếu} && \\
\end{flalign*}
$$
$$
\begin{align}
E(r_P) &= w_D \cdot E(r_D) + w_E \cdot E(r_E) \tag{1.3}\\\\
\sigma^2_P &= w^2_d \cdot \sigma^2_D + w^2_e \cdot \sigma^2_E + 2 \cdot w_D \cdot w_E \cdot Cov(r_D, r_E) \tag{2.2}\\
&= w^2_d \cdot \sigma^2_D + w^2_e \cdot \sigma^2_E + 2 \cdot w_D \cdot w_E \cdot \sigma_D \cdot \sigma_E \cdot \rho_{DE} \\\\
\end{align}
$$
### 2.2. Efficient Frontier
- Hệ số tương quan đi từ -1 đến 1. Rủi ro của danh mục sẽ cao hơn khi hệ số tương quan giữa 2 tài sản càng cao
- Khi 2 tài sản tương quan đồng biến hoàn toàn ***(p = 1)***, rủi ro của danh mục sẽ cao nhất:
	$$
	\begin{align}
	\sigma_P =  w_D \cdot \sigma_D + w_E \cdot \sigma_E \\
	\end{align}
	$$
- Khi 2 tài sản nghịch biến hoàn toàn ***(p = -1)***, rủi ro của danh mục sẽ thấp nhất:
	$$
	\begin{align}
	\sigma_P = \left| w_D \cdot \sigma_D - w_E \cdot \sigma_E \right| \\
	\end{align}
	$$
- Khi ***p = -1***, có thể có được một vị thế phòng ngừa rủi ro hoàn bằng cách xác định tỷ trọng cho mỗi tài sản như sau : `<< TH đặc biệt của công thức (4.1) và (4.2) >>`
	$$
	\begin{align}
	\sigma_P &= \left| w_D \cdot \sigma_D - w_E \cdot \sigma_E \right| = 0\\
	&\Leftrightarrow w_D \cdot \sigma_D = w_E \cdot \sigma_E = (1-w_D) \cdot \sigma_E\\\\
	&\Leftrightarrow w_D = \frac{\sigma_E}{\sigma_D + \sigma_E} = 1 - w_E\\
	&\Leftrightarrow w_E = \frac{\sigma_D}{\sigma_D + \sigma_E} = 1 - w_D\\
	\end{align}
	$$
---
- Để ***tối thiểu hóa rủi ro*** của danh mục, ta có thể tìm ra ***tỷ trọng tối ưu*** cho từng tài sản rủi ro bằng cách đạo hàm phương sai theo tỷ trọng :
$$
\begin{align}
\sigma^2_P &= w^2_d \cdot \sigma^2_D + (1-w_D)^2 \cdot \sigma^2_E + 2 w_D (1-w_D) \cdot \sigma_D \cdot \sigma_E \cdot \rho_{DE} \\\\
\Rightarrow \frac{d}{dw_D} \sigma^2_P &= 2w_D \cdot \sigma_D^2 - 2(1 - w_D) \cdot \sigma_E^2 + 2(1 - 2w_D) \cdot \sigma_D \cdot \sigma_E \cdot \rho_{DE} = 0 \\\\
\Leftrightarrow w^*_D &= \frac{\sigma_E^2 - \sigma_D \cdot \sigma_E \cdot \rho_{DE}}{\sigma_D^2 + \sigma_E^2 - 2 \cdot \sigma_D \cdot \sigma_E \cdot \rho_{DE}} 
= \frac{\sigma_E^2 - Cov(r_D, r_E)}{\sigma_D^2 + \sigma_E^2 - 2 \cdot Cov(r_D, r_E)} \tag{4.1}\\\\
w^*_E &= 1 - w^*_D \tag{4.2}\\
\end{align}
$$
---
![[MPT_efficient_frontier_1.png#center|560]]
- Biết trước rủi ro (độ lệch chuẩn) của tài sản A và B cho trước, A rủi ro cao hơn B, ta dùng công thức (2) để tính rủi ro của danh mục khi thay đổi tỷ trọng đầu tư vào tài sản A
	- Với ***p = 1***, không có điểm thấp nhất, rủi ro không thể đa dạng hóa
	- Với ***p = 0.5***, tồn tại 1 điểm thấp nhất, rủi ro của danh mục có thể được đa dạng hóa nếu phân bổ tài sản hợp lý
	- Với ***p = - 0.5***, rủi ro của danh mục có thể giảm xuống sâu hơn so với ***p = 0.5***, thể hiện đa sự đa dạng hóa hiệu quả hơn khi tài sản A giảm thì tài sản B sẽ tăng
	- Với ***p = -1***, rủi ro của danh mục có thể giảm xuống mức thấp nhất là 0 nếu chọn tỷ trọng phù hợp
---
![[MPT_efficient_frontier_2.png#center|480]]
- Ta xây dựng danh mục từ 2 tài sản rủi ro Security 1 và Security 2 với hệ số tương quan **`p`**:
	- Đường thẳng nét đứt `nếu p = 1`
		- Các danh mục nằm trên đường này không thể đa dạng hóa
	- Đường cong màu đen `nếu -1 < p < 1`
		- Phần cong hướng lên là ***đường biên hiệu quả (Efficient Frontier)*** – tập hợp các danh mục mang lại lợi suất cao nhất với một mức rủi ro cho trước
		- Phần cong hướng xuống là các danh mục không hiệu quả (Inefficient Portfolios) – có thể bị thay thế bởi danh mục khác có cùng rủi ro nhưng lợi suất cao hơn
		- Điểm G là ***danh mục phương sai tối thiếu (Global Minimum Variance Portfolio)*** - danh mục có rủi ro thấp nhất
	- Đường thẳng gãy khúc `nếu p = -1`
		- Danh mục có khả năng giảm rủi ro về 0
### 2.3. Tangency Portfolio
- Theo lý thuyết danh mục đầu tư hiện đại (Modern Portfolio Theory - MPT):
	- Sau khi xác định được tập hợp các danh mục rủi ro hiệu quả trên đường biên hiệu quả (Efficient Frontier) và một mức lãi suất phi rủi ro đã biết, ta lựa chọn **danh mục có tỷ lệ phần bù rủi ro trên mỗi đơn vị rủi ro (Sharpe Ratio) cao nhất**
	- Đường phân bổ vốn CAL được vẽ bằng cách nối điểm đại diện cho lãi suất phi rủi ro với danh mục được chọn
	- Danh mục tại điểm tiếp xúc giữa CAL và đường biên hiệu quả được gọi là danh mục tiếp điểm (Tangency Portfolio) - tại đó độ dốc CAL = độ dốc đường biên hiệu quả
---
- Cách xác định ***tỷ trọng tối ưu*** cho ***danh mục tiếp điểm***:
$$
\begin{align}
\text{Sharpe Ratio} &= \frac{E(r_P) - r_f}{\sigma_P}
\\
&\Rightarrow \frac{d}{dw_D} S =  \frac{\left [ \frac{d}{dw_D}E(r_P) \right ] \cdot \sigma_P - (E(r_P) - r_f) \cdot \left [ \frac{d}{dw_D} \sigma_P \right ]}{\sigma^2_P} = 0
\\
&\Rightarrow \frac{d}{dw_D}E(r_P) \cdot \sigma_P = (E(r_P) - r_f) \cdot \frac{d}{dw_D} \sigma_P
\\\\\\
\text{Trong đó: }\quad 
&E(r_P) = w_D \cdot E(r_D) + (1 - w_D) \cdot E(r_E)
\\
&\Rightarrow \frac{d}{dw_D} E(r_P) = E(r_D) - E(r_E)
\\
\text{và: }\quad 
&\sigma_P = \sqrt{\sigma^2_P}
\\
&\Rightarrow \frac{d}{dw_D} \sigma_P = \frac{1}{2 \sqrt{\sigma^2_P}} (\frac{d}{dw_D} \sigma^2_P)  = \frac{1}{\sigma_P}  [\ w_D \sigma_D^2 - (1 - w_D) \sigma_E^2 + (1 - 2w_D) \sigma_D \sigma_E \rho_{DE} \ ]
\\\\\\
\text{Thay: }\quad 
&\Rightarrow [\ E(r_D) - E(r_E)\ ] \cdot \sigma^2_P = [\ E(r_P) - r_f\ ] [\ w_D \sigma_D^2 - (1 - w_D) \sigma_E^2 + (1 - 2w_D) \sigma_D \sigma_E \rho_{DE} \ ]
\\\\
&\Rightarrow w_D^* = \frac{(E(r_D) - r_f) \cdot \sigma_E^2 - (E(r_E) - r_f) \cdot \sigma_D \sigma_E \rho_{DE} }{ (E(r_D) - r_f) \cdot \sigma_E^2 + (E(r_E) - r_f) \cdot \sigma_D^2 - (E(r_D) + E(r_E) - 2r_f) \cdot \sigma_D \sigma_E \rho_{DE} }
\end{align}
$$
# 3. Utility & Indifference Curve
- Nhà đầu tư thường quan tâm đến hai yếu tố chính: lợi nhuận kì vọng & rủi ro
- **Hàm hữu dụng (Utility Function)** thể hiện sự đánh đổi giữa rủi ro và lợi nhuận mà nhà đầu tư chấp nhận được. Công thức như sau:
	$$
	\begin{align}
	U &= E(r_P) - 0.5A \cdot \sigma^2_P \tag{5}\\
	\Leftrightarrow\  E(r_P) &= U + 0.5 \cdot A \cdot \sigma^2_P 
	\end{align}
	$$
- **Đường bàng quan (Indifference Curve):**
	- *Mỗi điểm trên đường bàng quan* đại diện cho một danh mục đầu tư mà nhà đầu tư xem là tương đương về mức độ thỏa mãn U, dù có sự khác nhau về rủi ro và lợi nhuận kỳ vọng
	- *Mỗi mức độ thỏa mãn U* khác nhau là mỗi đường bàng quan khác nhau
		- U càng cao thì đường bàng quan nằm cao hơn trên biểu đồ, phản ánh mức độ hài lòng cao hơn với danh mục đầu tư
		- U thấp thì đường bàng quan năm thấp hơn trên biểu đồ
		![[MPT_indifference_curve_1.png#center|480]]
	- *Mức ngại rủi ro A* sẽ quyết định độ dốc của đường bàng quan
		- A cao thì đường bàng quan dốc hơn, phản ánh nhà đầu tư yêu cầu phần bù rủi ro cao hơn `<< đạo hàm E(r)'(sigma) = A . sigma -> A cao hơn thì E(r) dốc hơn >>`
		- A thấp thì đường bàng quan thoải hơn
		![[MPT_indifference_curve_2.png#center|480]]

### 3.1. Mean-Variance Optimal Risky Portfolio on Efficient Frontier
- Công thức `(4.1)` và `(4.2)` dành cho việc tìm kiếm danh mục với phương sai tối thiểu (Minimum Variance Portfolio). Tuy vậy, danh mục không đảm bảo lợi nhuận cao cho những nhà đầu tư ưa thích rủi ro
- Tại mức rủi ro chấp nhận A, nhà đầu tư có thể xác định **tỷ trọng tối ưu** cho từng **tài sản rủi ro** nhằm **tối đa hóa giá trị hữu dụng (Mean-Variance Optimal)**. Đó là tiếp điểm (Tangency Point) giữa đường bàng quan và đường biên hiệu quả - tại đó độ dốc giữa 2 đường bằng nhau
	![[MPT_2.png#center|360]]
	$$
	\begin{align}
	U &= E(r_P) - 0.5A \cdot \sigma^2_P 
	\\
	&= w_D \cdot E(r_D) + (1 - w_D) \cdot E(r_E) - 0.5A \cdot \sigma^2_P
	\\\\
	\Rightarrow \frac{d}{dw_D} U &=  E(r_D) - E(r_E) - 0.5A \cdot (\frac{d}{dw_D} \sigma^2_P) = 0 
	\\\\
	\text{Trước đó: }\quad \frac{d}{dw_D} \sigma^2_P &= 2w_D \cdot \sigma_D^2 - 2(1 - w_D) \cdot \sigma_E^2 + 2(1 - 2w_D) \cdot \sigma_D \cdot \sigma_E \cdot \rho_{DE} 
	\\\\
	\Rightarrow E(r_D) - E(r_E) &= A \cdot [\ w_D \cdot \sigma_D^2 - (1 - w_D) \cdot \sigma_E^2 + (1 - 2w_D) \cdot \sigma_D \cdot \sigma_E \cdot \rho_{DE}\ ] 
	\\\\
	\Leftrightarrow E(r_D) - E(r_E) &= A \cdot [\ w_D (\sigma_D^2 + \sigma_E^2 - 2 \sigma_D \sigma_E \rho_{DE}) - \sigma_E^2 + \sigma_D \sigma_E \rho_{DE}\ ]
	\\\\
	\Leftrightarrow w^*_D &= \frac{E(r_D) - E(r_E) + A \cdot (\sigma_E^2 - \sigma_D \sigma_E \rho_{DE})}{ A \cdot (\sigma_D^2 + \sigma_E^2 - 2 \sigma_D \sigma_E \rho_{DE})} \tag{4.3}
	\\\\
	w^*_E &= 1 - w^*_D \tag{4.4}
	\\
	\end{align}
	$$
### 3.2. Mean-Variance Optimal Portfolio on CAL
- Công thức `(4.3)` và `(4.4)` tìm tỷ trọng để tối đa hóa giá trị hữu dụng cho danh mục chỉ gồm các tài sản rủi ro
- Tuy nhiên, trong thực tế, nhà đầu tư có thể phân bổ vốn giữa tài sản phi rủi ro (như trái phiếu chính phủ) và danh mục tài sản rủi ro tối ưu
- Tại tiếp điểm (Tangency Point) giữa đường bàng quan và CAL - tại đó độ dốc của 2 đường bằng nhau, nhà đầu tư đạt **giá trị hữu dụng tối đa (Mean-Variance Optimal)** với **tỷ trọng tối ưu** giữa **tài sản rủi ro và phi rủi ro** (y là tỷ trọng của tài sản rủi ro)
	$$
	\begin{align}
	U &= E(r_C) - 0.5A \cdot \sigma^2_C 
	\\
	&= y \cdot E(r_P) + (1 - y) \cdot r_f - 0.5A \cdot \sigma^2_P
	\\\\
	(4.3) \Rightarrow y^* &= \frac{E(r_P) - r_f}{ A \cdot \sigma^2_P} \tag{4.5}
	\\\\
	\end{align}
	$$
	