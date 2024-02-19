# Refs

## Refs là gì

Ref-reference tức là tham chiếu, Ref trong React cũng có ý nghĩa tương tự, nó giúp chúng ta khởi tạo và tham chiếu tới một giá trị nhất định, không thay đổi hay reset sau mỗi lần render.

Nó tương tự như state, tuy nhiên với ref, khi thay đổi giá trị nó sẽ không re-render. Vì vậy nó thường được xử lý các giá trị, tác vụ không cần phải re-render nhưng cần thay đổi được và lưu giá trị sau mỗi lần re-render.
Ví dụ: Sử dụng để lưu các elements dùng để thao tác DOM sau mỗi lần re-render, sử dụng để lưu một breakpoint, giá trị nào đó như nút dừng khi làm countdown,...

Một vài trường hợp hữu ích để sử dụng refs:

- Quản lý focus, text selection, hoặc media playback.

- Trigger animation của một element khác.

- Tích hợp những thư viện DOM từ bên thứ ba.

---

## Không nên lạm dụng Refs

Chúng ta hay có xu hướng sử dụng Refs để xử lý mọi thử xảy ra trong ứng dụng của mình. tuy nhiên khi các DOM bị thay đổi thì nó sẽ ảnh hưởng một phần nào đó đến quá trình render các component. Ngoài ra nó còn gây khó khăn cho việc kiểm soát code, ảnh hưởng tới hiệu năng mỗi lần re-render,...

Vì vậy, trừ khi bất khả kháng, chúng ta sẽ sử dụng Ref để tham chiếu tới các element trong DOM, còn nếu không, nên xem xét sử dung state.

---

## Phân biệt useRef và createRef trong React

Với `createRef` không thể sử dụng trong function component mà chỉ có thể sử dụng trong class component, còn `useRef` thì có thể.

Trong mỗi lần re-render, `useRef` sẽ không khởi tạo lại, nhưng `createRef` thì khởi tạo lại sau mỗi lần re-render.

Vì vậy, mỗi lần re-render cả component `createRef` sẽ không lưu trữ giá trị ref còn `useRef` thì có.

Dưới đây là bảng phân biệt giữa `useRef` và `createRef` trong React:

|                                 | useRef                | createRef       |
| ------------------------------- | --------------------- | --------------- |
| **Sử dụng trong**               | Functional Component¹ | Class Component |
| **Tạo mới mỗi lần re-render?**  | Không                 | Có              |
| **Lưu trữ giữa các lần render** | Có                    | Không           |

- `useRef` và `createRef` đều là cách để tạo ra một tham chiếu (ref) trong React.
- Trong Functional Component, chúng ta sử dụng `useRef` thay vì `createRef`. Nếu chúng ta tạo một ref bằng cách sử dụng `createRef` trong một Functional Component, React sẽ tạo mới một instance ref mỗi lần re-render thay vì giữ nguyên instance xuyên suốt các quá trình render.
- `useRef` giống như một "hộp", dùng để lưu các giá trị của một element sử dụng thuộc tính `.current`.
- `useRef` cho phép trạng thái của ref tồn tại giữa các lần render, mặc dù chúng ta không cố ý lưu trữ nó ở đâu.

---

## Khởi tạo và sử dụng Ref

Refs được khởi tạo bằng `React.createRef()` và được gắn vào các React element thông qua thuộc tính ref. Refs thường được gán cho một element nào đó, tại đó chúng ta có thể tham chiếu đến tất cả các thành phần bên trong nó.

Khi một element có chứa ref render, chúng ta có thể sử dụng một thuộc tính của ref là current để truy cập đến node hiện tại.

Nếu ref callback được định nghĩa như một inline function, nó sẽ được gọi 2 lần khi cập nhật, lần thứ 1 có giá trị là null và lần thứ 2 là DOM element. Điều này xảy ra bởi vì một instance của function được tạo ra sau mỗi lần render, React cần phải xóa những ref cũ và set up một cái mới. Chúng ta có thể tránh điều này bằng cách định nghĩa ref callback như một method trên class, nhưng nó cũng không quan trọng trong hầu hết các trường hợp.

Với function component, chúng ta có thể sử dụng một hook khác để khởi tạo ref là `useRef`
