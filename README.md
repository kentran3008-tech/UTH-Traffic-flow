# 🛵 UTH Traffic & Map

Cộng đồng sinh viên **UTH** chia sẻ tình trạng giao thông – *né kẹt xe thông minh!*

Ứng dụng web một trang (single-page) giúp sinh viên và giảng viên cập nhật các điểm nóng giao thông khu vực **Bình Thạnh** và quanh **cổng trường UTH (số 2 Võ Oanh)**.

## ✨ Tính năng

- 🏠 **Trang chủ** – cảnh báo giờ tan tầm, thống kê nhanh, các điểm nóng quanh cổng trường và lưu ý an toàn.
- 🛰️ **Bản đồ vệ tinh** – bản đồ tương tác (Leaflet + ảnh vệ tinh Esri), lọc theo mức độ kẹt xe, định vị GPS của bạn, nhảy nhanh về UTH.
- 💬 **Diễn đàn** – danh sách báo cáo từ cộng đồng, thả tim, xem vị trí trên bản đồ.
- 📍 **Báo cáo** – gửi thông tin giao thông mới, chọn vị trí trực tiếp trên bản đồ.
- 📱 Giao diện tối ưu cho điện thoại (cảm ứng).

## 🚀 Chạy thử

Không cần cài đặt hay build. Chỉ cần:

```bash
git clone https://github.com/<ten-cua-ban>/uth-traffic-map.git
cd uth-traffic-map
# mở trực tiếp index.html bằng trình duyệt, hoặc chạy server cục bộ:
python3 -m http.server 8000
# rồi vào http://localhost:8000
```

> Lưu ý: tính năng định vị GPS cần chạy qua `https://` hoặc `localhost`.

## 🌐 Đăng lên GitHub Pages

1. Vào **Settings → Pages** của repo.
2. Ở **Build and deployment**, chọn **Deploy from a branch**.
3. Chọn nhánh `main` và thư mục `/ (root)` rồi bấm **Save**.
4. Sau ~1 phút, trang chạy tại `https://<ten-cua-ban>.github.io/uth-traffic-map/`.

## 🧰 Công nghệ

- HTML, CSS, JavaScript thuần (không framework)
- [Leaflet 1.9.4](https://leafletjs.com/) – bản đồ tương tác
- [Esri World Imagery](https://www.arcgis.com/) – lớp ảnh vệ tinh

## 📁 Cấu trúc

```
uth-traffic-map/
├── index.html   # toàn bộ giao diện + logic
├── README.md
├── LICENSE
└── .gitignore
```

## ⚠️ Ghi chú

Dữ liệu báo cáo hiện là **dữ liệu mẫu lưu trong bộ nhớ trình duyệt** (mất khi tải lại trang). Để lưu lâu dài và chia sẻ giữa nhiều người dùng, cần gắn thêm backend/cơ sở dữ liệu (ví dụ Firebase hoặc Supabase).

## 📄 Giấy phép

[MIT](LICENSE)
