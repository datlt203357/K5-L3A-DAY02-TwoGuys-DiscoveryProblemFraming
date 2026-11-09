# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: TwoGuys
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Khi xử lý lỗi từng xuất hiện, tôi muốn tìm lại thông tin và cách xử lý cũ, để không phải hỏi người khác lần nữa.
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Đoàn Viết Huy| Khi bắt đầu làm lab, tôi muốn nhanh chóng tìm đúng yêu cầu, để làm bài đúng hướng.| Học viên làm lab| Phải mở và dò từng file hướng dẫn để tìm yêu cầu: khoảng 15 phút.| README đã chỉ dẫn các file; cụ thể chỗ nào khiến bạn vẫn phải dò thêm 15 phút?(Đạt)|
| 2 | Đoàn Viết Huy| Khi cùng nhóm vẽ Use Case, tôi muốn thống nhất cách đặt tên, để không phải sửa lại khi ghép bài.| Thành viên nhóm làm đồ án| Sửa tên và ghép lại sơ đồ Use Case sau khi phát hiện không thống nhất: 2 ngày.|Hai ngày sửa bài có phải chỉ vì tên Use Case không thống nhất, hay còn lỗi khác?(Đạt)|
| 3 | Đoàn Viết Huy| Khi ôn trước buổi kiểm tra, tôi muốn tìm nhanh tài liệu và ghi chú, để có thêm thời gian ôn bài.| Học viên chuẩn bị kiểm tra| Tìm lại nội dung trong vở ghi: khoảng 30 phút.| Nếu tìm ghi chú nhanh hơn, 20 phút tổng hợp tài liệu có còn cần thiết không?(Đạt)|
| 4 | Lê Thành Đạt| Khi nhận ticket từ BA, tôi muốn rõ đầu vào, đầu ra và ngoại lệ, để không phải hỏi lại trước khi code.| Người nhận ticket để code| Đọc ticket nhưng chưa rõ đầu vào, đầu ra hoặc ngoại lệ; phải hỏi lại BA. Cần xác nhận thời gian/số lần hỏi.| Lần gần nhất ticket thiếu thông tin gì và bạn phải hỏi lại BA bao nhiêu lần?(Huy)|
| 5 | Lê Thành Đạt| Khi chốt sprint hằng tuần, tôi muốn hoàn tất log ticket, để công việc đã làm được ghi nhận đầy đủ.| Người thực hiện công việc trong sprint| Bổ sung log ticket vào lúc chốt sprint. Cần xác nhận bước nào mất thời gian nhất.| Bước nào trong việc log ticket lúc chốt sprint khiến bạn mất thời gian nhất?(Huy)|
| 6 |Lê Thành Đạt | Khi xử lý lỗi từng xuất hiện, tôi muốn tìm lại thông tin và cách xử lý cũ, để không phải hỏi người khác lần nữa.| Người xử lý lỗi| Tìm lại thông tin và cách xử lý lỗi cũ. Cần xác nhận tìm ở đâu và mất bao lâu.| Lần gần nhất xử lý lại lỗi cũ, bạn đã tìm hướng xử lý ở đâu và mất bao lâu?(Huy)|
| 7 | | | | | |
| 8 | | | | | |
| 9 | | | | | |
| 10 | | | | | |
| 11 | | | | | |
| 12 | | | | | |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Tìm thông tin | #1 tìm yêu cầu lab, #3 tìm tài liệu ôn tập, #6 tìm thông tin lỗi cũ| Phải tìm lại thông tin nằm ở nhiều chỗ|
| B — Thống nhất và làm rõ | #2 tên Use Case, #4 ticket từ BA| Thông tin hoặc cách hiểu chưa thống nhất trước khi bắt đầu làm|
| C — Ghi nhận công việc | #5 log ticket khi chốt sprint| Cần ghi lại việc đã làm đúng hạn|

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: 
├── Học viên phải dò nhiều file mới tìm được yêu cầu lab (#1)
├── Học viên mất thời gian tìm lại ghi chú trước buổi kiểm tra (#3)
└── Người xử lý lỗi khó tìm lại thông tin về lỗi cũ (#6) 
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

-

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #6 — Tìm lại thông tin và cách xử lý lỗi cũ | 4 | 2 | 2 | 2 | 4 | 4 | 4 | **22** |
| #1 — Tìm đúng yêu cầu trong tài liệu lab | 5 | 4 | 3 | 4 | 5 | 4 | 5 | **30** |
| #2 — Thống nhất tên Use Case khi làm đồ án nhóm | 5 | 4 | 4 | 5 | 4 | 3 | 4 | **29** |

*Điểm tham khảo dựa trên thông tin hiện có; nhóm cần xem lại cùng nhau. #6 chưa có lần xử lý lỗi cụ thể, thời gian tìm kiếm hoặc quy trình từng bước nên các cột bằng chứng, quy trình và impact đang ở mức 2/5.*

**Candidate được chọn:** #6 — Tìm lại thông tin và cách xử lý lỗi cũ.

**Vì sao chọn (bản nháp, nhóm cần xác nhận):** Nhóm ưu tiên #6 để kiểm chứng sâu hơn việc người xử lý lỗi phải tìm lại thông tin và cách xử lý của lỗi từng xuất hiện. Bảng điểm hiện tại cho thấy #6 còn thiếu bằng chứng, quy trình cụ thể và số đo impact; vì vậy lựa chọn này là **tạm thời**. Ở CP4, nhóm cần ghi lại ít nhất một lần xử lý lỗi cũ thực tế: đã tìm ở đâu, mất bao lâu, tìm được gì và có phải hỏi người khác không. Nếu kiểm chứng không xác nhận pain này, nhóm sẽ xem lại lựa chọn.

**Vì sao loại các candidate còn lại (bản nháp, nhóm cần xác nhận):** #1 có số đo 20 phút nhưng mới dựa trên một lần tìm yêu cầu của một học viên và gắn với cấu trúc repo lab cụ thể. #2 có hậu quả 2 ngày sửa bài, nhưng nhóm cần tách phần thời gian do đặt tên không thống nhất khỏi các lỗi khác của sơ đồ; phương án thống nhất quy tắc đặt tên trước khi chia việc có thể đủ để thử trước. Nhóm tạm ưu tiên kiểm chứng #6 thay vì đào sâu hai ý này.

**Xử lý bất đồng (nếu có):**

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 |Những lỗi người dùng báo cáo có xu hướng lặp lại theo thời gian. | | | | |
| 2 |Người xử lý thường phải hỏi đồng nghiệp khi gặp lỗi đã từng xuất hiện. | | | | |
| 3 |Thông tin về lỗi cũ và cách xử lý đang phân tán ở nhiều nơi hoặc khó tìm. | | | | |
| 4 |Việc hỏi đồng nghiệp làm tăng thời gian xử lý lỗi. | | | | |
| 5 |Có nhiều người trong nhóm cùng gặp khó khăn tra cứu lỗi cũ. | | | | |
| 6 |Các công cụ hiện tại chưa đáp ứng tốt nhu cầu tìm lỗi tương tự và hướng xử lý.| | | | |

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
| Jira Cloud: tìm bằng JQL/từ khóa | https://support.atlassian.com/jira-software-cloud/docs/jql-operators/ | Tìm ticket cũ theo trường text, mô tả và từ khóa | Có sẵn nếu nhóm dùng Jira Cloud | Cần ticket được ghi đủ thông tin; nhóm chưa xác nhận công cụ đang dùng | Thử tìm kiếm có cấu trúc trước khi cân nhắc AI |
| GitHub Issues: tìm và lọc issue | https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests | Tìm issue cũ theo từ khóa và bộ lọc | Có sẵn nếu lỗi được ghi trong GitHub Issues | Không giúp nếu lịch sử lỗi nằm ngoài GitHub | Công cụ hiện có có thể giải một phần bước tìm |
| Jira Rovo: tìm work item bằng ngôn ngữ tự nhiên | https://support.atlassian.com/jira-software-cloud/docs/use-atlassian-intelligence-to-search-for-work-items/ | Hỗ trợ tạo truy vấn tìm ticket từ câu hỏi tự nhiên | Có thể giảm công viết JQL nếu tổ chức đã bật | Chất lượng có thể thay đổi; phụ thuộc quyền và cấu hình; nhóm chưa thử | AI là phương án sau Rule, cần người mở nguồn kiểm tra |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

*Nhóm phác thảo quy trình dưới đây để hình dung người xử lý sẽ tìm lại một lỗi cũ như thế nào. Nhóm chưa ghi nhận một ca xử lý cụ thể, nên các bước và thời gian cần được kiểm tra lại với người đã làm việc này.*

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
Nhận thông tin về lỗi
→ Xem lỗi xảy ra trong trường hợp nào
→ Lục lại ticket hoặc ghi chú về lỗi tương tự [bước có thể mất nhiều thời gian nhất]
→ Kiểm tra cách xử lý cũ còn phù hợp không
→ Sửa và thử lại
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Người xử lý lỗi | Thông tin lỗi mới nhận | Biết lỗi cần kiểm tra là gì | Chưa đo | Cần xác nhận lỗi được báo qua đâu |
| 2 | Người xử lý lỗi | Mô tả lỗi | Hiểu tình huống làm lỗi xuất hiện | Chưa đo | Có thể cần thử lại để thấy lỗi |
| 3 | Người xử lý lỗi | Dấu hiệu của lỗi | Tìm được ticket hoặc ghi chú cũ có liên quan | Chưa đo | Nhóm dự đoán bước này tốn thời gian nhất |
| 4 | Người xử lý lỗi | Thông tin lỗi cũ và lỗi hiện tại | Biết cách xử lý cũ có dùng lại được không | Chưa đo | Lỗi trông giống nhau chưa chắc cùng nguyên nhân |
| 5 | Người xử lý lỗi | Kết quả đối chiếu | Bản sửa đã được thử lại | Chưa đo | Cần xác nhận ai kiểm tra kết quả |

**Bottleneck nhóm đang nghi ngờ:** Bước 3, lục lại thông tin về lỗi cũ. Nhóm chưa biết bước này mất bao lâu trong thực tế; cần kiểm tra trước khi đặt mốc thời gian hiện tại và mục tiêu cải thiện.

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

*Phương án để nhóm cân nhắc, chưa thử trong thực tế. Bước AI chỉ có ý nghĩa nếu cách tìm bằng từ khóa và ghi chú có cấu trúc vẫn chưa đủ.*

```text
1. Người xử lý nhận lỗi và ghi lại triệu chứng chính.
2. Rule: tìm trong danh sách ticket/ghi chú cũ theo mã lỗi, từ khóa hoặc thành phần liên quan.
3. AI (nếu được phép dùng dữ liệu): gợi ý vài lỗi cũ có thể liên quan và dẫn về nguồn gốc.
4. Người xử lý mở nguồn gốc, so triệu chứng và nguyên nhân; tự quyết định có dùng lại cách xử lý không.
5. Người xử lý sửa lỗi, thử lại và ghi ngắn gọn cách xử lý vào ticket.
```

**Boundary:** AI chỉ gợi ý tài liệu để xem; không kết luận hai lỗi có cùng nguyên nhân, không tự sửa mã nguồn, không đóng ticket và không dùng dữ liệu mà nhóm không có quyền truy cập.

**Phương án quay về:** Nếu gợi ý sai, thiếu nguồn hoặc không có quyền dùng AI, người xử lý bỏ gợi ý và tìm ticket bằng từ khóa, hỏi người phụ trách hoặc xử lý theo quy trình hiện tại.

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 5 bước phác thảo | 5 bước đề xuất | Chưa xác minh với một ca xử lý thật |
| Tổng thời gian | Chưa đo | Mục tiêu: giảm ít nhất 50% thời gian **tìm thông tin lỗi cũ** | Cần đo mốc ban đầu trước khi thử; không tính thời gian sửa lỗi vào chỉ số này |
| Số bước thủ công | 5 bước | 3 bước chính: nhận/ghi triệu chứng, kiểm tra nguồn và sửa/thử lại | Rule và AI chỉ hỗ trợ tìm kiếm; con người vẫn quyết định |
| Bottleneck chính | Tìm lại ticket hoặc ghi chú cũ (giả định) | Kiểm tra các kết quả tìm được có đúng lỗi đang gặp không | Chỉ chuyển bottleneck nếu việc tìm thực sự được rút ngắn |
| Rủi ro mới phát sinh | Chưa đánh giá | Gợi ý nhầm lỗi tương tự; lộ thông tin nội bộ nếu đưa dữ liệu vào công cụ không được phép | Giữ bước người kiểm và kiểm tra quyền truy cập |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Người được giao xử lý lỗi phần mềm đã từng xuất hiện. Cần xác nhận vai trò cụ thể với người thực hiện. |
| **Quy trình** | Nhận thông tin lỗi → xem tình huống xảy ra → tìm ticket/ghi chú cũ → kiểm tra cách xử lý cũ → sửa và thử lại. Đây là quy trình phác thảo. |
| **Bottleneck** | Nhóm nghi ngờ bước tìm lại thông tin lỗi cũ mất nhiều thời gian vì thông tin nằm rải rác hoặc khó tìm bằng từ khóa. Chưa đo được thời gian. |
| **Impact** | Người xử lý có thể phải tìm lâu hoặc hỏi lại người khác trước khi bắt đầu sửa. Mức ảnh hưởng thực tế chưa được kiểm chứng. |
| **Success Metric** (baseline → target, cách đo) | Baseline: chưa đo. Mục tiêu đề xuất: giảm ít nhất 50% **thời gian tìm được nguồn lỗi cũ phù hợp** so với baseline, đồng thời không tăng số lần chọn nhầm tài liệu. Đo bằng cách ghi thời điểm bắt đầu tìm và thời điểm người xử lý xác nhận nguồn đúng trên các ca lỗi cũ tiếp theo. |
| **Boundary** (AI không được làm gì) | AI không tự kết luận nguyên nhân, không sửa mã nguồn, không đóng ticket và không truy cập dữ liệu ngoài quyền cho phép. Người xử lý phải mở nguồn và kiểm tra trước khi dùng lại cách sửa. |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

- AI phản biện bản nháp: chưa có baseline và chưa biết lỗi cũ xuất hiện đủ thường xuyên để việc cải thiện tìm kiếm mang lại giá trị hay không. Nhóm cần xác nhận bằng ca xử lý thật trước khi chốt Problem Statement và quyết định ở CP6.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **độ mơ hồ trung bình, độ phức tạp thấp–trung bình** (đánh giá sơ bộ).

Vì sao: Triệu chứng của hai lỗi có thể giống nhau nhưng nguyên nhân khác nhau, nên việc xác định lỗi cũ nào liên quan có độ mơ hồ. Tuy vậy, các bước nhận lỗi → tìm nguồn cũ → đối chiếu → sửa/kiểm tra tương đối cố định; chưa thấy nhu cầu để hệ thống tự quyết bước tiếp theo.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Ghi mã lỗi, triệu chứng, nguyên nhân, cách sửa và link ticket liên quan theo một mẫu chung. | Số ticket ít, người xử lý tìm lại được dễ dàng. | Mất công ghi chép; ghi thiếu thì vẫn khó tìm. | Nên làm ngay |
| **Rule** | Dùng bộ lọc/từ khóa theo mã lỗi, thành phần, nhãn và trạng thái; trả về link ticket gốc. | Dữ liệu được ghi tương đối nhất quán. | Có thể bỏ sót khi người viết dùng từ khác. | **Chọn để thử trước** |
| **Workflow** | Rule lấy danh sách ticket → AI gợi ý ticket tương tự kèm nguồn → người xử lý đối chiếu và quyết định. | Rule đã thử nhưng vẫn bỏ sót nhiều lỗi liên quan; dữ liệu được phép dùng. | AI gợi ý nhầm hoặc không có nguồn; cần người kiểm. | Chỉ xem xét sau khi đo |
| **Agent** | AI tự tìm nhiều nguồn, quyết định hướng điều tra và cập nhật ticket. | Chỉ khi quy trình có nhiều nhánh khó định trước và quyền truy cập/kiểm soát đã rõ. | Quyền truy cập rộng, khó kiểm soát quyết định sai. | Không chọn |

**Mức chọn:** Rule, kèm cách ghi ticket thống nhất (No AI). Chưa chọn Workflow hay Agent.

**Vì sao không chọn mức đơn giản hơn:** Mẫu ghi ticket giúp dữ liệu dễ đọc hơn nhưng không tự giúp tìm trong nhiều ticket cũ. Rule tìm theo mã lỗi, nhãn và từ khóa là bước thử tiếp theo hợp lý. Đây là suy luận từ quy trình phác thảo; nhóm cần kiểm chứng lượng ticket, cách ghi hiện tại và thời gian tìm thực tế. Jira và GitHub Issues đều đã có chức năng tìm kiếm/lọc, nên chưa có căn cứ để xây công cụ mới.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | *Nếu thử Workflow sau này:* danh sách ticket lỗi cũ có thể liên quan, mỗi gợi ý kèm link và lý do khớp. Giai đoạn Rule hiện tại chưa dùng AI. |
| **Judgment** — con người cân nhắc, quyết định gì? | Người xử lý đọc ticket gốc, so triệu chứng, môi trường và nguyên nhân; quyết định có dùng lại cách sửa không. |
| **Action** — hành động cuối cùng là gì, ai làm? | Người xử lý sửa/kiểm tra lỗi và cập nhật ticket; AI không tự làm. |
| **Outcome** — đo kết quả bằng gì? | Thời gian tìm được nguồn lỗi cũ đúng; số gợi ý sai; số lần phải hỏi người khác. Cần đo baseline trước. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Mô tả lỗi hiện tại và các ticket/ghi chú cũ được phép truy cập. Nhóm chưa xác nhận nguồn dữ liệu hay quyền sử dụng. |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Link nào người xử lý chấp nhận/bỏ qua và lý do; ticket được cập nhật sau khi xử lý. |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Nhóm đề xuất **hỗ trợ**: công cụ chỉ đưa link để người xử lý tự kiểm tra. Chưa có phỏng vấn để khẳng định đây là mong muốn của người dùng.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Với bước gợi ý tài liệu, báo nhầm có thể khiến người xử lý dùng sai cách sửa; bỏ sót khiến họ tiếp tục tìm thủ công. Nhóm tạm ưu tiên tránh báo nhầm bằng cách luôn hiện nguồn và không cho AI tự sửa. Cần hỏi người xử lý để xác nhận mức độ rủi ro.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Người được giao xử lý lỗi phần mềm từng xuất hiện; vai trò cụ thể cần xác nhận. |
| **Quy trình** | Nhận lỗi → xem triệu chứng → tìm ticket/ghi chú cũ bằng bộ lọc và từ khóa → đối chiếu → sửa, kiểm tra và cập nhật ticket. |
| **Bottleneck** | Nghi ngờ bước tìm ticket cũ; chưa có thời gian đo hoặc ca thực tế để xác nhận. |
| **Impact** | Có thể mất thời gian tìm lại thông tin hoặc phải hỏi người khác; mức ảnh hưởng chưa xác minh. |
| **Success Metric** (baseline → target, cách đo) | Đo thời gian từ lúc bắt đầu tìm đến khi người xử lý xác nhận đúng nguồn trên ít nhất 5 ca lỗi cũ. Baseline: chưa đo. Target đề xuất: trung vị thời gian tìm giảm ít nhất 50% so với baseline; không tăng số lần chọn nhầm ticket. Chỉ chốt target sau khi có baseline. |
| **Boundary** | Kết quả tìm kiếm chỉ là tài liệu tham khảo. Nếu sau này thử AI, AI không tự kết luận nguyên nhân, không sửa mã nguồn, không đóng ticket hoặc đọc dữ liệu ngoài quyền cho phép. |
| **AI intervention point** | Chưa dùng AI trong bước thử đầu. Nếu Rule không đủ, AI chỉ gợi ý ticket tương tự sau bước tìm kiếm và trước khi người xử lý đối chiếu. |
| **Mức chọn** | Rule trước; Workflow là phương án thử tiếp nếu có bằng chứng Rule không đủ. |
| **Rủi ro & người kiểm tra** | Nhầm ticket, bỏ sót lỗi cũ hoặc truy cập sai quyền. Người xử lý kiểm link, triệu chứng và nguyên nhân; người quản lý dữ liệu xác nhận quyền truy cập trước mọi thử nghiệm AI. |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Mức can thiệp | v0 phác thảo Rule và AI trong quy trình tương lai | v1 chọn Rule để thử trước; AI chỉ là phương án tiếp theo | Jira/GitHub đã có tìm kiếm và nhóm chưa có bằng chứng AI cần thiết. |
| Success Metric | Giảm 50% thời gian tìm, chưa có baseline | Đo trung vị trên ít nhất 5 ca, không tăng chọn nhầm ticket | Tách tốc độ khỏi độ đúng và quy định cách đo. |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Có nguồn gốc | Mỗi gợi ý dẫn đến ticket/ghi chú mà người xử lý có quyền mở | Không có link, link sai hoặc không mở được |
| 2 | Khớp triệu chứng | Lý do gợi ý chỉ ra triệu chứng hoặc mã lỗi trùng với nguồn | Chỉ nói “tương tự” mà không chỉ ra chỗ khớp |
| 3 | Không kết luận thay người | Ghi rõ đây là lỗi *có thể liên quan* và để người xử lý đối chiếu nguyên nhân | Khẳng định cùng nguyên nhân hoặc tự đề xuất sửa như chắc chắn đúng |
| 4 | Không bỏ sót nguồn đã biết | Với ca thử có ticket cũ đã xác nhận, ticket đó xuất hiện trong danh sách gợi ý | Ticket đúng có trong dữ liệu được phép dùng nhưng không được gợi ý |

*Bộ tiêu chí này dành cho phương án AI có thể thử sau này; nhóm chưa có đầu ra AI thật để chấm.*

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | Cao | Chưa có ca lỗi cũ cụ thể, tần suất hay thời gian tìm thực tế; chưa biết pain có đáng ưu tiên không. |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | Trung bình | Link nguồn giúp kiểm tra, nhưng chưa thử với người xử lý thật; gợi ý nhầm dễ gây hiểu sai. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | Trung bình | Jira/GitHub có tìm kiếm sẵn; chưa rõ nhóm dùng hệ thống nào và dữ liệu ticket có đủ nhất quán để tìm không. |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | Cao | Chưa xác nhận quyền truy cập dữ liệu, chính sách dùng AI hay người duy trì cách ghi ticket. |

### 8.2. Kết luận

**Quyết định:** **Not Yet đối với AI.** Có thể thử cải thiện cách ghi và tìm ticket bằng công cụ sẵn có trước.

**Lý do:** Rủi ro Value và Viability đang cao vì thiếu bằng chứng người dùng và quyền dữ liệu. Tìm kiếm theo từ khóa/bộ lọc đã có trong các công cụ quản lý ticket phổ biến; chưa đủ lý do để chọn Workflow hoặc Agent. Đây là kết luận dựa trên tài liệu sản phẩm và giả định của nhóm, chưa phải kết quả pilot.

**Nếu Go — pilot nhỏ nhất:** Chưa áp dụng cho AI. Bước thử ít rủi ro: thống nhất mẫu ghi lỗi và dùng bộ lọc/từ khóa sẵn có trên 5 ca lỗi cũ, ghi thời gian tìm và độ đúng.

**Nếu Not Yet — cần kiểm chứng gì trước:** Ghi lại ít nhất 5 ca lỗi từng xuất hiện, hỏi người xử lý đã tìm thông tin ở đâu và mất bao lâu; kiểm tra quyền dùng ticket trong công cụ AI. Nếu Rule vẫn tìm chậm hoặc bỏ sót, mới thử gợi ý AI có người duyệt.

**Nếu No-Go — nên làm gì thay AI:** Duy trì mẫu ghi lỗi, nhãn/từ khóa và hướng dẫn tìm kiếm trong công cụ ticket đang dùng.

**Ngưỡng dừng** (nếu sau 5 ca thử mà … thì quay về …): Nếu Rule không giảm được ít nhất 30% trung vị thời gian tìm so với baseline, xem lại cách ghi ticket và bộ lọc trước khi nâng mức can thiệp. Nếu sau này thử AI mà có một gợi ý không dẫn được về nguồn hoặc người xử lý dùng nhầm ticket để sửa lỗi, dừng thử AI và quay về tìm kiếm có người kiểm. Các ngưỡng này là đề xuất để nhóm duyệt, chưa có số liệu thực nghiệm.

---

## 9. Hạn chế và hướng tiếp theo

- Quy trình hiện tại và mức độ pain mới là phác thảo; nhóm chưa có ca lỗi cũ cụ thể để đo thời gian và xác định bottleneck.
- Chưa xác nhận nhóm dùng Jira, GitHub Issues hay hệ thống khác. Bảng research nêu khả năng của công cụ, không chứng minh nhóm đã dùng các tính năng đó.
- Bước tiếp theo là thu thập ca xử lý thật, đo baseline và thử cách ghi/tìm ticket có cấu trúc trước khi xem xét AI.

## 10. Tài liệu tham khảo

- Atlassian, [JQL operators](https://support.atlassian.com/jira-software-cloud/docs/jql-operators/) — trường tìm kiếm văn bản trong Jira Cloud.
- GitHub Docs, [Searching issues and pull requests](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests) — cách tìm và lọc issue.
- Atlassian, [Use Rovo to search for work items](https://support.atlassian.com/jira-software-cloud/docs/use-atlassian-intelligence-to-search-for-work-items/) — cách Rovo chuyển câu hỏi thành truy vấn tìm kiếm và các giới hạn.
