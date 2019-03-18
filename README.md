ĐỘ PHỨC TẠP THUẬT TOÁN
1)	khái niệm
-	Độ phức tạp thuật toán là lượng thời gian và bộ nhớ cần thiết
 Đánh giá thời gian cần thiết thực hiện thuật toán phụ thuộc vào kịch thước của dữ liệu và kí hiệu
T(n) là độ phức tập thuật toán.
# để tính T(n): đếm số câu lệnh phải thực hiện: các phép tính số học, so sánh , thời gian…
2)Xác định độ phức tạp của thuật toán
	a) quy tắc bỏ hằng số
	Nếu T(n)=O(c1,f(n)), c1:hằng số,c1>0  T có độ phức tạp
O(f(n)).
b) quy tắc cộng:
-giả sử thuật toán gồm 2 phần liên tiếp T1,T2. T1(n)=O(f(n)) .
T2(n)=O(g(n)).
T(n)=T1(n)+T2(n)=O(f(n)+g(n))
c) quy tắc lấy max:
T(n)=O(f(n)+g(n))T(n)=O(max(f(n),g(n)))
d) quy tắc nhân:
T(n)=O(f(n)).Nếu thực hiện K(n) lần thực hiện thuật toán T với 
K(n)=O(g(n))
 độ phức tạp tính toán O(g(n),f(n)).
3) Một số dạng hàm kí hiệu độ phức tạp thuật toán:
-Có thời gian là đa thức bậc k:
	P(n)=O(n^k)
Vd:
 Bài so sánh:
	For(int i=1;i<=n-1;i++)
		For(int j=1;j<=n;j++)
			If(a[i]>a[j])
				Swap(a[i],a[j]);

Ta đánh giá: số lần thực hiện câu lệnh so sánh:
	½*(n^2-n)
Ta lấy số bậc của đa thức
Hay độ phức tạp O(n^2).
Với độ phức tạp on^2 ta chị có thể xử lý n tới 5000.  ^.^
	##Nếu thuật toán có thời gian thực hiện:
		Loga(f(n)) thì có độ phức tạp là O(log(n))….
	Best thuật toán :  ( O(log(n)) ): 
		-Quick sort
		-Binary search
	- Nếu thuật toán có độ phức tạp là 1 hằng số, t/gian thực hiện
	không phụ thuộc vào kích thước dữ liệu vào thì độ phức tạp 
	của thuật toán đó là : O(1)…
	-Một số hàm thường dùng để ký hiệu độ phức tạp thuật toán:
	Lgn , n , nlogn, n^2, n^3
	-Một số độ phức tạp thuật toán:
		O(n) n gần bằng 25 triệu
		O(nlog(n))  n gần bằng 1 triệu
		O(n^2)n gần bằng 5000
		O(n^3) n gần bằng 300.
	4) 1 số ví dụ: 
	- tính tổng các số từ 1n
		Nhập n; O(1)
		S=0; O(1)
		For i=1n O(n)
			S=S+i;
		Xuất S; O(1)
		 độ fuck tạp O(n).
	
	Bài tập:
	1)phân tích thời gian thực hiện của chương trình sau\
	..xem bài 3.2 tài liệu chuyên tin
	// phương pháp giảm độ phức tạp: tạo mảng tính toán trước.
Ví dụ: Dãy con tổng bằng S
C1 dùng 2 for lồng nhau, hàm tính tổng ở trong cùng
 (dùng mảng tính toán trước)
TÍnh si= a1+a2+a3+..ai;  hàm tích lũy
Tổng các phần tử của dãy con trong đoạn i,j:
	T=S[j]-S[i].
