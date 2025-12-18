# Dataset Validator — K# v2.3

## ✅ Kiểm tra từng mục `questions[]`

1. `vn` không trùng
2. `k` đúng Onset/Rime/Coda/CAP
3. `trap[]` không trùng `k`
4. `trap[]` không shimmer
5. `CAP` nằm trong 18 ký tự chuẩn
6. `id` không trùng
7. `meaningVN` và `meaningEN` rõ ràng

---

## 🧪 Kiểm tra toàn bộ file

- Không có shimmer
- Không có mã Unicode ngoài ASCII
- Không có CAP sai
- Không có Onset/Rime/Coda sai

---

## 🛡️ Quy tắc bất biến

- Không sửa `k` nếu không có audit
- Không thêm CAP mới
- Không normalize tiếng Việt
