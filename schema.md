# K# Dataset Schema (v2.3 Zero‑Shimmer)

Tài liệu này mô tả cấu trúc chuẩn của hai tệp dữ liệu:

- `mnt_quiz_partA_1-2chu.json`
- `mnt_quiz_partB_3chu_troLen.json`

Cả hai tuân theo cùng một schema, chỉ khác về số lượng và độ dài cụm từ.

---

## ✅ 1. Cấu trúc tổng thể

```jsonc
{
  "version": "string",
  "approved_by": "string",
  "audit_status": "string",
  "file_type": "string",
  "id_range": "string",

  "protocol_rules": { ... },

  "tier_system": { ... },

  "mandatory_tests": {
    "<vn>": "<k>"
  },

  "questions": [
    {
      "id": number,
      "vn": "string",
      "k": "string",
      "min_score": number,
      "timer": number | null,
      "meaningVN": "string",
      "meaningEN": "string",
      "trap": ["string", "string", ...]
    }
  ]
}
