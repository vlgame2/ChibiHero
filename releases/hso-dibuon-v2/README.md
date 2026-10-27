# Bản vá đi buôn V2 — thử nghiệm

[Tải bản vá ZIP](./BAN_VA_DI_BUON_HOI_SINH_0S_V2.zip)

Dùng với bản Tool_HSO_Bach_Ho_New_FIX_CLR_DAY_DU đã cung cấp.

- Hồi sinh đi buôn: bỏ khoảng chờ cấu hình và độ trễ ngẫu nhiên ở mọi yêu cầu, gồm lần đầu mỗi lần chết và các lần thử lại, cho cả luồng cũ và V3.
- Thay thú nhanh theo nhánh đã phân tích từ bản tham chiếu; cần một lần xác nhận/thả thú bình thường trong phiên để học menu. Hỗ trợ lựa chọn lừa, lạc đà, bò đang có.

Đóng tool đích và các tab game của tool đó, sao chép thư mục tool đích thành bản thử, rồi chép AppManager.exe trong ZIP vào thư mục thử. Xem DOC_TRUOC.txt trong ZIP.

Đã kiểm tra bytecode ASM/JVM, 120 tình huống thời gian trên biểu thức bytecode, 5 giá trị cấu hình và 34 kiểm tra mô phỏng thay thú. Chưa chạy GUI Windows hoặc xác nhận trên server game thật. Thời gian mạng và server xử lý không được bảo đảm bằng 0.

Đối chiếu SHA-256 gói tải bằng SHA256SUMS.txt. Mã bản vá và kết quả kiểm tra có trong ZIP; gói không chứa tài khoản/data.db.
