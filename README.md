<h1 align='center'>VNScript</h1>
<h3 align='center'>Ngôn ngữ lập trình của người Việt, dành cho người Việt!</h3>

<hr/>

## Biến, hằng và lệnh gán

Biến và hằng trong VNScript được tạo ra khi thực hiện lệnh gán. Cú pháp của lệnh gán như sau: 

```
<biến> = <giá trị>
<hằng> = <giá trị>
```

Khi thực hiện lệnh gán, `<giá trị>` bên phải sẽ được gán vào `<biến>` hoặc `<hằng>` ở bên trái. Biến trong VNScript không cần khai báo trước kiểu dữ liệu cho biến, hằng.

```
x = 5
y = đúng
z = "Xin chào"
t = [12, sai, "Tạm biệt"]
```

Trong ví dụ ở trên, `x`, `y`, `z`, `t` là các biến và trong đó: 

- x có kiểu dữ liệu số
- y có kiểu dữ liệu logic
- z có kiểu dữ liệu xâu
- t có kiểu dũ liệu mảng

Trài ngược với biến, có thể thay đổi giá trị trong quá trình thực hiện chương trình thì hằng là giá trị bất biến từ đầu đến cuối chương trình.

```
    hằng a = 5
    a = 6
```

\hfil

Chương trình trên sẽ gặp lỗi vì a là một hằng và giá trị a đã được khởi tạo bằng 5 nên không thể chuyển thành 6 và chương trình sẽ báo lỗi.

\subsection{Các phép toán trên một số kiểu dữ liệu cơ bản}

Một số phép toán cơ bản với kiểu kí tự số và kiểu kí tự xâu:
\begin{itemize}
    \item Kiểu dữ liệu số: +, -, *, /, \% (chia lấy dư), ** (nâng lên lũy thừa)
    \item Kiểu dữ liệu xâu: + (nối xâu)
\end{itemize}

Ví dụ:

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
    a = 2**3 \quad\quad\quad\quad\quad\quad \\
    b = 5\%2 \quad\quad\quad\quad\quad\quad \\
    c = "Xin" + "Chào" \\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

Lúc này, giá trị của a là 8, của b là 1 và c là "XinChào".

\subsection{Các lệnh vào ra đơn giản}

$\>\>\>\>\>$ Trong VNScript, lệnh viết() có chức năng xuất dữ liệu ra màn hình. Lệnh viết() cho phép in một hoặc nhiều giá trị ra màn hình. Cú pháp của lệnh viết() như sau (với v1, v2,\ldots, vn là các giá trị cần đưa ra màn hình):

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 viết(v1, v2, v3,..., vn) \\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

Ví dụ sử dụng lệnh viết() để xuất ra màn hình dòng chữ "Xin chào":

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 viết("Xin chào") \\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

Để nhập dữ liệu vào chương trình bằng bàn phím, ta có thể dùng lệnh nhập(). Lệnh nhập sẽ trả về giá trị người dùng đã nhập dưới dạng số, logic, dữ liệu mảng hoặc dữ liệu kí tự. Cấu trúc chung của lệnh nhập() như sau:

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 <biến hoặc hằng> = nhập(<Văn bản hiển thị trong hộp thoại>) \\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

Ví dụ:

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 a = nhập("Hãy nhập giá trị a:") \\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

Khi đó, chưởng trình sẽ hiện lên một cửa sổ với dòng chữ "Hãy nhập giá trị a:" kèm theo một ô để nhập giá trị.

\subsection{Cấu trúc rẽ nhánh}

$\>\>\>\>\>$ Trong VNScript, biểu thức logic là biểu thức chỉ nhận giá trị đúng (true) hoặc sai (false).

\hfil

Các phép so sáng giá trị số trong VNScript:

\begin{equation*}
\begin{tabular}{ |c|c|c|c|c|c| } 
 \hline
 < & nhỏ hơn & > & lớn hơn & == & bằng nhau \\
 \hline
 <= & nhỏ hơn hoặc bằng & >= & lớn hơn hoặc bằng & != & khác nhau\\
 \hline
\end{tabular}
\end{equation*}

\hfil

Các phép toán của kiểu dữ liệu logic bao gồm phép `và', `hoặc' và `không'. Bảng các phép toán logic như sau: 

\hfil

\begin{minipage}{0.3\textwidth}
\begin{tabular}{|c|c|c|}
\hline
\multicolumn{3}{|c|}{Phép toán và} \\ \hline
X & Y & X và Y \\ \hline
đúng & đúng & đúng \\ \hline
đúng & sai & sai \\ \hline
sai & đúng & sai \\ \hline
sai & sai & sai \\ \hline
\end{tabular}
\end{minipage}
\hfill
\begin{minipage}{0.3\textwidth}
\begin{tabular}{|c|c|c|}
\hline
\multicolumn{3}{|c|}{Phép toán hoặc} \\ \hline
X & Y & X và Y \\ \hline
đúng & đúng & đúng \\ \hline
đúng & sai & đúng \\ \hline
sai & đúng & đúng \\ \hline
sai & sai & sai \\ \hline
\end{tabular}
\end{minipage}
\hfill
\begin{minipage}{0.3\textwidth}
\begin{tabular}{|c|c|c|}
\hline
\multicolumn{2}{|c|}{Phép toán không} \\ \hline
X & không phải X \\ \hline
đúng & sai \\ \hline
sai & đúng \\ \hline
\end{tabular}
\\ \\ \\
\end{minipage}

\hfil

Ví dụ:

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 x = 10; y = 5; z = 9 \quad\quad \\
 a = x < 11 và z > 5 \quad\quad \\
 b = x > 15 hoặc y < 9 \\
 c = không phải a \quad\quad\quad \\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

Ta có x = 10, z = 9 do đó x < 11 là đúng, z > 5 là đúng. Theo bảng toán `và' thì a = x < 11 và z > 5 nhận giá trị đúng.

Ta lại có x > 15 sai ( vì x = 10) nhưng y < 9 đúng (vì y = 5). Theo bảng toán `hoặc' suy ra b = x > 15 hoặc y < 9 nhận giá trị đúng.

Vì b đúng nên c = không phải b sẽ nhận giá trị sai.

\hfil

Để xử lí các tình huống rẽ nhánh, VNScript cũng có câu lệnh để mô tả cấu trúc rẽ nhánh:

\hfil

\textit{Câu lệnh rẽ nhánh dạng thiếu:}

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 nếu <điều kiện> làm \\
    <khối lệnh> \quad\quad\quad \\
 hết \quad\quad\quad\quad\quad\quad\quad\quad\quad \\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

VNScript sẽ kiểm tra <điều kiện> nếu đúng thì thực hiện <khối lệnh>, ngược lại thì bỏ qua chuyển sang lệnh tiếp theo sau lệnh nếu.

\hfil

\textit{Câu lệnh rẽ nhánh dạng đủ:}

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 nếu <điều kiện> làm \\
    <khối lệnh 1> \quad\quad \\
 còn không làm \quad\quad\quad\quad \\
    <khối lệnh 2> \quad\quad \\
 hết \quad\quad\quad\quad\quad\quad\quad\quad\quad \\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

Nếu <điều kiện> đúng thì VNScript sẽ thực hiện <khối lệnh 1>, ngược lại thì thực hiện <khối lệnh 2>.

\hfil

Ví dụ:

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 a = nhập() \quad\quad\quad\quad\quad\quad\quad\quad \\
 b = nhập() \quad\quad\quad\quad\quad\quad\quad\quad \\
 \\
 nếu a == 5 làm \quad\quad\quad\quad\quad\quad \\
    viết("a bằng 5") \quad\quad\quad\quad \\
 hết \quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad \\
 \\
 nếu a > b làm \quad\quad\quad\quad\quad\quad\quad \\
    viết("a lớn hơn b") \quad\quad\quad \\
 còn không làm \quad\quad\quad\quad\quad\quad\quad \\
    viết("a không lớn hơn b") \\
 hết \quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad \\
 \\
 \hline
\end{tabular}
\end{equation*}

Ở ví dụ trên, người dùng sẽ nhập vào hai giá trị a, b bằng bàn phím. Nếu a bằng 5 thì sẽ xuất ra màn hình dòng chữ "a bằng 5". Tiếp theo, chương trình sẽ so sánh a với b. Nếu a lớn hơn b thì xuất ra màn hình "a lớn hơn b" còn không thì xuất ra "a không lớn hơn b".

\subsection{Câu lệnh lặp với}

$\>\>\>\>\>$ Cú pháp của lệnh lặp với số lần biết trước trong VNScript như sau:

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 với <biểu thức 1> ; <biểu thức 2> ; <biểu thức 3> làm\\
    <khối lệnh> \quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad \\
 hết \quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad \\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

Trong đó: 

\begin{itemize}
\item <biểu thức 1> sẽ được thực hiện một lần trước khi thực thi khối lệnh lặp với
\item <biểu thức 2> sẽ được thực hiện mỗi tại lần lặp để xác định còn tiếp tục khối lệnh được hay không
\item <biểu thức 3> sẽ được thực hiện sau mỗi lần lặp
\end{itemize}

Ví dụ:

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 với i = 0 ; i < 5 ; i = i + 1 làm\\
    viết (i) \quad\quad\quad\quad\quad\quad\quad\quad\quad \\
 hết \quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad \\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

Ở ví dụ trên, chương trình sẽ viết ra màn hình các số từ 1 đến 4.

\subsection{Câu lệnh lặp khi}

$\>\>\>\>\>$ Câu lệnh lặp khi sẽ thực hiện khối lệnh với số lần lặp không biết trước. Khối lệnh lặp này sẽ được thực thi cho đến khi <điều kiện> = sai. 

\hfil

Cú pháp của câu lệnh lặp khi như sau:

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 khi <điều kiện> làm\\
    <khối lệnh> \quad\quad\quad \\
 hết \quad\quad\quad\quad\quad\quad\quad\quad\quad \\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

Ví dụ:

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 a = 0 \quad\quad\quad\quad\quad \\
 khi a > -15 làm\\
    viết(a) \quad \\
    a = a - 1 \\
 hết \quad\quad\quad\quad\quad\quad \\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

Khối lệnh trên sẽ xuất ra màn hình các giá trị a từ 0 trở về -15.

\subsection{Kiểu liệu danh sách}

$\>\>\>\>\>$ Kiểu dữ liệu danh sách trong VNScript được khởi tạo như sau (trong đó v1, v2,\ldots,vn là các giá trị của danh sách):

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 <tên danh sách> = [v1, v2,\ldots,vn] \\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

Để duyệt qua các phần tử của kiểu dữ liệu danh sách, ta có cú pháp: 

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 <tên danh sách> [ <vị trí của hạng tử trong dãy> ] \\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

\textbf{Chú ý:} Vị trí của kiểu dữ liệu dãy sẽ bắt đầu từ vị trí 0.

\hfil

Ví dụ:

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 danhsach = [1,2,5,4,3] \quad\quad\quad\quad \\
 viết(danhsach[0], danhsach[2])\\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

Trong ví dụ trên, chương trình sẽ xuất ra màn hình phần tử ở vị trí 0 và thứ 2 của dãy là 1 và 5.

\hfil

Một số lệnh làm việc với danh sách:
\begin{itemize}
    \item dài(<danh sách>) dùng để tính độ dài của <danh sách>
    \item <danh sách>.thêm(<giá trị>) dùng để thêm <giá trị> vào cuối <danh sách>
    \item <danh sách>.bỏ() dùng xóa giá trị cuối cùng của <danh sách>
\end{itemize}

\subsection{Hàm trong VNScript}

$\>\>\>\>\>$ Ngoài các hàm được thiết kế sẵn, VNScript còn cho phép người dùng tự thiết lập các hàm tự định nghĩa (các hàm của riêng mình).

\hfil

\textit{Cách viết hàm có trả lại giá trị:}

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 thuật toán <tên hàm> () \quad\quad\quad\quad \\
 <khối lệnh> \quad\quad \\
 trả về <giá trị> \\
 hết \quad\quad\quad\quad\quad\quad\quad\quad\quad\quad \\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

\textit{Cách viết hàm không trả lại giá trị:}

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 thuật toán <tên hàm> () \quad\quad\quad\quad \\
 <khối lệnh> \quad\quad \\
 hết \quad\quad\quad\quad\quad\quad\quad\quad\quad\quad \\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

Để gọi cách hàm tự định nghĩa, ta dùng cú pháp như sau:

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 <tên hàm>()\\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

Hoặc nếu hàm có các tham số: 

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 <tên hàm>(<tham số 1>, <tham số 2>,\ldots,<tham số n>)\\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

Ví dụ:

\begin{equation*}
\begin{tabular}{ |c| } 
 \hline
 \\
 hàm inten(ten) \quad\quad\quad\quad\quad\quad\quad\quad \\
 viết ("Xin chào" + ten) \quad\quad \\
 hết \quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad \\
 \\
 \hline
\end{tabular}
\end{equation*}

\hfil

Trong ví dụ trên, hàm inten() sẽ yêu cầu người dùng nhập tên và viết "Xin chào" kèm theo tên đã nhập.
