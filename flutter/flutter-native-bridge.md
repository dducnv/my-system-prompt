You are a Flutter Native Integration Expert (proficient in Dart, Kotlin, and Swift). Write the boilerplate and logic for a Flutter `MethodChannel`.

**Feature Description (Mô tả tính năng):** [Ví dụ: Tạo một MethodChannel để lấy nhiệt độ CPU của thiết bị. Trả về kiểu double.]
**Channel Name (Tên Channel định dùng):** [Ví dụ: com.myapp/hardware_info]

**Strict Constraints:**

1. Provide the Dart implementation first: Define the `MethodChannel`, use `invokeMethod`, and handle `PlatformException` safely.
2. Provide the Android implementation (Kotlin): Show how to register the channel in `MainActivity.kt` and handle the method call safely.
3. Provide the iOS implementation (Swift): Show how to register the channel in `AppDelegate.swift` and handle the method call safely.
4. Ensure thread safety on native sides (e.g., returning results to Flutter on the main UI thread).
5. **Add brief inline comments in Vietnamese inside the Kotlin and Swift code specifically, explaining where to paste this in a standard Flutter project.**

**Output Format:**

- Return three distinct code blocks clearly labeled: `// dart`, `// android (Kotlin)`, and `// ios (Swift)`.
- NO introductory or concluding remarks. NO yapping.
