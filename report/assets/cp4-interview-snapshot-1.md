# CP4 Interview Snapshot 1

> Chỉ điền sau khi phỏng vấn người thật. Không ghi tên thật, email, số điện thoại hoặc thông tin nội bộ. Ghi đúng ý người được hỏi; không tự tạo câu trích dẫn hay số liệu.

| Trường                                            | Nội dung |
| ------------------------------------------------- | -------- |
| Người được hỏi (vai trò, không ghi tên thật)      | Backend Engineer   |
| Ngày / cách phỏng vấn | Nhắn tin phỏng vấn qua điện thoại (9/11/2026) |
| Câu nói đáng nhớ nhất (nguyên văn)                | "Scan thì nhanh nhưng có chắc là báo lỗi đúng không?" |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Tuần trước PR bị pipeline chặn vì 8 finding Critical trong một thư viện xử lý ảnh; sau khi kiểm thì service không dùng tới phần bị lỗi, mất nửa buổi chờ DevOps xác nhận rồi mới merge |
| Hiện đang xử lý bằng cách nào (workaround)?       | Tự đọc advisory trên GitHub, tìm trong code xem có import hàm bị lỗi không, rồi nhắn DevOps xin thêm vào ignore file         |
| Mất bao lâu, bao lần?                             |Khoảng 20–30 phút mỗi lần tự kiểm, 1–2 lần/tuần; thời gian chờ DevOps xác nhận tính riêng          |
| Insight / opportunity rút ra                      |Thời gian chạy scan không phải vấn đề; pain nằm ở niềm tin vào kết quả: người dùng không chắc finding nào là thật nên phải tự kiểm lại. Xác nhận Opportunity A (báo nhầm) và B (phải tự đánh giá có ảnh hưởng không). Thêm góc nhìn mới: dev cũng chịu pain (bị chặn PR, phải chờ DevOps), không chỉ DevOps. Củng cố quyết định AI chỉ gợi ý kèm trích dẫn để người kiểm |
