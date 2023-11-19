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

`Lệnh khởi tạo:` Để khởi tạo một biến, ta dùng cú pháp `đặt`. Còn để khởi tạo một loại thuật toán, ta dùng cú pháp `thuật toán`, `hết`

```js
// Khởi tạo các biến a, b, c
đặt a = 5
đặt b = "Xin chào!"
đặt c = sai

thuật toán hello
  Các khối lệnh của bạn dành cho thuật toán `hello` ở đây
hết
```

`Các lệnh xuất-nhập:` Để xuất một giá trị ra màn hình, ta dùng lệnh `viết`. Để nhập một giá trị bằng bàn phím, ta dùng lệnh `nhập`

```js
đặt a = 'Chào bạn!'
viết (a) // Câu lệnh này sẽ viết `Chào bạn!` ra màn hình

đặt b = nhập()
bạn sẽ nhập giá trị b vào máy tính bằng bàn phím
```

`Khối lệnh điều kiện:` Để biểu diễn cấu trúc nếu-thì trong VNScript, ta dùng cú pháp `nếu`,`còn không`,`làm`,`hết`

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
