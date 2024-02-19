# `useState` trong React

## `useState` là gì?

Trong React, `useState` là một hook được sử dụng trong các function component để quản lý state. Nó cho phép chúng ta sử dụng state trong các function component theo cách tương tự như cách chúng ta sử dụng trong class component, mà không cần phải khai báo constructor hoặc sử dụng this.

`useState` trả về một mảng gồm hai giá trị:

State hiện tại: Đây là giá trị hiện tại của state. Chúng ta có thể truy cập nó bằng cách gọi phần tử đầu tiên của mảng.
Hàm cập nhật state: Đây là hàm được dùng để cập nhật state. Chúng ta có thể gọi hàm này với giá trị state mới để cập nhật state hiện tại.

Ví dụ:

```jsx
const [count, setCount] = useState(0);
```

Trong ví dụ này, count là giá trị state hiện tại và setCount là hàm cập nhật state. Chúng ta có thể sử dụng count trong bất kỳ phần nào của component và chúng ta có thể gọi setCount để cập nhật state.

---

## Khi nào nên sử dụng `useState`?

Chúng ta nên sử dụng `useState` khi chúng ta cần quản lý state trong một function component. State có thể được sử dụng để theo dõi dữ liệu đầu vào của người dùng, trạng thái của một thành phần hoặc bất kỳ thông tin nào khác cần được lưu trữ trong component.

Ví dụ, chúng ta có thể sử dụng `useState` để theo dõi số lượng lượt click vào một nút hoặc trạng thái của một modal.

---

## Cách sử dụng `useState`

Để sử dụng `useState`, chúng ta cần import nó vào component của mình:

```jsx
import { useState } from 'react';
```

Sau đó, chúng ta có thể khai báo một state bằng cách gọi `useState` với giá trị khởi tạo của state:

```jsx
const [count, setCount] = useState(0);
```

Giá trị khởi tạo của state có thể là bất kỳ loại dữ liệu nào, chẳng hạn như số, chuỗi hoặc đối tượng.

Để cập nhật state, chúng ta có thể gọi hàm `setCount` với giá trị state mới. Ví dụ:

```jsx
setCount(count + 1);
```

Khi chúng ta gọi `setCount`, React sẽ tự động re-render để hiển thị giá trị state mới.

---

## Các lưu ý khi sử dụng `useState`

Khi sử dụng state nói chung và `useState` nói riêng, chúng ta nên chú ý tới một số điều sau:

- Chỉ nên sử dụng `useState` trong các function component.
- Không nên sử dụng `useState` bên trong các vòng lặp hoặc các hàm khác.
- Nên đặt các state trong một đối tượng duy nhất để dễ quản lý.
- Nên sử dụng `useEffect` để cập nhật state từ các nguồn bên ngoài (ví dụ như API).

---

### 2 cách setState trong function component

Trả về trong hook useState có 2 dạng:

- 1 phần tử: Trả về một phần tử duy nhất chứa giá trị trạng thái hiện tại và một hàm để cập nhật giá trị trạng thái đó.

- 2 phần tử: Trả về một mảng gồm hai phần tử. Phần tử đầu tiên là giá trị trạng thái hiện tại, phần tử thứ hai là một hàm để cập nhật giá trị trạng thái đó.

Cách thứ hai an toàn hơn vì nó đảm bảo rằng giá trị trạng thái mới được tính toán dựa trên giá trị trạng thái hiện tại chính xác. Điều này đặc biệt quan trọng khi chúng ta đang cập nhật trạng thái trong một vòng lặp hoặc bộ hẹn giờ.

Ví dụ:

- Cách thứ nhất

  ```jsx
  function handleClick() {
  	setAge(age + 1); // setAge(42 + 1)
  	setAge(age + 1); // setAge(42 + 1)
  	setAge(age + 1); // setAge(42 + 1)
  }
  ```

- Cách thứ 2

  ```jsx
  function handleClick() {
  	setAge((a) => a + 1); // setAge(42 => 43)
  	setAge((a) => a + 1); // setAge(43 => 44)
  	setAge((a) => a + 1); // setAge(44 => 45)
  }
  ```

Trong ví dụ trên, nếu chúng ta sử dụng cách thứ nhất, giá trị trạng thái age sẽ không được cập nhật chính xác vì giá trị trạng thái hiện tại không được sử dụng để tính toán giá trị trạng thái mới. Điều này có thể dẫn đến lỗi.

---

### Sử dụng state với object, array

Với giá trị state được trả về bởi `useState`, nó ở trạng thái readonly tức là chỉ được đọc, tính toán,... không thể được ghi đè hay gán lại.

Ví dụ:

```jsx
const [form, setForm] = useState({
	name: 'F8',
	age: 100,
});

// Không nên thay đổi như này:
form.age = 101;

// Hãy thay đổi nó như này:
setForm({
	...form,
	age: 101,
});
```

---

## Kết luận

useState là một hook rất hữu ích trong React, cho phép chúng ta quản lý state trong các function component một cách dễ dàng. Hãy nắm rõ cách sử dụng `useState` để có thể xây dựng các ứng dụng React hiệu quả và dễ bảo trì. Tuy nhiên cần hiểu rõ về nó và tránh lạm dụng quá nhiều sẽ ảnh hưởng không tốt đến vấn đề hiệu năng.
