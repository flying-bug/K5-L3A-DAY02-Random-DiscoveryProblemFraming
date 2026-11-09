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

|   # | Người đưa ra      | Candidate (Job Story ngắn)                                                                                                                                                   | Actor                                        | Bottleneck                                                                                                                                           | Câu hỏi phản biện nhận được (ai hỏi)                                                                                                                                                                                        |
| --: | ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|   1 | Phạm Tuấn Cường   | Khi chuẩn bị nộp bài lab, tôi muốn đối chiếu bài mình với RUBRIC, CHECKPOINTS và SUBMISSION cùng lúc, để không mất điểm vì thiếu mục hoặc sai cấu trúc                       | Học viên                                     | 3 file hướng dẫn, khoảng 30 phút rà mỗi lab; lab trước bị trừ điểm vì sai tên file                                                                   | Doanh: 30p rà soát gồm những bước nào, bước nào chiếm nhiều thời gian?                                                                                                                                                      |
|   2 | Phạm Tuấn Cường   | Khi tới tối Chủ nhật, tôi muốn biết tuần tới có những deadline nào, để không bỏ sót bài nộp                                                                                  | Học viên                                     | Deadline nằm rải rác ở LMS, Discord, email; mất khoảng 20 phút/tuần để gom; tháng trước suýt trễ 1 bài vì thông báo đổi hạn nằm trong thread Discord | Đạt: Việc ở bước nào, mất bao nhiêu phút                                                                                                                                                                                    |
|   3 | Phạm Tuấn Cường   | Khi cài môi trường cho lab có code, tôi muốn chạy được code mẫu ngay lần đầu, để không mất thời gian giờ học vì lỗi cài đặt                                                  | Tôi                                          | Lần gần nhất mất 40 phút vì lỗi phiên bản Python; tôi đã gặp                                                                                         | Doanh: Nếu cài đặt thì cần mấy bước, quy trình?                                                                                                                                                                             |
|   4 | Đỗ Duy Bộ         | Khi khách hàng báo lỗi qua nhiều kênh, tôi muốn nhận ra những phản ánh cùng nói về một vấn đề, để biết vấn đề nào đang ảnh hưởng nhiều khách hàng nhất.                      | Nhân viên CSKH                               | đọc ~200 phản ánh và quyết định cái nào cùng một vấn đề, ~25 phút/tuần; khách mô tả cùng một lỗi bằng nhiều cách khác nhau nên dễ gom sai            | Doanh: Con số có khớp nhau không? Lần gần nhất gom sai là khi nào, hậu quả là gì?                                                                                                                                           |
|   5 | Đỗ Duy Bộ         | Khi cần làm theo một quy trình nội bộ, tôi muốn tìm được hướng dẫn đúng và còn hiệu lực, để hoàn thành công việc mà không phải hỏi đồng nghiệp nhiều lần.                    | Nhân viên                                    | hỏi đồng nghiệp 6 lần và chờ trả lời, ~15 phút, vì tài liệu không ghi ngày hiệu lực và người phụ trách                                               | Đạt: Vì sao bạn xác định nguyên nhân là thiếu ngày hiệu lực và người phụ trách? Có trường hợp tài liệu đủ hai thông tin này nhưng vẫn phải hỏi không?                                                                       |
|   6 | Đỗ Duy Bộ         | Khi bàn giao công việc, tôi muốn nắm được các quyết định, tài liệu và tiến độ liên quan, để tiếp nhận việc mà không phải hỏi lại từ đầu.                                     | Nhân viên nhận bàn giao việc từ đồng nghiệp  | đọc lại lịch sử chat/email để biết quyết định nào đã chốt và vì sao, ~12 phút                                                                        | Cường:Việc nhận bàn giao này diễn ra với tần suất nào (hàng ngày hay chỉ vài tháng một lần khi có người nghỉ/chuyển dự án)? 12 phút đọc lịch sử có đủ lớn để giải quyết so với các công việc lặp đi lặp lại hàng ngày không |
|   7 | Nguyễn Minh Đạt   | Khi bắt đầu bài lab hằng ngày, tôi muốn tìm đúng đề bài và phiên bản yêu cầu hiện hành, để bắt đầu làm đúng bài mà không phải hỏi lại                                        | Học viên                                     | Tìm tin nhắn hoặc đường dẫn đề bài: ước lượng 3 phút/lần trong tổng 5 phút                                                                           | Bộ: Bạn thường tìm đề bài lab ở đâu? Bạn mất bao lâu để tìm đúng đề bài? Bạn đã từng tìm nhầm hoặc dùng nhầm phiên bản đề bài chưa?                                                                                         |
|   8 | Nguyễn Minh Đạt   | Khi chuẩn bị nộp bài lab mỗi tối, tôi muốn biết bài đã đáp ứng đủ yêu cầu nội dung và quy cách nộp, để tránh bị trừ điểm vì thiếu mục hoặc đặt tên sai                       | Học viên trực tiếp hoàn thiện và nộp bài lab | Đối chiếu từng yêu cầu với phần tương ứng trong bài: ước lượng 20 phút/bài                                                                           | Cường: Trong 20 phút đấy thao tác nào tốn công nhất (đọc chữ, kiểm tra tên file, hay so sánh code)?                                                                                                                         |
|   9 | Nguyễn Minh Đạt   | Khi tiếp nhận repo bài lab có nhiều tài liệu, tôi muốn xác định rõ đầu ra phải nộp và tiêu chí hoàn thành, để triển khai đúng ngay từ đầu và tránh sửa lại vì bỏ sót yêu cầu | Học viên lần đầu đọc repo của một bài lab    | Đọc lại và tổng hợp yêu cầu: ước lượng 5-7 phút/bài. Dấu hiệu đã ghi nhận là phải đọc lại 2–3 lần/bài                                                | Bộ: Bạn đã từng bỏ sót yêu cầu hoặc phải sửa bài vì hiểu sai đề chưa?                                                                                                                                                       |
|  10 | Nguyễn Đăng Doanh | Khi bước security scan trong pipeline trả về danh sách lỗ hổng, tôi muốn biết cái nào thật sự phải xử lý trước, để không chặn release và không bỏ sót lỗ hổng nghiêm trọng   | Devops, Team Lead                            | Tra và đánh giá ngữ cảnh từng CVE: 65 phút/lần scan                                                                                                  | Cường 65 phút/lần scan đang tính cho bao nhiêu mã CVE? Tần suất scan là bao nhiêu lần một tuần, và 65 phút này có thực sự làm chậm thời gian release sản phẩm hay nhóm chỉ rà soát định kỳ?                                 |
|  11 | Nguyễn Đăng Doanh | Khi pipeline CI của một PR bị fail, tôi muốn biết nhanh fail do code, do test hay do hạ tầng, để trả lời dev và re-run hoặc sửa đúng chỗ                                     | Dev, DevOps                                  | Đọc log dài để tìm lỗi gốc: ~15 phút/lần                                                                                                             | Bộ: Tuần qua có bao nhiêu lần CI fail, và trong đó bao nhiêu lần do code, do test, do hạ tầng? Lỗi hạ tầng có hay lặp lại cùng vài thông báo trong log không?                                                               |
|  12 | Nguyễn Đăng Doanh | Khi deploy bản mới lên production, tôi muốn chắc chắn đã làm đủ các bước trước và sau deploy, để không gây sự cố vì quên bước                                                | DevOps                                       | Smoke test thủ công các luồng chính: ~12 phút/lần                                                                                                    | Đạt: Vấn đề chính là quên bước hay smoke test mất thời gian? Bằng chứng hiện tại đang nói về thời gian kiểm tra                                                                                                             |

### 2.2. Cluster

| Cluster                                     | Các candidate                                                                             | Pattern chung                                                                                             |
| ------------------------------------------- | ----------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| A — Kiểm đủ trước khi giao đi               | #1, #8 (kiểm bài trước khi nộp), #12 (kiểm bước trước/sau deploy)                         | Trước một mốc cố định (nộp bài, deploy), phải tự đối chiếu với một danh sách yêu cầu/bước, dễ sót khi vội |
| B — Tìm và hiểu đúng thông tin hiện hành    | #5 (quy trình nội bộ), #6 (bàn giao), #7 (tìm đúng đề bài), #9 (xác định đầu ra phải nộp) | Thông tin cần dùng nằm rải rác ở nhiều nơi, không rõ bản nào còn hiệu lực nên phải đọc lại hoặc hỏi lại   |
| C — Phân loại và ưu tiên lượng lớn tín hiệu | #4 (phản ánh khách hàng), #10 (danh sách CVE), #11 (log CI fail)                          | Phải đọc nhiều đầu vào không có cấu trúc để xếp loại và chọn cái cần xử lý trước                          |
| D — Câu hỏi lặp lại giữa người với người    | #2 (ai làm phần nào), #3 (lỗi git trên Discord)                                           | Cùng một câu hỏi bị hỏi lại nhiều lần vì thông tin không nằm ở chỗ chung ai cũng thấy                     |

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

| Candidate                                   | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain |   Tổng |
| ------------------------------------------- | -------: | -----------: | -----------------: | -------------: | ----------: | -------------------------------------: | ---------------: | -----: |
| #10 Ưu tiên xử lý lỗ hổng sau security scan |        4 |            4 |                  3 |              5 |           3 |                                      5 |                2 | **26** |
| #11 Xác định nguyên nhân CI fail            |        4 |            4 |                  3 |              4 |           3 |                                      4 |                3 |     25 |
| #4 Gom phản ánh khách hàng cùng một vấn đề  |        4 |            4 |                  3 |              2 |           3 |                                      4 |                2 |     22 |

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

|   # | Giả định                                                                                                                                                 | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước?       |
| --: | -------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------- | ---------------: | ---------------------: | ----------------------- |
|   1 | DevOps/dev ngoài nhóm cũng mất ≥ 30 phút cho mỗi lần triage kết quả security scan, và việc này lặp lại ≥ 1 lần/tuần                                      | Value                                              |                5 |                      2 | ✅ Ưu tiên 1            |
|   2 | Phần lớn finding (≥ 50%) mỗi lần scan là nhiễu nhận ra được bằng dấu hiệu rõ: package chỉ dùng lúc build/test, chưa có bản vá, hoặc trùng lần scan trước | Value                                              |                5 |                      2 | ✅ Ưu tiên 2            |
|   3 | Bước tốn thời gian nhất là đánh giá CVE có thật sự ảnh hưởng hệ thống (chiếm ≥ 1/2 thời gian triage), không phải bước lọc nhiễu                          | Value                                              |                5 |                      1 | ✅ Ưu tiên 3            |
|   4 | Triage chậm đã từng làm trễ release ít nhất 1 lần trong 3 tháng gần nhất                                                                                 | Value                                              |                4 |                      1 | ✅                      |
|   5 | Scanner team đang dùng đã có sẵn tính năng lọc (theo mức nghiêm trọng, bỏ lỗ hổng chưa có bản vá, bỏ qua theo mã CVE) nhưng chưa bật hoặc chưa cấu hình  | Feasibility                                        |                4 |                      1 | ✅                      |
|   6 | Công ty cho phép đưa thông tin lỗ hổng và đoạn code vào công cụ AI bên ngoài                                                                             | Viability                                          |                5 |                      1 | — Hỏi Team Lead sau lab |

_Điền 4–6 giả định; xóa dòng thừa._

Giả định nhóm kiểm chứng trong buổi này: #1 → #5. Cách kiểm: phỏng vấn 2–3 DevOps/dev ngoài nhóm theo The Mom Test, hỏi về lần scan gần nhất: số finding, bao nhiêu cái phải xử lý, thời gian từng bước, có làm trễ release không, đang dùng scanner và bộ lọc nào. Giả định #5 kiểm thêm bằng research (mục 3.3). Giả định #6 chưa kiểm được trong buổi vì cần hỏi Team Lead của công ty.

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường                                            | Nội dung |
| ------------------------------------------------- | -------- |
| Người được hỏi (vai trò, không ghi tên thật)      |          |
| Câu nói đáng nhớ nhất (nguyên văn)                |          |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? |          |
| Hiện đang xử lý bằng cách nào (workaround)?       |          |
| Mất bao lâu, bao lần?                             |          |
| Insight / opportunity rút ra                      |          |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
| ----- | ----------------: | ----------------- | ----------------- |
|       |                   |                   |                   |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern             | Link                                                                                                                | Giải bước nào trong quy trình?                                                                                                                                                       | Điểm mạnh                                                                                       | Khoảng trống / rủi ro                                                                                                                                    | Bài học cho nhóm                                                                                                                       |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| GitHub Dependabot auto-triage rules  | https://docs.github.com/en/code-security/dependabot/dependabot-auto-triage-rules/about-dependabot-auto-triage-rules | Lọc nhiễu: preset tự bỏ qua cảnh báo ít ảnh hưởng của dependency chỉ dùng lúc phát triển (development-scoped)                                                                        | Bật mặc định cho repo public; cảnh báo tự mở lại nếu dependency chuyển sang dùng cho production | Preset chỉ áp dụng cho npm; repo private phải tự bật; tự tạo rule cần license GitHub Code Security/Advanced Security                                     | Lọc nhiễu bằng **Rule** đã có sẵn trên thị trường, không cần AI                                                                        |
| Trivy — lọc kết quả                  | https://trivy.dev/latest/docs/configuration/filtering/                                                              | Lọc nhiễu + lưu quyết định cũ: lọc theo mức nghiêm trọng (`--severity`), bỏ lỗ hổng chưa có bản vá (`--ignore-unfixed`), file `.trivyignore` ghi mã CVE kèm ngày hết hạn, hỗ trợ VEX | Miễn phí; `.trivyignore` có ngày hết hạn, đúng cách lưu quyết định cũ theo mã CVE               | `--ignore-unfixed` ẩn cả lỗ hổng Critical chưa có bản vá, trong khi chúng có thể vẫn cần biện pháp tạm; định dạng YAML và Rego còn thử nghiệm            | Nhánh "đánh giá lại từ đầu" giải được bằng **No AI/Rule**; phải cẩn thận để lọc nhiễu không làm lọt Critical                           |
| FIRST EPSS                           | https://www.first.org/epss/                                                                                         | Ưu tiên: mỗi ngày cho mỗi CVE một xác suất 0–1 bị khai thác trong 30 ngày tới                                                                                                        | Miễn phí, có CSV/API; dùng kết hợp với CVSS để xếp thứ tự                                       | Là xác suất chung trên mọi hệ thống, không biết hệ thống của mình có thật sự gọi tới đoạn code bị lỗi không                                              | Xếp thứ tự bằng **Rule** (CVSS + EPSS) được; phần ngữ cảnh riêng vẫn cần người                                                         |
| Snyk — Priority Score + Reachability | https://docs.snyk.io/scan-fix-and-prevent/fix/prioritize-issues-for-fixing/reachability-analysis                    | Đánh giá ngữ cảnh: chấm điểm ưu tiên dựa trên CVSS, xu hướng, khả năng code gọi tới (reachability), có exploit hay không                                                             | Giải đúng phần khó nhất (nhánh "có thật sự ảnh hưởng không")                                    | GA chỉ cho Java, JS/TS, Python; dùng qua CLI/CI còn Early Access; phải upload mã nguồn; trang ghi rõ "NO PATH FOUND" không có nghĩa là chắc chắn an toàn | Thị trường đã có công cụ làm phần ngữ cảnh, nhưng kết quả **không chắc chắn** nên vẫn cần người duyệt; upload code là rủi ro Viability |

**Kết luận research:** Phần lọc nhiễu và lưu quyết định cũ đã có công cụ làm bằng Rule (Dependabot, Trivy). Phần xếp ưu tiên chung có EPSS miễn phí. Chỉ phần "CVE có thật sự ảnh hưởng hệ thống mình không" là còn mơ hồ: Snyk có làm nhưng kết quả không chắc chắn và phải upload code. Đây là chỗ duy nhất có thể cân nhắc AI, và luôn phải có người duyệt.

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
HIỆN TẠI — 5 bước, khoảng 65 phút/lần scan, 3 lần/tuần, 5/5 bước thủ công
(khoảng 40 finding/lần scan)

[1 Mở báo cáo scan, xuất danh sách finding: 5']
→ [2 Lọc nhiễu thủ công: mở từng finding xem package chỉ dùng build/test, đã có bản vá chưa: 12']
→ [3 Tra lại quyết định cũ trong chat/ticket: 8']
→ [4 Đánh giá ngữ cảnh: đọc advisory, tìm xem code có gọi tới phần bị lỗi không: 30'] ← BOTTLENECK
→ [5 Xếp ưu tiên, tạo ticket cho dev, báo Team Lead nếu chặn release: 10']
```

| Bước | Actor                         | Input                                                                    | Output                                                       | Thời gian / tần suất | Ghi chú                                                                                                             |
| ---: | ----------------------------- | ------------------------------------------------------------------------ | ------------------------------------------------------------ | -------------------- | ------------------------------------------------------------------------------------------------------------------- |
|    1 | DevOps                        | Kết quả scan từ pipeline CI (Trivy/Dependabot)                           | Danh sách khoảng 40 finding (mã CVE, package, mức CVSS)      | 5' · 3 lần/tuần      | Scan chạy tự động, nhưng việc đọc kết quả thì thủ công                                                              |
|    2 | DevOps                        | Danh sách finding, file dependency (`package.json`, `requirements.txt`…) | Khoảng 15 finding còn lại sau khi bỏ nhiễu                   | 12'                  | Nhiễu nhận ra được bằng dấu hiệu rõ nhưng vẫn phải mở từng cái (Opportunity A, giả định #2)                         |
|    3 | DevOps                        | Khoảng 15 finding, lịch sử chat/ticket                                   | Khoảng 10 finding chưa từng đánh giá                         | 8'                   | Quyết định cũ không lưu theo mã CVE nên khó tìm lại; nhiều lúc đánh giá lại từ đầu (Opportunity C)                  |
|    4 | DevOps (hỏi thêm dev khi cần) | Khoảng 10 finding, advisory (NVD, GitHub Advisory), mã nguồn             | Kết luận từng finding: ảnh hưởng / không ảnh hưởng / chưa rõ | 30'                  | Phải tra nhiều nguồn và đọc code (Opportunity B, giả định #3). **Handoff:** hỏi dev phụ trách module khi không chắc |
|    5 | DevOps → Team Lead            | Kết luận bước 4                                                          | Ticket cho dev; quyết định chặn hoặc cho release             | 10'                  | **Handoff:** Team Lead quyết khi có Critical chặn release; quyết định bỏ qua chỉ ghi trong chat                     |

**Bottleneck chính:** Bước 4, đánh giá CVE có thật sự ảnh hưởng hệ thống mình không, mất khoảng 30/65 phút (≈ 46%). Bước 2 và 3 cộng thêm khoảng 20 phút là việc lặp lại, giải được bằng Rule.

_Thời gian từng bước là ước lượng từ con số 65 phút của Doanh. Cần kiểm lại bằng phỏng vấn ở CP4 (giả định #1, #2, #3)._

### 4.2. Quy trình tương lai

```text
TƯƠNG LAI — 5 bước, khoảng 25 phút/lần scan, 2/5 bước thủ công

[1 Lọc nhiễu tự động: bỏ package chỉ dùng build/test, áp quyết định cũ: 1']
     ← RULE (Dependabot auto-triage, Trivy --severity, .trivyignore/VEX có ngày hết hạn)
→ [2 Xếp thứ tự theo CVSS + EPSS: 1']
     ← RULE (script đọc API EPSS)
→ [3 Tóm tắt advisory + chỉ ra chỗ code gọi tới phần bị lỗi, đề xuất "có thể ảnh hưởng / có vẻ không", kèm trích dẫn: 3']
     ← AI (chỉ cho khoảng 10 finding còn lại)
→ [4 DevOps kiểm trích dẫn, quyết định từng finding: 15']
     ← CON NGƯỜI (điểm kiểm soát chính)
→ [5 Tạo ticket, ghi quyết định bỏ qua vào .trivyignore kèm lý do + ngày hết hạn; Team Lead duyệt nếu chặn release: 5']
     ← CON NGƯỜI

BOUNDARY:
- AI không tự đánh dấu bỏ qua finding, không tự sửa code hay nâng version, không tự chặn/mở release.
- Finding Critical/High luôn qua người duyệt, kể cả khi AI nói "không ảnh hưởng".
- Rule không được ẩn Critical chưa có bản vá (không dùng --ignore-unfixed cho Critical);
  các finding này chuyển sang danh sách "cần biện pháp tạm".
- Chưa đưa mã nguồn vào AI bên ngoài khi Team Lead chưa cho phép (giả định #6).

PHƯƠNG ÁN QUAY VỀ:
- AI sai hoặc không chạy → DevOps tự đánh giá như bước 4 cũ; Rule ở bước 1–2 vẫn giữ nguyên.
- Quyết định bỏ qua hết hạn → finding tự hiện lại ở lần scan sau, DevOps đánh giá lại.
```

Nếu chỉ dùng Rule (bỏ bước 3 AI), thời gian ước lượng còn khoảng 40 phút: bước 2 và 3 cũ gần như biến mất, nhưng bước đánh giá ngữ cảnh vẫn nguyên 30 phút. Số này dùng để so sánh các mức ở CP6.

### 4.3. Before / after

| Chỉ số               |                   Trước |                                                                                                                                                      Sau (kỳ vọng) | Ghi chú                                                                                                                               |
| -------------------- | ----------------------: | -----------------------------------------------------------------------------------------------------------------------------------------------------------------: | ------------------------------------------------------------------------------------------------------------------------------------- |
| Số bước              |                       5 |                                                                                                                                                                  5 | Số bước giữ nguyên, nhưng 2 bước lọc/tra cũ chuyển sang Rule                                                                          |
| Tổng thời gian       |   65'/lần · ≈ 195'/tuần |                                                                                                                                             ≈ 25'/lần · ≈ 75'/tuần | Chỉ Rule: khoảng 40'/lần                                                                                                              |
| Số bước thủ công     |                     5/5 |                                                                                                                                                                2/5 | Con người vẫn quyết định và tạo ticket                                                                                                |
| Bottleneck chính     | Đánh giá ngữ cảnh (30') |                                                                                                                                  DevOps duyệt đề xuất của AI (15') | Chấp nhận được vì đây là điểm kiểm soát để không lọt Critical                                                                         |
| Rủi ro mới phát sinh |                       — | AI kết luận "không ảnh hưởng" sai → bỏ sót lỗ hổng; Rule lọc quá tay làm ẩn Critical; quyết định bỏ qua hết hạn mà không ai xem; lộ mã nguồn khi dùng AI bên ngoài | Xử lý bằng boundary (Critical/High luôn qua người, không ẩn Critical chưa có bản vá), ngày hết hạn và hỏi Team Lead trước khi dùng AI |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** |DevOps engineer phụ trách tích hợp dependency/container scan vào CI/CD ở một team phát triển ~20–50 dev; gián tiếp là dev chủ repo nhận ticket sửa lỗ hổng |
| **Quy trình** |Mỗi lần scan chạy trên nhánh main hoặc trước release (3 lần/tuần): mở report → lọc High/Critical → đánh giá từng CVE → đánh dấu bỏ qua hoặc tạo ticket → quyết định chặn hay cho release → ghi lại ngoại lệ |
| **Bottleneck** |Bước đánh giá ngữ cảnh từng finding High/Critical (CVE có thật sự ảnh hưởng hệ thống mình không): ~30 trên tổng ~65 phút mỗi lần |
| **Impact** |DevOps mất ~2–2,5 giờ/tuần cho việc lặp lại; ~2 lần/tháng release bị chặn bởi finding sau đó được xác định là không ảnh hưởng; khi có quá nhiều cảnh báo, lỗ hổng thật dễ bị bỏ sót và dev mất niềm tin vào scan |
| **Success Metric** (baseline → target, cách đo) |(1) Thời gian triage: ~65'/lần → dưới 20'/lần; đo bằng DevOps tự ghi thời gian mỗi lần scan trong 4 tuần. (2) Release bị chặn oan (finding chặn release, sau đó được đánh dấu "không ảnh hưởng"): ~2/tháng → 0; đếm qua lịch sử pipeline và ignore file. (3) Guardrail: 0 finding Critical có bản vá bị bỏ qua sai; rà lại toàn bộ finding bị bỏ qua vào cuối mỗi tuần. Baseline hiện là ước lượng, sẽ bấm giờ lại ở 2 lần scan tới. |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) |Không tự bỏ qua finding, không tự cho qua hay chặn release, không tự sửa ignore file hay ticket, không truy cập secret/dữ liệu production. Mọi finding không bị quy tắc cố định lọc phải được DevOps xác nhận; finding Critical bị đánh giá "không ảnh hưởng" cần lead duyệt; mọi ngoại lệ có hạn tối đa 90 ngày |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

- Baseline là ước lượng của một người. Đồng ý. Đã ghi rõ trong metric; sẽ thay bằng số bấm giờ thật và số từ phỏng vấn ở CP4.
- Metric thời gian có thể "đạt" bằng cách bỏ qua hết cảnh báo. Đồng ý. Đã thêm metric guardrail (3): không bỏ qua sai finding Critical có bản vá.
- "Release bị chặn oan" chưa có định nghĩa, khó đếm. Đồng ý. Đã định nghĩa là finding đã chặn release nhưng sau đó được đánh dấu "không ảnh hưởng".
- Boundary trong v0 đã nhắc tới AI, có phải đang lẫn giải pháp vào problem không? Không đồng ý. Template yêu cầu trường Boundary ghi AI không được làm gì; các trường Actor, Quy trình, Bottleneck, Impact, Metric không chứa giải pháp nào.

---

## 6. Mức can thiệp AI (CP6)


### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: Độ mơ hồ cao × Độ phức tạp cao — đánh giá sơ bộ.

Vì sao:

Mơ hồ cao: Đánh giá một CVE có ảnh hưởng đến hệ thống phụ thuộc vào phiên bản, cách sử dụng dependency và môi trường triển khai. Thông tin có thể thiếu hoặc mâu thuẫn; không thể chỉ dựa vào mức độ nghiêm trọng để kết luận.

Phức tạp cao: Quy trình dự kiến gồm đọc kết quả scan → đối chiếu quyết định cũ → tra thông tin CVE → xem ngữ cảnh hệ thống → đề xuất ưu tiên → người phụ trách duyệt. Dữ liệu đến từ nhiều nguồn và các bước phụ thuộc nhau.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Chuẩn hóa checklist triage; lưu quyết định theo CVE, dependency, phiên bản, ngữ cảnh, người duyệt và thời hạn xem lại. | Thời gian chủ yếu mất vì thiếu quy trình hoặc không tìm lại được quyết định cũ. | Tái sử dụng quyết định đã hết phù hợp; thông tin không được cập nhật. | Là nền tảng cho mọi phương án. |
| **Rule** | Chuẩn hóa và đối chiếu finding trùng; đánh dấu trường hợp cần kiểm tra; xếp thứ tự sơ bộ theo tiêu chí đã thống nhất. Giữ được danh sách đầy đủ để người duyệt xem. | Tiêu chí rõ và xử lý được phần lớn trường hợp mà không cần đọc hiểu ngữ cảnh phức tạp. | Quy tắc sai hoặc lọc quá mạnh khiến finding quan trọng bị ẩn. | Làm đối chứng trước |
| **Workflow** | Rule xử lý dữ liệu có cấu trúc → AI tổng hợp bằng chứng và thông tin còn thiếu → DevOps kiểm tra, quyết định ưu tiên. | Sau khi áp dụng Rule, việc đọc và tổng hợp ngữ cảnh vẫn là bottleneck đáng kể. | AI diễn giải sai, dẫn nguồn không khớp hoặc kết luận quá mức từ dữ liệu thiếu. | Đề xuất thử có điều kiện. |
| **Agent** | AI tự chọn bước tra cứu tiếp theo và công cụ trong phạm vi được cấp; người phụ trách vẫn duyệt quyết định cuối. | Các ca thực tế đòi hỏi đường đi linh hoạt mà Workflow định sẵn không đáp ứng được. | Khó kiểm soát phạm vi truy cập, số lượt thực hiện, chi phí và chuỗi suy luận sai. | Chưa chọn |

**Mức chọn:** Đề xuất Workflow có AI hỗ trợ tổng hợp bằng chứng, chưa đưa vào vận hành thực tế.

**Vì sao không chọn mức đơn giản hơn:** No AI và Rule có thể giải quyết phần chuẩn hóa, đối chiếu và lưu quyết định. Giả thuyết còn cần kiểm chứng là phần đọc hiểu ngữ cảnh riêng của hệ thống vẫn chiếm nhiều thời gian sau các cải tiến này. Nếu thử nghiệm cho thấy No AI hoặc Rule đã đạt mục tiêu, nhóm sẽ chọn mức đó và bỏ bước AI. Hiện chưa đủ bằng chứng để khẳng định Workflow tốt hơn.
 

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Tổng hợp bằng chứng, thông tin còn thiếu và đề xuất ưu tiên từng finding; dẫn nguồn, không tự kết luận khi thiếu dữ liệu. |
| **Judgment** — con người cân nhắc, quyết định gì? | DevOps kiểm tra; người có thẩm quyền quyết định ưu tiên và chấp nhận rủi ro. |
| **Action** — hành động cuối cùng là gì, ai làm? | DevOps cập nhật triage/ticket sau duyệt. AI không tự bỏ qua cảnh báo, sửa code hoặc cho phép release. |
| **Outcome** — đo kết quả bằng gì? | Mục tiêu giảm ≥30% thời gian triage; không bỏ sót Critical trong tập đánh giá. Baseline 65 phút/lần cần đo lại; tính cả thời gian review. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Kết quả scan, CVE, phiên bản dependency, ngữ cảnh hệ thống và quyết định cũ. Chưa xác nhận đủ dữ liệu và quyền sử dụng. |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Ghi chỉnh sửa của người duyệt và lỗi trên tập mẫu để cải thiện prompt, rule và đầu vào. |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng: Chọn augment: AI soạn nháp phần nhận định từ dữ liệu có sẵn; PM/PO kiểm tra, chỉnh sửa và gửi. Phỏng vấn cho thấy 2/3 người mất nhiều thời gian nhất ở phần narrative. Tuy nhiên, chưa có bằng chứng họ muốn giao hoàn toàn việc viết hoặc leadership chấp nhận bản nháp AI. Với team chỉ cần số liệu, ưu tiên template + dashboard.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào: Ưu tiên tránh bỏ sót rủi ro/blocker có trong dữ liệu, vì có thể khiến leadership chậm can thiệp. Đây là đánh giá sơ bộ, cần xác nhận thêm với người dùng. Mỗi nhận định phải dẫn nguồn; thiếu thông tin phải ghi rõ. PM/PO đối chiếu rủi ro và số liệu trước khi gửi; AI không tự sửa số liệu hoặc gửi báo cáo.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường                                          | Nội dung                        |
| ----------------------------------------------- | ------------------------------- |
| **Actor**                                       |                                 |
| **Quy trình**                                   |                                 |
| **Bottleneck**                                  |                                 |
| **Impact**                                      |                                 |
| **Success Metric** (baseline → target, cách đo) |                                 |
| **Boundary**                                    |                                 |
| **AI intervention point**                       |                                 |
| **Mức chọn**                                    | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra**                     |                                 |

**Thay đổi so với v0 và lý do:**

| Trường | v0  | v1  | Vì sao đổi |
| ------ | --- | --- | ---------- |
|        |     |     |            |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

|   # | Tiêu chí | Đạt khi | Không đạt khi |
| --: | -------- | ------- | ------------- |
|   1 |          |         |               |
|   2 |          |         |               |
|   3 |          |         |               |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro          | Câu hỏi                                                           | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
| --------------- | ----------------------------------------------------------------- | ----------------------------------------------------- | ------------------ |
| **Value**       | Người dùng có thật sự cần và sẽ dùng không?                       |                                                       |                    |
| **Usability**   | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? |                                                       |                    |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không?                     |                                                       |                    |
| **Viability**   | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành?     |                                                       |                    |

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
