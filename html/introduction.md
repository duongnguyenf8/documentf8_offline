# Introduction

## Lập trình web là gì? Thiết kế web là gì?

Lập trình web:

- **Định nghĩa:** Lập trình web là quá trình tạo ra các trang web hoặc ứng dụng web bằng việc sử dụng các ngôn ngữ lập trình như HTML, CSS và JavaScript.

- **Nhiệm vụ:** Lập trình web giúp xây dựng giao diện và chức năng cho các trang web và ứng dụng web, đảm bảo chúng hoạt động tốt trên các trình duyệt khác nhau.

Thiết kế web:

- **Định nghĩa:** Thiết kế web là quá trình tạo ra giao diện và trải nghiệm người dùng cho các trang web và ứng dụng web.

- **Nhiệm vụ:** Thiết kế web tập trung vào việc sắp xếp các thành phần trên trang, chọn màu sắc, font chữ, hình ảnh và các yếu tố khác để tạo ra trải nghiệm hấp dẫn và thân thiện với người dùng.

## Phương pháp học lập trình hiệu quả

- Xác định mục tiêu học tập (Frontend || Backend || Fullstack)

- Chia nhỏ mục tiêu thành các bước nhỏ hơn (các kỹ năng cần học, các dự án cần thực hiện, v.v.)

- Tìm hiểu cách học phù hợp với bản thân (sách, video học, bài tập thực hành, tham gia dự án, v.v.)

- Tạo lịch trình học tập có cấu trúc và tuân thủ (Học trên lớp, học tại nhà, v.v.)

- Thực hành thường xuyên để củng cố kiến thức

  - Bằng cách thực hành các bài tập có sẵn (Giúp rèn luyện kỹ năng lập trình cơ bản)

  - Bằng cách thực hành các dự án thực tế (Giúp rèn luyện kỹ năng lập trình nâng cao)

  - Bằng cách tự tạo ra các dự án thực tế (Giúp rèn luyện kỹ năng phân tích, thiết kế và triển khai dự án)

- Tìm kiếm và tham gia cộng đồng học tập, nhóm thảo luận để có sự hỗ trợ và cải thiện kỹ năng

  - Không ngại hỏi, ngại khó khăn, không ngại chia sẻ kiến thức

  - Cải thiện kỹ năng research, đọc hiểu tài liệu tiếng Anh

    - Trước khi hỏi người khác, hãy tự tìm hiểu và thử giải quyết vấn đề trước

## Cơ chế hoạt động của website - trình duyệt (Request - Response)

- Định nghĩa:

  - Trình duyệt: Phần mềm được sử dụng để truy cập và hiển thị các trang web.

  - Request: Yêu cầu được gửi từ trình duyệt đến máy chủ web để yêu cầu nội dung của một trang web cụ thể.

  - Response: Phản hồi từ máy chủ web đối với yêu cầu của trình duyệt, chứa dữ liệu và thông tin cần thiết để hiển thị trang web.

- Cơ chế hoạt động:

  - Bước 1: Trình duyệt gửi yêu cầu HTTP đến máy chủ web.

    - Có thể qua một máy chủ DNS trước.

  - Bước 2: Máy chủ web nhận yêu cầu và xử lý nó.

    - Máy chủ DNS sẽ tiếp nhận yêu cầu và xử lý để lấy được địa chỉ IP của máy chủ web.

    - Sau đó trả về trình duyệt địa chỉ IP của máy chủ web để trình duyệt có thể gửi yêu cầu đến máy chủ web.

  - Bước 3: Máy chủ web tạo ra một response HTTP chứa thông tin và dữ liệu của trang web được yêu cầu.

  - Bước 4: Response được gửi từ máy chủ web đến trình duyệt.

  - Bước 5: Trình duyệt nhận response và hiển thị nội dung trang web cho người dùng.

## HTTP Request - Response

- Định nghĩa:

  - HTTP (Hypertext Transfer Protocol): Giao thức truyền tải dữ liệu giữa trình duyệt và máy chủ web.

  - Request: Yêu cầu được gửi từ trình duyệt đến máy chủ web để yêu cầu nội dung của một trang web cụ thể.

  - Response: Phản hồi từ máy chủ web đối với yêu cầu của trình duyệt, chứa dữ liệu và thông tin cần thiết để hiển thị trang web.

- Cấu trúc một HTTP Request:

  - Phương thức Request (GET, POST, PUT, DELETE, v.v.)

  - URL của trang web được yêu cầu

  - Headers (tiêu đề) chứa các thông tin bổ sung như User-Agent, Content-Type, v.v.

  - Body (thân) chứa dữ liệu được gửi kèm theo (chỉ trong một số phương thức như POST)

- Cấu trúc một HTTP Response:

  - Status code (mã trạng thái) để chỉ trạng thái của yêu cầu (200 OK, 404 Not Found, v.v.)

  - Headers (tiêu đề) chứa các thông tin bổ sung như Content-Type, Content-Length, v.v.

  - Body (thân) chứa nội dung của trang web hoặc dữ liệu phản hồi từ máy chủ
