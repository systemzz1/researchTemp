# Metadata: Dữ liệu sản lượng cây trồng 24 tỉnh miền Bắc năm 2024

## Tổng quan
- **Tên bộ dữ liệu**: Sản lượng cây trồng các tỉnh miền Bắc năm 2024
- **Phạm vi**: 24 tỉnh/thành phố miền Bắc (theo hành chính cũ)
- **Năm dữ liệu**: 2024 (số sơ bộ)
- **Ngày truy xuất**: 2025-08-24
- **Đơn vị**: Nghìn tấn (kton)

## Danh sách 24 tỉnh
1. Hà Nội
2. Vĩnh Phúc
3. Bắc Ninh
4. Bắc Giang
5. Hưng Yên
6. Hải Dương
7. Thái Bình
8. Hà Nam
9. Nam Định
10. Ninh Bình
11. Lào Cai
12. Yên Bái
13. Điện Biên
14. Lai Châu
15. Sơn La
16. Hòa Bình
17. Thái Nguyên
18. Phú Thọ
19. Tuyên Quang
20. Cao Bằng
21. Bắc Kạn
22. Lạng Sơn
23. Hà Giang
24. Quảng Ninh

---

## Nguồn dữ liệu chính (Annual crops - Cây hàng năm)

### 1. Viện Môi trường Nông nghiệp (MTNN)
- **URL**: https://mtnongnghiep.com/index.php/du-lieu-trong-trot/
- **Bảng**: "Dữ liệu lĩnh vực trồng trọt 2024" (wpDataTable ID 34)
- **Phạm vi**: 63 tỉnh, năm 2017-2024
- **Các chỉ tiêu**: 
  - Lúa: Diện tích, năng suất, sản lượng (cả năm + chia vụ: Đông-Xuân, Hè-Thu, Mùa)
  - Ngô: Diện tích, năng suất, sản lượng
  - Sắn: Diện tích, năng suất, sản lượng
- **Đơn vị**: Diện tích (nghìn ha), Năng suất (tạ/ha), Sản lượng (nghìn tấn)
- **Tính chất**: Số liệu sơ bộ năm 2024

### Cột dữ liệu sử dụng (từ bảng HTML):
| Cột | Chỉ tiêu | Vị trí trong bảng |
|-----|----------|-------------------|
| 8 | Sản lượng lúa cả năm | SL lúa cả năm |
| 11 | Sản lượng lúa Đông-Xuân | SL lúa ĐX |
| 14 | Sản lượng lúa Hè-Thu | SL lúa HT |
| 17 | Sản lượng lúa Mùa | SL lúa Mùa |
| 20 | Sản lượng ngô | SL ngô |
| 23 | Sản lượng sắn | SL sắn |

---

## Nguồn dữ liệu bổ sung (Perennial crops - Cây lâu năm)

### 2. Tổng cục Thống kê (GSO) - Nguồn chính thức
- **URL chính**: https://www.gso.gov.vn/so-lieu-thong-ke/ → Mục "Nông, lâm nghiệp và thủy sản"
- **Các bảng liên quan**:
  - **Bảng 36**: Diện tích hiện có một số cây lâu năm chủ yếu (theo tỉnh)
  - **Bảng 37**: Diện tích cho sản phẩm một số cây lâu năm chủ yếu (theo tỉnh)
  - **Bảng 38**: Sản lượng một số cây lâu năm chủ yếu (theo tỉnh)
- **Truy cập**: Chọn năm 2024 → Tải file Excel (.xlsx)
- **Lưu ý**: GSO thường công bố số liệu năm trước vào Quý 1 năm sau

### 3. Niên giám thống kê tỉnh (Chi tiết nhất)
- **URL**: https://niengiamthongke.net/ hoặc trang web Cục Thống kê từng tỉnh
- **Phạm vi**: 25 Niên giám riêng biệt (mỗi tỉnh 1 file)
- **Nội dung**: Sản lượng chi tiết theo huyện, đầy đủ loại cây ăn quả, cây công nghiệp
- **Các loại cây chính miền Bắc**:
  - **Cây ăn quả**: Cam sành, Bưởi, Xoài, Vải, Nhãn, Mận, Đào, Lê, Hồng, Chanh, Quýt, Bơ, Sầu riêng (ít)
  - **Cây công nghiệp**: Trà (Thái Nguyên, Phú Thọ, Yên Bái, Hà Giang...), Cà phê (Sơn La, Điện Biên, Lai Châu), Hồ tiêu (Yên Bái, Lào Cai), Điều, Cao su (ít)
  - **Khác**: Chè, Mít, Thiều, Long nhãn...

### 4. Cục Trồng trọt / Bộ NN&PTNT
- **Dashboard**: https://giamsatdanhgia.mard.gov.vn/Reports/Dashboard.aspx
- **Báo cáo**: Chọn "Lĩnh vực Trồng trọt - cây công nghiệp và cây ăn quả" / "Lĩnh vực Trồng trọt - cây hàng năm"
- **Báo cáo quý/năm**: Báo cáo lúa gạo quý, báo cáo cây ăn quả thường niên

### 5. Các nguồn khác
- **Viện MTNN - Lâm nghiệp**: https://mtnongnghiep.com/index.php/du-lieu-lam-nghiep/ (dữ liệu rừng, gỗ)
- **Thông cáo báo chí GSO**: Quý/năm (có số liệu tóm tắt sản lượng lúa theo vụ, vùng)

---

## Phương pháp tính toán

### Phần trăm cho Pie Chart
```
% loại cây = (Sản lượng loại cây / Tổng sản lượng 3 loại cây hàng năm) × 100
```

### Tổng sản lượng năm = Lúa cả năm + Ngô + Sắn

### Lưu ý quan trọng
1. **Chỉ bao gồm 3 cây hàng năm**: Lúa, Ngô, Sắn
2. **KHÔNG bao gồm cây lâu năm** (trà, cà phê, cam, bưởi, vải, nhãn, mận, đào, chè, hồ tiêu...)
3. **Cần bổ sung dữ liệu cây lâu năm** từ GSO Bảng 38 hoặc Niên giám tỉnh để có Pie Chart đầy đủ
4. Số liệu 2024 là **số sơ bộ** (chưa chính thức)

---

## Cách sử dụng dữ liệu cho Pie Chart

### File JSON: `pie_chart_data_2024.json`
Cấu trúc:
```json
{
  "metadata": { ... },
  "data": {
    "Hà Nội": {
      "province": "Hà Nội",
      "total_annual_kton": 935.2,
      "crops": [
        {"name": "Lúa", "production_kton": 862.8, "percentage": 92.25, "category": "annual"},
        {"name": "Ngô", "production_kton": 61.2, "percentage": 6.54, "category": "annual"},
        {"name": "Sắn", "production_kton": 11.2, "percentage": 1.20, "category": "annual"},
        {"name": "Cây lâu năm (cần bổ sung)", "production_kton": null, "percentage": null, "category": "perennial"}
      ]
    },
    ...
  }
}
```

### File CSV: `pie_chart_data_2024.csv`
Các cột: province, crop_name, crop_name_en, category, production_kton, percentage, note

---

## Hướng dẫn bổ sung dữ liệu cây lâu năm

### Option 1: Từ GSO (khuyên dùng cho dữ liệu quốc gia)
1. Vào https://www.gso.gov.vn/so-lieu-thong-ke/
2. Chọn "Nông, lâm nghiệp và thủy sản"
3. Tìm Bảng 38: "Sản lượng một số cây lâu năm chủ yếu"
4. Chọn năm 2024 → Tải Excel
5. Lọc 24 tỉnh miền Bắc
6. Merge vào JSON theo province

### Option 2: Từ Niên giám tỉnh (chi tiết nhất)
1. Vào https://niengiamthongke.net/
2. Tải 24 file Niên giám 2024 của 24 tỉnh
3. Mở sheet "Sản lượng các loại cây trồng" hoặc tương tự
4. Tổng hợp các loại cây ăn quả, cây công nghiệp

### Option 3: Từ Dashboard MARD (trực quan)
1. Vào https://giamsatdanhgia.mard.gov.vn/Reports/Dashboard.aspx
2. Chọn báo cáo "Lĩnh vực Trồng trọt - cây công nghiệp và cây ăn quả"
3. Chọn từng tỉnh → Xem/Xuất báo cáo

---

## Liên hệ / Cập nhật
- Dữ liệu được truy xuất ngày 2025-08-24
- Số liệu 2024 là sơ bộ, sẽ được cập nhật khi GSO công bố số chính thức
- Đề nghị kiểm tra lại với Niên giám tỉnh khi công bố chính thức