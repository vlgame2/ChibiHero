# Đi buôn V4 — hồi sinh tại chỗ, kéo thú gần và chờ hết stun

[Tải bản V4 thử nghiệm](./BAN_VA_DI_BUON_V4_STUN_2_O.zip)

- **Delay hồi sinh = 1:** gửi yêu cầu hồi sinh tại chỗ ngay trong nhịp phát hiện chết, mỗi lần chết. Mức 2–15 giữ đúng số giây. Dùng lại yêu cầu tại chỗ có sẵn trong bản đích/tham chiếu; không thêm nhánh dùng vàng. Game xử lý ngọc/vật phẩm hồi sinh.
- Nhánh đi buôn xử lý chết trước các chỗ có thể thoát sớm do thiếu thú/hàng hoặc chờ công thức V3. Không phụ thuộc tùy chọn hồi sinh Farm. Mức 1 thử lại tối đa 4 lần/giây nếu vẫn chưa sống.
- Kéo thú trong khoảng **2 ô**; dừng chờ hoặc đi bộ lại gần nếu thú tụt lại. Cắt đường đi đã xếp sẵn khi vượt phạm vi.
- Khi thú bị **trói, choáng, ru ngủ, đóng băng**, nhân vật đi lại cạnh rồi đứng chờ. Chỉ kéo tiếp khi hết mọi hiệu ứng đang chồng. Dùng cờ hiệu ứng chặn di chuyển của game, không suy đoán từ việc đứng yên.
- Giữ thay thú nhanh và sửa máy chủ Bạch Hổ New của V3. Chỉ đổi JAR đi buôn; JAR Farm, core V3, các method .NET và launcher giữ nguyên.

**Cài:** đóng tool và các tab game của tool đó. Sao chép thư mục tool đầy đủ sang thư mục thử, chép `AppManager.exe` trong ZIP vào đó rồi mở. Vào Buôn, đặt Delay hồi sinh = 1 và bấm Áp dụng lại. Giữ bản cũ để quay lại; xem `DOC_TRUOC.txt` trong ZIP.

Đã kiểm tra nhánh update đi buôn đến bộ ghi gói thật bằng giao diện/đồng hồ/đường đi/vận chuyển mạng giả lập: 626 xác nhận gồm nhiều lần chết, thời gian 1–15, hiệu ứng chồng và đường đi dài. Launcher gốc đã kiểm đủ 14 bundle, nạp các class của bản vá và chạy bộ đọc delay sau bước xử lý class. Gói chứa mã bản vá, báo cáo và nhật ký kiểm tra.

**Chưa chạy GUI Windows hoặc thử trên server thật.** Gửi yêu cầu ngay không bảo đảm server cho đứng dậy tức thì. Nếu vẫn chờ khoảng 5 giây, dùng `trade-v4-diagnostic.log` tại thư mục làm việc của game để đối chiếu thời điểm phát hiện chết, gửi yêu cầu và nhận trạng thái sống. Nhật ký không ghi tài khoản/mật khẩu.

Đối chiếu SHA-256 bằng `SHA256SUMS.txt`. Gói không chứa dữ liệu tài khoản/data.db.
