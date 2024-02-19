# Hocs trong react

## HOCs là gì

Higher-order component (HOC) là một kĩ thuật nâng cao trong React để tái sử dụng logic của component. HOC không thuộc React API. Nó là một pattern được sinh ra từ khả năng sử dụng kết hợp (compositional) của React.

Chính xác hơn: higher-order component là một hàm nhận vào một component và trả về một component mới.

Với các component, nó có tác dụng chuyển đổi các props thành UI. Còn với HOC, nó có tác dụng chuyển đổi 1 component thành 1 component khác.

HOC không chỉnh sửa, làm thay đổi component đầu vào mà nó chỉ kế thừa các hành vi của component đó. Một HOC sẽ tính toán, thay đổi component gốc bằng cách gói nó vào một component khác. Một HOC là một hàm không có tác dụng phụ (side-effects).

---

## Cách đặt tên HOC để tiện cho việc debug

Những container component tạo bởi HOCs đều xuất hiện trong `React Developer Tools` như bao component khác. Để dễ debug, chọn tên sao cho nó thể hiện rằng nó được sinh ra từ HOC.

Một quy ước thông dụng là thêm **with** với các component để có thể đọc thành một câu có ý nghĩa phù hợp với HOC

Ví dụ:

```js
const NavbarWithRouter = withRouter(Navbar);
```

Ở đây tức là Navbar sẽ được sử dụng Router, hay nếu một component được sử dụng context(React) thì sẽ đặt tên là:

```js
const ComponentHaveContextProps = withContext(Component);
```

---

## Lưu ý khi sử dụng HOCs

HOC giúp chúng ta thêm các tính năng mới vào component. Không nên thay đổi mạnh mẽ cấu trúc. component trả về từ HOC nên có chung interface với component con.

HOC giúp chúng ta thêm các tính năng mới vào component. Chúng không nên thay đổi mạnh mẽ cấu trúc. component trả về từ HOC nên có chung interface với component con:

```js
const NavbarWithRouter = withRouter(Navbar);
```

Thông thường, HOC nhận nhiều tham số. Trong ví dụ với Relay, config object được dùng để chỉ ra dữ liệu phụ thuộc của component:

```js
const CommentWithRelay = Relay.createContainer(Comment, config);
```

---

### Không dùng HOC bên trong hàm render

Thuật toán diffing của React (gọi là Reconciliation) dùng nhận dạng của component để quyết định xem có nên cập nhật subtree hay mount một cái mới. Nếu một component trả về giống (===) với component từ lần render trước, React sẽ đệ quy cập nhật subtree bằng so sánh (diffing) với cái mới.

Vấn đề ở đây không chỉ là về hiệu năng - việc remount một component gây ra tình trạng cả **state** cũng như những **children** đều bị mất.

---

### Refs không được truyền xuống

Mặc dù quy ước của HOC là truyền tất cả props xuống component, nhưng điều này **không áp dụng với refs**. Bởi vì ref không hẳn là một prop - như key, nó được xử lý bởi React. Nếu chúng ta thêm một ref vào một element mà component là kết quả từ HOC, refs sẽ mặc nhiên là của container ngoài cùng nhất, không phải component được bao bọc.

Giải pháp cho vấn đề này là dùng forwardRef API của React.
