## 1. Các thuộc tính định dạng văn bản

CSS cung cấp nhiều thuộc tính để định dạng văn bản trong các phần tử HTML.

Dưới đây là một số thuộc tính phổ biến:

- `color`: Định nghĩa màu sắc của văn bản.

- `font-family`: Thiết lập kiểu font chữ.

- `font-size`: Định nghĩa kích thước font chữ.

- `font-style`: Thiết lập kiểu font chữ (ví dụ: italic, oblique).

- `font-weight`: Xác định độ đậm của font chữ.

- `text-align`: Căn chỉnh văn bản theo chiều ngang.

- `text-decoration`: Thiết lập gạch chân, gạch ngang hoặc gạch chân trên văn bản.

- `text-transform`: Chuyển đổi kiểu chữ (ví dụ: uppercase, lowercase, capitalize).

- `text-indent`: Xác định khoảng cách thụt đầu dòng đầu tiên của một đoạn văn bản.

- `line-height`: Định nghĩa khoảng cách dòng giữa các dòng văn bản.

- `letter-spacing`: Xác định khoảng cách giữa các ký tự trong một đoạn văn bản.

- `word-spacing`: Định nghĩa khoảng cách giữa các từ trong một đoạn văn bản.

- `white-space`: Xác định cách xử lý khoảng trắng trong một đoạn văn bản.

- `vertical-align`: Căn chỉnh văn bản theo chiều dọc.

- `text-shadow`: Tạo bóng cho văn bản.

- `background-color`: Thiết lập màu nền.

Ví dụ sử dụng các thuộc tính định dạng văn bản:

```css
p {
  color: red;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 16px;
  font-style: italic;
  font-weight: bold;
  text-align: center;
  text-decoration: underline;
  text-transform: uppercase;
  text-indent: 20px;
  line-height: 1.5;
  letter-spacing: 2px;
  word-spacing: 5px;
  white-space: nowrap;
  vertical-align: middle;
  text-shadow: 2px 2px 5px #ccc;
  background-color: #f2f2f2;
}
```

## 2. Thuộc tính background

Thuộc tính `background` trong CSS cho phép bạn định nghĩa hình nền cho một phần tử HTML.

Dưới đây là một số thuộc tính phổ biến:

- `background-color`: Thiết lập màu nền.

- `background-image`: Định nghĩa hình ảnh nền.

- `background-repeat`: Xác định cách lặp lại hình ảnh nền.

- `background-position`: Thiết lập vị trí ban đầu của hình ảnh nền.

# Giảng về thuộc tính `transform` và ứng dụng trong thực tế

## Thuộc tính `transform`

- Định nghĩa: Thuộc tính `transform` trong CSS cho phép bạn biến đổi, xoay, co giãn hoặc biến đổi hình dạng các phần tử HTML.
- Cú pháp: `transform: <transform-function>`
- Các giá trị của `<transform-function>`:
  - `translate()`: Dịch chuyển phần tử theo trục X và trục Y.
  - `scale()`: Thay đổi tỷ lệ kích thước của phần tử.
  - `rotate()`: Xoay phần tử theo góc quay.
  - `skew()`: Nghiêng phần tử theo trục X và trục Y.
  - `matrix()`: Kết hợp các phép biến đổi tùy chỉnh.

## Ứng dụng trong thực tế

Thuộc tính `transform` có rất nhiều ứng dụng trong phát triển web, từ tạo hiệu ứng chuyển động cho phần tử, xoay ảnh, tạo hiệu ứng hover cho các nút, đến tạo các slider 3D và biến đổi hình dạng phức tạp. Dưới đây là một ví dụ về cách sử dụng thuộc tính `transform` trong thực tế:

````html
<!DOCTYPE html>
<html>
  <head>
    <style>
      .card {
        width: 200px;
        height: 200px;
        background-color: #f0f0f0;
        transition: transform 0.3s;
      }

      .card:hover {
        transform: rotate(15deg);
      }
    </style>
  </head>
  <body>
    <div class="card">
      <!-- Nội dung thẻ -->
    </div>
  </body>
</html>

Ví dụ sử dụng thuộc tính background: ```css div { background-color: #f2f2f2;
background-image: url("background.jpg"); background-repeat: no-repeat;
background-position: center top; }
````

## 3. Thuộc tính border

Thuộc tính `border` trong CSS được sử dụng để định nghĩa đường viền cho một phần tử HTML.

Dưới đây là một số thuộc tính phổ biến:

- `border-width`: Định nghĩa độ dày của đường viền.

- `border-style`: Thiết lập kiểu đường viền (ví dụ: solid, dotted, dashed).

- `border-color`: Xác định màu sắc của đường viền.

- `border-radius`: Định nghĩa độ cong của góc đường viền.

Ví dụ sử dụng thuộc tính border:

```css
button {
  border-width: 1px;
  border-style: solid;
  border-color: #ccc;
  border-radius: 4px;
}
```

## 4. Thuộc tính kích thước

CSS cung cấp các thuộc tính để định nghĩa kích thước của các phần tử HTML. Dưới đây là một số thuộc tính phổ biến:

- `width`: Thiết lập chiều rộng của phần tử.

- `height`: Định nghĩa chiều cao của phần tử.

- `max-width`: Xác định chiều rộng tối đa của phần tử.

- `max-height`: Thiết lập chiều cao tối đa của phần tử.

- `min-width`: Xác định chiều rộng tối thiểu của phần tử.

- `min-height`: Thiết lập chiều cao tối thiểu của phần tử.

Ví dụ sử dụng thuộc tính kích thước:

```css
img {
  width: 100%;
  height: auto;
  max-width: 500px;
  max-height: 500px;
  min-width: 200px;
  min-height: 200px;
}
```

## 5. Thuộc tính căn chỉnh văn bản

CSS cho phép bạn căn chỉnh văn bản trong các phần tử HTML.

Dưới đây là một số thuộc tính căn chỉnh văn bản:

- `text-align`: Căn chỉnh văn bản theo chiều ngang (left, right, center, justify).

- `line-height`: Định nghĩa khoảng cách dòng giữa các dòng văn bản.

- `text-indent`: Xác định khoảng cách thụt đầu dòng đầu tiên của một đoạn văn bản.

Ví dụ sử dụng thuộc tính căn chỉnh văn bản:

```css
p {
  text-align: center;
  line-height: 1.5;
  text-indent: 20px;
}
```

## 6. Thuộc tính opacity, filter

Thuộc tính `opacity` trong CSS cho phép điều chỉnh độ mờ của một phần tử.

Giá trị của `opacity` nằm trong khoảng từ 0 đến 1, với 0 là hoàn toàn trong suốt và 1 là không mờ.

Thuộc tính `filter` cho phép bạn áp dụng các hiệu ứng hình ảnh, như làm mờ, đổ bóng, đổi màu, vv.

Ví dụ sử dụng thuộc tính opacity và filter:

```css
div {
  opacity: 0.5;
  filter: blur(5px);
  filter: brightness(50%);
  filter: contrast(200%);
  filter: drop-shadow(16px 16px 20px blue);
  filter: grayscale(50%);
  filter: hue-rotate(90deg);
  filter: invert(75%);
  filter: opacity(25%);
  filter: saturate(30%);
  filter: sepia(60%);
}
```

## 6.5 Thuộc tính `overflow` và ứng dụng

Thuộc tính overflow trong CSS được sử dụng để xác định cách xử lý nội dung bị tràn ra khỏi phần tử chứa.

Dưới đây là mô tả về thuộc tính overflow và các giá trị tương ứng:

- `overflow: visible;`: Giá trị mặc định. Cho phép nội dung tràn ra khỏi phần tử chứa nếu nó vượt quá kích thước của phần tử.

- `overflow: hidden;`: Ẩn nội dung tràn ra khỏi phần tử chứa và không hiển thị nội dung bị trên lên.

- `overflow: scroll;`: Hiển thị thanh cuộn ngang và dọc cho phần tử chứa, ngay cả khi nội dung không tràn ra.

- `overflow: auto;`: Tự động hiển thị thanh cuộn chỉ khi nội dung tràn ra khỏi phần tử chứa.

Ví dụ sử dụng thuộc tính opacity và filter:

```css
div {
  width: 200px;
  height: 100px;
  overflow: hidden;
  overflow: scroll;
  overflow: visible;
  overflow: auto;
}
```

Ứng dụng của thuộc tính overflow:

- Tạo khung trượt (slider) cho nội dung tràn ra khỏi kích thước hiển thị ban đầu.

- Tạo menu dọc cuộn (vertical scroll menu) cho danh sách dài.

- Tạo hiệu ứng tràn ngập (overflow effect) bằng cách làm tràn nội dung từ phần tử cha sang phần tử con.

## 7. Thuộc tính padding, margin

Thuộc tính `padding` trong CSS được sử dụng để tạo khoảng cách giữa nội dung và đường viền của một phần tử.

Thuộc tính `margin` được sử dụng để tạo khoảng cách giữa các phần tử.

Cả hai thuộc tính này có thể có giá trị dương hoặc âm.

Ví dụ sử dụng thuộc tính padding và margin:

```css
div {
  padding: 10px;
  margin: 20px;
  padding: -10px;
  margin: -20px;
}
```

## 8. Box Model CSS

Box Model trong CSS mô tả cách mà các phần tử HTML được hiển thị và tương tác với nhau.

Box Model bao gồm các thành phần sau:

- `Content`: Nội dung của phần tử, chẳng hạn như văn bản hoặc hình ảnh.

- `Padding`: Khoảng cách giữa nội dung và đường viền.

- `Border`: Đường viền bao quanh phần tử.

- `Margin`: Khoảng cách giữa các phần tử.

CSS Box Model có thể được điều chỉnh bằng cách sử dụng các thuộc tính padding, border và margin.

Ví dụ sử dụng Box Model:

```css
div {
  content: "This is a box";
  margin: 20px;
  padding: 10px;
  border: 5px solid #ccc;
}
```

## 9. Chồng chéo CSS và thứ tự ưu tiên

Khi áp dụng nhiều quy tắc CSS cho cùng một phần tử, thứ tự và ưu tiên của các quy tắc đó được quyết định bằng cách sử dụng cơ chế "chồng chéo".

Các quy tắc CSS được áp dụng theo thứ tự sau:

- Quy tắc CSS nằm trong file external CSS có ưu tiên thấp nhất.

- Quy tắc CSS nằm trong thẻ `<style>` có ưu tiên thấp hơn so với các quy tắc CSS nằm trong phần tử HTML.

- Quy tắc CSS nằm trong inline CSS có ưu tiên cao nhất.

Ngoài ra, các quy tắc CSS còn có thể có mức độ ưu tiên cao hơn thông qua sử dụng các selector cụ thể như ID selector hoặc class selector.

Ví dụ về chồng chéo CSS:

```css
/* Quy tắc CSS nằm trong file external CSS */
p {
  color: blue;
}
```

```html
<style>
  /* Quy tắc CSS nằm trong thẻ <style> */
  p {
    color: red;
  }
</style>
<!-- Quy tắc CSS nằm trong inline CSS -->
<p style="color: green;">Đây là một đoạn văn.</p>
```

## 10. Reset CSS? Tại sao phải Reset CSS

Reset CSS là một kỹ thuật trong việc làm sạch và chuẩn hóa các giá trị mặc định của các thuộc tính trong CSS.

Lý do chúng ta cần Reset CSS là vì các trình duyệt web có các giá trị mặc định khác nhau cho các thuộc tính của các phần tử HTML. Điều này có thể dẫn đến sự không nhất quán giữa các trình duyệt và giao diện của trang web.

Bằng cách áp dụng Reset CSS, chúng ta có thể đảm bảo rằng các phần tử HTML sẽ có cùng một giá trị mặc định trên tất cả các trình duyệt, và từ đó xây dựng giao diện của trang web một cách nhất quán.

Có nhiều cách để áp dụng Reset CSS, một số phổ biến là sử dụng các file CSS đã được chuẩn hóa sẵn như Normalize.css hoặc viết các quy tắc Reset CSS tự định nghĩa.

Ví dụ về Reset CSS:

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
```

# 11. Thuộc tính float và clear

## Thuộc tính float:

Định nghĩa: Thuộc tính `float` được sử dụng để định vị phần tử theo hướng di chuyển trong layout.

Cách sử dụng: Đặt giá trị `float` là `left` hoặc `right` cho phần tử cần định vị.

Ví dụ:

<htmlcss-snippet>

```html
<style>
  .box {
    float: left;
    width: 200px;
    height: 200px;
    background-color: red;
  }
</style>

<div class="box"></div>
<p>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque sit amet
  felis sed risus tincidunt posuere.
</p>
```

</htmlcss-snippet>

Trong ví dụ trên, phần tử có class "box" sẽ được định vị bên trái và văn bản trong thẻ `<p>` sẽ luồn qua phần tử "box".

---

## Thuộc tính clear:

Định nghĩa: Thuộc tính `clear` được sử dụng để xác định xem phần tử có được phép di chuyển qua các phần tử đang float không.

Cách sử dụng: Đặt giá trị `clear` là `left`, `right`, `both`, hoặc `none` cho phần tử cần xác định.

Ví dụ:

<htmlcss-snippet>

```html
<style>
  .box {
    float: left;
    width: 200px;
    height: 200px;
    background-color: red;
  }

  .clear-box {
    clear: both;
  }
</style>

<div class="box"></div>
<div class="clear-box"></div>
<p>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque sit amet
  felis sed risus tincidunt posuere.
</p>
```

</htmlcss-snippet>

Trong ví dụ trên, phần tử có class "clear-box" sẽ được xác định không được phép di chuyển qua phần tử "box", văn bản trong thẻ `<p>` sẽ hiển thị bên dưới các phần tử đang float.

## Ví dụ:

Sử dụng float để làm chữ bao quanh ảnh

<htmlcss-snippet>

```html
<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  .float {
    float: left;
    margin: 10px;
    border-radius: 50%;
    shape-outside: ellipse(50% 50% at 50% 50%);
  }
  .shape_out_side {
    width: 500px;
    height: 500px;
    margin: 10px;
  }
</style>
<img src="https://picsum.photos/300/300" alt="random img" class="float" />
<p class="shape_out_side">
  Lorem ipsum dolor sit amet consectetur adipisicing elit. Ex, facilis!
  Explicabo tenetur commodi error earum harum officia sint nam perspiciatis
  fugit, quia facere assumenda beatae enim neque rem dolores dolorem accusantium
  dignissimos voluptatum accusamus natus perferendis autem rerum! Dolorem ad
  quidem nobis! Laudantium, similique asperiores! Nihil aliquid eum iure rerum
  eveniet, quod in culpa, saepe odit quidem vel corrupti explicabo, placeat
  beatae. Provident, blanditiis quidem voluptates labore optio, libero maiores
  facilis sequi reiciendis dolore fugiat vel ratione amet similique maxime
  repellendus omnis. Quam hic dolores a labore vero, et excepturi dolorum?
  Corporis doloribus architecto at adipisci, accusamus deleniti magnam, odio
  quas porro ullam obcaecati error tenetur esse exercitationem aliquid tempora
  culpa ipsum sapiente in voluptatem minus nisi ut optio! Possimus suscipit
  deleniti laborum voluptatem ducimus. Autem sequi sapiente asperiores
  perspiciatis aut quo, beatae quasi, reprehenderit distinctio repudiandae
  cumque temporibus non fugiat ea expedita numquam minus quae! Aut temporibus,
  quia animi exercitationem molestias quaerat rem eius blanditiis deserunt
  dignissimos debitis ratione reiciendis, in cum id magni nisi neque iusto
  repudiandae ipsa. Vitae ad laudantium cum quis dolore saepe excepturi, vel
  sint, expedita beatae ullam eligendi? Ullam expedita asperiores cupiditate,
  debitis placeat doloremque nihil aliquid, impedit corrupti ad autem
  accusantium magnam ducimus.
</p>
```

</htmlcss-snippet>

# Thuộc tính display và các tình huống nâng cao

## Các giá trị cho `display`:

Có rất nhiều giá trị cho thuộc tính `display` trong CSS, mỗi giá trị sẽ có một cách hiển thị khác nhau.

Dưới đây là một số giá trị phổ biến của thuộc tính `display`:

- `block`: Hiển thị phần tử dưới dạng khối.

- `inline`: Hiển thị phần tử dưới dạng nội dòng.

- `inline-block`: Hiển thị phần tử dưới dạng nội dòng nhưng vẫn có thể thiết lập kích thước và padding.

- `none`: Ẩn phần tử.

## Ví dụ sử dụng thuộc tính display:

---

### 1. Display: block

Thuộc tính `display: block` có nghĩa là phần tử sẽ được hiển thị dưới dạng khối, tức là nó sẽ chiếm hết chiều rộng của phần tử cha và nằm trên một dòng riêng, các phần tử khác sẽ không thể nằm cùng dòng với phần tử này.

Một số thẻ có thuộc tính `display: block` mặc định: `<div>`, các thẻ heading `<h1>` => `<h6>`, `<p>`, `<form>`, `<header>`, `<footer>`, `<section>`, `<article>`, `<aside>`, `<nav>`, `<ul>`, `<li>`, `<table>`, `<blockquote>`, `<address>`, `<canvas>`, `<dd>`, `<dl>`, `<dt>`, `<fieldset>`, `<figcaption>`, `<figure>`, `<hr>`, `<legend>`, `<main>`, `<ol>`, `<pre>`, `<section>`, `<summary>`, `<time>`, `<video>`, `<audio>`, `<embed>`, `<iframe>`, `<img>`, `<object>`, `<param>`, `<picture>`, `<source>`, `<track>`, `<svg>`, `<math>`, `<button>`, `<datalist>`, `<keygen>`, `<label>`, `<meter>`, `<output>`, `<progress>`, `<select>`, `<textarea>`, `<details>`, `<dialog>`, `<menu>`, `<menuitem>`, `<summary>`.

<htmlcss-snippet>

```html
<style>
  .box {
    display: block;
    width: 200px;
    height: 200px;
    background-color: red;
    color: #fff;
  }
</style>

<span class="box">Hello F8</span>
<p>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque sit amet
  felis sed risus tincidunt posuere.
</p>
```

</htmlcss-snippet>

---

### 2. Display: inline

Thuộc tính `display: inline` có nghĩa là phần tử sẽ được hiển thị dưới dạng nội dòng, tức là nó sẽ nằm trên cùng một dòng với các phần tử khác, và nó sẽ chỉ chiếm chiều rộng bằng với nội dung bên trong.

Một số thẻ có thuộc tính `display: inline` mặc định: `<span>`, `<a>`, `<abbr>`, `<acronym>`, `<b>`, `<bdo>`, `<big>`, `<br>`, `<button>`, `<cite>`, `<code>`, `<dfn>`, `<em>`, `<i>`, `<img>`, `<input>`, `<kbd>`, `<label>`, `<map>`, `<object>`, `<output>`, `<q>`, `<samp>`, `<script>`, `<select>`, `<small>`, `<span>`, `<strong>`, `<sub>`, `<sup>`, `<textarea>`, `<time>`, `<tt>`, `<var>`.

<htmlcss-snippet>

```html
<style>
  .box {
    display: inline;
    width: 200px;
    height: 200px;
    background-color: red;
    color: #fff;
  }
</style>

<div class="box">Hello F8</div>
<p>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque sit amet
  felis sed risus tincidunt posuere.
</p>
```

</htmlcss-snippet>

---

### 3. Display: inline-block

Thuộc tính `display: inline-block` có nghĩa là phần tử sẽ được hiển thị dưới dạng nội dòng nhưng vẫn có thể thiết lập kích thước và padding.

Một số thẻ có thuộc tính `display: inline-block` mặc định: `<img>`, `<input>`, `<button>`, `<textarea>`, `<select>`, `<iframe>`, `<canvas>`, `<video>`, `<audio>`, `<embed>`, `<object>`, `<applet>`, `<math>`, `<svg>`.

<htmlcss-snippet>

```html
<style>
  .box {
    display: inline-block;
    width: 50px;
    height: 50px;
    background-color: red;
    color: #fff;
  }
</style>

<div class="box">Hello F8</div>
<span>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque sit amet
  felis sed risus tincidunt posuere.
</span>
```

</htmlcss-snippet>

---

### 4. Display: none

Thuộc tính `display: none` có nghĩa là phần tử sẽ bị ẩn đi, tức là nó sẽ không được hiển thị trên trang web.

<htmlcss-snippet>

```html
<style>
  .box {
    display: none;
    width: 200px;
    height: 200px;
    background-color: red;
    color: #fff;
  }
</style>

<div class="box">Hello F8</div>

<p>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque sit amet
  felis sed risus tincidunt posuere.
</p>
```

</htmlcss-snippet>

---

## Các thuộc tính `display` nâng cao:

> Các thuộc tính `display` khác như: `flex`, `grid`, `table`, `list-item`,... sẽ được học ở các bài học sau.

# Thuộc tính position và các kỹ thuật xử lý nâng cao

## Thuộc tính position

Thuộc tính `position` trong CSS cho phép bạn kiểm soát cách phần tử được định vị trong layout. Dưới đây là một số giá trị phổ biến của thuộc tính `position` và các kỹ thuật xử lý nâng cao:

- `static`: Định vị mặc định của phần tử. Phần tử sẽ theo dòng và không bị ảnh hưởng bởi các thuộc tính `top`, `bottom`, `left`, `right` hoặc `z-index`.

- `relative`: Định vị phần tử theo vị trí ban đầu và có thể dịch chuyển bằng các thuộc tính `top`, `bottom`, `left`, `right`. Phần tử không bị ảnh hưởng bởi các phần tử khác.

- `absolute`: Định vị phần tử một cách tuyệt đối dựa trên phần tử cha gần nhất có thuộc tính `position` khác `static`. Phần tử sẽ di chuyển dựa trên các thuộc tính `top`, `bottom`, `left`, `right`.

- `fixed`: Định vị phần tử một cách tuyệt đối dựa trên cửa sổ trình duyệt. Phần tử sẽ luôn hiển thị ở vị trí cố định kể cả khi cuộn trang.

- `sticky`: Kết hợp giữa `relative` và `fixed`. Phần tử sẽ định vị như `relative` khi nằm trong khoảng một vùng nhất định, sau đó chuyển sang `fixed` khi cuộn trang.

Các kỹ thuật xử lý nâng cao:

- `z-index`: Thuộc tính `z-index` xác định vị trí sắp xếp 3D của phần tử. Giá trị lớn hơn sẽ đặt phần tử phía trên các phần tử khác.

- `overflow`: Thuộc tính `overflow` xác định cách xử lý nội dung của phần tử khi nó vượt qua kích thước được chỉ định. Các giá trị phổ biến bao gồm `visible`, `hidden`, `scroll` và `auto`.

- `clip-path`: Thuộc tính `clip-path` xác định hình dạng của phần tử bằng cách cắt bỏ các phần không mong muốn.

- `transform`: Thuộc tính `transform` cho phép bạn thay đổi hình dạng, kích thước và vị trí của phần tử bằng cách sử dụng các phép biến đổi như xoay, co giãn, dịch chuyển và nhiều hơn nữa.

---

## Ví dụ sử dụng thuộc tính position

Ví dụ sử dụng thuộc tính position:

<htmlcss-snippet>

```html
<style>
  .container {
    position: relative;
    width: 300px;
    height: 200px;
    background-color: #f1f1f1;
  }

  .box {
    position: absolute;
    top: 50px;
    left: 50px;
    width: 100px;
    height: 100px;
    background-color: #ff0000;
  }

  .fixed-box {
    position: fixed;
    top: 50px;
    right: 50px;
    width: 100px;
    height: 100px;
    background-color: #00ff00;
  }

  .sticky-box {
    position: sticky;
    top: 20px;
    width: 100px;
    height: 100px;
    background-color: #0000ff;
  }

  div {
    border: 2px solid #333;
  }

  span {
    color: #fff;
    background-color: #333;
    padding: 5px;
  }
</style>

<div class="container">
  <span>Relative</span>
  <div class="box">
    <span>Absolute</span>
  </div>
</div>

<div class="fixed-box">
  <span>Fixed</span>
</div>

<div style="height: 2000px;">
  <span>Static</span>
  <div class="sticky-box">
    <span>Sticky</span>
  </div>
</div>
```

</htmlcss-snippet>

---

## Các lưu ý khi sử dụng thuộc tính position

Các lưu ý khi sử dụng thuộc tính position:

- Khi sử dụng thuộc tính `position: absolute` hoặc `position: fixed`, phần tử sẽ được định vị dựa trên phần tử cha gần nhất có thuộc tính `position` khác `static`.

- Khi sử dụng thuộc tính `position: sticky`, phần tử sẽ được định vị dựa trên phần tử cha gần nhất có thuộc tính `position` khác `static` và có thuộc tính `overflow` khác `visible`.

- Khi sử dụng thuộc tính `position: sticky`, phần tử sẽ không hoạt động nếu nó nằm trong phần tử cha có thuộc tính `overflow` là `hidden`, `scroll` hoặc `auto`.

- Thuộc tính `position: absolute` sẽ không hoạt động nếu phần tử cha có thuộc tính `overflow` là `hidden`, `scroll` hoặc `auto`.

- Thuộc tính `position: absolute` sẽ không hoạt động nếu phần tử cha có thuộc tính `transform` khác `none`.

- Khi sử dụng `position: relative` theo giá trị `%` thì thành phần cha cần có width và height để phần tử con có thể tính toán được vị trí.

- Thuộc tính `position: relative` làm cho phần tử có z-index cao hơn các phần tử anh em của nó.

- Thuộc tính `position: absolute` làm cho phần tử biến mất khỏi luồng của trang, nó không chiếm không gian trống.

- Thuộc tính `position: absolute` khi sử dụng sẽ luôn bám theo phần tử cha gần nhất có thuộc tính `position` khác `static`.

- Thuộc tính `position: fixed` làm cho phần tử biến mất khỏi luồng của trang, nó không chiếm không gian trống.

- Thuộc tính `position: fixed` luôn luôn bám theo `<body></body>`.

# Thuộc tính list-style

## Định dạng danh sách (List Style)

Trong HTML và CSS, bạn có thể định dạng các danh sách bằng cách sử dụng thuộc tính `list-style`. Thuộc tính này cho phép bạn tùy chỉnh kiểu, biểu tượng và văn bản liên quan đến danh sách. Dưới đây là một số giá trị phổ biến của thuộc tính `list-style`:

- `list-style-type`: Kiểu danh sách.

  - `none`: Không hiển thị biểu tượng danh sách.
  - `disc`: Hiển thị dưới dạng các chấm tròn.
  - `circle`: Hiển thị dưới dạng các vòng tròn.
  - `square`: Hiển thị dưới dạng các hình vuông.
  - `decimal`: Hiển thị dưới dạng các số thập phân (1, 2, 3, ...).
  - `lower-alpha`: Hiển thị dưới dạng chữ thường (a, b, c, ...).
  - `upper-alpha`: Hiển thị dưới dạng chữ hoa (A, B, C, ...).
  - `lower-roman`: Hiển thị dưới dạng số La Mã chữ thường (i, ii, iii, ...).
  - `upper-roman`: Hiển thị dưới dạng số La Mã chữ hoa (I, II, III, ...).

- `list-style-position`: Vị trí của biểu tượng danh sách.

  - `inside`: Hiển thị biểu tượng bên trong phần tử danh sách.
  - `outside`: Hiển thị biểu tượng bên ngoài phần tử danh sách.

- `list-style-image`: Đường dẫn đến hình ảnh sẽ được sử dụng làm biểu tượng danh sách.

---

## Ví dụ sử dụng thuộc tính list-style

Ví dụ sử dụng thuộc tính `list-style-type`:

<htmlcss-snippet>

```html
<style>
  ul {
    list-style: square;
  }

  ol {
    list-style: upper-roman;
  }
</style>

<h2>Danh sách không đánh số</h2>
<ul>
  <li>Phần tử 1</li>
  <li>Phần tử 2</li>
  <li>Phần tử 3</li>
</ul>

<h2>Danh sách đánh số</h2>
<ol>
  <li>Phần tử 1</li>
  <li>Phần tử 2</li>
  <li>Phần tử 3</li>
</ol>
```

</htmlcss-snippet>

---

Ví dụ sử dụng thuộc tính `list-style-position`:

<htmlcss-snippet>

```html
<style>
  ul {
    list-style: square inside;
  }

  ol {
    list-style: upper-roman outside;
  }
  ul,
  ol {
    border-left: 2px solid #f00;
  }
</style>

<h2>Danh sách không đánh số</h2>

<ul>
  <li>Phần tử 1</li>
  <li>Phần tử 2</li>
  <li>Phần tử 3</li>
</ul>

<h2>Danh sách đánh số</h2>

<ol>
  <li>Phần tử 1</li>
  <li>Phần tử 2</li>
  <li>Phần tử 3</li>
</ol>
```

</htmlcss-snippet>

---

Ví dụ sử dụng thuộc tính `list-style-image`:

<htmlcss-snippet>

```html
<style>
  ul {
    list-style-image: url("https://picsum.photos/20/20");
  }
</style>

<h2>Danh sách không đánh số</h2>

<ul>
  <li>Phần tử 1</li>
  <li>Phần tử 2</li>
  <li>Phần tử 3</li>
</ul>
```

</htmlcss-snippet>

---

## Các lưu ý khi sử dụng thuộc tính list-style

Các lưu ý khi sử dụng thuộc tính `list-style`:

- Thuộc tính `list-style` là một thuộc tính rút gọn của `list-style-type`, `list-style-position` và `list-style-image`.

- Thuộc tính `list-style` có thể được sử dụng với bất kỳ phần tử nào bằng cách sử dụng thuộc tính `display: list-item`.

# Nguyên tắc kế thừa trong CSS

## Nguyên tắc kế thừa trong CSS

Trong CSS, nguyên tắc kế thừa cho phép các phần tử con kế thừa các thuộc tính từ phần tử cha của chúng. Điều này giúp giảm việc lặp lại mã CSS và làm cho việc quản lý phong cách trang web dễ dàng hơn. Dưới đây là một số nguyên tắc kế thừa quan trọng trong CSS:

- `color`: Màu sắc chữ được kế thừa từ màu chữ của phần tử cha gần nhất, nếu không có thì lấy từ mặc định trình duyệt, thường là màu đen.

- `font-family`: Phông chữ được kế thừa từ font của phần tử cha gần nhất, nếu không có thì lấy từ mặc định trình duyệt, thường là Times New Roman.

- `font-size`: Kích thước chữ được kế thừa từ font-size của phần tử cha gần nhất, nếu không có thì lấy từ mặc định trình duyệt, thường là 16px.

- `font-weight`: Độ đậm của chữ được kế thừa từ font-weight của phần tử cha gần nhất, nếu không có thì lấy từ mặc định trình duyệt, thường là 400.

- `text-align`: Căn chỉnh văn bản được kế thừa từ phần tử cha gần nhất, nếu không có thì lấy từ mặc định trình duyệt, thường là left.

- `line-height`: Khoảng cách giữa các dòng trong văn bản được kế thừa từ phần tử cha gần nhất, nếu không có thì lấy từ mặc định trình duyệt, thường là 1.2.

---

## Ví dụ về nguyên tắc kế thừa

Ở trong ví dụ này, chúng ta sẽ thấy các thuộc tính `color`, `font-family`, `font-size`, `font-weight`, `text-align`, `line-height`, `margin` và `padding` được thẻ `<p>` kế thừa từ thẻ `.box` và thẻ `<span>` kế thừa từ thẻ `<p>`.

<htmlcss-snippet>

```html
<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  .box {
    width: 200px;
    height: 400px;
    background-color: red;
    color: #fff;
    font-size: 20px;
    font-weight: bold;
    text-align: center;
    line-height: 1.5;
    margin: 20px;
    padding: 20px;
  }
</style>

<div class="box">
  <p>
    Hello F8
    <span>
      Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque sit
      amet felis sed risus tincidunt posuere.
    </span>
  </p>
</div>
```

</htmlcss-snippet>

---

## Lưu ý sử dụng nguyên tắc kế thừa

- Không phải tất cả các thuộc tính đều được kế thừa từ phần tử cha.
  - Ví dụ, các thuộc tính `margin` và `padding` không được kế thừa.
- Các thuộc tính được kế thừa sẽ áp dụng cho tất cả các phần tử con, bao gồm cả các phần tử con lồng nhau.
- Có thể ghi đè lên giá trị kế thừa bằng cách xác định giá trị cho thuộc tính đó trực tiếp cho phần tử con.
- Để ngăn chặn việc kế thừa một thuộc tính, có thể sử dụng giá trị `initial` hoặc `unset` cho thuộc tính đó.

---

Tham khảo thêm tại: [developer.mozilla.org](https://developer.mozilla.org/CSS/inheritance)

# Kỹ thuật CSS Sprites

## Kỹ thuật CSS Sprites

Kỹ thuật CSS Sprites là một phương pháp tối ưu hóa tải trang web bằng cách kết hợp nhiều hình ảnh nhỏ thành một hình ảnh lớn duy nhất, và sử dụng CSS để hiển thị chỉ một phần của hình ảnh lớn này cho mỗi phần tử trên trang.

Lợi ích chính của CSS Sprites bao gồm:

- Giảm số lượng yêu cầu HTTP: Thay vì tải nhiều hình ảnh nhỏ, chỉ cần tải một hình ảnh lớn duy nhất.
- Giảm thời gian tải trang: Một lần tải hình ảnh lớn và sử dụng cache để hiển thị các phần tử trên trang.
- Tối ưu hóa hiệu suất: Giảm kích thước dữ liệu tải xuống, giảm băng thông mạng và giúp trang web hoạt động nhanh hơn.

Dưới đây là một ví dụ cơ bản về việc sử dụng CSS Sprites:

<htmlcss-snippet>

```html
<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  body {
    width: 100vw;
    min-height: 100vh;
    margin: 0 auto;
  }
  .example {
    width: 300px;
    height: 300px;
    display: flex;
    justify-content: space-between;
  }
  .sprite {
    width: 50px;
    height: 50px;
    background-image: url("https://picsum.photos/200/200");
    background-repeat: no-repeat;
  }

  .sprite-1 {
    background-position: 0 0;
  }

  .sprite-2 {
    background-position: -50px 0;
  }

  .sprite-3 {
    background-position: -100px 0;
  }

  .sprite-4 {
    background-position: -150px 0;
  }
</style>

<div class="example">
  <div class="sprite sprite-1"></div>
  <div class="sprite sprite-2"></div>
  <div class="sprite sprite-3"></div>
  <div class="sprite sprite-4"></div>
</div>
```

</htmlcss-snippet>

---

## Các lưu ý khi sử dụng CSS Sprites

- Các hình ảnh trong CSS Sprites nên có kích thước bằng nhau.

---

# Sử dụng thư viện Font Icon (Font-Awesome) và các kỹ thuật liên quan

## Sử dụng thư viện Font Icon (Font-Awesome) và các kỹ thuật liên quan

Thư viện Font Icon, ví dụ như Font-Awesome, cung cấp một tập hợp các biểu tượng được thiết kế bằng các ký tự và các tệp font đặc biệt. Bằng cách sử dụng Font Icon, bạn có thể thêm các biểu tượng vào trang web của mình mà không cần sử dụng hình ảnh. Dưới đây là các bước để sử dụng Font-Awesome và các kỹ thuật liên quan:

## Các bước để sử dụng Font-Awesome

### Bước 1: Liên kết thư viện Font-Awesome

Thêm đoạn mã sau vào phần `<head>` của tệp HTML của bạn để liên kết với thư viện Font-Awesome:

```html
<link
  rel="stylesheet"
  href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css"
  integrity="sha512-..."
  crossorigin="anonymous"
/>
```

### Bước 2: Sử dụng biểu tượng Font-Awesome

Sử dụng các biểu tượng Font-Awesome bằng cách thêm các lớp CSS tương ứng vào phần tử HTML của bạn.
Dưới đây là ví dụ về việc sử dụng biểu tượng cụ thể:

<htmlcss-snippet>

```html
<link
  rel="stylesheet"
  href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css"
  integrity="sha512-..."
  crossorigin="anonymous"
/>

<i class="fas fa-heart"></i>
```

</htmlcss-snippet>

---

Trong ví dụ trên, chúng ta sử dụng lớp CSS fas để chỉ định rằng đó là một biểu tượng từ Font-Awesome, và fa-heart là lớp cụ thể cho biểu tượng trái tim.

### Bước 43 Tùy chỉnh biểu tượng Font-Awesome

Có thể tùy chỉnh biểu tượng Font-Awesome bằng cách sử dụng các thuộc tính CSS như `color`, `font-size`, `font-weight`, `text-align`, `line-height`, `margin` và `padding`...

<htmlcss-snippet>

```html
<link
  rel="stylesheet"
  href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css"
  integrity="sha512-..."
  crossorigin="anonymous"
/>

<style>
  .icon {
    color: red;
    font-size: 50px;
  }
</style>

<i class="fas fa-heart icon"></i>
```

</htmlcss-snippet>

Trong ví dụ trên, chúng ta tùy chỉnh:

- Màu sắc của biểu tượng bằng thuộc tính `color`: red

- Kích thước của biểu tượng bằng thuộc tính `font-size`: 50px

---

## Các lớp CSS Font-Awesome

Dưới đây là một số lớp CSS Font-Awesome phổ biến:

- `fas`: Font-Awesome Solid

- `fab`: Font-Awesome Brands

- `far`: Font-Awesome Regular

- `fa-xs`: Kích thước nhỏ

- `fa-sm`: Kích thước nhỏ

- `fa-lg`: Kích thước lớn

- Còn nhiều class khác, tham khảo tại [fontawesome.com](https://fontawesome.com/v5.15/how-to-use/on-the-web/referencing-icons/basic-use)

---

# Sử dụng biến trong CSS: Biến toàn cục, biến cục bộ

## Biến trong CSS là gì?

Biến trong CSS:

- Định nghĩa: Biến là một giá trị được lưu trữ và tái sử dụng trong CSS.

- Tác dụng: Chúng giúp làm cho mã CSS trở nên dễ dàng quản lý và tiết kiệm thời gian khi muốn thay đổi các giá trị được sử dụng nhiều lần trong trang web.

---

## Biến toàn cục (Global Variables)

Biến toàn cục (Global Variables):

- Định nghĩa: Biến toàn cục được khai báo và có thể sử dụng trong toàn bộ tệp CSS hoặc các tệp CSS khác.

- Cách khai báo: Sử dụng từ khóa `--` trước tên biến và gán giá trị cho nó trong phần khai báo CSS của root (`:root`).

- Cách sử dụng: Để sử dụng biến toàn cục, sử dụng hàm `var()` và truyền tên biến vào như giá trị của thuộc tính.

- Ví dụ:

<htmlcss-snippet>

```html
<style>
  :root {
    --primary-color: #fad500;

    --background-color: #333333;
  }

  .button {
    background-color: var(--background-color);
    color: var(--primary-color);
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
  }

  .box {
    background-color: var(--primary-color);
    width: 300px;
    height: 200px;
    text-align: center;
  }
</style>

<div class="box">
  <button class="button">Hello F8</button>
</div>
```

</htmlcss-snippet>

Trong ví dụ này, chúng ta đã định nghĩa hai biến toàn cục là `--primary-color` và `--background-color` và sử dụng chúng trong các thuộc tính `background-color` và `color` của các phần tử.

---

## Biến cục bộ (Local Variables)

Biến cục bộ (Local Variables):

- Định nghĩa: Biến cục bộ chỉ tồn tại trong phạm vi của một phần tử hoặc một nhóm phần tử được xác định bởi một lớp hoặc một ID.

- Cách khai báo: Sử dụng từ khóa `--` trước tên biến và gán giá trị cho nó trong khối CSS của phần tử hoặc nhóm phần tử.

- Cách sử dụng: Giống như biến toàn cục, sử dụng hàm `var()` và truyền tên biến vào như giá trị của thuộc tính.

- Ví dụ:

<htmlcss-snippet>

```html
<style>
  .box {
    --box-width: 300px;
    --box-height: 200px;
    --color: #fad500;
    --background-color: #333333;
    width: var(--box-width);
    height: var(--box-height);
    text-align: center;
  }

  .box .content {
    background-color: var(--background-color);
    color: var(--color);
  }
</style>

<div class="box">
  <h2 clas="content">Hello F8</h2>
</div>
```

</htmlcss-snippet>

Trong ví dụ này, chúng ta đã định nghĩa các biến cục bộ là `--box-width`, `--box-height`, `--color` và `--background-color` và sử dụng chúng trong các thuộc tính `width`, `height`, `background-color` và `color` của các phần tử.

---

## Các lưu ý khi sử dụng biến trong CSS

Các lưu ý khi sử dụng biến trong CSS:

- Biến toàn cục có thể được sử dụng trong bất kỳ phần tử nào trong tệp CSS.

- Biến cục bộ chỉ có thể được sử dụng trong phạm vi của phần tử hoặc nhóm phần tử được xác định bởi một lớp hoặc một ID.

- Biến toàn cục và biến cục bộ có thể được sử dụng trong các tệp CSS, HTML khác nhau.
