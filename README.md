# Website Công ty TNHH Sâm Tưởng

Website giới thiệu dịch vụ cho thuê xe 4-45 chỗ tại Phường Quảng Thuận, Quảng Trị (Quảng Bình cũ).

---

## 📁 Cấu trúc thư mục

```
sam-tuong-website/
├── index.html              ← File HTML chính (nội dung website)
├── README.md               ← File hướng dẫn này
└── assets/
    ├── css/
    │   └── style.css       ← Toàn bộ style CSS
    └── images/             ← Hình ảnh công ty
        ├── chu-cong-ty.jpg
        ├── xe-transit-doi.jpg
        ├── xe-khach-samco.jpg
        ├── xe-ford-moi.jpg
        ├── xe-mg-moi.jpg
        └── bien-hieu.jpg
```

---

## 🚀 Cách chạy thử website

### Cách 1: Mở trực tiếp
Click đúp vào file `index.html` để mở bằng trình duyệt (Chrome, Firefox, Edge...).

### Cách 2: Dùng Live Server trên VS Code (khuyến nghị)
1. Mở VS Code
2. Mở thư mục dự án (File → Open Folder)
3. Cài extension **"Live Server"** (của Ritwick Dey)
4. Click chuột phải vào `index.html` → chọn **"Open with Live Server"**
5. Website sẽ tự động refresh mỗi khi bạn lưu file

---

## ✏️ Cách chỉnh sửa nội dung phổ biến

### 1. Thay số điện thoại
Mở `index.html`, tìm (Ctrl+F) và thay:
- `0988 201 387` → số hotline chính mới
- `0352 183 557` → số hotline phụ mới
- `0988201387` → số điện thoại trong link `tel:` (không dấu cách)
- `0352183557` → số điện thoại trong link `tel:` (không dấu cách)

### 2. Thay địa chỉ
Tìm `Quảng Thuận` hoặc `QL1A, Phường Quảng Thuận` để cập nhật địa chỉ.

### 3. Thay link Google Maps
Tìm `maps.app.goo.gl/wmAL72KYXcDmA4o99` — thay bằng link Maps mới của bạn.

Nếu muốn thay cả **iframe bản đồ nhúng**, tìm đoạn:
```html
<iframe src="https://www.google.com/maps?q=..."
```
Rồi thay `q=` phía sau bằng địa chỉ mới (thay khoảng trắng bằng `+`).

### 4. Thay ảnh
- Đặt ảnh mới vào thư mục `assets/images/`
- Trong `index.html`, tìm thẻ `<img src="assets/images/TÊN-ẢNH.jpg">` và đổi tên file.
- **Gợi ý**: Giữ ảnh dưới 200KB để trang load nhanh. Có thể dùng [tinypng.com](https://tinypng.com) để nén ảnh.

### 5. Đổi màu chủ đạo
Mở `assets/css/style.css`, tìm đoạn `:root` ở đầu file:
```css
:root {
  --red-brand: #c62828;   /* đỏ thương hiệu */
  --jade-deep: #1a3028;   /* xanh rêu đậm */
  --gold: #d4a04c;        /* vàng ánh kim */
  ...
}
```
Đổi mã màu hex là toàn bộ website sẽ tự đổi theo.

### 6. Thay đánh giá khách hàng
Tìm phần `<section class="test">` trong `index.html`, thay nội dung trong `<p class="test-text">` và tên/vai trò trong `<strong>` và `<small>`.

### 7. Thêm/xóa dịch vụ
Tìm phần `<section class="services"` — copy/sửa các khối `<div class="service-card">`.

---

## 🌐 Cách đưa website lên Internet (deploy)

### Cách dễ nhất: Netlify (miễn phí)
1. Đăng ký tài khoản tại [netlify.com](https://netlify.com)
2. Kéo thả cả thư mục `sam-tuong-website/` vào Netlify
3. Website sẽ có link dạng `sam-tuong.netlify.app` trong 30 giây
4. Mua domain riêng (ví dụ `samtuong.vn`) và trỏ về — xong

### Hoặc: GitHub Pages (miễn phí)
1. Tạo repo GitHub
2. Upload toàn bộ thư mục
3. Vào Settings → Pages → chọn branch `main` → Save
4. Website sẽ online tại `username.github.io/tên-repo`

### Hoặc thuê hosting Việt Nam
Upload file qua FTP lên hosting của bạn (Mắt Bão, Tenten, Nhân Hòa, Vinahost...).

---

## 🔧 Công cụ khuyên dùng

- **VS Code** — editor chính
- **Extension Live Server** — xem preview realtime
- **Extension Prettier** — tự format code gọn đẹp
- **tinypng.com** — nén ảnh trước khi upload
- **realfavicongenerator.net** — tạo favicon (biểu tượng tab trình duyệt)

---

## 📧 Hỗ trợ

Nếu cần chỉnh sửa phức tạp hơn (thêm form liên hệ tự gửi email, tích hợp đặt xe online, thêm trang con...), bạn có thể thuê developer hỗ trợ hoặc quay lại nhờ trợ giúp thêm.

---

**Công ty TNHH Sâm Tưởng** · Thành lập 2008 · Quảng Thuận, Quảng Trị (Quảng Bình cũ)
Hotline: 0988 201 387 · 0352 183 557
