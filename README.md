<h1 align='center'>VNScript</h1>
<h3 align='center'>Ngôn ngữ lập trình của người Việt, dành cho người Việt!</h3>

<hr/>

## Sơ lược
### Mô tả
VNScript là một ngôn ngữ lập trịnh dựa trên JavaScript, được thiết kế để dễ học và sử dụng, giúp bạn có thể bắt đầu lập trình ngay lập tức mà không cần phải lo lắng về những khái niệm phức tạp!

### Cú pháp
Cú pháp của VNScript tương tự như JavaScript, nhưng có một số điểm khác biệt nhỏ để phù hợp với tiếng Việt. Ví dụ, VNScript sử dụng các từ khóa tiếng Việt, các ký tự Unicode và các dấu câu tiếng Việt.

### Ứng dụng
VNScript có thể được sử dụng để phát triển nhiều loại ứng dụng, bao gồm:
- **Ứng dụng web:** VNScript có thể được sử dụng để phát triển các ứng dụng web tương tác, chẳng hạn như trò chơi, ứng dụng quản lý và ứng dụng thương mại điện tử.
- **Ứng dụng di động:** VNScript có thể được sử dụng để phát triển các ứng dụng di động cho các nền tảng Android và iOS khi đi kèm với framework React Native.
- **Ứng dụng máy tính:** VNScript, kết hợp với React, VueJs, Astro, ... có thể được sử dụng để phát triển các ứng dụng máy tính cho các hệ điều hành Windows, macOS và Linux.

## Hướng dẫn sử dụng
VNScript hỗ trợ nhiều tính năng vô cùng đồ sộ và sau đây là cú pháp, cách sử dụng VNScript:

`Lệnh khởi tạo:` Để khởi tạo một biến, ta dùng cú pháp `đặt`. Còn để khởi tạo một loại thuật toán, ta dùng cú pháp `thuật toán`

```js
// Khởi tạo các biến a, b, c
đặt a = 5
đặt b = "Xin chào!"
đặt c = sai

// Khởi tạo thuật toán `hello` không có bất kì hàm số nào
thuật toán hello 
  Các khối lệnh của bạn dành cho thuật toán `hello` ở đây
hết

// Khởi tạo thuật toán `byebye` có các hàm số
thuật toán byebye (hàm số 1, hàm số 2,...) 
  Các khối lệnh của bạn dành cho thuật toán `hello` ở đây
hết
```

Để gọi một thuật toán, ta dùng cấu trúc `tên thuật toán + (các tham số nếu có)`
```js
đặt b = 0
thuật toán a
  b = 5
hết

a() // lúc này, b = 5
```

Trong một thuật toán, để trả về giá trị từ một thuật toán, ta dùng lệnh `trả về`

```js
thuật toán trave5
  trả về 5
hết

đặt b = trave5() // Lúc này, b sẽ bằng 5
```

`Các lệnh xuất-nhập:` Để xuất một giá trị ra màn hình, ta dùng lệnh `viết`. Để nhập một giá trị bằng bàn phím, ta dùng lệnh `nhập`

```js
đặt a = 'Chào bạn!'
viết (a) // Câu lệnh này sẽ viết `Chào bạn!` ra màn hình

đặt b = nhập()
bạn sẽ nhập giá trị b vào máy tính bằng bàn phím
```

`Khối lệnh điều kiện:` Để biểu diễn cấu trúc nếu-thì trong VNScript, ta dùng cú pháp `nếu`,`còn không`

Ta kiểm tra điều kiện bằng các dấu `==`, `!=`, `>`, `<`, `<=`, `>=`
```js
a == b  sẽ trả về đúng khi a bằng b
a != b  sẽ trả về đúng khi a không bằng b
a > b  sẽ trả về đúng khi a lớn hơn b
a < b  sẽ trả về đúng khi a nhỏ hơn b
a >= b  sẽ trả về đúng khi a lớn hơn hoặc bằng b
a <= b  sẽ trả về đúng khi a nhỏ hơn hoặc bằng b
```

Khi kiểm tra các điều kiện, ta có thể dùng cú pháp `và`, `hoặc`, `đúng`, `sai`

```js
đặt a = đúng, b = sai

viết (a == đúng và b == đúng) // sẽ in sai
viết (a == đúng hoặc b == đúng) // sẽ in đúng
```

Sau đây là một ví dụ cho việc sử dụng khối lệnh điều kiện
```js
// Khối lệnh `nếu` đơn giản
nếu dieukien1 làm
  // Các khối lệnh khác của bạn ở đây
hết

// Khối lệnh `nếu-còn không`
nếu dieukien1 làm
  // Các khối lệnh của bạn nếu dieukien1 là đúng ở đây
hết còn không làm
  // Các khối lệnh của bạn nếu dieukien1 là sai ở đây
hết

// Khối lệnh `nếu-còn không nếu-còn không`
nếu dieukien1 làm
  // Các khối lệnh của bạn nếu dieukien1 là đúng ở đây
hết còn không nếu dieukien2 làm
  // Các khối lệnh của bạn nếu dieukien1 sai, dieukien2 đúng ở đây
hết còn không làm
  // Các khối lệnh của bạn nếu dieukien1, dieukien2 là sai ở đây
hết
```

`Khối lệnh lặp:` Ta có thể dùng các cú pháp `với` hoặc `khi` để biểu diễn khối lệnh lặp

```js
// Khối lệnh này sẽ in ra các giá trị từ 0 đến 9
với i = 0; i < 10; i = i + 1 làm
  viết (i)
hết

//Khối lệnh này sẽ in ra các giá trị từ 5 đến 7
đặt a = 5
khi a != 10 làm
  viết(a)
  a = a + 1
hết
```
