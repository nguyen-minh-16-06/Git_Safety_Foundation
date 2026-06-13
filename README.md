# Git_Safety_Foundation
# Báo Cáo Hoàn Thành Khóa Học Git Foundation - AKA Lab

## 1. Nhật ký Quá trình học tập
- Đã hoàn thành lộ trình Microsoft Learn - GitHub Foundations (Part 1 & Part 2).
- Đã nắm vững quy trình GitHub Flow bao gồm: Tạo repository, phân nhánh, commit có thông điệp rõ ràng, tạo và review Pull Request.

## 2. Các tính năng GitHub UI đã thực hành thành công
- Thao tác quản lý mã nguồn, tạo và chỉnh sửa hoàn toàn qua các file tài liệu cấu hình dạng Markdown (`.md`).
- Xử lý xung đột trực quan bằng công cụ "Resolve conflicts" tích hợp sẵn trên trình duyệt khi hai nhánh cùng sửa một dòng file.
- Sử dụng tính năng "Revert Pull Request" để loại bỏ các nội dung/mã nguồn lỗi do AI tạo ra một cách an toàn mà không làm mất lịch sử hệ thống.

## 3. Danh sách minh chứng kết quả thực hiện
- **Link GitHub Repository:** https://github.com/nguyen-minh-16-06/Git_Safety_Foundation
- **Danh sách các Branch đã tạo (Tối thiểu 3):** `main`, `feature/hand-detection`, `feature/robot-control`, `bugfix/parameter-tuning`, `feature/ai-wrong-docs`.
- **Danh sách Pull Requests (Tối thiểu 2):** - PR số 1 (Gộp tính năng nhận diện tay): https://github.com/nguyen-minh-16-06/Git_Safety_Foundation/tree/3b4bca89fef8f84f82700e738f225850f6a17ff6
  - PR số 2 (Gộp thông số cấu hình robot): https://github.com/nguyen-minh-16-06/Git_Safety_Foundation/tree/2857841ceef5acd356cd1bf5f86b89e542c2a744
- **Minh chứng giải quyết Conflict:** Đã xử lý xung đột thành công tại PR đối với file `project_overview.md`: https://github.com/nguyen-minh-16-06/Git_Safety_Foundation/commit/4208b887152447551ed825e83ac03932eec1294a
- **Minh chứng Rollback/Revert:** Đã thực hiện xóa bỏ commit lỗi thông qua PR Revert tại link: https://github.com/nguyen-minh-16-06/Git_Safety_Foundation/commit/c5a608fa2d10bc2cfb7ea2557990491eac4445ac

## 4. Tư duy sử dụng Git khi bước vào khóa học Vibe Code với AI
Khi phát triển phần mềm trong kỷ nguyên AI Coding, tốc độ sinh mã nguồn và tài liệu của AI là rất lớn nhưng đi kèm rủi ro tạo ra các lỗi logic tiềm ẩn hoặc phá vỡ kiến trúc hệ thống hiện tại. Tôi sẽ áp dụng Git làm "Phanh an toàn" theo nguyên tắc:
1. **Tuyệt đối không can thiệp thẳng vào nhánh chính:** Mọi yêu cầu hay prompt đưa cho AI sinh ra đều phải được đưa vào một nhánh `feature/...` riêng biệt để cô lập rủi ro.
2. **Chia nhỏ checkpoint để commit:** Cứ sau mỗi lần prompt AI thành công một phân đoạn nhỏ và kiểm tra thấy hoạt động ổn định, tôi sẽ thực hiện commit ngay để làm điểm tựa quay lại nếu các prompt sau đó làm hỏng hệ thống.
3. **Sử dụng Pull Request làm lưới lọc:** Trước khi gộp bất kỳ đoạn code nào của AI vào nhánh chính, tôi sẽ dùng giao diện so sánh dòng (diff) trên PR để rà soát kỹ lưỡng, đảm bảo hiểu rõ những gì AI đã thay đổi.
