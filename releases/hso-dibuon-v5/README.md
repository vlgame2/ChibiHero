# Đi buôn V5 — khôi phục dắt thú, lại cạnh thú bị stun, thay thú lúc chết

> **TẠM NGỪNG SỬ DỤNG V5 — CHƯA XÁC MINH AN TOÀN.** Người dùng báo Windows Defender phát hiện `AppManager.exe` trong ZIP là `Trojan:Win32/Wacatac.H!ml`, trạng thái xử lý chưa hoàn tất. Chưa xác định đây là báo nhầm hay mã độc thực sự. Không tắt bảo vệ, thêm ngoại lệ, Allow/Restore hoặc ép chạy để dùng bản này.
>
> Các kiểm tra chức năng/bytecode và SHA-256 bên dưới không phải chứng nhận sạch mã độc. Mẫu tải từ GitHub khớp gói đã đóng; bản thực thi gốc bị làm rối mã chưa được kiểm tra toàn bộ. Chưa có kết quả quét Defender độc lập để gỡ cảnh báo. Bản V5 này không được khuyến nghị sử dụng trong lúc chờ đánh giá.

Gói V5 được giữ để đối chiếu; không khuyến nghị tải hoặc chạy.

- Bỏ phần giới hạn/cắt đường đi mới của V4 đối với thú khỏe, khôi phục cách dắt thú bình thường vốn có. Đã tái hiện lỗi V4 xóa đoạn đang đi do hiểu sai chỉ số đường.
- Chỉ khi thú bị **trói, choáng, ru ngủ hoặc đóng băng**, nhân vật còn sống mới đi bộ lại sát cạnh (khoảng 1 ô). Nhánh thay thú ít máu đợi tới cạnh rồi mới gửi yêu cầu. Khi hết toàn bộ hiệu ứng thì kéo tiếp.
- Khi nhân vật chết, nhánh đi buôn vẫn gửi yêu cầu thay/thả thú qua menu đã học, dùng ngưỡng HP thay thú đã đặt. Chuỗi thay đang làm có thể hoàn thành sau khi nhân vật sống lại; không tự thả thú chỉ vì đang chết và chưa thấy thú.
- **Delay hồi sinh = 1:** gửi yêu cầu tại chỗ ngay trong nhịp phát hiện chết, trước thay thú và ghi nhật ký. Mức 2–15 giữ số giây. Mức 1 thử lại tối đa 4 lần/giây. Game xử lý ngọc/vật phẩm hồi sinh.
- Giữ Bạch Hổ New, core, Farm, launcher và các phương thức .NET từ bản trước. Không xóa dữ liệu tài khoản.

**Cài:** đóng tool và toàn bộ tab game của tool đó. Sao chép thư mục tool đầy đủ thành bản thử, chép `AppManager.exe` trong ZIP vào đó rồi mở. Vào Buôn, đặt Delay hồi sinh = 1 và bấm Áp dụng lại. Giữ bản cũ để quay lại; xem `DOC_TRUOC.txt` trong ZIP.

Nhánh thay thú nhanh vẫn cần một lần xác nhận/thả thú bình thường mỗi phiên để học menu hợp lệ. Không giả trạng thái còn sống hay xóa hiệu ứng. Server có thể từ chối thay thú khi nhân vật còn chết, và có thể trì hoãn hồi sinh.

Đã chạy 662 xác nhận với nhánh update và bộ ghi gói thật, giả lập đồng hồ/giao diện/đường đi/vận chuyển mạng; có ca tái hiện lỗi V4, kiểm tra lại cạnh trước thay, yêu cầu thay/thả khi chết, và mô hình nhân vật đi/bò theo qua 300 khung hình. Launcher gốc kiểm đủ 14 bundle, nạp class mới và chạy bộ đọc delay sau xử lý class.

**Chưa chạy GUI Windows hoặc thử trên server thật.** Gói có mã bản vá và log kiểm tra. Nhật ký bản mới là `trade-v5-diagnostic.log`, không ghi tài khoản/mật khẩu. Đối chiếu SHA-256 trong `SHA256SUMS.txt`; gói không chứa data.db.
