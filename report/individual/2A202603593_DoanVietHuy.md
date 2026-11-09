# Báo cáo cá nhân — Đoàn Viết Huy

## 1. Thông tin học viên

- Họ tên: Đoàn Viết Huy
- MSSV: 2A202603593
- Email trường: 26ai.huydv3@vinuni.edu.vn
- Tên nhóm:
- Link repo nhóm: https://github.com/datlt203357/K5-L3A-DAY02-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi cần đọc tài liệu để làm lab, tôi muốn nhanh chóng nắm được ý chính và các yêu cầu cần làm, để chuẩn bị bài đúng hạn. | Tôi | Lần gần nhất mất khoảng 20 phút để tìm phần yêu cầu bài. |
| 2 | Tốn thời gian | Khi cùng nhóm vẽ sơ đồ Use Case cho đồ án, tôi muốn các phần dùng tên nhất quán, để ghép bài mà không phải sửa nhiều. | Tôi và các thành viên nhóm | Trong buổi họp kiểm tra tuần trước, nhóm phát hiện mỗi người đặt tên Use Case một kiểu và mất tròn 2 ngày để sửa. |
| 3 | Tốn thời gian | Khi ôn bài trước buổi kiểm tra, tôi muốn tìm lại đúng ghi chú và tài liệu cần học, để có thời gian tập trung ôn tập. | Tôi | Trước buổi kiểm tra thường xuyên thứ Sáu tuần trước, tôi mất 10 phút tìm trên LMS, 30 phút tìm trong vở và 20 phút tổng hợp lại (tổng khoảng 1 tiếng). |
| 4 | Pain từ người khác | Khi đã hẹn đi chơi với bạn, tôi muốn nhớ được thời gian hẹn, để cả hai không bỏ lỡ cuộc gặp. | Tôi và bạn | Thứ Bảy tuần trước, tôi và bạn cùng quên một cuộc hẹn đi chơi. |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi gặp một khái niệm khó trong bài giảng, tôi muốn tìm được cách giải thích dễ hiểu, để tiếp tục theo kịp bài học. | Tôi | Trong buổi học thứ Sáu tuần trước, tôi gặp khó với gradient descent và hỏi AI để hiểu thêm. Tôi mới nhớ được một lần như vậy. |

**Tôi dùng AI ở CP1:** AI giúp diễn đạt các ý theo mẫu Job Story. Tôi bỏ những gợi ý không gắn với trải nghiệm của mình và bổ sung các lần việc đó thật sự xảy ra.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

Các mục tiêu dưới đây là mức tôi muốn thử ở lần sau, chưa phải kết quả đã đạt được.

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tìm yêu cầu trong tài liệu lab | Đã gặp thật: đọc README khoảng 5 phút, dò từng file khoảng 15 phút. | Cần kiểm chứng liệu người khác cũng gặp khó khăn tương tự. |
| 2 | Không thống nhất tên Use Case trong đồ án nhóm | Có sự cố cụ thể và hậu quả đo được: mất 2 ngày sửa. | Chưa rõ nhóm đã thống nhất quy tắc đặt tên ban đầu hay chưa. |
| 3 | Tìm và tổng hợp tài liệu trước buổi kiểm tra | Có quy trình 3 bước và thời gian từng bước: 10 + 30 + 20 phút. | Chưa biết việc này có lặp lại ở các buổi kiểm tra khác không. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi cần đọc tài liệu để làm lab, tôi muốn nhanh chóng nắm được ý chính và các yêu cầu cần làm, để chuẩn bị bài đúng hạn. |
| Actor | Tôi, học viên làm bài lab. |
| Thời điểm / bối cảnh | Khi mới mở repo để bắt đầu làm lab. |
| Quy trình hiện tại (3–7 bước) | Mở repo → đọc README.md (khoảng 5 phút) → mở và dò từng file hướng dẫn (khoảng 15 phút) → tìm được yêu cầu cần làm. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Mở và dò từng file vì chưa biết file nào chứa yêu cầu cần tìm: khoảng 15 phút. |
| Impact (nếu không giải thì sao) | Mất khoảng 20 phút trước khi xác định được yêu cầu bài và bắt đầu làm. |
| Success metric (baseline → target) | Baseline: khoảng 20 phút. Mục tiêu đề xuất: tìm đúng yêu cầu trong tối đa 5 phút ở lần làm lab tiếp theo; bấm giờ từ lúc mở repo đến khi xác định được mục cần làm. Chưa thử. |
| Phương án không dùng AI | Đưa chỉ dẫn nổi bật lên đầu README: “Làm gì?” → CHECKPOINTS.md; “Nộp thế nào?” → SUBMISSION.md; “Xem ví dụ?” → docs/02-deliverable-example.md. README đã có bảng hướng dẫn, nên cần làm đường đi đến yêu cầu dễ nhận ra hơn thay vì thêm một mục lục trùng lặp. Chưa thử. |
| Giả thuyết về AI (nếu có) | Chưa thấy cần AI. Tôi muốn thử làm chỉ dẫn trong README rõ hơn trước. |
| Cảm nhận nhanh | No AI trước. |

Quy trình nháp hiện tại:

```text
Mở repo (thao tác bắt đầu)
→ Đọc README.md (~5 phút)
→ Mở và dò từng file hướng dẫn (~15 phút) [BOTTLENECK]
→ Tìm được yêu cầu cần làm (kết quả)
Tổng thời gian tìm yêu cầu: ~20 phút.
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi cùng nhóm vẽ sơ đồ Use Case cho đồ án, tôi muốn các phần dùng tên nhất quán, để ghép bài mà không phải sửa nhiều. |
| Actor | Các thành viên nhóm làm đồ án. |
| Thời điểm / bối cảnh | Khi chia nhau vẽ Use Case và họp kiểm tra bản ghép. |
| Quy trình hiện tại (3–7 bước) | Mỗi người vẽ phần Use Case được giao → cả nhóm họp kiểm tra và thấy cách đặt tên không khớp → sửa lại các sơ đồ. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước sửa tên và chỉnh lại các sơ đồ sau buổi họp: mất tròn 2 ngày. Chưa đo riêng thời gian từng thao tác. |
| Impact (nếu không giải thì sao) | Nhóm phải dành 2 ngày làm lại thay vì tiếp tục hoàn thiện đồ án. |
| Success metric (baseline → target) | Baseline: 2 ngày sửa sơ đồ sau khi phát hiện tên không thống nhất. Mục tiêu đề xuất: không quá nửa ngày sửa tên ở đồ án tiếp theo; ghi lại thời gian sửa thực tế. Cần xác nhận phần nào của 2 ngày là do tên và phần nào do lỗi khác. |
| Phương án không dùng AI | Trước khi chia việc, thống nhất tên Use Case là cụm động từ + đối tượng, giữ một bảng thuật ngữ chung và kiểm một sơ đồ mẫu. Đây là đề xuất, chưa thử. |
| Giả thuyết về AI (nếu có) | Chưa thấy cần AI để cả nhóm thống nhất tên gọi. |
| Cảm nhận nhanh | No AI trước. |

Quy trình nháp hiện tại:

```text
Mỗi người vẽ phần Use Case được giao [chưa nhớ thời gian]
→ Cả nhóm họp kiểm tra, phát hiện tên không khớp [chưa nhớ thời gian]
→ Sửa lại các sơ đồ [BOTTLENECK: mất tròn 2 ngày]
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi ôn bài trước buổi kiểm tra, tôi muốn tìm lại đúng ghi chú và tài liệu cần học, để có thời gian tập trung ôn tập. |
| Actor | Tôi, học viên chuẩn bị kiểm tra thường xuyên. |
| Thời điểm / bối cảnh | Trước buổi kiểm tra thường xuyên thứ Sáu tuần trước. |
| Quy trình hiện tại (3–7 bước) | Tìm tài liệu trên LMS (10 phút) → tìm trong vở ghi (30 phút) → tổng hợp lại (20 phút). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Tìm lại nội dung trong vở ghi: 30 phút, lâu nhất trong ba bước. |
| Impact (nếu không giải thì sao) | Dành khoảng 1 tiếng để tìm và tổng hợp tài liệu trước khi tập trung ôn bài. |
| Success metric (baseline → target) | Baseline: 40 phút tìm tài liệu (10 phút LMS + 30 phút vở), thêm 20 phút tổng hợp. Mục tiêu đề xuất: tìm trong tối đa 15 phút, tổng thời gian chuẩn bị không quá 35 phút; bấm giờ riêng hai phần ở lần ôn tiếp theo. Chưa thử. |
| Phương án không dùng AI | Sau mỗi buổi học, ghi chủ đề và từ khóa ở đầu trang vở, đánh dấu trang cần ôn và lưu link tài liệu LMS theo buổi. Đây là đề xuất, chưa thử. |
| Giả thuyết về AI (nếu có) | Chưa thấy cần AI cho bước tìm tài liệu; thử cách ghi chú dễ tra lại trước. |
| Cảm nhận nhanh | No AI trước. |

Quy trình nháp hiện tại:

```text
Tìm tài liệu trên LMS (10 phút)
→ Tìm trong vở ghi (30 phút) [BOTTLENECK]
→ Tổng hợp lại (20 phút)
Tổng thời gian: khoảng 60 phút.
```

### Card muốn pitch nhất

- Card số: **#2 — không thống nhất tên Use Case khi làm đồ án nhóm.**
- Vì sao: Tôi đã gặp việc này trong đồ án; cả nhóm mất tròn 2 ngày sửa sau khi họp kiểm tra, nên có hậu quả cụ thể để trao đổi.
- Câu hỏi muốn nhóm phản biện: **Nếu thống nhất quy tắc đặt tên từ đầu, liệu có tránh được phần lớn thời gian sửa, hay còn nguyên nhân khác khiến nhóm phải làm lại sơ đồ?**

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card #1: README đã có bảng chỉ dẫn các file. Cần xem vì sao tôi vẫn mất 15 phút dò file. | Đồng ý một phần | README có bảng, nhưng tôi vẫn không nhận ra phải mở file nào trước. Tôi đổi đề xuất từ thêm mục lục sang làm phần chỉ dẫn ở đầu README dễ thấy và cụ thể hơn. |
| Card #2: Chưa rõ cả 2 ngày sửa bài có phải chỉ do tên Use Case không thống nhất. | Đồng ý | Tôi ghi rõ nhóm phải sửa lại các sơ đồ sau khi phát hiện tên không thống nhất, nhưng chưa tách được thời gian sửa tên khỏi các lỗi khác. |
| Card #3: Tìm tài liệu và tổng hợp tài liệu là hai việc khác nhau. | Đồng ý | Tôi tách 40 phút tìm tài liệu (10 phút LMS, 30 phút vở) và 20 phút tổng hợp để lần sau đo riêng. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Tôi chuẩn bị 3 Card: tìm yêu cầu lab, thống nhất tên Use Case, tìm tài liệu ôn tập. | Nhóm có thêm 3 candidate để so sánh ở CP3. |
| Phản biện bài của bạn khác | Tôi ghi trong bảng pitch câu hỏi cho Đạt: “Lần gần nhất xử lý lại lỗi cũ, bạn đã tìm hướng xử lý ở đâu và mất bao lâu?” | Câu hỏi giúp nhóm thấy #6 còn thiếu một ca xử lý cụ thể và thời gian tìm. Báo cáo chưa ghi câu trả lời của Đạt. |
| Nhận phản biện | Đạt hỏi vì sao tôi vẫn dò file 15 phút dù README đã có chỉ dẫn; Đạt cũng hỏi liệu 20 phút tổng hợp tài liệu có còn cần thiết nếu tìm ghi chú nhanh hơn. | Tôi giữ nhận định rằng chỉ dẫn README chưa đủ rõ với mình; với Card #3, tôi tách 40 phút tìm và 20 phút tổng hợp để đo riêng. |
| Gom cluster / cây OST | Tôi tham gia CP3, sắp xếp các candidate về tìm thông tin, làm rõ cách hiểu và ghi nhận công việc. | Nhóm nhìn ra #1, #3 và #6 cùng có bước tìm lại thông tin. |
| Chọn candidate problem | Tôi và Đạt thống nhất chọn #6 — tìm lại thông tin và cách xử lý lỗi cũ. | Nhóm chuyển sang phác thảo quy trình và tìm cách kiểm chứng; lựa chọn vẫn cần bằng chứng thực tế. |
| Kiểm chứng / research | Tôi không trực tiếp phụ trách CP4. | Bảng research của nhóm đã có nguồn, nhưng phần kiểm chứng với người thật còn thiếu. |
| Quy trình nhóm | Tôi phụ trách CP5: xem bản phác thảo quy trình và yêu cầu viết lại cho tự nhiên, dễ hiểu. | Mục 4 của báo cáo nhóm đã có sơ đồ và bảng trước/sau; thời gian từng bước vẫn chưa đo. |
| Problem Statement | Tôi phụ trách CP5: đối chiếu Problem Statement v0 với bài mẫu. | Nhóm nhận ra Success Metric còn thiếu baseline thực tế. |
| Mức can thiệp AI | Tôi không trực tiếp phụ trách CP6. | Bản nhóm hiện chọn thử Rule trước; cần nhóm xác nhận mức chọn cuối. |
| Quyết định | Tôi không trực tiếp phụ trách CP6. | Bản nháp nhóm hiện kết luận Not Yet với AI. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Nhờ AI gợi ý cách viết Job Story. | Tôi hiểu cấu trúc câu cần viết. | AI đưa vài ví dụ chung, không phải việc tôi từng gặp. | Tôi thay bằng những lần mình nhớ được, như mất 20 phút tìm yêu cầu lab và 2 ngày sửa sơ đồ. |
| CP2 Problem Card | Nhờ AI viết nháp và phản biện ba Card. | AI giúp tôi nhìn rõ bước nào tốn thời gian. | AI chưa biết chính xác vì sao tôi dò file lâu và phần nào trong 2 ngày sửa là do tên Use Case. | Tôi làm rõ bước dò file mất 15 phút; tách 40 phút tìm tài liệu khỏi 20 phút tổng hợp. |
| CP4 Research | Nhờ AI tìm tài liệu về cách tra lại ticket. | Có link để nhóm xem các chức năng sẵn có. | Tài liệu về Jira hay GitHub không chứng minh nhóm mình dùng các công cụ đó. | Tôi cần mở lại nguồn và hỏi người xử lý thật trước khi kết luận. |
| CP5 Quy trình | Nhờ AI phác thảo quy trình xử lý lỗi cũ. | Có khung để thảo luận. | AI tự suy ra các bước; nhóm chưa đo thời gian. | Tôi yêu cầu viết lại dễ hiểu hơn và giữ nhãn “chưa đo” ở phần thiếu dữ liệu. |
| CP5–6 Problem Statement | Nhờ AI chỉ ra chỗ thiếu trong bản nháp. | AI nhắc rằng chưa có thời gian ban đầu để so với mục tiêu. | Chưa thể nói bước tìm lỗi cũ là nghẽn nhất khi chưa quan sát ca thật. | Tôi giữ đây là giả định cần kiểm tra, chưa ghi thành kết quả. |
| CP6 Mức can thiệp / quyết định | Nhờ AI so sánh bốn mức can thiệp. | Nhóm có phương án thử tìm bằng công cụ sẵn có trước. | Chọn AI ngay sẽ vội khi chưa thử cách tìm đơn giản. | Bản nháp nhóm chọn Rule trước và Not Yet với AI; cả nhóm còn phải chốt lại. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Khi xem ba ý của Đạt về ticket BA, log công việc và lỗi cũ, tôi thấy ý tìm lỗi cũ khá gần công việc lập trình. Nhưng nhóm vẫn thiếu một lần xảy ra cụ thể: lỗi gì, tìm ở đâu, mất bao lâu. Card Use Case của tôi thì có buổi họp kiểm tra và hai ngày sửa bài để đối chiếu. Tôi thấy một vấn đề nghe hợp lý vẫn cần bằng chứng trước khi chọn.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Bản nháp CP5 từng đưa AI vào bước gợi ý ticket cũ khá sớm. Sau khi xem tài liệu về Jira và GitHub Issues, hướng đề xuất đổi thành ghi ticket rõ hơn, rồi thử từ khóa và bộ lọc trước. Nếu vẫn tìm khó thì mới cân nhắc AI. Cách này hợp lý hơn khi nhóm còn chưa đo được bước tìm lỗi cũ mất bao lâu.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Có. Ở Card ôn tập, ban đầu tôi chỉ ghi tổng cộng một tiếng. Sau phản biện về việc 20 phút tổng hợp vẫn có thể cần thiết, tôi tách lại: 40 phút tìm tài liệu và 20 phút tổng hợp. Nếu thử cách ghi chú mới, tôi sẽ đo hai phần riêng, không chỉ nhìn tổng thời gian.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Nhóm chưa có phỏng vấn hay khảo sát về lỗi cũ, nên tôi chưa thể nói kết quả kiểm chứng làm mình bất ngờ. Phần research cho thấy Jira và GitHub Issues đã có cách tìm ticket; Jira còn có Rovo. Nhưng tài liệu sản phẩm không cho biết nhóm mình dùng công cụ nào hay ticket có được ghi đủ không. Research giúp thu hẹp phương án, chứ chưa thay được việc hỏi người thật.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Khó nhất là viết Success Metric. Nhóm muốn giảm thời gian tìm lỗi cũ nhưng chưa biết hiện mất bao lâu. Viết “tìm nhanh hơn” thì không đo được, còn tự điền số phút thì không đúng. Bản nháp vì thế ghi baseline chưa đo và nêu cách đo: từ lúc bắt đầu tìm đến khi người xử lý xác nhận được ticket đúng.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại, tôi sẽ hỏi Đạt về một lần xử lý lỗi cũ trước khi chấm điểm #6: lỗi được báo ở đâu, đã tìm thế nào và mất bao lâu. Tôi cũng sẽ hỏi rõ vì sao nhóm chọn #6 dù điểm tham khảo thấp hơn hai ý còn lại. Khi có câu trả lời, nhóm sẽ viết quy trình và quyết định cuối chắc hơn, thay vì để nhiều chỗ “chưa xác minh”.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Vấn đề nhóm chọn là người xử lý lỗi khó tìm lại thông tin và cách sửa của lỗi từng xuất hiện. Quy trình nhóm phác thảo gồm nhận lỗi, xem triệu chứng, tìm ticket cũ, đối chiếu rồi sửa và thử lại; bước tìm ticket đang được nghi là chỗ nghẽn, nhưng chưa đo. Chỉ số cần theo dõi là thời gian tìm được nguồn cũ đúng, cùng số lần chọn nhầm ticket hoặc phải hỏi người khác. Nếu sau này dùng AI, AI chỉ được gợi ý tài liệu có nguồn, không tự kết luận nguyên nhân, sửa mã nguồn hay đóng ticket. Trong bản báo cáo, nhóm đề xuất thử cách ghi ticket thống nhất và tìm bằng bộ lọc hoặc từ khóa, tức mức Rule. Quyết định dự kiến đối với AI là Not Yet vì nhóm chưa có baseline, ca lỗi thực tế và xác nhận quyền dùng dữ liệu.

---

## 7. Tài liệu tham khảo

- GitHub Docs, [About the repository README file](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes) — căn cứ cho phương án chỉ dẫn trực tiếp từ README ở Card #1.
- IBM, [Use cases](https://www.ibm.com/docs/en/dma?topic=diagrams-use-cases) — tên Use Case nên ngắn, duy nhất và mô tả hành động; căn cứ cho quy tắc đặt tên ở Card #2.
- Cornell Learning Strategies Center, [The Cornell Note-taking System](https://lsc.cornell.edu/notes.html) — gợi ý dùng từ khóa/câu hỏi để dễ xem lại ghi chú ở Card #3.
- Atlassian, [JQL operators](https://support.atlassian.com/jira-software-cloud/docs/jql-operators/) — chức năng tìm theo nội dung ticket trong Jira Cloud.
- GitHub Docs, [Searching issues and pull requests](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests) — cách tìm và lọc issue.
- Atlassian, [Use Rovo to search for work items](https://support.atlassian.com/jira-software-cloud/docs/use-atlassian-intelligence-to-search-for-work-items/) — tìm ticket bằng câu hỏi ngôn ngữ tự nhiên trong Jira Cloud.

Các nguồn trên chỉ hỗ trợ đề xuất cách cải thiện; không thay thế bằng chứng về trải nghiệm của tôi.

