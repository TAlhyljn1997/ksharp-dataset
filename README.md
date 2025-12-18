# ksharp-dataset
Official dataset for K# v2.3 Zero‑Shimmer Protocol, including Part A (1–2 syllables) and Part B (3+ syllables).
# K# Dataset v2.3 — Zero‑Shimmer Vietnamese Encoding Corpus

Bộ dữ liệu chính thức dành cho **K# v2.3 Zero‑Shimmer Protocol**, bao gồm toàn bộ từ đơn, từ ghép, và cụm từ 3 chữ trở lên.  
Dataset này được thiết kế để phục vụ:

- Đấu Trường An Lạc (ALSA)
- KHD Tone Academy
- Ri‑Lingua / K# training
- AI agents trong hệ sinh thái RI‑Ecosys
- Các nhà phát triển muốn tích hợp K# vào ứng dụng, game, hoặc hệ thống học tập

---

## 📦 Nội dung dataset

Repo này bao gồm hai tệp JSON:

### **1. `mnt_quiz_partA_1-2chu.json`**
- ID: **1 → 150**
- Từ đơn & từ ghép (1–2 chữ)
- Mỗi mục gồm:
  - `vn`: tiếng Việt
  - `k`: mã K# v2.3
  - `trap`: danh sách mồi sai
  - `meaningVN`, `meaningEN`
  - `tier_system`
  - `mandatory_tests`

### **2. `mnt_quiz_partB_3chu_troLen.json`**
- ID: **201 → 350**
- Cụm từ 3 chữ trở lên
- Bao gồm các câu:
  - triết lý
  - đạo đức
  - ALSA Arena
  - RL‑law
  - Resontologic
  - KHD_CAP
- Cấu trúc tương tự Part A nhưng mở rộng hơn

---

## 🎯 Mục tiêu của dataset

- Chuẩn hóa việc học K#  
- Tạo sân chơi luyện tốc độ (ALSA)  
- Huấn luyện AI theo chuẩn **Zero‑Shimmer**  
- Cung cấp bộ dữ liệu sạch, audit 100% bởi `.ljn Authority`  
- Làm nền tảng cho các ứng dụng K# trong tương lai  

---

## 🧬 K# Encoding Pipeline (tóm tắt)

1. **Onset Law**  
   đ=y, tr=j, ch=f, nh=z, kh=q, ng=w, ph=p, d=d

2. **Rime Law**  
   iêu=el, yêu=yu, ươi/uôi=ol, uyên=yln

3. **Coda Law**  
   ng=w, nh=f, ch=j

4. **CAP Matrix (Tone + Variant)**  
   | Tone   | Plain | Hat | Hook |
   |--------|-------|-----|------|
   | Ngang  | N     | Y   | M    |
   | Sắc    | S     | T   | X    |
   | Huyền  | L     | D   | K    |
   | Hỏi    | Q     | B   | V    |
   | Nặng   | P     | F   | H    |
   | Ngã    | Z     | G   | R    |

---

## 🧪 Ví dụ

| Tiếng Việt | K# |
|-----------|----|
| người     | wolK |
| mạnh      | mafH |
| yêu       | yuS |
| trắng     | jafwN |

---

## 📚 Cách sử dụng dataset

### ✅ Dùng cho game / app
- Load JSON  
- Lấy `vn` để hiển thị  
- So sánh input người chơi với `k`  
- Dùng `trap[]` để tạo lựa chọn sai  

### ✅ Dùng cho AI
- Fine‑tune hoặc prompt‑train theo chuẩn Zero‑Shimmer  
- Không suy diễn  
- Không tự sửa lỗi chính tả  
- Không normalize  

### ✅ Dùng cho nghiên cứu
- Phân tích CAP distribution  
- Kiểm tra tính nhất quán của K#  
- Tạo mô hình học âm vị học tiếng Việt  

---

## 📄 License

MIT License + RL‑Law Protection  
Xem file `LICENSE` để biết chi tiết.

---

## 👤 Maintainer

**Ba Phúc Trần**  
Founder — RI‑Ecosys Research  
Tác giả Thuyết Resontologic & K# v2.3 Zero‑Shimmer Protocol

---

## 🕊️ Tuyên ngôn

> “Giữa hỗn loạn, vẫn An Lạc.  
> Sức mạnh đến từ sự hiện diện.”  
