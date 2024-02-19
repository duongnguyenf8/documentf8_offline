## Module 9: NodeJS + ExpressJS

### Kiến thức NodeJS nền tảng

- Tổng quan về lập trình Back-end, cách back-end hoạt động
- Tổng quan về NodeJS
- Xây dựng ứng dụng NodeJS đầu tiên
- Sử dụng CommonJS và ES Module
- Xuất nội dung HTML, Json
- Đọc nội dung file HTML
- Sử dụng Nodemon
- Xử lý Routing trong NodeJS
- Http Get
- Http Post
- Xử lý form trong NodeJS
- Validate Form với NodeJS
- Upload File với NodeJS
- Session trong NodeJS
- Cookie trong NodeJS

### ExpressJS Framework

#### Kiến thức căn bản

- Tổng quan về ExpressJS Framework
- Cài đặt Express Generator
- Các thành phần của ExpressJS
- Cấu trúc Folder của Express Generator
- Tìm hiểu Lifecycle Request
- Middleware ExpressJS: Global Middleware, Routing Middleware
- Tự xây dựng Middleware ExpressJS
- Routing ExpressJS và các kỹ thuật xử lý
- Request và Response trong ExpressJS
- Render giao diện trong ExpressJS
- Xây dựng trang Error

#### Mô hình MVC

- Tổng quan về mô hình MVC
- Làm việc với Controller (C)

* Cách xây dựng Controller
* Cách tổ chức Action
* Phân chia nhóm Controller

- Làm việc với View (V)

* Phân chia view hiệu quả
* Gửi và nhận dữ liệu từ Controller sang View
* Cú pháp trong Template Engine Ejs
* Giới thiệu Master Layout Ejs
* Xây dựng giao diện theo Master Layout

- Làm việc với Model (M)

* Tư duy xây dựng Model đúng
* Demo xây dựng Controller - Model - View với dữ liệu Fake

### Cơ sở dữ liệu (MySQL)

- Tổng quan về CSDL và các loại CSDL
- Phần mềm và công cụ cần chuẩn bị
- Kiến thức SQL - Thao tác với Database
- Kiến thức SQL - Các kiểu dữ liệu trong SQL
- Kiến thức SQL - Tạo bảng
- Kiến thức SQL - Thêm, sửa, xóa dữ liệu
- Kiến thức SQl - Thiết lập các ràng buộc
- Kiến thức SQL - Truy vấn dữ liệu
- Kiến thức SQl - Join Table
- Kiến thức SQL - SubQuery
- Kiến thức SQL - Import và Export Database
- Thiết kế Database bằng công cụ: phpmyadmin, navicat,...
- Thực hành: Xây dựng Database Web bán hàng

### Thao tác NodeJS với MySQL

- Xây dựng file config để lưu các cấu hình
- Tìm hiểu về file .env và cách sử dụng
- Tìm hiểu về sequelize và sequelize-cli
- Kết nối Database với Sequelize ORM
- Tạo Model với Sequelize và các kỹ thuật
- Thao tác với cấu trúc bảng sử dụng Sequelize
- Migrate thông qua sequelize-cli
- Các kỹ thuật khi thao tác với Migrate
- Tư duy xây dựng Migrate hiệu quả để làm việc team
- Sequelize Relationship: HasOne, BelongsTo, HasMany, BelongsToMany
- Các thao tác với dữ liệu: thêm, sửa, xóa, truy vấn
- Các kỹ thuật nâng cao khi thao tác với dữ liệu trong Sequelize

### Mail trong NodeJS (nodemailer)

- Tìm hiểu các tình huống với email trong NodeJS
- Tìm hiểu package nodemailer
- Tìm hiểu SMTP, cách lấy thông tin SMTP của gmail
- Thiết lập cấu hình SMTP trong file config
- Thao tác gửi email với nodemailer
- Thao tác với Template Email
- Làm việc với Notication Email với package có sẵn

### Authentication với NodeJS

- Tìm hiểu Passport.js
- Cấu hình sử dụng Passport.js
- Xây dựng chức năng Login sử dụng Passport.js
- Tìm hiểu các Middleware trong Passport.js
- Xây dựng chức năng đăng xuất
- Kiểm tra trạng thái đăng nhập
- Tích hợp đăng nhập mạng xã hội
- Thực hành xây dựng ứng dụng Authentication hoàn chỉnh

### Phân quyền người dùng trong NodeJS

- Tổng quan về phân quyền người dùng
- Mối quan hệ giữa phân quyền và xác thực người dùng
- Tìm hiểu về Access Control List(ACL)
- Tìm hiểu về mô hình Role Based Access Control(RBAC)
- Phân quyền vai trò với package node_acl
- Xây dựng Middleware cho các Route
- Tư duy phân tích Database phân quyền động
- Thực hành xây dựng ứng dụng phân quyền hoàn chỉnh

### Xử lý hàng đợi (Queue) trong NodeJS

- Tổng quan về Queue và các tình huồng cần sử dụng Queue
- Tìm hiểu về Kue và các tính năng
- Cài đặt Redis và Kue
- Tạo worker job
- Quản lý các jobs
- Thực hành xây dựng chức năng gửi email hàng loạt sử dụng Queue
- Xử lý job scheduling, cronjob trong NodeJS

### Cache trong NodeJS

- Tìm hiểu về Redis
- Cách sử dụng Redis trong thực tế
- Cache dữ liệu với Redis trong NodeJS

### RESTFul API với NodeJS

- Tổng quan về API và Restful API
- Các nguyên tắc khi thiết kế RestFul API
- Xây dựng RESTFul API hoàn chỉnh với tình huống thực tế
- Tìm hiểu về CORS
- Passing CORS khi sử dụng API cho Client

### RESTFul API Authentication và Authorization với NodeJS

- Tìm hiểu về cookie-based authentication vs token-based authentication
- Tại sao nên dùng Token-based?
- Tìm hiểu JWT, cách JWT hoạt động
- Tại sao phải quản lý expire trong accessToken
- Sự khác nhau của accessToken và refreshToken
- Đặt expire accessToken và refreshToken như thế nào là hợp lý?
- Xác thực API với Authorization Bearer
- Xây dựng Authentication - Authorization API hoàn chỉnh

### OAuth 2.0 trong NodeJS

- Tìm hiểu về OAuth 2.0 Server và tình huống trên thực tế
- Tìm hiểu về node-oauth2-server
- Xây dựng CSDL cho OAuth
- Xây dựng Route và OAuth 2.0 service
- Xây dựng ứng dụng thực tế sử dụng OAuth 2.0

### MVCS Architecture - Repository Pattern

- Tìm hiểu về kiến trúc MVCS
- Cách triển khai kiến trúc MVCS trong thực tế
- Nâng cấp mô hình MVC lên MVCS
- Tìm hiểu về Repository Pattern và tình huống trong thực tế

### Bảo mật và các hình thức tấn công

- XSS
- SQL Injection
- CSRF
- HTML Injection
- File Upload Attack
- .env attack
