# Java-Springboot
1. Anotation
- @RequestMapping("/user"): base URL
- @PostMapping("/"): tạo mới tài nguyên
- @PutMapping("/{userId}"): cập nhật toàn bộ
- @PatchMapping("/{userId}"): cập nhật một phần
- //
- @PathVariable: lấy dữ liệu từ URL
- @RequestBody: lấy dữ liệu từ body của request, chuyển từ json thành java POST, PUT (vì cần truyền dữ liệu trong body).
- @RequestParam: lấy dữ liệu từ qua URL thay vì body POST, PUT, DELETE
- @Component: class không phải Service, Repository hay Controller.
- @Autowired: tự động inject 1 bean mà không cần từ khóa new
- @Primary: đánh dấu bean ưu tiên
- @Qualifier: chỉ định để inject
- @ComponentScan: chỉ định component cần scan

- @Configuration: chứa các thông tin cấu hình ứng dụng
- @Bean: đánh dấu một method trong class cấu hình( @Configuration)
- @Query: tạo câu truy vấn

- @NotNull: không rỗng, string...
- @NotEmpty: collection không được để trống
- @Pattern: regex validate
- @valid: xác thực, @Valid @RequestBody

- @Operation(...): thuộc Swagger giúp mô tả API
2. Lý thuyết
- enum là 1 kiểu dữ liệu chứa các giá trị cố định
- lombok: giảm bớt mã lặp lại bằng cách cung cấp anotation tự động tạo getter, setter

- ORM: cách tiếp cận ánh xạ từ bảng đến class không cần resultSet của JDBC
- JPA là 1 interface đặc tả của ORM.
- Hibernate là triển khai của JPA, ORM, hiệu suất cao
- so sách hibernate với JDBC
t

- Post: có request body, không @PathVariable
- GET: không request body, có thể có @PathVariable
- PUT: có cả 2
- Delete: có  @PathVariable
- Serializable : class có thể chuyển đổi thành chuỗi byte, thường dùng cho DTO
- có 2 cách kết nối DB: JDBC hoặc framework

- Tight-coupling: liên kết chặt, khi 2 class liên kết chặt với nhau thì sửa class A cũng phải sửa cả class B nữa
- Loose-coupling: ngược lại dùng DI
- DI là 1 phương pháp lập trình giúp giảm sự phụ thuộc giữa các lớp trong java( constructor, setter, interface)
  - VD: tiêm service vào class client bằng constructor injection
  - public Clinent(MessageService messageserviceParam){ this.messageService =messageserviceParam}
  - tiêm sự phụ thuộc vào constructor

- Anotation: chú thích, bổ sung thông tin cho mã nguồn
- @Component: đánh dấu là cần được quản lí bởi spring container, không cần khởi tạo vẫn có thể dùng
- @Autowired: tiêm đối tượng ở bên dưới vào cho class
- Bean: Object được quản lí bởi IOC được gọi là bean
    
