# TEEN YÊU BIỂN ĐẢO - LỊCH 2027 (Kế hoạch L27)

Ứng dụng web tương tác niên lịch 2027 kết hợp giáo dục chủ quyền biển đảo Việt Nam dành cho học sinh và giáo viên THCS.

## Tính năng nổi bật

- **Lịch Tháng & Năm (2026–2027)**: Song hành Dương lịch và Âm lịch (Bính Ngọ – Đinh Mùi), ngày Hoàng Đạo, các ngày lễ lớn và sự kiện lịch sử biển đảo Việt Nam.
- **Ghi chú cá nhân & Kế hoạch dạy học**: Tạo, phân loại (`Soạn giáo án`, `Hoạt động Đội/Đoàn`, `Kiểm tra`, `Sự kiện ngoại khóa`) và lưu tự động trên `localStorage`.
- **Hải Trình Biển Đảo (Bản đồ tương tác)**: 15 tọa độ đảo tiền tiêu, quần đảo Hoàng Sa, Trường Sa, Nhà giàn DK1.
- **EduHub & Đố Vui Biển Đảo**: Chuyên đề dạy học liên môn, thử thách hành động xanh, trắc nghiệm cấp Chứng nhận Danh dự và tính năng viết thư gửi chiến sĩ hải quân.
- **In Lịch Bàn A4 & Âm thanh sóng biển**: Hỗ trợ in từng trang lịch theo tháng và âm thanh sóng biển tổng hợp qua Web Audio API.

## Cài đặt & chạy cục bộ

```bash
npm install
npm run dev
```

## Kiểm tra kiểu & đóng gói production

```bash
npm run lint
npm run build
npm run preview
```

## Triển khai lên GitHub Pages

Repository đã cấu hình sẵn workflow tại `.github/workflows/deploy.yml` và đường dẫn tương đối (`base: './'`) trong `vite.config.ts`:

1. Đẩy mã nguồn lên nhánh `main` trên GitHub.
2. Vào **Settings → Pages** của repository, ở mục **Build and deployment → Source** chọn **GitHub Actions**.
3. Workflow sẽ tự động chạy `npm run lint`, `npm run build` và xuất bản thư mục `dist/` lên GitHub Pages.
