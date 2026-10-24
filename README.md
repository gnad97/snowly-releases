# Snowly

Công cụ hỗ trợ chơi **ARAM** cho League of Legends trên Windows: tự lấy tướng bạn thích từ bench, tự xin đổi tướng với đồng đội, tự chấp nhận trận, gợi ý Lõi Nâng Cấp, đồng hồ nhà lính và thứ tự nâng kỹ năng ngay trong game, cùng nhiều tiện ích khác.

> Repo này chỉ chứa **bản cài đặt** để tải. Mã nguồn không công khai.

## Tải về

1. Vào trang **[Releases](../../releases/latest)** và tải file **`Snowly_..._x64-setup.exe`**.
2. Chạy file vừa tải để cài (chỉ cần file `.exe`, bỏ qua `latest.json`).
3. Mở **League of Legends**, sau đó mở Snowly. App tự nhận League Client khi bạn đăng nhập.

Windows có thể hiện cảnh báo SmartScreen khi chạy bộ cài lần đầu vì app chưa có chứng chỉ ký số của nhà phát hành. Bấm **Thông tin thêm → Vẫn chạy** nếu bạn tin tưởng nguồn tải.

Lần sau có bản mới, app sẽ tự đề nghị cập nhật, bạn không cần tải lại thủ công.

**Yêu cầu:** Windows 10/11 (cần WebView2, Windows 11 có sẵn), League of Legends đã cài, có kết nối mạng.

## Tính năng chính

### Tự lấy tướng theo Danh Sách Ưu Tiên
Bạn tự xếp danh sách tướng yêu thích (`#1` là ưu tiên nhất) bằng cách kéo thả. Hai tính năng dưới đây phối hợp theo thứ tự **bench trước, trade sau**:
- **Tự Lấy Bench:** tướng ưu tiên cao hơn tướng đang cầm vừa lên bench là app lấy ngay, không bao giờ đổi xuống tướng kém hơn.
- **Tự Trade Đồng Đội:** sau khi lấy được tướng tốt nhất ở bench, nếu đồng đội còn cầm tướng ưu tiên cao hơn thì app xin đổi. Bị từ chối thì không xin lại đúng người và đúng tướng đó. Trong lúc trade, có tướng tốt hơn nhả ra bench thì app lấy bench trước rồi xin trade tiếp nếu đồng đội vẫn còn tướng cao hơn. Bỏ qua người bạn đã đưa vào danh sách chặn trade.
- **Tự trả lời lời xin đổi:** nhận lời đổi sang tướng ưu tiên hơn, từ chối tướng kém hơn (đi cùng Tự Trade).
- **Ưu tiên lấy ở game này:** chuột phải một tướng trên bench hoặc đội hình để ưu tiên nó hơn mọi thứ hạng, chỉ trong ván hiện tại.

### Tự động hoá phòng chờ và cuối trận
- **Auto Chấp Nhận** trận khi tìm được.
- **Auto Start:** tự bấm tìm trận khi bạn là chủ phòng (chọn khi 1 mình hoặc từ 2 người), có ô nhập số giây chờ trước khi bấm. Tự tắt khi có người từ chối hoặc huỷ tìm trận.
- **Auto Skip End Game:** tự bỏ qua màn vinh danh, về lại phòng và đóng popup thông thạo tướng.
- **Auto Flash:** tự đặt Tốc Biến đúng phím D hoặc F theo ý bạn.
- **Auto Import Build:** khi chốt tướng, tự tạo bộ trang bị (Item Set) trong game và đổi sang cặp phép bổ trợ tốt nhất.

### Overlay trong game
Overlay là cửa sổ riêng, trong suốt và không chặn chuột, không can thiệp vào tiến trình game. Cần để game ở chế độ **Borderless** hoặc **Windowed**, tỉ lệ 16:9. Tính năng này do hệ thống bật theo từng thời điểm; nếu chưa được bật, dòng cài đặt sẽ ẩn trong app.
- **Lõi Nâng Cấp (ARAM: Hỗn Loạn):** hiện khiên bậc S…D ngay trên từng thẻ lõi khi bạn chọn lõi (lõi ngoài gợi ý của tướng hiện dấu "?").
- **Đồng hồ nhà lính:** đếm ngược thời gian hồi sinh nhà lính ngay trên minimap.
- **Gợi ý nâng kỹ năng:** mũi tên và viền vàng trên nút nâng kỹ năng theo thứ tự gợi ý của tướng.

### Giao diện chọn tướng và phòng chờ
- Bench 10 ô bấm để swap, thẻ bài tướng đầu ván, đội hình 5 người với phép bổ trợ, thứ hạng ưu tiên và trạng thái trade.
- **Bảng Lõi Nâng Cấp** của tướng đang cầm, chia theo độ hiếm kèm bậc.
- Splash theo skin đang chọn, dải trang phục chỉ gồm skin bạn sở hữu.
- Phòng chờ: mời bạn bè (có thể kéo thả), đổi mode ARAM, tìm trận, Ready Check.
- **Thống kê ván đấu** lưu ngay trên máy: số ván cầm được tướng ưu tiên, số ván đổi nhờ bench / trade, thời gian chờ trận.

### Tài khoản, thông báo và khay hệ thống
- Setting, Danh Sách Ưu Tiên và danh sách chặn trade được lưu theo tài khoản LoL trên máy chủ. Đổi máy, đăng nhập lại là có đủ. Các công tắc có tác dụng ngay khi bật hoặc tắt.
- **Thông báo trong app:** chuông trên thanh điều hướng, đánh dấu đã đọc, sao chép nhanh key và mã giao dịch.
- **Khay hệ thống:** đóng cửa sổ chỉ thu xuống khay, bật tắt nhanh các tính năng tự động từ menu khay.
- Khi hệ thống bảo trì, app hiện màn "Đang bảo trì" kèm khung giờ và tự vào lại khi xong.

## Bản Free và bản có key

Tất cả tính năng dùng được ở mọi gói. Khác biệt chính là **độ trễ khi giành tướng** (lấy bench / xin đổi): gói cao hơn lấy nhanh hơn, và chức năng **chặn trade với người chơi** chỉ dành cho một số gói. Thời gian cụ thể và danh sách gói do hệ thống quy định, hiển thị ngay trong app.

Nhập key ở card **Bản Quyền** trong tab **Cài Đặt**. Mỗi key gắn với một tài khoản LoL, có thể có hạn theo ngày hoặc vĩnh viễn. Muốn mua hoặc gia hạn key, chọn gói trong app rồi thanh toán bằng mã QR chuyển khoản; key tự cập nhật sau khi thanh toán thành công. Key hết hạn hoặc bị vô hiệu hoá thì app chạy như bản Free.

## Dữ liệu và quyền riêng tư

- App giao tiếp với League Client qua API nội bộ trên máy bạn và chỉ hoạt động khi client đang mở. Trong trận, app chỉ đọc dữ liệu trận và chụp màn hình để vẽ overlay, không inject, không đọc bộ nhớ game và không tự bấm phím.
- Để đăng nhập, app lấy mã xác thực (ID token) từ League Client và gửi lên máy chủ, máy chủ tự xác minh danh tính. Ngoài ra app đồng bộ phiên bản app, setting, Danh Sách Ưu Tiên và danh sách chặn trade. App không đọc hay gửi mật khẩu Riot của bạn.
- App cần kết nối mạng để dùng. Mất kết nối máy chủ thì các tính năng tự động tạm dừng cho tới khi kết nối lại.

## Lưu ý

Snowly là sản phẩm độc lập, **không được Riot Games xác nhận hay bảo trợ** và không liên kết với Riot Games. League of Legends là thương hiệu của Riot Games, Inc. Công cụ sử dụng API nội bộ của League Client, hãy tự cân nhắc khi sử dụng. Quản trị viên có thể chặn tài khoản hoặc tạm khoá app khi cần.

## Hỗ trợ

Mọi chi tiết và hỗ trợ liên hệ: **gnad.dev97@gmail.com**

© DangTH. Vui lòng không sao chép dưới mọi hình thức.
