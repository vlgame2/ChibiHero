# HSO Manager phục hồi 0.2 — bản Windows

[Tải gói Windows](HSO-Manager-Windows-v0.2.zip?raw=1). Nếu đang xem tệp ZIP trên GitHub, chọn **Download raw file**.

Giải nén toàn bộ vào thư mục mới, rồi chạy `ChibiHero.Manager.exe`. Giữ các DLL và thư mục `engine` đi kèm. Không cần tải mã nguồn để chạy.

Đóng manager gốc trước khi bấm MỞ GAME vì game dùng cổng TCP 8888. Trong Nguồn game, có thể chọn JAR hợp lệ có sẵn hoặc tải bằng key hợp lệ của bạn; chế độ tải cần chọn `HsoManager.exe` gốc chưa sửa. Cần Java 8. Đọc `HUONG-DAN.txt` trong gói để thực hiện. Không gửi key/mật khẩu cho người khác.

Đã phục hồi quản lý tài khoản, cấu hình HSO, kênh TCP và luồng tải game. Đã loại LHT. 126 kiểm tra tự động/fixture đạt trên Linux; bản Windows đã build nhưng chưa được thử đăng nhập game thật. Hiệu quả auto và chiến trường HSO còn cần xác minh; đây chưa phải bản phục hồi hoàn chỉnh 100% hoặc bản không cần key.

`SHA256SUMS` ghi checksum của gói. Nhánh tải xuống này chỉ thêm gói Windows và hướng dẫn; nhánh main và các tệp phát triển không thay đổi.
