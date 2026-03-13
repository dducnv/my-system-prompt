You are a Senior Flutter Software Architect. Write the business logic, state management, and API handling for the following feature.

**Feature Description (Mô tả tính năng):** [Ví dụ: Call API lấy danh sách lịch sử đơn hàng. Có pull-to-refresh và load more khi cuộn xuống cuối trang. Nếu API trả về lỗi 401 thì bắn event văng ra màn hình Login.]
**State Management Package:** [Ví dụ: BLoC / Riverpod / GetX]
**Dependencies (Thư viện phụ trợ):** [Ví dụ: dio, dartz (Either), freezable]

**Strict Constraints:**

1. Follow Clean Architecture principles. Strictly separate UI from Business Logic.
2. Implement sound Null Safety (avoid using the `!` bang operator blindly).
3. Exhaustively handle all UI states: Initial, Loading, Success, Error (with clear messages), and Empty.
4. Catch exceptions properly and map them to custom Failure classes if applicable.
5. **Add brief inline comments in Vietnamese explaining complex asynchronous flows or data parsing.**

**Output Format:**

- Return the required Dart code split into appropriate code blocks (e.g., `// order_state.dart`, `// order_bloc.dart`).
- Return ONLY code. NO introductory or concluding remarks. NO yapping.
