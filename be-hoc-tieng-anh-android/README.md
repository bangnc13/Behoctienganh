# Bé Học Nói Tiếng Anh (app Android)

Bé xem hình, nghe đọc mẫu, đọc lại và được chấm 1-3 sao.
Giao diện là web (thư mục `www`), đóng gói thành app Android bằng Capacitor.
GitHub Actions tự build ra file APK, không cần cài Android Studio.

## Build APK trên điện thoại hoặc máy tính
1. Tạo repo mới trên GitHub (ví dụ `be-hoc-tieng-anh`).
2. Tải toàn bộ file trong thư mục này lên repo (giữ nguyên cấu trúc, nhớ có thư mục `.github/workflows`).
3. Vào tab **Actions**, chọn workflow **Build APK**, bấm **Run workflow**. Chờ khoảng 5-8 phút.
4. Mở lần chạy xong, kéo xuống mục **Artifacts**, tải `be-hoc-tieng-anh-apk` (file zip), giải nén ra `app-debug.apk`.
5. Chép APK vào điện thoại, mở file, cho phép "cài từ nguồn không xác định", cài đặt.
6. Mở app, bấm Nói lần đầu sẽ hỏi quyền micro, chọn Cho phép.

## Sửa nội dung
Sửa danh sách `WORDS` trong `www/index.html` (từ, nghĩa tiếng Việt, emoji), commit lên GitHub là Actions build lại bản mới.

## Lưu ý
- APK này là bản debug, đủ để dùng cá nhân. Muốn đưa lên Google Play cần ký bản release.
- Nhận giọng nói dùng dịch vụ của Google trên máy (cần cài Google app, có thể cần mạng tùy máy).
- Nếu build lỗi, mở log của bước bị đỏ và gửi cho mình.
