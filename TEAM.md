# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: Random
- Candidate problem nhóm chọn (1 câu):
- Quyết định cuối (Go / Not Yet / No-Go):

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 |Đỗ Duy Bộ |2A202603591|Trưởng nhóm|https://github.com/flying-bug|
| 2 |Phạm Tuấn Cường|2A202603584|Thành Viên|https://github.com/Ptuancuong|
| 3 | Nguyễn Minh Đạt | 2A202603582 | Thành Viên | https://github.com/nguyenminhdat6401 |
| 4 |Nguyễn Đăng Doanh |2A202603597 |Thành Viên |https://github.com/doanhnguyen28 |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | | | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | | | Assumption map, snapshot hoặc survey |
| CP4 — Research | | | Bảng research có link |
| CP5 — Quy trình trước/sau | | | Quy trình + bảng before/after |
| CP5 — Problem Statement v0 | | | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | | | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | | | 4 rủi ro + Go/Not Yet/No-Go |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### DoDuyBo-2A202603591

**Phần việc phụ trách:**

-

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

-

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

-

**Điều mình học được từ phần nhóm:**

-


### NguyenDangDoanh-2A202603597

**Phần việc phụ trách:**
- Người đưa ra candidate được chọn (#10 — triage kết quả security scan); giải thích quy trình scan cho cả nhóm vì là thành viên duy nhất làm DevOps
- Phản biện card của các bạn ở CP3
- Viết cây OST (mục 2.3)
- Cùng Cường viết quy trình trước/sau (mục 4) và góp phần viết Problem Statement v0 (mục 5)
- Rà soát tính nhất quán giữa các mục 4–8 của báo cáo nhóm


**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):
- Pitch 3 card #10, #11, #12 và đưa vào bảng pitch mục 2.1
- Đặt câu hỏi phản biện cho Cường (#1, #3) và Bộ (#4); câu hỏi về số liệu của #4 là một lý do nhóm loại #4 ở mục 2.4
- Sau câu hỏi của Cường về con số 65 phút, tách quy trình thành 5 bước có thời gian, chỉ ra bottleneck thật là bước đánh giá ngữ cảnh (~30/65 phút)
- Viết cây OST mục 2.3: 1 outcome, 3 opportunity, gạch bỏ 3 ý là solution đội lốt
- Viết quy trình hiện tại, quy trình tương lai và bảng before/after ở mục 4, gồm con số "chỉ Rule còn ~40 phút/lần" dùng làm lập luận cho mức Workflow ở CP6
- Sửa các chỗ mâu thuẫn trong báo cáo nhóm: Problem Statement v0 lệch với mục 4.1, ô ma trận ở mục 6.1, mức chọn ở 6.2 lệch với Problem Statement v1, các placeholder còn sót
- Phỏng vấn 1 Backend Engineer ngoài nhóm theo The Mom Test, viết snapshot-1


**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):
- Mục 2.1, các dòng #10–#12 và câu hỏi phản biện ở dòng #1, #3, #4: commit `3f81912` (add pitch group report), `ba7cc89` (add question for gr member), `630fca2`
- Mục 2.3: commit `05afa8a` (add 2.3 ost)
- Mục 4 và 5: commit `d4fc312` (add cp5), `7a65eee` (modify cp5)
- Rà soát mục 1, 2, 5–9: commit `3886a05` (modify team report)
- File `cp4-interview-snapshot-1.md` trong `report/assets/`


**Điều mình học được từ phần nhóm:**
- Bottleneck phải là một bước cụ thể. Khi bị hỏi con số 65 phút gồm những gì, mình mới thấy chỉ khoảng 30 phút là phần thật sự khó, còn lại Rule làm được
- Nên research công cụ có sẵn trước khi nghĩ tới AI: Trivy và Dependabot đã giải được phần lọc nhiễu, nên AI chỉ cần chen vào đúng một bước
- Kiểm chứng với người thật cần chuẩn bị từ trước buổi học; nhóm chưa làm kịp phần này trong buổi nên Value vẫn chỉ ở mức TB

### HoTen-MSSV

**Phần việc phụ trách:**

-

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

-

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

-

**Điều mình học được từ phần nhóm:**

-