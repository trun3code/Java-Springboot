# Java-Springboot
1. Anotation
- @RequestMapping("/user"): base URL
- @PostMapping("/"): tạo mới tài nguyên
- @PutMapping("/{userId}"): cập nhật toàn bộ
- @PatchMapping("/{userId}"): cập nhật một phần
- //
- @PathVariable: lấy dữ liệu từ URL
- @RequestBody: lấy dữ liệu từ body của request, chuyển từ json thành java
- @RequestParam: lấy dữ liệu từ query string
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
2. Lý thuyết
- enum là 1 kiểu dữ liệu chứa các giá trị cố định
- lombok: giảm bớt mã lặp lại bằng cách cung cấp anotation tự động tạo getter, setter
- JPA là 1 interface
   
