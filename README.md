# 🚀 Ultimate Developer Prompt Library

Bộ sưu tập System Prompts tối ưu dành cho AI (Claude 3.5/4.6, Gemini 3.1 Pro, GPT-4o). Repo này được thiết kế để chuẩn hóa quy trình phát triển phần mềm, tập trung mạnh vào **Flutter (Mobile)**, **Web**, và **Automation**.

## 🧠 Nguyên tắc vàng (Core Principles)

- **Hybrid Framework:** Sử dụng **Tiếng Anh** cho các chỉ thị kỹ thuật (để AI đạt hiệu năng logic tối đa) và **Tiếng Việt** cho phần bối cảnh/nghiệp vụ.
- **Context Control:** Quản lý ngữ cảnh thông qua quy trình Handoff bài bản để tránh AI bị "ngáo" trong các đoạn chat dài.
- **Minimalist Code:** Luôn ưu tiên trả về **Modified parts only** để tiết kiệm Token và dễ dàng tích hợp vào Codebase hiện tại.

---

## 📂 Danh mục Prompts

### 🔄 1. Context Management (Quản lý Ngữ cảnh)

_Duy trì "trí nhớ" cho AI xuyên suốt dự án._

| File                      | Mục đích                                                          |
| :------------------------ | :---------------------------------------------------------------- |
| `app_context_template.md` | Định nghĩa Tech Stack, Coding Rules và Kiến trúc dự án.           |
| `wrap-up.md`              | Đóng gói tiến độ và logic hiện tại (Handoff) trước khi đóng chat. |
| `boot-up.md`              | Khôi phục bối cảnh từ phiên cũ vào phiên chat mới.                |

### 💙 2. Flutter Development (Chuyên sâu Mobile)

_Tối ưu hóa vòng đời phát triển ứng dụng Flutter._

| File                             | Mục đích                                                           |
| :------------------------------- | :----------------------------------------------------------------- |
| `flutter-ui-widget.md`           | Tạo UI Widget chuẩn Material 3, Responsive, dùng `const`.          |
| `flutter-state-logic.md`         | Viết logic BLoC, Riverpod, xử lý API và Clean Architecture.        |
| `flutter-boilerplate-gen.md`     | Tự động sinh Model (Freezed/JSON) từ dữ liệu API thô.              |
| `flutter-animation-optimizer.md` | Tạo hiệu ứng 60/120fps bằng `AnimatedBuilder` & `RepaintBoundary`. |
| `flutter-push-handler.md`        | Xử lý Push Notification (FCM/OneSignal) cho 3 trạng thái app.      |
| `flutter-native-bridge.md`       | Viết Method Channel cho Android (Kotlin) và iOS (Swift).           |
| `flutter-refactor.md`            | Sửa lỗi lồng ghép (Nesting Hell) và tối ưu hóa Linting.            |
| `flutter-security-audit.md`      | Kiểm tra Memory Leaks và các lỗ hổng bảo mật Mobile.               |
| `flutter-testing.md`             | Viết Unit Test và Widget Test (Mocktail/Mockito).                  |

### 🚀 3. Mobile Release & Automation

_Đưa ứng dụng từ Local lên các chợ ứng dụng (Stores)._

| File                      | Mục đích                                                          |
| :------------------------ | :---------------------------------------------------------------- |
| `flutter-localization.md` | Dịch app đa ngôn ngữ (.arb/.json) mà không làm hỏng Key/Variable. |
| `app-store-metadata.md`   | Viết mô tả chuẩn ASO (SEO cho Store) để tăng lượt tải app.        |
| `cicd-fastlane-helper.md` | Viết Fastfile để tự động hóa việc Build và Deploy app lên Store.  |

### 🌐 4. Web Development (Fullstack)

_Chuyên biệt cho React, Next.js và Node.js._

| File                        | Mục đích                                                       |
| :-------------------------- | :------------------------------------------------------------- |
| `ui-component-generator.md` | Tạo Web Component chuẩn Accessibility (ARIA) và Responsive.    |
| `core-logic-handler.md`     | Xử lý logic Backend, bảo mật đầu vào, và Error Handling.       |
| `system-architecture.md`    | Tư vấn thiết kế Database và Architecture Flow (Sơ đồ Mermaid). |
| `code-review-refactor.md`   | Review code, tối ưu Bundle size và chuyển đổi JS sang TS.      |

### 🛠️ 5. Common Utilities (Tiện ích dùng chung)

_Áp dụng cho mọi dự án phần mềm._

| File                       | Mục đích                                                      |
| :------------------------- | :------------------------------------------------------------ |
| `common-debugger.md`       | Phân tích Stack Trace và tìm nguyên nhân gốc rễ của Bug.      |
| `common-code-explainer.md` | Giải thích logic code phức tạp bằng Tiếng Việt súc tích.      |
| `common-regex-sql.md`      | Chuyên gia về Regular Expression và truy vấn SQL tối ưu.      |
| `common-doc-generator.md`  | Tự động viết README, Swagger hoặc tài liệu API chuyên nghiệp. |

---

## ⌨️ Sử dụng nhanh với VS Code Snippets

Đừng copy-paste thủ công. Hãy đưa các Prompt này vào **Global Snippets**:

1. `Cmd + Shift + P` -> **Configure User Snippets**.
2. Chọn file `ai-prompts.code-snippets` và dán cấu hình của bạn.

**Mẹo gọi nhanh:**

- `!fl-ui`: Tạo UI Flutter.
- `!fl-model`: Sinh Model từ JSON.
- `!debug`: Sửa lỗi nhanh.
- `!aso`: Viết mô tả app lên Store.

---

## 💡 Tips & Tricks

- **Luôn yêu cầu:** _"Modified parts only. No yapping."_ để nhận code ngắn gọn nhất.
- **Tư duy Plan-then-Code:** Với các task khó, hãy bảo AI _"Write a plan first, code later"_ để đảm bảo logic đúng hướng trước khi sinh code dài.

---

_Created and maintained by Developer Community. Happy Coding!_ 🚀
