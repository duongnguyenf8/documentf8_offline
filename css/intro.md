## Tổng quan về CSS

CSS (Cascading Style Sheets) là một ngôn ngữ định dạng được sử dụng để tạo kiểu cho các trang web.

- Nó giúp điều chỉnh màu sắc, font chữ, kích thước và bố cục của các phần tử trên trang web.
- CSS hoạt động dựa trên nguyên tắc kế thừa và ưu tiên, cho phép tùy chỉnh kiểu dáng của nhiều phần tử cùng một lúc.
- CSS cũng là một ngôn ngữ đơn giản, nó bao gồm các bộ chọn (selectors) và các thuộc tính
  (properties) để xác định cách các phần tử HTML hiển thị trên trang web
- Các tệp tin CSS có phần mở rộng .css

## 2. Cách học CSS hiệu quả

Để học CSS hiệu quả, bạn có thể áp dụng các phương pháp sau:

**Tìm hiểu cú pháp**: Hãy tìm hiểu cú pháp và cách viết CSS đúng.

- Hiểu rõ cách chọn phần tử và áp dụng kiểu dáng cho chúng.

**Thực hành**: Tạo các bản mẫu trang web đơn giản và thực hành viết CSS cho chúng.

- Điều này giúp bạn áp dụng kiến thức và rèn kỹ năng.

**Đọc và tham khảo tài liệu**: Đọc các tài liệu, sách, và tài liệu hướng dẫn về CSS để hiểu rõ hơn về các khái niệm và phương pháp sử dụng.

**Làm việc với dự án thực tế**: Tham gia vào các dự án thực tế hoặc tạo ra dự án của riêng bạn để áp dụng CSS vào trang web thực tế.

- Điều này giúp bạn trải nghiệm thực tế và đối mặt với các thách thức.

**Tham gia cộng đồng**: Tham gia các diễn đàn, nhóm học tập hoặc cộng đồng trực tuyến để học từ người khác và chia sẻ kiến thức của bạn.

## 3 cách tích hợp CSS vào trang web

Có ba cách chính để tích hợp CSS vào trang web:

1. **Inline CSS**: Sử dụng thuộc tính `style` trong các phần tử HTML để thiết lập kiểu dáng cho từng phần tử.

- Ví dụ:

  ```html
  <p style="color: blue;">Đây là một đoạn văn.</p>
  ```

2. **Internal CSS**: Sử dụng thẻ `<style>` để định nghĩa CSS trong phần `<head>` của trang web.

Kiểu css chỉ áp dụng cho trang web hiện tại.

- Ví dụ:

  ```html
  <head>
  	<style>
  		p {
  			color: blue;
  		}
  	</style>
  </head>
  ```

3. **External CSS**: Sử dụng một tệp CSS riêng biệt
   - Sau đó liên kết tệp đó với trang web bằng cách sử dụng thẻ `<link>`.

- Ví dụ:

  ```html
  <head>
  	<link rel="stylesheet" href="style.css" />
  </head>
  ```

## 4. Bộ chọn CSS (CSS Selector) từ cơ bản đến nâng cao

CSS Selector là cách chọn các phần tử HTML mà bạn muốn áp dụng kiểu dáng.

Dưới đây là một số bộ chọn CSS từ cơ bản đến nâng cao:

- **Tên thẻ**: Chọn các phần tử dựa trên tên thẻ.

  Ví dụ:

  - `p` sẽ chọn tất cả các phần tử `<p>` trên trang.

- **ID**: Sử dụng thuộc tính `id` của phần tử để chọn duy nhất một phần tử trên trang.

  - Ví dụ:

    - `#header` sẽ chọn phần tử có `id="header"`.

- **Class**: Sử dụng thuộc tính `class` của phần tử để chọn một nhóm các phần tử.

  - Ví dụ:

    - `.highlight` sẽ chọn tất cả các phần tử có `class="highlight"`.

- **Bộ chọn con**: Sử dụng các bộ chọn con để chọn các phần tử con của một phần tử khác.

  - Ví dụ:

    - `ul li` sẽ chọn tất cả các phần tử `<li>` trong một danh sách không thứ tự.

- **Bộ chọn kết hợp**: Kết hợp các bộ chọn để chọn các phần tử cùng thỏa mãn nhiều điều kiện.

  - Ví dụ:

    - `ul.highlighted li` sẽ chọn tất cả các phần tử `<li>` trong một

      danh sách không thứ tự có `class="highlighted"`.

- **Bộ chọn tiếp theo**: Chọn phần tử kế tiếp của một phần tử cụ thể.

  - Ví dụ:

    - `h1 + p` sẽ chọn phần tử `<p>` đầu tiên sau một phần tử `<h1>`.

- **Bộ chọn con trực tiếp**: Chọn phần tử con trực tiếp của một phần tử cụ thể.

  - Ví dụ:

    - `ul > li` sẽ chọn tất cả các phần tử `<li>` là con trực tiếp của một danh sách không thứ tự.

- **Bộ chọn đệm**: Chọn phần tử nằm giữa hai phần tử khác.

  - Ví dụ:

    - `h1 ~ p` sẽ chọn tất cả các phần tử `<p>` nằm giữa hai phần tử `<h1>`.

- **Bộ chọn thuộc tính**: Chọn các phần tử dựa trên giá trị của thuộc tính.

  - Công thức:

    - `ten_the[ten_thuoc_tinh="gia_tri"]`

  - Ví dụ:

    - `input[type="text"]` sẽ chọn tất cả các phần tử `<input>` có thuộc tính `type="text"`.

    - `a[title]` sẽ chọn tất cả các phần tử `<a>` có thuộc tính `title`.

    - `a[href^="https"]` sẽ chọn tất cả các phần tử `<a>` có thuộc tính `href` bắt đầu bằng `https`.

    - `a[href$=".pdf"]` sẽ chọn tất cả các phần tử `<a>` có thuộc tính `href` kết thúc bằng `.pdf`.

    - `a[href*="w3schools"]` sẽ chọn tất cả các phần tử `<a>` có thuộc tính `href` chứa chuỗi `"w3schools"`.

## 5. Pseudo Elements

Pseudo Elements trong CSS cho phép bạn chọn và tạo kiểu cho các phần tử mà không phải thêm thẻ HTML.

Dưới đây là một số pseudo elements phổ biến:

- `::before`: Tạo một phần tử ảo trước phần tử được chọn và cho phép bạn tạo kiểu cho nó.

- `::after`: Tạo một phần tử ảo sau phần tử được chọn và cho phép bạn tạo kiểu cho nó.

- `::first-line`: Chọn dòng đầu tiên trong một phần tử và cho phép bạn tạo kiểu cho dòng đó.

- `::first-letter`: Chọn ký tự đầu tiên trong một phần tử và cho phép bạn tạo kiểu cho ký tự đó.

Ví dụ sử dụng `::before` để thêm một biểu tượng trước mỗi phần tử `<p>`:

```css
p::before {
	content: '⭐️';
}
```

Ví dụ sử dụng `::after` để thêm một biểu tượng sau mỗi phần tử `<p>`:

```css
p::after {
	content: '⭐️';
}
```

Ví dụ sử dụng `::first-line` để làm nổi bật dòng đầu tiên trong một phần tử `<p>`:

```css
p::first-line {
	color: red;
}
```

Ví dụ sử dụng `::first-letter` để làm nổi bật ký tự đầu tiên trong một phần tử `<p>`:

```css
p::first-letter {
	color: red;
}
```

## 6. Pseudo Classes:

Pseudo Classes trong CSS cho phép bạn chọn và tạo kiểu cho các phần tử trong các trạng thái hoặc vị trí khác nhau.

Dưới đây là một số pseudo classes phổ biến:

- `:hover`: Chọn phần tử khi con trỏ di chuột qua phần tử đó.

- `:active`: Chọn phần tử khi nó đang được nhấp chuột.

- `:focus`: Chọn phần tử khi nó đang trong trạng thái được tập trung.

- `:nth-child(n)`: Chọn phần tử con thứ n trong một phần tử cha.

Ví dụ sử dụng `:hover` để thay đổi màu nền của một phần tử khi di chuột qua:

```css
button:hover {
	background-color: yellow;
}
```

Ví dụ sử dụng `:active` để thay đổi màu nền của một phần tử khi nó được nhấp chuột:

```css
button:active {
	background-color: yellow;
}
```

Ví dụ sử dụng `:focus` để thay đổi màu nền của một phần tử khi nó được tập trung:

```css
input:focus {
	background-color: yellow;
}
```

Ví dụ sử dụng `:nth-child(n)` để thay đổi màu nền của phần tử con thứ 2 trong một phần tử cha:

```css
ul li:nth-child(2) {
	background-color: yellow;
}
```

## 7. Các đơn vị thường dùng trong CSS

Khi sử dụng CSS để định dạng các giá trị, bạn có thể sử dụng các đơn vị sau:

- **px (pixel)**: Đơn vị đo độ dài tuyệt đối, dựa trên pixel.

- **% (percent)**: Đơn vị đo độ phần trăm của một giá trị so với giá trị gốc.

- **em**: Đơn vị đo độ phần trăm của font-size của phần tử cha.

- **rem**: Đơn vị đo độ phần trăm của font-size của phần tử gốc (thường là phần tử `<html>`).

- **vh (viewport height)**: Đơn vị đo độ phần trăm của chiều cao viewport.

- **vw (viewport width)**: Đơn vị đo độ phần trăm của chiều rộng viewport.

- **pt (point)**: Đơn vị đo độ dài dựa trên điểm ấn in.

- **cm (centimeter)**: Đơn vị đo độ dài dựa trên centimes.

- **mm (millimeter)**: Đơn vị đo độ dài dựa trên millimes.

- **in (inch)**: Đơn vị đo độ dài dựa trên inch.

Ví dụ sử dụng các đơn vị trong CSS:

```css
.example {
	width: 100vw;
	height: 100vh;
	margin: 1cm;
	margin-bottom: 2em;
	font-size: 16px;
	padding: 1rem;
	padding-left: 1mm;
	border: 1pt solid black;
	max-width: 2in;
}
```
