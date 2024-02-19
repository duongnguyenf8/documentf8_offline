# Fetch API trong React JS

Fetching data là một kỹ thuật không thể thiếu trong bất cứ một ứng dụng react nào sử dụng dữ liệu từ bên ngoài, có rất nhiều cách để fetching data, tuy nhiên cách thường được sử dụng là phương thức `fetch()` trong JS

- Phương pháp này giúp đơn giản hóa việc lấy thông tin từ internet bằng fetch()
- Nó cho phép chúng ta gửi thêm chi tiết đến máy chủ, như chúng ta là ai hoặc loại dữ liệu chúng ta muốn.
- Nó được thiết kế để hoạt động tốt trong hầu hết các trình duyệt web mới hơn.
- Phương pháp này hỗ trợ các phương pháp khác nhau. Chúng cung cấp cho chúng ta sự linh hoạt trong việc tương tác với API.
- Phương thức này là một phương thức của vanilla JS. Chúng ta có thể sử dụng nó mà không cần bất kỳ thư viện bên ngoài hoặc phụ thuộc nào. Điều này làm cho nó nhẹ và hiệu quả.

```jsx
import { useState, useEffect } from 'react';
const Photos = () => {
	const [photos, setPhotos] = useState([]);
	useEffect(() => {
		fetch('https://jsonplaceholder.typicode.com/photos')
			.then((res) => {
				return res.json();
			})
			.then((data) => {
				console.log(data);
				setPhotos(data);
			});
	}, []);
	return (
		<div>
			{photos.map((photo) => (
				<img key={photo.id} src={photo.url} alt={photo.title} width={100} />
			))}
		</div>
	);
};
export default Photos;
```

---

## Sử dụng các thư viện fetching

Một số thư viện được sinh ra để fetching data, ví dụ lớn nhất như axios, swr, ...

### Sử dụng SWR để fetching data

Vì nó là một thư viện bên ngoài, chúng ta cần cài đặt các package cần thiết để sử dụng nó trong dự án React của mình:

```bash
npm i swr
```

Trong SWR, nó có sử dụng các hooks cần thiết và build sẵn, thích hợp cho React, việc của chúng ta chỉ là sử dụng nó, tham số đầu vào của `useSWR` gồm có đường dẫn call và `fetcher()`, ngoài ra còn có các options nếu cần thay đổi. Phương thức fetcher là một hàm call API được sử dụng để call, quyết định các tham số truyền vào body, headers,...

Nó thường được build như này:

```js
const fetcher = (...args) => fetch(...args).then((res) => res.json());
export default fetcher;
```

Để sử dụng SWR, chúng ta có thể sử dụng hook useSWR như sau:

```jsx
import useSWR from 'swr';

const fetcher = (...args) => fetch(...args).then((res) => res.json());

const Photos = () => {
	const {
		data: countries,
		error,
		isValidating,
	} = useSWR('https://restcountries.com/v2/all', fetcher, {
		fallbackData: [],
	});

	if (error) return <div className='failed'>failed to load</div>;
	if (isValidating) return <div className='Loading'>Loading...</div>;

	return (
		<div>
			{countries &&
				countries.map((country, index) => (
					<img key={index} src={country.flags.png} alt='flag' width={100} />
				))}
		</div>
	);
};

export default Photos;
```

Ở đây, chúng ta thấy nó đã trả về các biến một cách hợp lý, chỉ việc sử dụng mà không cần xử lý lỗi hay loading,...
