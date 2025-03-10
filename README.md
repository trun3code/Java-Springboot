# Java-Springboot
1. Anotation
- @RequestMapping("/user"): base URL
- @PostMapping("/"): tạo mới tài nguyên
- @PutMapping("/{userId}"): cập nhật toàn bộ
- @PatchMapping("/{userId}"): cập nhật một phần
- //
- @PathVariable: lấy dữ liệu từ URL
- @RequestBody: lấy dữ liệu từ body của request
- @RequestParam: lấy dữ liệu từ query string
- @Component: class không phải Service, Repository hay Controller.
- @Autowired: tự động inject 1 bean mà không cần từ khóa new
- @Primary: đánh dấu bean ưu tiên
- @Qualifier: chỉ định để inject
- @ComponentScan: chỉ định component cần scan

