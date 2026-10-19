# Thực hành phối màu Newsletter Trello với Adobe Color

Đồ án mẫu cho bài CodeGym: **2 phiên bản newsletter có cùng nội dung / bố cục Bootstrap nhưng sử dụng 2 bảng màu khác nhau**.

## Cấu trúc thư mục

```text
trello_newsletter_adobe_color/
├── index.html                  # Trang so sánh hai phiên bản
├── newsletter_version1.html    # Xanh dương – xanh ngọc (tương đồng)
├── newsletter_version2.html    # Cam đất – xanh teal (bổ túc)
├── newsletter.css              # Các lớp CSS dùng chung
├── preview_newsletter_version1.png        # Ảnh xem trước bản 1 (nếu có)
├── preview_newsletter_version2.png        # Ảnh xem trước bản 2 (nếu có)
├── preview_index.png           # Ảnh trang so sánh
└── README.md                   # Hướng dẫn
```

## Bảng màu

### Phiên bản 1 — Tương đồng (Analogous)

| Vai trò | Mã HEX | Mô tả |
|---|---|---|
| Primary | `#164BA3` | Xanh dương đậm: hero, CTA, tiêu đề nhỏ |
| Secondary | `#137EA8` | Xanh cyan: dải gradient và thanh tiến độ |
| Accent | `#008C88` | Xanh ngọc: màu nhấn |
| Soft background | `#EDF7FF` | Nền xanh rất nhạt |
| Heading | `#15314F` | Chữ tiêu đề dễ đọc |

Cảm nhận: **tin cậy, hiện đại, tập trung**.

### Phiên bản 2 — Bổ túc (Complementary)

| Vai trò | Mã HEX | Mô tả |
|---|---|---|
| Primary | `#A94C2F` | Cam đất: màu chủ đạo |
| Secondary | `#16636A` | Teal: màu đối lập gần bổ túc với cam đất |
| Accent | `#E4A85B` | Vàng cam: điểm nhấn |
| Soft background | `#FFF6EC` | Nền kem ấm |
| Heading | `#2D3D3C` | Chữ xám xanh đậm |

Cảm nhận: **ấm áp, sáng tạo, gần gũi**.

Nguyên lý phối màu tham khảo từ [Adobe Color](https://color.adobe.com/create/color-wheel): quy tắc Analogous và Complementary. Các giá trị HEX trong bài là **bộ màu tự xây dựng theo các quy tắc này**, không phải một chủ đề đã lưu trong tài khoản Adobe Color.

## Cách chạy bài

1. Giải nén toàn bộ thư mục (nếu tải dạng ZIP).
2. Mở `index.html` bằng Google Chrome, Edge hoặc trình duyệt khác.
3. Chọn **Xem phiên bản 1** hoặc **Xem phiên bản 2**.
4. Có thể mở trực tiếp cả hai file `newsletter_version*.html` để so sánh.

Dùng **Bootstrap 5.3.3 qua CDN** cho hệ thống grid / utility. File `newsletter.css` có các thiết lập responsive dự phòng, vì vậy ngay cả khi không có mạng trang vẫn có bố cục và màu sắc cơ bản.

## Các thành phần đáp ứng yêu cầu

- Header có logo chữ Trello minh họa bằng CSS và tiêu đề bản tin.
- Có hero, nội dung giới thiệu, các thẻ thông tin (card), nút CTA, hướng dẫn 3 bước và footer.
- Sử dụng Bootstrap (`container`, `row`, `col-md-4`, `col-lg-6`, `h-100`, `d-flex`...) và CSS responsive.
- 2 file HTML chỉ khác phần khai báo biến màu; nội dung / bố cục thống nhất để so sánh.
- Màu CSS quản lý bằng biến `:root` trong `<style>` của từng trang.
- Tương phản chữ trên nền được chọn theo hướng dễ đọc; có nhãn / ngữ nghĩa HTML.
- Nút **Khám phá mẹo mới** cuộn đến nội dung; **Khám phá Trello** mở trang Trello.
- Không cần file ảnh ngoài: minh họa bảng công việc bằng HTML/CSS.

## Cách nộp bằng GitHub (không cần dùng dòng lệnh)

1. Truy cập https://github.com/new, tạo repository tên `trello-newsletter-adobe-color`, chọn **Public**.
2. Trong repository, nhấn **Add file → Upload files**.
3. Chọn **các file bên trong thư mục bài làm** (`index.html`, `newsletter.css`, `newsletter_version1.html`, `newsletter_version2.html`, `README.md` và ảnh xem trước nếu có), không cần upload `.zip`.
4. Nhấn **Commit changes**. Sao chép link repository dạng `https://github.com/TEN_TAI_KHOAN/trello-newsletter-adobe-color` và dán vào bài nộp.
5. (Tùy chọn) **Settings → Pages → Build and deployment → Deploy from a branch**, Branch **main** / **root**, sau đó sử dụng link trang chạy trực tiếp dạng `https://TEN_TAI_KHOAN.github.io/trello-newsletter-adobe-color/`.

**Ghi chú:** Mẫu được tự thiết kế dựa trên mô tả đề và hình dung giao diện Trello, không sử dụng newsletter gốc vì đề chưa cung cấp file offline. Nội dung là bản demo học tập, không phải bản tin chính thức của Trello.
