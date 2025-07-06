# 🔤 Chuyển Đổi Văn Bản Thành Slug Chuẩn SEO trong Google Sheets

Đây là một hàm tùy chỉnh (`Custom Function`) cho Google Sheets, giúp bạn **chuyển đổi văn bản tiếng Việt có dấu thành định dạng slug** không dấu, dùng cho URL hoặc SEO.

---

## 🚀 Tính năng

- Chuyển chữ thường → chữ hoa
- Loại bỏ dấu tiếng Việt (á → a, ộ → o, đ → d, ...)
- Thay thế khoảng trắng bằng dấu gạch ngang (`-`)
- Xoá ký tự đặc biệt (ví dụ: `, . ? ! @ $`)
- Rút gọn nhiều dấu gạch thành 1
- Loại bỏ dấu `-` ở đầu và cuối

---

## ✨ Ví dụ sử dụng

| Văn bản đầu vào                                 | Kết quả slug                       |
|--------------------------------------------------|------------------------------------|
| `Tẩy tế bào chết - Bí kíp làm đẹp`              | `tay-te-bao-chet-bi-kip-lam-dep`   |
| `Sữa Rửa Mặt Ý Dĩ Nhân Đỏ (Mới)`                | `sua-rua-mat-y-di-nhan-do-moi`     |
| `TOP 10 Kem Chống Nắng tốt nhất 2025!`          | `top-10-kem-chong-nang-tot-nhat-2025` |

---

## 📌 Cách sử dụng trong Google Sheets

1. Mở file Google Sheets của bạn
2. Chọn menu **Tiện ích mở rộng > Apps Script**
3. Xóa hết và **dán đoạn mã trong file `Code.gs`**
4. Bấm **Lưu (Ctrl+S)** và đóng cửa sổ Apps Script
5. Quay lại bảng tính, sử dụng như công thức thường:

```excel
=ChangeToSlug(A2)
