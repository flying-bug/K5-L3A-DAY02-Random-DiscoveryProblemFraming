# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Đăng Doanh 
- MSSV: 2A202603597
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Random
- Link repo nhóm:

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Lặp lại|Khi pipeline CI của một PR bị fail, tôi muốn biết nhanh fail do code, do test hay do hạ tầng, để trả lời dev và re-run hoặc sửa đúng chỗ |DevOps, Dev|Dev hỏi "sao pipeline fail" 5-7 lần 1 tuần; mỗi lần đọc log và xác định lỗi mất 15'-20' |
| 2 |Lặp lại|Khi deploy bản mới lên production, tôi muốn chắc chắn đã làm đủ các bước trước và sau deploy, để không gây sự cố vì quên bước (backup, kiểm config, smoke test)|DevOps, Team Dev, User |3 lần deploy/tuần, mỗi lần 30', 3-5 sự cố/tháng do quên hoặc sai bước |
| 3 |Tốn thời gian|Khi bước security scan trong pipeline trả về danh sách lỗ hổng, tôi muốn biết cái nào thật sự phải xử lý trước, để không chặn release và không bỏ sót lỗ hổng nghiêm trọng |DevOps, Team Lead |Mỗi lần scan ra 8-10 findings High/Critical; triage mất 60'/lần, 2-3 lần/tuần; 2 lần release bị chặn tháng qua |
| 4 |Tốn thời gian|Khi build Docker image trong CI chạy chậm, tôi muốn biết bước nào trong build tốn thời gian nhất, để dev không phải chờ lâu mới có kết quả |DevOps, Dev |Mỗi build mất 30', 6-10 build/ngày|
| 5 |Lặp lại|Khi certificate, token hoặc license sắp hết hạn, tôi muốn được biết trước đủ sớm, để gia hạn trước khi service lỗi |DevOps, User|Đang quản lý 30 cert/token, 2 sự cố do hết hạn trong nửa năm|
| 6 |Cần đọc, tổng hợp nhiều thông tin |Khi cần sửa một pipeline/job cũ không có tài liệu, tôi muốn hiểu nó làm gì và phụ thuộc vào gì, để sửa mà không làm hỏng chỗ khác |DevOps |3 lần/tháng, mỗi lần đọc yaml và script mất 30'|
| 7 |Pain từ người khác |Khi dev cần thêm biến môi trường hoặc secret cho service, họ muốn biết gửi yêu cầu cho ai và bao lâu xong, để không bị block |Dev, DevOps |6-10 yêu cầu/tuần, mỗi yêu cầu cần 10p xử lý |
| 8 |Pain từ người khác |Khi có nhân viên mới vào team, họ muốn biết cách truy cập vào các môi trường và quy trình deploy |Người mới, DevOps |Onboarding mất ~ 3 ngày, trả lời 15 câu hỏi lặp lại cho mỗi người |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.
- Giữ ý #8 do AI gợi ý, vì đã gặp trong công việc 
- Bỏ ý "AI agent tự động vận hành và tự sửa toàn bộ hệ thống" vì quá rộng và nhiều rủi ro với production

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |Triage kết quả security scan trong pipeline (#3) |Gắn với việc đang làm hằng tuần; quy trình rõ; có cả phần đúng/sai rõ và phần cần đánh giá ngữ cảnh, nên so sánh được Rule và Workflow |Rule theo severity + bản fix có thể đã giải được phần lớn; chưa có số liệu về tỉ lệ cảnh báo không áp dụng |
| 2 |Xác định nguyên nhân pipeline CI fail (#1) |Lặp lại nhiều lần mỗi tuần, nhiều dev bị ảnh hưởng |Bottleneck thật có thể là thiếu quy ước xử lý test flaky chứ không phải đọc log |
| 3 |Làm đủ các bước khi deploy production (#2) |Sự cố production có impact lớn, quy trình cố định |Nhiều khả năng chỉ cần checklist và script, không có gì để AI làm |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi bước dependency/container scan trong pipeline trả về danh sách lỗ hổng, tôi muốn biết cái nào thật sự phải xử lý trước, để không chặn release vì cảnh báo không áp dụng và không bỏ sót lỗ hổng nghiêm trọng |
| Actor |DevOps phụ trách tích hợp security scan vào CI/CD; dev nhận ticket sửa |
| Thời điểm / bối cảnh |Mỗi lần scan chạy trên nhánh main hoặc trước khi release |
| Quy trình hiện tại (3–7 bước) |1. Pipeline chạy scan → 2. Mở report, lọc theo severity → 3. Với từng finding High/Critical: tra CVE, kiểm package có thật sự được dùng ở runtime không, có bản fix chưa → 4. Đánh dấu "không áp dụng/chấp nhận rủi ro" hoặc tạo ticket cho dev → 5. Quyết định chặn hay cho release → 6. Ghi lại ngoại lệ |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 3, tra và đánh giá ngữ cảnh từng CVE: 65' phút/lần scan |
| Impact (nếu không giải thì sao) | Release bị chặn oan hoặc lỗ hổng thật bị lọt; dev dần bỏ qua cảnh báo vì quá nhiều; tôi mất 2-3 giờ/tuần cho việc lặp lại|
| Success metric (baseline → target) |Thời gian triage: ~60 phút/lần → dưới 20 phút/lần; số lần release bị chặn vì cảnh báo không áp dụng: 2/tháng → 0|
| Phương án không dùng AI |Policy cố định trong pipeline: chỉ chặn Critical/High có bản fix và nằm trong dependency runtime; file ignore bắt buộc có lý do và ngày hết hạn|
| Giả thuyết về AI (nếu có) |Rule xử lý phần lớn; với phần còn lại, Workflow: AI tóm tắt CVE và gợi ý mức ưu tiên theo ngữ cảnh repo, DevOps quyết định ignore hay release |
| Cảm nhận nhanh | Rule, có thể thêm Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 60'/lần scan, 5-7 lần/tuần

[Pipeline chạy scan: 10' (tự động)] → [Mở report, lọc severity: 5']
→ [Tra CVE + đánh giá ngữ cảnh từng finding: 30'] ← BOTTLENECK
→ [Đánh dấu / tạo ticket: 10'] → [Quyết định chặn/cho release: 3'] → [Ghi ngoại lệ: 2']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi pipeline CI của một PR bị fail, tôi muốn biết nhanh fail do code, do test flaky hay do hạ tầng, để trả lời dev và re-run hoặc sửa đúng chỗ |
| Actor |DevOps engineer; dev chủ PR |
| Thời điểm / bối cảnh | Giờ làm việc, khi dev ping trên chat sau khi pipeline đỏ|
| Quy trình hiện tại (3–7 bước) |1. Dev ping báo pipeline fail → 2. Mở job log → 3. Đọc log tìm dòng lỗi gốc → 4. Phân loại: lỗi code / test flaky / hạ tầng → 5. Re-run, báo dev sửa, hoặc sửa runner → 6. Trả lời dev |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 3, đọc log dài để tìm lỗi gốc: ~10 phút/lần |
| Impact (nếu không giải thì sao) | Dev bị block chờ trả lời; tôi bị ngắt việc ~6 lần/tuần|
| Success metric (baseline → target) |Thời gian từ lúc dev ping đến lúc biết nguyên nhân: ~18 phút → dưới 5 phút; số lần dev phải ping: ~6/tuần → 3/tuần. Đếm qua tin nhắn trong 2 tuần |
| Phương án không dùng AI |Trang "lỗi CI thường gặp và cách xử lý"; quy ước gắn tag test flaky; dashboard tình trạng runner |
| Giả thuyết về AI (nếu có) |Rule: regex nhận diện các pattern lỗi đã biết và comment phân loại lên PR. AI chỉ cần cho lỗi lạ chưa có pattern |
| Cảm nhận nhanh | Rule |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 18 phút/lần, ~6 lần/tuần

[Dev ping] → [Mở job log: 2'] → [Đọc log tìm lỗi gốc: 10'] ← BOTTLENECK
→ [Phân loại nguyên nhân: 3'] → [Re-run / báo dev / sửa runner: 2'] → [Trả lời dev: 1']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi deploy bản mới lên production, tôi muốn chắc chắn đã làm đủ các bước trước và sau deploy, để không gây sự cố vì quên bước |
| Actor | DevOps Engineer|
| Thời điểm / bối cảnh |Mỗi lần release, 3–4 lần/tuần |
| Quy trình hiện tại (3–7 bước) |1. Nhận yêu cầu deploy → 2. Kiểm config và secret môi trường → 3. Backup DB/snapshot nếu có migration → 4. Chạy deploy → 5. Smoke test thủ công → 6. Theo dõi metric sau deploy → 7. Thông báo team |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 5, smoke test thủ công các luồng chính: ~12 phút/lần |
| Impact (nếu không giải thì sao) |Sự cố production, phải rollback; tháng qua 1 lần |
| Success metric (baseline → target) |Số sự cố do quên/sai bước: ~1/tháng → 0; thời gian một lần deploy: ~40 → dưới 25 phút. Đo qua lịch sử deploy và postmortem trong 4 tuần |
| Phương án không dùng AI |Runbook/checklist bắt buộc trong template release; người thứ hai xác nhận trước khi deploy production |
| Giả thuyết về AI (nếu có) |Không cần AI: smoke test script tự chạy sau deploy và tự rollback khi health check fail là Rule |
| Cảm nhận nhanh | No AI / Rule  |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 40 phút/lần deploy

[Nhận yêu cầu] → [Kiểm config/secret: 5'] → [Backup/snapshot: 5'] → [Chạy deploy: 8']
→ [Smoke test thủ công: 12'] ← BOTTLENECK → [Theo dõi metric: 8'] → [Thông báo team: 2']
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Đây là việc tôi trực tiếp làm hằng tuần nên có số liệu thật; bài toán có cả phần Rule giải được rõ ràng và phần cần đánh giá ngữ cảnh, nên nhóm sẽ phải lập luận thật sự giữa Rule và Workflow thay vì nhảy thẳng sang AI.
- Câu hỏi muốn nhóm phản biện: Một policy cố định (severity + có bản fix + dependency runtime) đã đủ chưa, hay phần tốn thời gian thật là đánh giá ngữ cảnh mà rule không làm được?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card #1: "security scan" quá rộng, SAST, dependency scan và container scan có quy trình triage khác nhau | Đồng ý | Thu hẹp còn dependency/container scan, vì cả hai đều dựa trên CVE nên quy trình tra cứu giống nhau |
| Card #1: chưa có baseline về số cảnh báo không áp dụng, nên chưa chứng minh được pain | Đồng ý | Thêm metric "số lần release bị chặn vì cảnh báo không áp dụng", đo qua lịch sử pipeline |
| Card #1: policy theo severity và bản fix có thể giải phần lớn, đang nhảy sang AI quá sớm | Đồng ý một phần | Đổi cảm nhận nhanh từ Workflow sang Rule trước; Workflow chỉ cho phần rule không xử lý được |
| Card #2: bottleneck có thể là thiếu quy ước test flaky, không phải bước đọc log | Chưa chắc | Ghi vào "điều còn chưa chắc", sẽ hỏi nhóm khi pitch |
| Card #3: đây là vấn đề quy trình, không có gì để AI dự đoán | Đồng ý | Giữ cảm nhận No AI / Rule, ghi rõ giải pháp là checklist + script |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card |Pitch 3 card: #10 triage kết quả security scan, #11 xác định nguyên nhân CI fail, #12 làm đủ các bước khi deploy production. Đưa 3 card vào bảng pitch  |#10 được nhóm chọn làm candidate cuối |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: với Cường #1 "30 phút rà soát gồm những bước nào, bước nào chiếm nhiều thời gian?"; với Cường #3 "Nếu cài đặt thì cần mấy bước, quy trình thế nào?"; với Bộ #4 "Con số ~200 phản ánh trong ~25 phút/tuần có khớp nhau không? Lần gần nhất gom sai là khi nào, hậu quả là gì?"  |Câu hỏi với #4 cho thấy số liệu chưa khớp và chưa có ví dụ gom sai cụ thể; đây là một trong các lý do nhóm loại #4 ở mục 2.4 |
| Nhận phản biện | Câu hỏi tôi nhận được: Cường hỏi #10 "65 phút/lần scan đang tính cho bao nhiêu mã CVE? Tần suất bao nhiêu lần/tuần? Có thật sự làm chậm release không?"; Bộ hỏi #11 "Tuần qua bao nhiêu lần CI fail, bao nhiêu do code/test/hạ tầng?"; Đạt hỏi #12 "Vấn đề chính là quên bước hay smoke test mất thời gian?"| Tôi đã sửa gì: với #10, tách 65 phút thành 5 bước có số phút, ghi rõ ~40 finding/lần, 3 lần/tuần, và chỉ ra bottleneck thật là bước đánh giá ngữ cảnh ~30 phút chứ không phải cả 65 phút (mục 4.1). Với #12, nhận ra bằng chứng của mình đang nói về thời gian chứ không phải việc quên bước, nên card này yếu hơn và không đưa vào shortlist|
| Gom cluster / cây OST |Viết cây OST ở mục 2.3 cho bài security scan: 1 outcome, 3 opportunity, gạch bỏ 3 ý là solution đội lốt |Cây OST làm nền cho việc tách phần Rule giải được (nhánh A, C) và phần còn mơ hồ (nhánh B) ở CP5–CP6 |
| Chọn candidate problem |Giải thích quy trình scan cho cả nhóm vì chỉ tôi làm DevOps; cung cấp số liệu baseline cho #10 |Nhóm chọn #10; Bộ ban đầu muốn chọn #4 nhưng đồng ý #10 vì impact lớn hơn |
| Kiểm chứng / research |Chuẩn bị bộ câu hỏi phỏng vấn theo The Mom Test cho DevOps/dev ngoài nhóm. Phần research công cụ ở mục 3.3 do Bộ phụ trách |Chưa phỏng vấn được người ngoài nhóm trong buổi lab; đây là điểm yếu nhất của bài nhóm |
| Quy trình nhóm |Cùng Cường viết mục 4: quy trình hiện tại, quy trình tương lai, bảng before/after |Quy trình cho thấy chỉ dùng Rule còn ~40 phút/lần, chưa đạt target 30 phút; con số này là lập luận chính cho mức Workflow ở CP6 |
| Problem Statement |Góp phần viết Problem Statement v0 (mục 5); rà lại v0 và v1 cho khớp với quy trình ở mục 4|Sửa các chỗ v0 lệch với 4.1 (số bước, bottleneck, Impact ~3 giờ/tuần) |
| Mức can thiệp AI |Góp ý mục 6.1 và 6.2: đổi ô ma trận sang "mơ hồ cao × phức tạp thấp", bổ sung lý do vì sao không chọn mức đơn giản hơn và vì sao không chọn Agent |Mục 6 nhất quán với lựa chọn Workflow 2 giai đoạn ở mục 7 |
| Quyết định |Góp ý quyết định Not Yet cho bước AI, Go cho phần Rule, và các ngưỡng dừng |Quyết định khớp với rủi ro Viability mức Cao (chưa biết công ty có cho đưa mã nguồn vào AI bên ngoài không) |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Nhờ Claude soạn nháp bảng scan từ bối cảnh công việc DevOps của tôi | Viết đúng dạng Job Story, trải đủ 4 lăng kính | Không biết số liệu thật, tự ước lượng theo mức "điển hình" | Thay bằng ước lượng từ công việc của tôi, bỏ các ý không đúng với hệ thống công ty |
| CP2 Problem Card | Nhờ Claude soạn nháp card và đóng vai PM hoài nghi phản biện | Chỉ ra "security scan" quá rộng, thiếu baseline, nhảy sang AI quá sớm | Số liệu trong card lệch với số liệu nhóm dùng sau này | Thu hẹp còn dependency/container scan; đổi cảm nhận từ Workflow về Rule; sửa số cho khớp báo cáo nhóm |
| CP3 Pitch / OST | Nhờ Claude gợi ý câu hỏi phản biện và soạn nháp cây OST, bảng chấm điểm. Lab quy định CP3 tự pitch và tự phản biện; tôi ghi lại để minh bạch | Câu hỏi bám đúng lỗi hay gặp: bottleneck ghi số liệu thay vì một bước | Bảng chấm điểm soạn trên shortlist khác với shortlist cuối của nhóm | Nhóm tự chấm lại #10, #11, #4 và tự viết lý do loại |
| CP4 Research | Nhờ Claude tìm công cụ đã có (Dependabot, Trivy, EPSS) và soạn câu hỏi phỏng vấn | Tìm ra phần lọc nhiễu đã có công cụ giải bằng Rule | Không thay được phỏng vấn người thật | Tự mở kiểm từng link; ghi rõ nhóm chưa phỏng vấn được người ngoài nhóm |
| CP5 Quy trình | Nhờ Claude soạn nháp quy trình trước/sau và Problem Statement v0 | Chia rõ bước Rule / AI / con người, có boundary và phương án quay về | Bản nháp có 6 bước và target dưới 20'/lần, không đạt được với chính quy trình tương lai (~25') | Nhóm vẽ lại 5 bước theo thực tế; đổi target thành ≤ 30'/lần |
| CP5–6 Problem Statement | Nhờ Claude rà soát v0, v1 và tiêu chí đánh giá | Phát hiện mâu thuẫn giữa mục 4, 5, 6, 7 (số bước, Impact, mức chọn) | Một số đề xuất dùng lại số liệu cũ | Đối chiếu từng con số với mục 4.1 trước khi sửa |
| CP6 Mức can thiệp / quyết định | Nhờ Claude soạn nháp 4 rủi ro, quyết định và ngưỡng dừng | Gợi ý tách Go cho Rule, Not Yet cho bước AI | Chọn ô ma trận vẫn phải tự lập luận; bản đầu của nhóm xếp sai ô | Đổi sang "mơ hồ cao × phức tạp thấp" vì các bước cố định, chỉ còn một bước mơ hồ |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Phần lớn problem của Cường và Đạt xoay quanh việc nộp bài lab, còn của Bộ là công việc CSKH và tài liệu nội bộ. Khi gom cluster, tôi thấy problem của mình (#10, #11) và của Bộ (#4) thực chất cùng một kiểu: phải đọc rất nhiều đầu vào không có cấu trúc để chọn ra cái cần xử lý trước. Lĩnh vực khác nhau nhưng pattern giống nhau, và điều này giúp nhóm hiểu bài security scan dù chỉ tôi làm DevOps. Tôi cũng nhận ra nhiều card, kể cả card của tôi, ghi số liệu vào cột bottleneck thay vì chỉ ra một bước cụ thể.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Có. Khi viết cây OST, tầng opportunity ban đầu có các ý như "AI tự triage và đánh dấu bỏ qua lỗ hổng", "cần dashboard tổng hợp lỗ hổng", "đổi sang công cụ scan khác". Nhóm đối chiếu với quy tắc "thấy tên công cụ, tính năng hay chữ AI ở tầng này thì gạch bỏ" và chuyển chúng xuống danh sách solution đội lốt. Sau đó research cho thấy Dependabot và Trivy đã làm được phần lọc nhiễu, nên nhóm thu hẹp chỗ cần AI xuống đúng một bước đánh giá ngữ cảnh thay vì cả quy trình triage.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Có. Khi pitch #10, tôi ghi bottleneck là "tra và đánh giá ngữ cảnh từng CVE: 65 phút/lần". Cường hỏi 65 phút đó tính cho bao nhiêu CVE, mấy lần một tuần, và có thật sự làm chậm release không. Tôi không trả lời được ngay vì 65 phút là tổng cả quá trình. Khi tách ra từng bước ở mục 4.1, tôi thấy bước đánh giá ngữ cảnh chỉ khoảng 30 phút, còn khoảng 20 phút là lọc nhiễu và tra quyết định cũ, những việc Rule làm được. Từ đó tôi bỏ ý định dùng AI cho cả quy trình triage.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Điều làm tôi bất ngờ nhất đến từ research: các công cụ tôi đang dùng hằng ngày như Trivy đã có sẵn lọc theo mức nghiêm trọng, bỏ qua theo mã CVE kèm ngày hết hạn, chỉ là team chưa cấu hình hết. Nghĩa là một phần pain có thể chỉ là thiếu cấu hình, không cần AI. Tôi cũng bất ngờ khi Snyk, công cụ chuyên làm phần "code có gọi tới chỗ bị lỗi không", ghi rõ kết quả của họ không chắc chắn. Về phỏng vấn, nhóm chưa phỏng vấn được người ngoài nhóm trong buổi, nên tôi chưa có bằng chứng con số 65 phút của mình là phổ biến.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Khó nhất là viết Success Metric khi baseline chỉ là ước lượng của tôi. Bản v0 đặt target dưới 20 phút/lần, nhưng khi vẽ quy trình tương lai thì chính thiết kế của nhóm cũng mất khoảng 25 phút, nên phải đổi thành ≤ 30 phút. Ngoài ra metric chỉ đo thời gian thì có thể "đạt" bằng cách bỏ qua hết cảnh báo, nên phải thêm guardrail không bỏ sót Critical/High.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Tôi sẽ bấm giờ thật vài lần scan và hẹn trước 2–3 đồng nghiệp để phỏng vấn trước buổi học, vì phần kiểm chứng là chỗ yếu nhất của bài. Tôi cũng sẽ tự viết nhiều hơn thay vì để AI soạn nháp rồi sửa, vì có những con số AI ước lượng tôi phải đối chiếu lại nhiều lần. Về phản biện, tôi sẽ hỏi nhóm sớm hơn câu "nếu chỉ bật đúng cấu hình Trivy thì còn lại bao nhiêu phút?", vì câu đó quyết định có cần AI hay không.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
Problem: mỗi lần security scan ra khoảng 40 finding, DevOps mất khoảng 65 phút để biết cái nào thật sự phải xử lý, 3 lần mỗi tuần. Quy trình gồm 5 bước, trong đó bước nghẽn là đánh giá xem CVE có thật sự ảnh hưởng hệ thống không, khoảng 30 phút; lọc nhiễu và tra quyết định cũ thêm khoảng 20 phút. Metric là giảm thời gian triage xuống ≤ 30 phút/lần tính cả thời gian người duyệt, với guardrail không bỏ sót finding Critical/High nào. Boundary: AI không được tự bỏ qua finding, không sửa ignore file, không quyết định chặn hay mở release, và không nhận mã nguồn khi Team Lead chưa cho phép. Mức can thiệp là Workflow: Rule lọc nhiễu và xếp ưu tiên theo CVSS + EPSS, AI chỉ ở một bước gắn nhãn "có thể ảnh hưởng / có vẻ không / chưa đủ thông tin" kèm trích dẫn, DevOps quyết định. Không chọn Rule vì chỉ Rule còn khoảng 40 phút, chưa đạt target; không chọn Agent vì các bước đã cố định. Quyết định là Not Yet cho bước AI vì rủi ro Viability cao (chưa biết công ty cho đưa code ra ngoài không), nhưng Go cho phần Rule chạy thử 2 tuần; nếu Rule đã đạt ≤ 30 phút thì dừng ở Rule.

---

## 7. Tài liệu tham khảo

- docs/01-worksheet.md, docs/02-deliverable-example.md, docs/03-international-frameworks.md 
- GitHub Docs — Dependabot auto-triage rules: https://docs.github.com/en/code-security/concepts/supply-chain-security/dependabot-auto-triage-rules
- Trivy — Filtering: https://trivy.dev/latest/docs/configuration/filtering/
- FIRST — EPSS: https://www.first.org/epss/
- Snyk Docs — Reachability analysis: https://docs.snyk.io/scan-fix-and-prevent/fix/prioritize-issues-for-fixing/reachability-analysis
- Rob Fitzpatrick — The Mom Test: https://www.momtestbook.com/
- Teresa Torres — Opportunity Solution Trees: https://www.producttalk.org/opportunity-solution-trees/
- Anthropic — Building Effective Agents: https://www.anthropic.com/research/building-effective-agents
