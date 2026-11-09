# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm:
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu):
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 |Phạm Tuấn Cường |Khi chuẩn bị nộp bài lab, tôi muốn đối chiếu bài mình với RUBRIC, CHECKPOINTS và SUBMISSION cùng lúc, để không mất điểm vì thiếu mục hoặc sai cấu trúc |Học viên |3 file hướng dẫn, khoảng 30 phút rà mỗi lab; lab trước bị trừ điểm vì sai tên file |Doanh: 30p rà soát gồm những bước nào, bước nào chiếm nhiều thời gian? |
| 2 |Phạm Tuấn Cường |Khi tới tối Chủ nhật, tôi muốn biết tuần tới có những deadline nào, để không bỏ sót bài nộp|Học viên |Deadline nằm rải rác ở LMS, Discord, email; mất khoảng 20 phút/tuần để gom; tháng trước suýt trễ 1 bài vì thông báo đổi hạn nằm trong thread Discord |Đạt: Việc ở bước nào, mất bao nhiêu phút|
| 3 |Phạm Tuấn Cường |Khi cài môi trường cho lab có code, tôi muốn chạy được code mẫu ngay lần đầu, để không mất thời gian giờ học vì lỗi cài đặt |Tôi |Lần gần nhất mất 40 phút vì lỗi phiên bản Python; tôi đã gặp |Doanh: Nếu cài đặt thì cần mấy bước, quy trình?|
| 4 |Đỗ Duy Bộ|Khi khách hàng báo lỗi qua nhiều kênh, tôi muốn nhận ra những phản ánh cùng nói về một vấn đề, để biết vấn đề nào đang ảnh hưởng nhiều khách hàng nhất. |Nhân viên CSKH|đọc ~200 phản ánh và quyết định cái nào cùng một vấn đề, ~25 phút/tuần; khách mô tả cùng một lỗi bằng nhiều cách khác nhau nên dễ gom sai |Doanh: Con số có khớp nhau không? Lần gần nhất gom sai là khi nào, hậu quả là gì? |
| 5 |Đỗ Duy Bộ|Khi cần làm theo một quy trình nội bộ, tôi muốn tìm được hướng dẫn đúng và còn hiệu lực, để hoàn thành công việc mà không phải hỏi đồng nghiệp nhiều lần.|Nhân viên|hỏi đồng nghiệp 6 lần và chờ trả lời, ~15 phút, vì tài liệu không ghi ngày hiệu lực và người phụ trách | Đạt: Vì sao bạn xác định nguyên nhân là thiếu ngày hiệu lực và người phụ trách? Có trường hợp tài liệu đủ hai thông tin này nhưng vẫn phải hỏi không? |
| 6 |Đỗ Duy Bộ|Khi bàn giao công việc, tôi muốn nắm được các quyết định, tài liệu và tiến độ liên quan, để tiếp nhận việc mà không phải hỏi lại từ đầu.|Nhân viên nhận bàn giao việc từ đồng nghiệp| đọc lại lịch sử chat/email để biết quyết định nào đã chốt và vì sao, ~12 phút |Cường:Việc nhận bàn giao này diễn ra với tần suất nào (hàng ngày hay chỉ vài tháng một lần khi có người nghỉ/chuyển dự án)? 12 phút đọc lịch sử có đủ lớn để giải quyết so với các công việc lặp đi lặp lại hàng ngày không |
| 7 | Nguyễn Minh Đạt | Khi bắt đầu bài lab hằng ngày, tôi muốn tìm đúng đề bài và phiên bản yêu cầu hiện hành, để bắt đầu làm đúng bài mà không phải hỏi lại | Học viên | Tìm tin nhắn hoặc đường dẫn đề bài: ước lượng 3 phút/lần trong tổng 5 phút |Bộ: Bạn thường tìm đề bài lab ở đâu? Bạn mất bao lâu để tìm đúng đề bài? Bạn đã từng tìm nhầm hoặc dùng nhầm phiên bản đề bài chưa? |
| 8 | Nguyễn Minh Đạt | Khi chuẩn bị nộp bài lab mỗi tối, tôi muốn biết bài đã đáp ứng đủ yêu cầu nội dung và quy cách nộp, để tránh bị trừ điểm vì thiếu mục hoặc đặt tên sai | Học viên trực tiếp hoàn thiện và nộp bài lab | Đối chiếu từng yêu cầu với phần tương ứng trong bài: ước lượng 20 phút/bài |Cường: Trong 20 phút đấy thao tác nào tốn công nhất (đọc chữ, kiểm tra tên file, hay so sánh code)? |
| 9 | Nguyễn Minh Đạt | Khi tiếp nhận repo bài lab có nhiều tài liệu, tôi muốn xác định rõ đầu ra phải nộp và tiêu chí hoàn thành, để triển khai đúng ngay từ đầu và tránh sửa lại vì bỏ sót yêu cầu | Học viên lần đầu đọc repo của một bài lab | Đọc lại và tổng hợp yêu cầu: ước lượng 5-7 phút/bài. Dấu hiệu đã ghi nhận là phải đọc lại 2–3 lần/bài |Bộ: Bạn đã từng bỏ sót yêu cầu hoặc phải sửa bài vì hiểu sai đề chưa?|
| 10 |Nguyễn Đăng Doanh |Khi bước security scan trong pipeline trả về danh sách lỗ hổng, tôi muốn biết cái nào thật sự phải xử lý trước, để không chặn release và không bỏ sót lỗ hổng nghiêm trọng |Devops, Team Lead |Tra và đánh giá ngữ cảnh từng CVE: 65 phút/lần scan |Cường 65 phút/lần scan đang tính cho bao nhiêu mã CVE? Tần suất scan là bao nhiêu lần một tuần, và 65 phút này có thực sự làm chậm thời gian release sản phẩm hay nhóm chỉ rà soát định kỳ? |
| 11 |Nguyễn Đăng Doanh |Khi pipeline CI của một PR bị fail, tôi muốn biết nhanh fail do code, do test hay do hạ tầng, để trả lời dev và re-run hoặc sửa đúng chỗ |Dev, DevOps |Đọc log dài để tìm lỗi gốc: ~15 phút/lần |Bộ: Tuần qua có bao nhiêu lần CI fail, và trong đó bao nhiêu lần do code, do test, do hạ tầng? Lỗi hạ tầng có hay lặp lại cùng vài thông báo trong log không?|
| 12 |Nguyễn Đăng Doanh |Khi deploy bản mới lên production, tôi muốn chắc chắn đã làm đủ các bước trước và sau deploy, để không gây sự cố vì quên bước |DevOps |Smoke test thủ công các luồng chính: ~12 phút/lần | Đạt: Vấn đề chính là quên bước hay smoke test mất thời gian? Bằng chứng hiện tại đang nói về thời gian kiểm tra |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Kiểm đủ trước khi giao đi | #1, #8 (kiểm bài trước khi nộp), #12 (kiểm bước trước/sau deploy) | Trước một mốc cố định (nộp bài, deploy), phải tự đối chiếu với một danh sách yêu cầu/bước, dễ sót khi vội |
| B — Tìm và hiểu đúng thông tin hiện hành | #5 (quy trình nội bộ), #6 (bàn giao), #7 (tìm đúng đề bài), #9 (xác định đầu ra phải nộp) | Thông tin cần dùng nằm rải rác ở nhiều nơi, không rõ bản nào còn hiệu lực nên phải đọc lại hoặc hỏi lại |
| C — Phân loại và ưu tiên lượng lớn tín hiệu | #4 (phản ánh khách hàng), #10 (danh sách CVE), #11 (log CI fail) | Phải đọc nhiều đầu vào không có cấu trúc để xếp loại và chọn cái cần xử lý trước |
| D — Câu hỏi lặp lại giữa người với người | #2 (ai làm phần nào), #3 (lỗi git trên Discord) | Cùng một câu hỏi bị hỏi lại nhiều lần vì thông tin không nằm ở chỗ chung ai cũng thấy |

### 2.3. Opportunity Solution Tree rút gọn

```text
OUTCOME: Giảm thời gian DevOps triage kết quả security scan (hiện ~[65] phút/lần scan) mà không để lọt lỗ hổng Critical
├── Opportunity A: Phần lớn finding là nhiễu nhận ra được bằng dấu hiệu rõ ràng (package chỉ dùng lúc build/test, hoặc chưa có bản vá nên chưa thể xử lý), nhưng vẫn phải mở xem từng cái
├── Opportunity B: Với các finding còn lại, muốn biết CVE có thật sự ảnh hưởng hệ thống mình không thì phải tra nhiều nguồn và đọc code, mất nhiều thời gian nhất
└── Opportunity C: Cùng một CVE xuất hiện lại ở nhiều lần scan và nhiều repo, phải đánh giá lại từ đầu vì không tìm lại được lần quyết định trước
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- ✗ "AI tự triage và tự đánh dấu bỏ qua lỗ hổng" → là giải pháp, lại còn vượt boundary (AI tự quyết thay người)
- ✗ "Cần dashboard tổng hợp lỗ hổng" → là tính năng/công cụ, không phải pain
- ✗ "Đổi sang công cụ scan khác ít báo nhầm hơn" → là giải pháp; pain thật nằm ở nhánh A

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #10 Ưu tiên xử lý lỗ hổng sau security scan | 4 | 4 | 3 | 5 | 3 | 5 | 2 | **26** |
| #11 Xác định nguyên nhân CI fail | 4 | 4 | 3 | 4 | 3 | 4 | 3 | 25 |
| #4 Gom phản ánh khách hàng cùng một vấn đề | 4 | 4 | 3 | 2 | 3 | 4 | 2 | 22 |

**Candidate được chọn:** #10 — Khi security scan trả về danh sách lỗ hổng, DevOps muốn biết cái nào thật sự phải xử lý trước, để không chặn release và không bỏ sót lỗ hổng nghiêm trọng.

**Vì sao chọn:**
- Bottleneck lớn nhất trong shortlist: ~65 phút/lần scan, 3 lần/tuần (số liệu của Doanh).
- Hậu quả nghiêm trọng ở cả hai phía: triage chậm thì chặn release; bỏ sót thì để lọt lỗ hổng Critical. Vì vậy Impact được 5.
- So sánh rõ được cả 4 mức: chỉ sửa quy trình, ví dụ ghi lại quyết định cũ theo mã CVE (No AI); lọc nhiễu theo phạm vi build/test và trạng thái bản vá (Rule); đánh giá ngữ cảnh các ca khó có người duyệt (Workflow); tự động bỏ qua hoặc tự sửa (Agent). Mỗi mức giải một phần khác nhau của bài toán.

**Vì sao loại các candidate còn lại:**
- #11 (CI fail): điểm gần bằng #10, nhưng mỗi lần chỉ ~15 phút và chưa có số lần fail/tuần (câu hỏi của Bộ chưa có số liệu trả lời). Hậu quả khi chẩn đoán sai chủ yếu là mất thời gian re-run, nhẹ hơn để lọt lỗ hổng bảo mật.
- #4 (phản ánh khách hàng): bottleneck chỉ ~25 phút/tuần cho 1 người. Khi Doanh hỏi về lần gom sai gần nhất, Bộ chưa đưa được ví dụ cụ thể / ghi đúng câu trả lời thật. Nội dung phản ánh có thông tin cá nhân của khách nên rủi ro về dữ liệu cao. Trong nhóm chỉ Bộ có trải nghiệm.

**Xử lý bất đồng (nếu có):** Bộ ban đầu muốn chọn #4 vì có số liệu của chính mình, nhưng đồng ý chọn #10 vì impact và hậu quả lớn hơn. Nhóm lo #10 chỉ có Doanh hiểu domain, nên thống nhất Doanh giải thích quy trình scan cho cả nhóm và hẹn 2–3 người làm DevOps/dev ngoài nhóm để phỏng vấn ở CP4.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này:

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | |
| Câu nói đáng nhớ nhất (nguyên văn) | |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | |
| Hiện đang xử lý bằng cách nào (workaround)? | |
| Mất bao lâu, bao lần? | |
| Insight / opportunity rút ra | |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| | | | |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| | | | | | |
| | | | | | |
| | | | | | |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | | | |
| Tổng thời gian | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Rủi ro mới phát sinh | | | |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

-

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
