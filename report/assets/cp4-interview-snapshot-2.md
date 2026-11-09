# CP4 Interview Snapshot 2

> Chỉ điền sau khi phỏng vấn người thật. Không ghi tên thật, email, số điện thoại hoặc thông tin nội bộ. Ghi đúng ý người được hỏi; không tự tạo câu trích dẫn hay số liệu.

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Backend dev kiêm DevOps, startup khoảng 8 dev, 2 repo trên GitHub; dùng Dependabot |
| Ngày / cách phỏng vấn | Hỏi qua điện thoại |
| Câu nói đáng nhớ nhất (nguyên văn) | "Có bản vá thì cứ merge PR của Dependabot, test xanh là xong, ít khi ngồi đọc CVE." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | tuần trước có 9 cảnh báo Dependabot, merge 7 PR nâng version, 2 cái chưa có bản vá thì để đó |
| Hiện đang xử lý bằng cách nào (workaround)? | Không triage theo từng lần scan, dồn cảnh báo lại xử lý cuối tuần bằng cách merge PR nâng version. Chưa bật auto-triage rules |
| Mất bao lâu, bao lần? | Khoảng 20 phút/tuần. Chưa từng trễ release vì scan |
| Insight / opportunity rút ra | Phản bác: ở team nhỏ, ít repo, pain thấp; cách "có bản vá thì nâng version" (No AI) là đủ. Problem chỉ đáng giải ở team lớn hơn, nhiều repo |
