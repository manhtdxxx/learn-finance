	# 1. Simple Index Model - SIM
### 1.1. Assumption
- Quan hệ tuyến tính giữa lợi suất của tài sản tài chính và lợi suất toàn thị trường
- Rủi ro của chứng khoán bao gồm hai thành phần:
	- Rủi ro hệ thống (rủi ro thị trường)
	- Rủi ro phi hệ thống (rủi ro đặc thù của công ty, không liên quan tới thị trường)
- Rủi ro phi hệ thống có kỳ vọng = 0
- Rủi ro phi hệ thống của các tài sản không có sự tương quan với nhau
- Beta là hằng số -> mối quan hệ giữa giá chứng khoán và chỉ số thị trường ổn định theo thời gian
- ...
### 1.2. Regression Equation
- **Lợi suất vượt trội (Excess Return):**
$$
\begin{flalign*}
 r_M &: \text{lợi suất của thị trường} && \\
 r_i &: \text{lợi suất của tài sản rủi ro thứ } i && \\
r_f &: \text{lợi suất của tài sản phi rủi ro} && \\
R_M &: \text{lợi suất vượt trội của thị trường} && \\
R_i &: \text{lợi suất vượt trội tài sản rủi ro thứ i} &&
\end{flalign*}
$$
$$
\begin{align}
R_M &= r_M - r_f\\
R_i &= r_i - r_f\\\\
\end{align}
$$
- **Phương trình hồi quy:** 
`<< khi có dữ liệu của lợi suất chứng khoán i và lợi suất thị trường trong quá khứ thì ta thực hiện hồi quy để tìm alpha, beta, phương sai của rủi ro phi hệ thống >>`
$$
\begin{flalign*}
\alpha_i &: \text{hệ số chặn của chứng khoán i} &&\\
\beta_i &: \text{độ nhạy cảm của chứng khoán i so với thị trường} &&\\
\epsilon_i(t) &: \text{rủi ro phi hệ thống của chứng khoán i tại thời điểm t } (E(\epsilon_i) = 0)
\end{flalign*}
$$
$$
\begin{align}
R_i(t) &= \alpha_i + \beta_i \cdot R_m(t) + \epsilon_i(t)\\\\
\end{align}
$$
- **Đại lượng thống kê:**
$$
\begin{align}
E(R_i) &= \alpha_i + \beta_i \cdot E(R_m) \tag{1}\\\\
\sigma^2_i &= \beta^2_i \cdot \sigma^2_M + \sigma^2(e_i) \tag{2}\\\\
Cov(r_i, r_j) &= \beta_i \cdot \beta_j \cdot \sigma^2_M \tag{3}\\\\
Corr(r_i, r_j) &= \frac{Cov(r_i, r_j)}{\sigma_i \cdot \sigma_j} = \frac{\beta_i \cdot \beta_j \cdot \sigma^2_M}{\sigma_i \cdot \sigma_j} \tag{4}\\
&= \frac{\beta_i \cdot \sigma^2_M \cdot \beta_j \cdot \sigma^2_M}{\sigma_i \cdot \sigma_M \cdot \sigma_j \cdot \sigma_M} = Corr(r_i, r_M) \cdot Corr(r_j, r_M)\\\\
\end{align}
$$
### 1.3. Portfolio Diversification
- **Lợi suất vượt trội của danh mục đầu tư** của các tài sản có tỷ trọng bằng nhau (w = 1/n)
	$$
	\begin{align}
	R_p = \sum_{i=1}^n wi \cdot R_i &= \frac{1}{n} \sum_{i=1}^n (\alpha_i + \beta_i \cdot R_m + \epsilon_i)\\\\
	&= (\frac{1}{n} \sum_{i=1}^n \alpha_i) + (\frac{1}{n} \sum_{i=1}^n \beta_i) \cdot R_m + (\frac{1}{n} \sum_{i=1}^n \epsilon_i)\\\\
	&= \alpha_p + \beta_p \cdot R_M + \epsilon_p\\\\
	\end{align}
	$$
- **Phương sai của danh mục đầu tư:**
	$$
	\begin{align}
	\sigma^2_p = \beta^2_p \cdot \sigma^2_M + \sigma^2(\epsilon_p)\\\\
	\end{align}
	$$
	-  Khi n càng lớn:
		- Rủi ro phi hệ thống ***(Unsystematic Risk)*** trở nên không đáng kể do là ngẫu nhiên từ phân phối có trung bình bằng 0, khi lấy trung bình thì chúng triệt tiêu
		- Rủi ro hệ thống ***(Systematic Risk)*** tồn tại bất kể mức độ đa dạng hóa của danh mục. Beta là tham số cố định cho từng tài sản, không mất đi khi lấy trung bình
		![[unsystematic_risk.png#center|560]]
# 2. Capital Asset Pricing Model - CAPM
### 2.1. Assumption
- Thị trường hoàn hảo `Perfect Capital Market`
	- Không phí giao dịch, không thuế
	- Thông tin hoàn hảo và có sẵn cho tất cả nhà đầu tư
	- Không giới hạn trong việc bán khống
	- Tồn tại cùng một lãi suất phi rủi ro mà nhà đầu tư có thể vay và cho vay không giới hạn
	- Không có sự thao túng thị trường
	- Tài sản có thể chia nhỏ vô hạn `Infinite Divisible Asset`
- Các nhà đầu tư 
	- Có hành vi hợp lý `Mean-Variance Optimal`: tối đa hóa lợi nhuận kỳ vọng dựa trên rủi ro
	- Có kỳ vọng đồng nhất `Homogenous Expectations`: mọi nhà đầu tư đều có cùng kỳ vọng về lợi nhuận, rủi ro và tương quan giữa các tài sản
	- Có cùng một khoảng thời gian đầu tư
- ...
### 2.2. Component Breakdown
- **Danh mục thị trường:**
	- Gồm ***toàn bộ các tài sản rủi ro*** hiện đang được giao dịch trên thị trường
	- Tỷ trọng của một cổ phiếu trong danh mục được đo lường bằng giá trị thị trường của cổ phiếu đó trên tổng danh mục đầu tư
- **Phần bù rủi ro:**
	- Là ***phần lợi suất kỳ vọng vượt trên lãi suất phi rủi ro*** để bù đắp cho nhà đầu tư về việc chấp nhận rủi ro đầu tư vào danh mục thị trường
	- Nếu phần bù rủi ro của danh mục thị trường > mức ngại rủi ro trung bình của các nhà đầu tư, nhà đầu tư sẽ tăng tỷ trọng đầu tư vào tài sản rủi ro --> cầu chứng khoán tăng, đẩy giá lên cao --> lợi suất của danh mục thị trường giảm --> phần bù rủi ro của danh mục thị trường giảm
	- Như vậy, phần bù rủi ro phải vừa đủ để nhà đầu tư có thể an tâm nắm giữ danh mục thị trường
		$$
		\begin{align}
		E(r_M) - r_f = \bar{A} \cdot \sigma^2_M\\\\
		\end{align}
		$$
- **Lợi suất kỳ vọng của chứng khoán riêng lẻ**
	- Nhà đầu tư muốn biết liệu đầu tư vào từng chứng khoán riêng lẻ có hấp dẫn hay không? 
	- Nhưng rủi ro của chứng khoán riêng lẻ không phải là độ lệch chuẩn tổng thể của danh mục thị trường. Vậy phần rủi ro nào thực sự ảnh hưởng đến lợi suất kỳ vọng của chứng khoán riêng lẻ?
	- Với ***danh mục thị trường đã đa dạng hóa***, rủi ro phi hệ thống có thể gần như bị triệt tiêu. Vì vậy, ta ***chỉ cần*** xác định định ***rủi ro hệ thống*** của chứng khoán riêng lẻ dựa trên công thức:
		$$
		\begin{align}
		\beta_i &= \frac{Cov(r_i, r_M)}{Var(r_M)} = \frac{Cov(r_i, r_M)}{\sigma^2_M}\\
		\end{align}
		$$
	- ***Lợi suất kỳ vọng của chứng khoán riêng lẻ*** được tính dựa trên rủi ro hệ thống (beta):
		$$
		\begin{align}
		E(r_i) &= r_f + \beta_i \cdot [\ E(r_M) - r_f\ ]\\\\
		\end{align}
		$$
### 2.3. Stock Market Line (SML)

| **Tiêu chí**      | **SML <br>(Security Market Line)**                                           | **CML <br>(Capital Market Line)**                                                                              | **CAL <br>(Capital Allocation Line)**                                                                                                                        |
| ----------------- | ---------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Áp dụng           | Cho từng ***tài sản riêng lẻ***                                              | Cho ***danh mục hiệu quả*** (danh mục thị trường + tài sản phi rủi ro)                                         | Cho ***bất kỳ danh mục*** rủi ro + tài sản phi rủi ro                                                                                                        |
| Thước đo rủi ro   | ***Beta*** (rủi ro hệ thống của từng tài sản riêng lẻ)                       | ***Độ lệch chuẩn (σ)*** – rủi ro tổng thể của danh mục hiệu quả                                                | ***Độ lệch chuẩn (σ)*** – rủi ro tổng thể của danh mục bất kỳ                                                                                                |
| Thành phần rủi ro | ***Chỉ xét rủi ro hệ thống*** (CAPM giả định đã loại bỏ rủi ro phi hệ thống) | Giả định ***đã đa dạng hóa hoàn toàn rủi ro phi hệ thống***                                                    | Có thể ***chưa đa dạng hóa hết rủi ro phi hệ thống***, tùy thuộc vào danh mục được chọn                                                                      |
| Ý nghĩa đường     | Mối quan hệ giữa Beta và lợi suất kỳ vọng (theo CAPM)                        | Hiệu quả tối ưu giữa rủi ro và lợi suất khi dùng danh mục thị trường. Chỉ tồn tại ***một đường CML duy nhất*** | Biểu diễn mọi lựa chọn kết hợp giữa tài sản rủi ro và phi rủi ro. Có ***nhiều đường CAL***, mỗi đường tùy thuộc vào danh mục rủi ro được chọn bởi nhà đầu tư |
| Độ dốc            | $$E(r_m) - r_f$$                                                             | $$\frac{E(r_m) - r_f}{\sigma_m}$$                                                                              | $$\frac{E(r_p) - r_f}{\sigma_p}$$                                                                                                                            |
| Đối tượng sử dụng | Nhà phân tích chứng khoán, dùng để định giá tài sản phiếu                    | Nhà đầu tư theo danh mục thị trường và tài sản phi rủi ro (chiến lược tối ưu thị trường)                       | Nhà đầu tư cá nhân với khẩu vị rủi ro riêng, chọn danh mục rủi ro bất kỳ kết hợp tài sản phi rủi ro                                                          |
- **Đường thị trường chứng khoán SML**
	![[SML.png#center|480]]
	- Nếu tài sản 
		- Nằm bên trái `beta = 1` --> tài sản có rủi ro thấp, và mức sinh lời cũng thấp hơn thị trường ***(defensive)***
		- Nằm bên phải `beta = 1` --> tài sản có rủi ro cao hơn thị trường, đòi hỏi mức sinh lời cao hơn ***(aggressive)***
		- Nằm trên SML --> tài sản được định giá thấp theo CAPM ***(undervalued)***, mức sinh lời thực cao hơn lý thuyết --> nên mua
		- Nằm dưới SML --> tài sản được định giá cao theo CAPM ***(overvalued)***, mức sinh lời thực thấp hơn lý thuyết --> nên bán
	---
	- Chênh lệch giữa tỷ lệ lợi tức kỳ vọng thực tế và tỷ lệ lợi tức đo lượng bởi CAPM trên một cổ phiếu gọi là ***α*** của cổ phiếu đó, hay là ***phần tỷ lệ lợi tức được định giá sai*** trên thị trường
		$$
		\begin{align}
		E(r_i) &= \alpha_i + r_f + \beta_i \cdot [\ E(r_M) - r_f\ ]\\\\
		\end{align}
		$$
# 3. Arbitrage Pricing Theory - APT
### 3.1. Assumption
- APT là một mô hình định giá tài sản thay thế cho mô hình CAPM. Nó cho rằng **lợi suất kỳ vọng của một tài sản là hàm tuyến tính của nhiều yếu tố rủi ro hệ thống**. VD: lãi suất, lạm phát, tăng trưởng kinh tế, ...
- Danh mục có **đủ chứng khoán để đa dạng hóa rủi ro đặc thù**
- **Các cơ hội kinh doanh chênh lệch giá không tồn tại lâu dài.** Khi có tài sản bị định giá sai, nhiều người sẽ cùng tận dụng cơ hội kiếm lời, khiến giá nhanh chóng về mức hợp lý, nên cơ hội chênh lệch giá không tồn tại lâu
### 3.2. Equation
- **Với 1 tài sản rủi ro:**
$$
\begin{flalign*}
 E(r_i) &: \text{lợi suất kỳ vọng của tài sản rủi ro i} && \\
r_f &: \text{lợi suất của tài sản phi rủi ro} && \\
b_{ij} &: \text{Độ nhạy của tài sản i với yếu tố j} && \\
F_j &: \text{Phần bù rủi ro do yếu tố j} && \\
m &= \text{Số lượng các yếu tố rủi ro hệ thống như (GDP, lạm phát, lãi suất, ...)}
\end{flalign*}
$$
$$
\begin{align}
E(r_i) = r_f + \sum_{j=1}^m \ b_{ij} \cdot F_j
\end{align}
$$
- **Với danh mục đầu tư:**
$$
\begin{flalign*}
E(r_p) &: \text{lợi suất kỳ vọng của danh mục P} && \\
r_{pf} &: \text{Lợi suất phi rủi ro của danh mục P} && \\
b_{pj} &: \text{Độ nhạy của danh mục P yếu tố j} && \\
F_j &: \text{Phần bù rủi ro do yếu tố j} &&
\end{flalign*}
$$
$$
\begin{align}
E(r_p) = \sum_{i=1}^n wi \cdot E(r_i) &= \sum_{i=1}^n wi \cdot \left[ \sum_{j=1}^m \ b_{ij} \cdot F_j \right ]\\\\
&= r_f \cdot \sum_{i=1}^n w_i + \sum_{j=1}^m \left[ F_j \cdot \sum_{i=1}^n \left [ w_i \cdot b_{ij} \right ] \right]\\\\
&= r_{pf} + \sum_{j=1}^m\ b_{pj} \cdot F_j \\
\end{align}
$$
### 3.3. How to arbitrage
- **Arbitrage (Kinh doanh chênh lệch giá)** là chiến lược mua một tài sản ở thị trường này và đồng thời bán nó ở thị trường khác để kiếm lời từ chênh lệch giá
- ***Ví dụ:***
	- Giá cổ phiếu ABC
		- Sàn A: 100$
		- Sàn B: 105$
	- ***Cách thực hiện arbitrage:***
		- Bước 1: Vay cổ phiếu ABC và thực hiện bán khống ***(short-selling)*** ở sàn B. ``<< bán tài sản mà bạn chưa sở hữu >>`
		- Bước 2: Số tiền bán được thực hiện mua cổ phiếu ở sàn A, lãi 5$.
		- Bước 3: Trả lãi số cổ phiếu ở đã vay ở bước 1. `<< nhận lãi mà k phải bỏ vốn đầu tư >>`
- ***Thực tế rất khó thực hiện:***
	- Tồn tại phí giao dịch trên sàn
	- Cơ hội tồn tại rất ngắn
	- Tính thanh khoản
	- Giới hạn short-selling