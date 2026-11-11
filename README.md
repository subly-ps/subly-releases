# Subly — ScreenTranslator

Dịch phụ đề game sang tiếng Việt theo thời gian thực, đọc thành giọng nói và dịch cả màn hình.
Hoạt động với **PS5** (qua Remote Play) hoặc bất kỳ cửa sổ nào trên máy Mac. Có app cho **điện thoại** (Android, iPhone/iPad) và máy tính (macOS).

Đây là trang **tải bản cài đặt**. Mã nguồn không công khai.

## Tải về

Vào mục **Releases** (cột bên phải) và tải bản mới nhất cho thiết bị của bạn:

| Thiết bị | File | Ghi chú |
|---|---|---|
| Android | `Subly-android-*.apk` | Cài trực tiếp |
| iPhone / iPad | `Subly-ios-*-unsigned.ipa` | File chưa ký, tự ký bằng Apple ID (Sideloadly/AltStore/ESign) |
| macOS | `Subly-macOS-*.zip` | Kéo vào Applications |

---

## Cài trên điện thoại

### Android (APK)

1. Tải file `Subly-android-*.apk`.
2. Mở file; nếu máy hỏi, bật **Cho phép cài từ nguồn này**.
3. Bấm **Cài đặt** → **Mở**. (Cài đè được lên bản cũ, không cần gỡ.)

### iPhone / iPad (IPA — file chưa ký)

File `.ipa` không ký sẵn, bạn tự ký bằng Apple ID (miễn phí) rồi cài — chọn một cách:

- **Sideloadly** (máy tính, dễ nhất): cắm iPhone, kéo `.ipa` vào, nhập Apple ID → Start. <https://sideloadly.io>
- **AltStore** / **ESign**: cài thẳng trên máy, chọn file `.ipa`.

Apple ID miễn phí dùng được **7 ngày** (hết hạn thì ký lại). Lần đầu mở: **Cài đặt → Cài đặt chung → VPN & Quản lý thiết bị** → tin cậy hồ sơ của bạn.

### Dùng lần đầu (điện thoại)

1. **Thêm máy PX5:** bật Remote Play trên máy, nhập **mã PIN** vào app (chỉ làm một lần).
2. **Chọn game:** từ thư viện game mẫu hoặc nhập tên game.
3. **Key dịch (khuyến nghị):** ⚙ → *AI* → dán **Gemini API key miễn phí** (<https://aistudio.google.com/apikey>). Không có key thì dùng Google dịch.
4. **Kết nối & bắt đầu** để vừa chơi vừa hiện phụ đề, hoặc **Chỉ xem** để đọc lại cốt truyện / phụ đề đã lưu.

---

## Cài trên macOS

1. Giải nén file `.zip`, kéo **Subly.app** vào thư mục **Applications**.
2. Mở **Terminal** (Launchpad → Khác → Terminal), dán lệnh dưới rồi bấm Enter:

   ```sh
   xattr -dr com.apple.quarantine /Applications/Subly.app
   ```

   App ký bằng chứng chỉ riêng, chưa notarize nên macOS chặn với thông báo *"không thể mở"* hoặc *"đã bị hỏng"* — lệnh này gỡ cờ chặn đó. Vẫn không mở được thì chạy `xattr -cr /Applications/Subly.app`.
   Không muốn dùng Terminal: mở app một lần (bị chặn), rồi vào **Cài đặt hệ thống → Quyền riêng tư & Bảo mật**, kéo xuống bấm **Vẫn mở**.
3. Mở Subly. Khi app hỏi quyền **Ghi màn hình**, hãy cho phép, rồi thoát hẳn app và mở lại.
4. Các bản sau app tự cập nhật trong chính app.

## Hỗ trợ

App miễn phí. Cần hỗ trợ cài đặt, liên hệ Telegram **[@subly_ps](https://t.me/subly_ps)** hoặc **@lipnguyen**.
