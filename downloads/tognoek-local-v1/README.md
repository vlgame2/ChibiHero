# Tognoek — gói vá thử chế độ cục bộ v1

[Tải gói vá Windows](Tognoek-local-patch-v1.zip?raw=1) — khoảng 150 KB.

1. Đóng `tognoek-sv.exe` đang chạy.
2. Giải nén toàn bộ ZIP vào thư mục thường.
3. Bấm đúp `apply-local.cmd`, chọn `tognoek-sv.exe` trong bộ `release` gốc đã được kiểm tra.
4. Công cụ tạo thư mục `release-local-ngày-giờ` cạnh thư mục gốc và mở thư mục mới.
5. Mở `tognoek-sv.exe` trong thư mục mới, thử một tài khoản trước rồi kiểm tra các chức năng cần dùng. Không cần nhập key cho chế độ thử cục bộ.

Gói vá chỉ nhận EXE có SHA-256 `7b7c467fcb3211b7a288a309874cbaf9ff81b7695fccedc75cbdc49f6e41b3cb`, tạo EXE thử có SHA-256 `c75ee6f9a48e7ab7620df40f05cd64bc7d01caa8a86945d054ffeab8664b09df`. Công cụ sao chép thư mục và vá bản sao; dữ liệu tài khoản đi kèm được sao chép trên máy của bạn.

Quyền chức năng chuyển sang dữ liệu cục bộ, xử lý các chỗ ghi đè từ cache và bỏ luồng cập nhật key trung tâm; các khối Java nhúng giữ nguyên. Gói chỉ chứa mã vá, hướng dẫn và bằng chứng kiểm tra, không chứa EXE/game gốc.

**Bản thử chưa chạy trên Windows/game thật.** Đã đạt 16 kiểm tra mô phỏng cho mã mới tự viết, xác minh PE/ASLR/unwind và đối chiếu tĩnh các điểm đọc/ghi quyền. PowerShell tạo bản sao cũng chưa được chạy trên Windows. Chưa xác nhận đã loại bỏ các chức năng mạng/cập nhật/chat khác của chương trình gốc.

Xem `HUONG-DAN.txt`, `validation.json` trong ZIP và `SHA256SUMS` cạnh gói tải xuống.
