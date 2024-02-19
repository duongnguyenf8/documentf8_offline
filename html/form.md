### Thẻ form

- Thẻ form dùng để tạo ra một form nhập liệu trên trang web.
- form là một nhóm các phần tử nhập liệu.
- Các thẻ form thường được sử dụng:
  - `<form>`: Tạo ra một form nhập liệu.
  - `<input>`: Tạo ra một ô nhập liệu.
  - `<textarea>`: Tạo ra một ô nhập liệu dài.
  - `<button>`: Tạo ra một nút bấm.
  - `<select>`: Tạo ra một danh sách lựa chọn.
  - `<option>`: Tạo ra một lựa chọn trong danh sách.
  - `<label>`: Tạo ra một nhãn cho ô nhập liệu.
- Có hai cách để gửi dữ liệu từ form lên máy chủ bằng thuộc tính action của thẻ form:
  - Phương thức GET: Dữ liệu được gửi lên máy chủ dưới dạng chuỗi truy vấn.
  - Phương thức POST: Dữ liệu được gửi lên máy chủ dưới dạng một gói tin.
- Các phần tử và thuộc tính thường dùng trong form

  - Thẻ input:

    - `type="radio"`: Tạo ra một ô nhập liệu dạng nút radio.

      ```html
      <input type="radio" name="gioi_tinh" value="nam" /> Nam
      <input type="radio" name="gioi_tinh" value="nu" /> Nữ
      ```

      - Lưu ý thẻ input dạng radio phải có thuộc tính name giống nhau để nhóm các nút radio lại với nhau.
      - Ví dụ mẫu khi sử dụng thẻ input dạng radio:

        <htmlcss-snippet>

        ```html
        <input type="radio" name="gioi_tinh" value="nam" /> Nam
        <input type="radio" name="gioi_tinh" value="nu" /> Nữ
        ```

        </htmlcss-snippet>

      - Nên lồng thẻ input dạng radio vào thẻ label để khi click vào label thì nút radio cũng được chọn.

        <htmlcss-snippet>

        ```html
        <label> <input type="radio" name="gioi_tinh" value="nam" /> Nam </label>
        <label> <input type="radio" name="gioi_tinh" value="nu" /> Nu </label>
        ```

        </htmlcss-snippet>

      - Có thể sử dụng thuộc tính checked để chọn một nút radio mặc định.

        <htmlcss-snippet>

        ```html
        <label>
          <input type="radio" name="gioi_tinh" value="nam" checked /> Nam
        </label>
        <label> <input type="radio" name="gioi_tinh" value="nu" /> Nu </label>
        ```

        </htmlcss-snippet>

      - Có thể sử dụng thuộc tính disabled để vô hiệu hóa một nút radio.

        <htmlcss-snippet>

        ```html
        <label>
          <input type="radio" name="gioi_tinh" value="nam" disabled /> Nam
        </label>
        ```

        </htmlcss-snippet>

      - Có thể sử dụng thuộc tính required để bắt buộc người dùng phải chọn một nút radio.

        <htmlcss-snippet>

        ```html
        <form>
          <label>
            <input type="radio" name="gioi_tinh" value="nam" required /> Nam
          </label>
          <label> <input type="radio" name="gioi_tinh" value="nu" /> Nu </label>
          <input type="submit" value="Gui" />
        </form>
        ```

        </htmlcss-snippet>

    - `type="checkbox"`: Tạo ra một ô nhập liệu dạng checkbox.

      ```html
      <input type="checkbox" name="so_thich" value="doc_sach" /> Đọc sách
      <input type="checkbox" name="so_thich" value="nghe_nhac" /> Nghe nhạc
      ```

      - Lưu ý thẻ input dạng checkbox phải có thuộc tính name giống nhau để nhóm các ô checkbox lại với nhau.
      - Ví dụ mẫu khi sử dụng thẻ input dạng checkbox:

        <htmlcss-snippet>

        ```html
        <input type="checkbox" name="so_thich" value="doc_sach" /> Đọc sách
        <input type="checkbox" name="so_thich" value="nghe_nhac" /> Nghe nhạc
        ```

        </htmlcss-snippet>

      - Nên lồng thẻ input dạng checkbox vào thẻ label để khi click vào label thì ô checkbox cũng được chọn.

        <htmlcss-snippet>

        ```html
        <label>
          <input type="checkbox" name="so_thich" value="doc_sach" /> Đọc sách
        </label>
        ```

        </htmlcss-snippet>

      - Có thể sử dụng thuộc tính checked để chọn một ô checkbox mặc định.

        <htmlcss-snippet>

        ```html
        <label>
          <input type="checkbox" name="so_thich" value="doc_sach" checked /> Đọc
          sách
        </label>
        <label>
          <input type="checkbox" name="so_thich" value="nghe_nhac" /> Nghe nhạc
        </label>
        ```

        </htmlcss-snippet>

    - `type="text"`: Tạo ra một ô nhập liệu dạng text.

      ```html
      <input type="text" name="ho_ten" />
      ```

      - Ví dụ mẫu khi sử dụng thẻ input dạng text:

        <htmlcss-snippet>

        ```html
        <form action="xu_ly" method="post">
          <input type="text" name="ho_ten" />
          <input type="submit" value="Gửi" />
        </form>
        ```

        </htmlcss-snippet>

      - Có thể sử dụng thuộc tính value để đặt giá trị mặc định cho ô nhập liệu.

        <htmlcss-snippet>

        ```html
        <input type="text" name="ho_ten" value="Nguyễn Văn A" />
        <input type="text" name="ho_ten" placeholder="Khong co value" />
        ```

        </htmlcss-snippet>

      - Có thể sử dụng thuộc tính placeholder để đặt một giá trị mặc định cho ô nhập liệu.

        <htmlcss-snippet>

        ```html
        <input type="text" name="ho_ten" placeholder="Nhập họ tên" />
        ```

        </htmlcss-snippet>

    - `type="password"`: Tạo ra một ô nhập liệu dạng password.

      ```html
      <input type="password" name="mat_khau" />
      ```

      - Ví dụ mẫu khi sử dụng thẻ input dạng password:

        <htmlcss-snippet>

        ```html
        <form action="xu_ly" method="post">
          <input type="password" name="mat_khau" />
          <input type="submit" value="Gửi" />
        </form>
        ```

        </htmlcss-snippet>

      - Có thể sử dụng thuộc tính value để đặt giá trị mặc định cho ô nhập liệu.

        <htmlcss-snippet>

        ```html
        <input type="password" name="mat_khau" value="123456" />
        ```

        </htmlcss-snippet>

      - Có thể sử dụng thuộc tính placeholder để đặt một giá trị mặc định cho ô nhập liệu.

        <htmlcss-snippet>

        ```html
        <input type="password" name="mat_khau" placeholder="Nhập mật khẩu" />
        ```

        </htmlcss-snippet>

    - `type="file"`: Tạo ra một ô nhập liệu dạng file.

      ```html
      <input type="file" name="hinh_anh" />
      ```

      - Ví dụ mẫu khi sử dụng thẻ input dạng file:

        <htmlcss-snippet>

        ```html
        <form action="xu_ly" method="post">
          <input type="file" name="hinh_anh" />
          <input type="submit" value="Gửi" />
        </form>
        ```

        </htmlcss-snippet>

      - Có thể sử dụng thuộc tính accept để chỉ định loại file được chọn.

        <htmlcss-snippet>

        ```html
        <input type="file" name="hinh_anh" accept="image/*" />
        ```

        </htmlcss-snippet>

      - Có thể sử dụng thuộc tính multiple để cho phép chọn nhiều file.

        <htmlcss-snippet>

        ```html
        <input type="file" name="hinh_anh" multiple />
        ```

        </htmlcss-snippet>

    - `type="hidden"`: Tạo ra một ô nhập liệu ẩn.

      ```html
      <input type="hidden" name="ma" value="123" />
      ```

      - Ví dụ mẫu khi sử dụng thẻ input dạng hidden:

        <htmlcss-snippet>

        ```html
        <form action="xu_ly" method="post">
          <input type="hidden" name="ma" value="123" />
          <input type="submit" value="Gửi" />
        </form>
        ```

        </htmlcss-snippet>

    - `type="date"`: Tạo ra một ô nhập liệu dạng ngày tháng.

      ```html
      <input type="date" name="ngay_sinh" />
      ```

      - Ví dụ mẫu khi sử dụng thẻ input dạng date:

        <htmlcss-snippet>

        ```html
        <form action="xu_ly" method="post">
          <input type="date" name="ngay_sinh" />
          <input type="submit" value="Gửi" />
        </form>
        ```

        </htmlcss-snippet>
