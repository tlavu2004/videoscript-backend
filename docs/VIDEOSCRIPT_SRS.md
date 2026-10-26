# ĐẶC TẢ YÊU CẦU PHẦN MỀM - VIDEOSCRIPT

## A. Giới thiệu chung

### 1. Tên phần mềm

VideoScript (AI Short Video Creator) – Nền tảng tạo video ngắn theo xu hướng bằng trí tuệ nhân tạo

### 2. Mục tiêu

- Phát triển một ứng dụng hỗ trợ người dùng tạo ra video ngắn dạng TikTok, YouTube Shorts từ nội dung theo xu hướng hiện tại
- Sử dụng các công nghệ AI như LLM, TTS, và xử lý video tự động.
- Phần mềm hướng đến mục tiêu hỗ trợ sáng tạo nội dung dễ dàng hơn cho người dùng phổ thông, sinh viên, người yêu thích multimedia.

### 3. Phạm vi ứng dụng

- Người dùng cần tạo video ngắn học thuật, truyền thông, giải trí, lan tỏa kiến thức.
- Nhóm sinh viên cần tạo sản phẩm minh họa cho các chiến dịch truyền thông.
- Người học muốn thực hành với các công nghệ AI đa phương tiện hiện đại.

## B. Chức năng chính (MVP)

| ID | Chức năng                   | Mô tả                                                               |
|----|-----------------------------|---------------------------------------------------------------------|
| F1 | Gợi ý chủ đề theo xu hướng  | Gợi ý nội dung đang được quan tâm thông qua từ khóa và API trend    |
| F2 | Sinh kịch bản video tự động | Tạo nội dung mô tả theo cấu trúc hấp dẫn, sinh động                 |
| F3 | Tạo giọng đọc AI            | Chuyển văn bản thành giọng nói qua công nghệ Text-to-Speech         |
| F4 | Tạo video tự động           | Ghép ảnh nền, giọng đọc và phụ đề thành một video hoàn chỉnh        |
| F5 | Chỉnh sửa cơ bản            | Cho phép người dùng thêm hiệu ứng chữ, sticker, nhạc nền            |
| F6 | Xuất video                  | Tải video dưới định dạng .mp4 để chia sẻ hoặc sử dụng trong bài học |
| F7 | Quản lý video đã tạo        | Lưu trữ và xem lại các video từng được tạo qua hệ thống             |

## C. Yêu cầu phi chức năng

- Hiệu năng: Video ngắn (dưới 1 phút) được xử lý trong vòng 60 giây
- Khả năng mở rộng: Dễ dàng tích hợp các API mới, thêm chức năng nâng cao
- Giao diện: Giao diện đơn giản, thân thiện với người mới
- Bảo mật: Tài khoản người dùng được xác thực và thông tin được mã hóa
- Tài liệu kỹ thuật: Có tài liệu mô tả từng module để dễ bảo trì và nâng cấp

## D. Luồng hoạt động chính

1. Nhập từ khóa chủ đề
2. Sinh kịch bản từ AI
3. TTS tạo giọng đọc
4. Chọn hình nền phù hợp
5. Chèn phụ đề tự động
6. Xem trước và tải video

## E. Giao diện người dùng đề xuất

- Trang chủ: nhập từ khóa & xem đề xuất xu hướng
- Trang soạn kịch bản & chọn giọng đọc
- Trang xem trước video & tùy chỉnh đơn giản
- Dashboard video đã tạo

## F. Yêu cầu công nghệ

- Frontend: ReactJS / Next.js + TailwindCSS (đã có).
- Backend: Microservices - Java Spring + Python (chỉ những service liên quan tới AI).
- AI NLP: (hãy đề xuất các mô hình bên thứ 3 miễn phí)
- TTS: (hãy đề xuất các mô hình bên thứ 3 miễn phí)
- Video Processing: (hãy đề xuất)
- Database: PostgreSQL và MongoDB (tùy service phù hợp)
- Lưu trữ: Cloudinary

## G. Phân công nhóm đề xuất

- Dev Frontend: Xây dựng giao diện & chức năng người dùng (đã có)
- Dev Backend: Viết API, điều phối xử lý AI (cần tập trung)
- AI Integrator: Gắn kết LLM, TTS, video render (cần tập trung)
- Test, viết tài liệu (đã có)

## H. Tiêu chí đánh giá

- Giao diện dễ dùng
- Có thể tạo được video từ nội dung do AI sinh
- Tích hợp TTS và xử lý video cơ bản
- Tài liệu rõ ràng, có sơ đồ hệ thống
