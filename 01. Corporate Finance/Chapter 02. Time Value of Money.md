# 1.  Giá trị thời gian của tiền
- Giá trị của lượng *tiền hôm nay* có giá trị > giá trị của *lượng tiền tương tự* trong *tương lai* do khả năng sinh lời tiềm năng của nó
- Nguyên nhân ... > ... :
	- ***Chi phí cơ hội của việc sử dụng tiền:*** số tiền nhàn rỗi để trong két sắt sẽ khiến các nhà đầu tư mất đi một khoản sinh lời trong tương lai qua việc đầu tư
	- ***Lạm phát:*** sức mua của tiền sẽ giảm trong tương lai nếu lạm phát tăng
	- ***Rủi ro:*** các nhà đầu tư có thể thất bại và mất trắng khoản tiền
### 1.1. Future Value of Money (FV)
##### 1.1.1 Giá trị tương lai của 1 khoản tiền
- Trong n năm, gửi tiền chỉ 1 lần vào đầu/cuối năm thứ 1, và rút tiền đầu/cuối năm thứ n
$$FV_n = PV\cdot (1 + i)^n = PV\cdot FVF(i,n)$$
##### 1.1.2 Giá trị tương lai của dòng tiền đều
###### Dòng tiền đều ở cuối kỳ **(ordinary annuity)**
- Trong n năm, *gửi tiền vào cuối mỗi năm* với cùng 1 lượng tiền, và *rút tiền cuối năm thứ n*
$$
\begin{align}
FVA_n &= CF + CF\cdot(1+i) + CF\cdot(1+i)^2 +\ ...\ + CF\cdot(1+i)^{n-1}\\
&= CF\cdot ( 1 + (1+i) + (1+i)^2 + ... + (1+i)^{n-1}) \\
&= CF\cdot FVFA_{(i,n)} \\\\ 
FVA_n &= CF\cdot \sum_{t=1}^n (1+i)^{n-t} \\\\
FVA_n &= CF\cdot \frac{(1+i)^n - 1}{i} 
\end{align}
$$
---
###### Dòng tiền đều ở đầu kỳ **(annuity due)**
- Trong n năm, *gửi tiền vào đầu mỗi năm* với cùng 1 lượng tiền, và *rút tiền cuối năm thứ n*
$$
\begin{align}
FVA_n &= CF\cdot(1+i) + CF\cdot(1+i)^2 + \ ... \ + CF\cdot(1+i)^n\\
&= CF\cdot ((1+i) + (1+i)^2 + \ ... \ + (1+i)^n)\\
&= CF\cdot ( 1 + (1+i) + (1+i)^2 + ... + (1+i)^{n-1}) \cdot (1+i)\\
&= CF\cdot FVFA_{(i,n)} \cdot (1+i) \\\\ 
FVA_n &= CF\cdot \sum_{t=1}^n (1+i)^n\\\\
FVA_n &= CF\cdot \frac{(1+i)^n - 1}{i} \cdot (1+i)
\end{align} 
$$
##### 1.1.3 Giá trị tương lai của dòng tiền biến thiên
- Trong n năm, gửi tiền vào đầu/cuối mỗi năm với lượng tiền khác nhau mỗi năm (CF thay đổi), và rút tiền cuối năm thứ n
$$
\begin{align}
Đầu \ kì: \ FV_n &= (CF_t \cdot \sum_{t=1}^n (1+i)^{n-t}) \cdot (1+i) \\\\
Cuối \ kì: \ FV_n &= CF_t \cdot \sum_{t=1}^n (1+i)^{n-t}
\end{align} 
$$
### 1.2. Present Value of Money (PV)
##### 1.2.1 Giá trị hiện tại của 1 khoản tiền
$$PV = FV_n \cdot \frac{1}{(1 + i)^n} = FV_n \cdot PVF(i,n)$$
##### 1.2.2 Giá trị hiện tại của dòng tiền đều
###### Dòng tiền đều cuối kì
- Khi đã dự tính lượng tiền mỗi ***cuối*** kì, thì cần tính giá trị hiện tại cho dòng tiền để khi gửi NH/đầu tư ***đầu*** kì để sau này phân bổ = tổng các lượng tiền dự tính mỗi ***cuối*** kì đó.
- $$
\begin{align}
PVA_n &= CF \cdot (\frac{1}{1+i} + (\frac{1}{1+i})^2 +  \ ... \ + (\frac{1}{1+i})^{n-1} + (\frac{1}{1+i})^n)\\
&= CF \cdot PVFA_{(i,n)}\\\\
PVA_n &= CF \cdot \sum_{t=1}^n (\frac{1}{1+i})^t \\\\
PVA_n &= CF \cdot \frac{1-(\frac{1}{1+i})^n}{i}
\end{align}
$$
---
###### Dòng tiền đều đầu kì
- Khi đã dự tính lượng tiền mỗi ***đầu*** kì, thì cần tính giá trị hiện tại cho dòng tiền để khi gửi NH/đầu tư ***đầu*** kì để sau này phân bổ = tổng các lượng tiền dự tính mỗi ***đầu*** kì đó.
- $$
\begin{align}
PVA_n &= CF \cdot (1 + \frac{1}{1+i} + (\frac{1}{1+i})^2 +  \ ... \ + (\frac{1}{1+i})^{n-2} + (\frac{1}{1+i})^{n-1})\\
&= CF \cdot (\frac{1}{1+i} + (\frac{1}{1+i})^2 +  \ ... \ + (\frac{1}{1+i})^{n-1} + (\frac{1}{1+i})^n) \cdot (1+i)\\
&= CF \cdot PVFA_{(i,n)} \cdot (1+i)\\\\
PVA_n &= CF \cdot \sum_{t=1}^n (\frac{1}{1+i})^{n-t}\\\\
PVA_n &= CF \cdot \frac{1-(\frac{1}{1+i})^n}{i} \cdot (1+i)
\end{align}
$$
---
###### Dòng tiền đều vô hạn **(perpetuity)**
- Khi `n --> +∞`   thì  `(1/(1+i))^n --> 0`
$$
\begin{align}
Cuối \ kì: \ PVA_n &= CF \cdot \frac{1-(\frac{1}{1+i})^n}{i} = CF \cdot \frac{1}{i} \\\\
Đầu \ kì: \ PVA_n &= CF \cdot \frac{1-(\frac{1}{1+i})^n}{i} \cdot (1+i) = CF \cdot \frac{1}{i} \cdot (1+i)
\end{align}
$$
### 1.3. Interest
- Khi đi mua dưới hình thức trả góp theo kì ***(giá trị = FV)*** để mua hàng ***(giá trị = PV)*** và người bán không cho lãi suất thì cần tính để so sánh với lãi suất thị trường xem có nên vay hay không
1. **Lãi suất theo năm**
2. **Lãi suất < 1 năm**
	- Công thức FV cho 1 khoản tiền sau n năm khi tính lãi theo kì < 1 năm :
		- `i_eff (effective interest/năm): dùng khi NH tính lãi theo kì < 1 năm`
		- `i (nominal interest/năm) : dùng khi NH chỉ tính lãi theo năm`
		- `m (số kỳ tính lãi/năm)`
		- `n (số năm)`
			- `Nửa năm: m = 2 (tính lãi 2 lần/năm)`
			- `Hàng quý: m = 4`
			- `Hàng tháng: m = 12`
			- `Hàng ngày: m = 365`
			$$
			\begin{align}
			FV_n &= PV \cdot (1 + \frac{i}{m})^{m \cdot n}\\
			&= PV \cdot (1+((1 + \frac{i}{m})^{m} - 1))^n\\
			&= PV \cdot (1+i_{eff})^n\\\\
			=>\ i_{eff} &= (1+\frac{i}{m})^m -1\\
			\end{align}
			$$
# 2. Tỷ suất sinh lời & Rủi ro
### 2.1 Tỷ suất sinh lời
$$Tỷ\ suất\ sinh\ lời = \frac{Thu\ nhập\ về\ tài\ sản + Thay\ đổi\ về\ giá\ tài\ sản}{Giá\ tài\ sản\ đầu\ kỳ}$$
$$Tỷ\ suất\ sinh\ lời\ kì\ vọng = \sum_{i=1}^n\ Tỷ\ suất\ sinh\ lời\ i \cdot Xác\ suất\ xảy\ ra\ i$$
### 2.2 Rủi ro
- Mức độ rủi ro của một khoản đầu tư được đo lường bởi *mức độ biến động* của các khả năng sinh lời trong điều kiện kinh tế khác nhau so với mức sinh lời kỳ vọng
$$
\begin{align}
Phương\ sai &= \sum_{i=1}^n\ Xác\ suất\ xảy\ ra\ i \cdot (Tỷ\ suất\ sinh\ lời\ i - Tỷ\ suất\ sinh\ lời\ kì\ vọng)^2\\\\
Độ\ lệch\ chuẩn &= \sqrt{Phương\ sai}
\end{align}
$$
