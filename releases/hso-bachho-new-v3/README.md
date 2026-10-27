# Bạch Hổ New — bản vá V3 thử nghiệm

[Tải bản V3](./BAN_VA_BACH_HO_NEW_V3.zip)

- Thay mục Lậu (vị trí 8) bằng Bạch Hổ New, địa chỉ 103.77.166.204:19129.
- Xóa mục Bạch Hổ New thêm riêng ở vị trí 9; danh sách còn 9 mục, chỉ một Bạch Hổ New.
- Ánh xạ tên/lựa chọn cũ 9 về 8, giữ địa chỉ Bạch Hổ khi đọc cache sảnh hoặc kết nối lại.
- Giữ các thay đổi đi buôn của V2: hồi sinh không thêm khoảng chờ phía tool và nhánh thay thú nhanh.

Đóng tool và các tab game của tool đó, sao chép thư mục tool đích thành bản thử, rồi chép AppManager.exe trong ZIP vào thư mục thử. Không xóa dữ liệu tài khoản. Xem DOC_TRUOC.txt trong ZIP.

Đã tái hiện lỗi chỉ số 9 với cache ngắn trong trình đọc cache V2. Bản sửa đạt 74 kiểm tra Java với giao diện/mạng giả lập và 84 kiểm tra ánh xạ/danh sách .NET bằng trình diễn giải CIL giới hạn; 14 class Java đã kiểm bytecode ASM/JVM. Chưa chạy GUI Windows hoặc đăng nhập server thật. Hãy kiểm tra đăng nhập, quay về sảnh và đăng nhập lần hai trên bản thử.

Đối chiếu SHA-256 bằng SHA256SUMS.txt. Gói không chứa tài khoản/data.db.
