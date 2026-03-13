# 🚀 My System Prompt Library

Chào mừng bạn đến với kho lưu trữ các câu lệnh hệ thống (System Prompts) cá nhân. Bộ thư viện này được thiết kế để tối ưu hóa hiệu suất làm việc với AI (Claude 3.5/4.6, Gemini 3.1 Pro, GPT-4o), tập trung mạnh vào mảng **Mobile (Flutter)** và **Web Development**.

## 🧠 Triết lý thiết kế (Core Philosophy)

- **Hybrid Framework:** Sử dụng **Tiếng Anh** cho khung lệnh kỹ thuật (để AI đạt logic tốt nhất) và **Tiếng Việt** cho phần mô tả bối cảnh/nghiệp vụ.
- **Context Management:** Giải quyết triệt để vấn đề "tràn bộ nhớ" của AI thông qua quy trình Handoff bài bản.
- **Efficiency First:** Luôn yêu cầu AI chỉ trả về phần code thay đổi (**Modified parts only**) để tiết kiệm thời gian và tài nguyên.

---

## 📂 Cấu trúc Thư mục & Ý nghĩa

### 🔄 1. Context Handoff (Quản lý Ngữ cảnh)

_Bộ công cụ giúp duy trì sự liền mạch khi làm việc với các Project lớn._

| File                      | Mục đích                             | Cách sử dụng                                      |
| :------------------------ | :----------------------------------- | :------------------------------------------------ |
| `app_context_template.md` | Định nghĩa Tech Stack, Coding Rules. | Nạp vào dòng đầu tiên khi bắt đầu Project mới.    |
| `wrap-up.md`              | Tóm tắt tiến độ và logic hiện tại.   | Dùng ở cuối phiên chat cũ trước khi đóng.         |
| `boot-up.md`              | Khôi phục bối cảnh từ phiên cũ.      | Dùng ở đầu phiên chat mới để AI "nhập cuộc" ngay. |

### 💙 2. Flutter (Mobile Specialized)

_Tập trung vào hiệu suất, Widget Tree và Native Integration._

| File                             | Mục đích                                                           |
| :------------------------------- | :----------------------------------------------------------------- |
| `flutter-ui-widget.md`           | Tạo UI Widget chuẩn Material 3, Responsive, dùng `const` triệt để. |
| `flutter-state-logic.md`         | Viết logic xử lý State (BLoC, Riverpod) và tích hợp API.           |
| `flutter-animation-optimizer.md` | Tạo/Tối ưu Animation 60/120fps, dùng `AnimatedBuilder`.            |
| `flutter-refactor.md`            | Refactor code, giảm Nesting Hell, sửa lỗi Linting.                 |
| `flutter-security-audit.md`      | Kiểm tra Memory Leaks (Dispose controllers) và bảo mật local.      |
| `flutter-testing.md`             | Tự động sinh Unit Test và Widget Test (Mocktail/Mockito).          |
| `flutter-native-bridge.md`       | Cấu hình Method Channel cho Android (Kotlin) và iOS (Swift).       |

### 🌐 3. Web (Frontend & Backend)

_Linh hoạt cho React, Next.js, Node.js và các Framework hiện đại._

| File                        | Mục đích                                                    |
| :-------------------------- | :---------------------------------------------------------- |
| `ui-component-generator.md` | Tạo Component chuẩn Accessibility (ARIA) và Responsive CSS. |
| `core-logic-handler.md`     | Xử lý logic Backend, bảo mật đầu vào, Error Handling.       |
| `system-architecture.md`    | Tư vấn thiết kế Database, System Flow và vẽ sơ đồ Mermaid.  |
| `code-review-refactor.md`   | Tối ưu Performance, Bundle size và chuyển đổi JS sang TS.   |

### 🛠️ 4. Common (Công cụ dùng chung)

_Áp dụng cho mọi ngôn ngữ lập trình._

| File                       | Mục đích                                                   |
| :------------------------- | :--------------------------------------------------------- |
| `common-debugger.md`       | Phân tích Stack Trace, tìm Root Cause và đề xuất cách Fix. |
| `common-code-explainer.md` | Giải thích logic code phức tạp bằng Tiếng Việt súc tích.   |
| `common-regex-sql.md`      | Chuyên gia về Regular Expression và truy vấn SQL tối ưu.   |

---

## ⌨️ Cách tích hợp vào VS Code (Snippets)

Để gọi nhanh các Prompt này, bạn nên cấu hình **Global Snippets** trong VS Code:

1. Nhấn `Cmd + Shift + P` -> chọn **Configure User Snippets**.
2. Tạo file mới tên là `ai-prompts.code-snippets`.
3. Định nghĩa các prefix như: `!fl-ui`, `!fl-logic`, `!debug`, `!handoff`.

**Mẫu Snippet tham khảo:**

```json
{
  "Flutter UI Builder": {
    "prefix": "!fl-ui",
    "body": [
      "Refer to /flutter/flutter-ui-widget.md:",
      "Description: [${1:Mô tả UI}]",
      "Params: [${2:Tham số}]",
      "Output: Modified parts only. No yapping."
    ]
  }
}
```
