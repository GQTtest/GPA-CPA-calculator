# GPA Calculator

Công cụ tính GPA theo học kỳ và CPA toàn khóa (thang 4), chạy hoàn toàn trên trình duyệt, chỉ một file HTML.

## Chạy

```bash
git clone git@github.com:<username>/gpa-calculator.git
cd gpa-calculator
```

Mở `index.html` bằng trình duyệt (double-click là được). Không cần cài thêm gì.

## Cách dùng

1. Bấm **Thêm môn**, nhập học kỳ, tên môn, số tín chỉ và điểm chữ.
2. CPA và GPA từng học kỳ cập nhật ngay khi bạn sửa.
3. Dữ liệu lưu trong `localStorage` của trình duyệt, tắt trang mở lại vẫn còn.

## Công thức

GPA = Σ (tín chỉ × điểm hệ 4) / Σ tín chỉ

Bảng quy đổi nằm ở biến `SCALE` đầu phần `<script>` trong `index.html`:

| Điểm chữ | A+ | A | B+ | B | C+ | C | D+ | D | F |
|---|---|---|---|---|---|---|---|---|---|
| Hệ 4 | 4.0 | 4.0 | 3.5 | 3.0 | 2.5 | 2.0 | 1.5 | 1.0 | 0 |

Đối chiếu với quy chế của trường và sửa nếu khác.

## Hạn chế đã biết

- Mỗi dòng đều được tính vào điểm, chưa có tùy chọn bỏ qua môn học lại hoặc môn không tính GPA.
- Dữ liệu chỉ nằm trên một trình duyệt, chưa có xuất/nhập file.

## License

MIT
