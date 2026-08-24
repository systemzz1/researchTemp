# 🌾 Sản lượng cây trồng miền Bắc 2024

Trực quan hóa dữ liệu sản lượng và xuất khẩu cây trồng của 24 tỉnh miền Bắc Việt Nam năm 2024.

## Mục đích

Đây là bài research mình làm cho bạn gái, tổng hợp số liệu về sản lượng các giống cây chủ đạo ở miền Bắc — chia làm cây hàng năm (lúa, ngô, sắn) và cây lâu năm (trà, cà phê, cam, bưởi, vải, nhãn, xoài...). Dữ liệu được hiển thị dưới dạng biểu đồ tròn (pie chart) kèm số liệu xuất khẩu.

## Điểm đặc biệt

Toàn bộ ứng dụng chỉ nằm trong **1 file HTML duy nhất** — `chart_standalone.html`. Người không biết lập trình vẫn có thể mở được chỉ bằng cách **click đôi vào file**, không cần cài đặt hay chạy server gì thêm.

## Cách sử dụng

1. Clone repo hoặc tải file `chart_standalone.html`
2. Click đôi vào file để mở trên trình duyệt
3. Chọn tỉnh ở dropdown
4. Chọn tab: Tất cả / Cây hàng năm / Cây lâu năm / Xuất khẩu / Tổng quan XK

## Dữ liệu

- **Sản lượng**: Viện Môi trường Nông nghiệp (Viện MTNN) + Niên giám tỉnh 2024
- **Xuất khẩu**: GSO, Hải quan, MARD, báo cáo tỉnh — chỉ các dữ liệu đã được xác minh, không tự tạo số liệu
- **Phạm vi**: 24 tỉnh miền Bắc, 33 loại cây

## File

| File | Mô tả |
|------|-------|
| `chart_standalone.html` | File chính — mở bằng trình duyệt, hoạt động offline |
| `pie_chart_data_2024.json` | Dữ liệu sản lượng (62 KB) |
| `export_data_2024.json` | Dữ liệu xuất khẩu (253 KB) |
| `metadata.md` | Nguồn dữ liệu & phương pháp |
