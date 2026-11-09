# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Lê Thành Đạt
- MSSV: 2A202603579
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: TwoGuys
- Link repo nhóm: https://github.com/datlt203357/K5-L3A-DAY02-TwoGuys-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính                         | Job Story: Khi… tôi muốn… để…                                                                                                                       | Ai chịu ảnh hưởng?             | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng)                                   |
|---:|-----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------|---------------------------------------------------------------------------------------------|
| 1 | Lặp lại                           | Khi đến lịch chốt sprint công việc hàng tuần, tôi muốn hoàn thành log ticket công việc, để công sức làm việc của tôi đc ghi nhận đầy đủ.            | BA, PM, Manager                | 40-60 phút để log ticket vào cuối tuần                                                      |
| 2 | Cần đọc, tổng hợp nhiều thông tin | Khi cần sửa một tính năng mà tôi không làm, tôi muốn tìm tài liệu mô tả về tính năng đó, để hiểu luồng logic hiện tại của tính năng.                | BA, Developer, Tester          | Mất 1–3 giờ để hiểu một tính năng phức tạp                                                  |
| 3 | Lặp lại                           | Khi nhận ticket từ BA, tôi muốn hiểu rõ điều kiện đầu vào, đầu ra và các trường hợp ngoại lệ, để không phải hỏi lại nhiều lần trước khi code.       | PM, Manager, kế toán           | Mất 15–30 phút tổng hợp mỗi tháng                                                           |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi nhận yêu cầu từ khách hàng, tôi muốn hiểu rõ mong muốn của họ, để không phải hỏi lại                                                            | BA, Developer, Tester          | Số lần BA phải hỏi lại khách hàng để làm rõ yêu cầu,số vòng trao đổi để thống nhất yêu cầu. |
| 5 | Lặp lại: Tốn thời gian            | Khi tới cuối tháng, quản lý cần danh sách thông tin các ngày làm việc OT của tôi, để báo cáo và ghi nhận phụ cấp.                                   | PM, Manager                    | Cuối tháng mất thời gian tổng hợp lại từng ngày và số giờ OT                                |
| 6 | Lặp lại                           | Khi bắt đầu một sprint mới, tôi muốn xác định các ticket chưa được cập nhật trạng thái, để đảm bảo không bỏ sót công việc đang thực hiện.           | BA, PM                         | Thời gian kiểm tra và tổng hợp trạng thái ticket đầu sprint                                 |
| 7 | Lặp lại; Tốn thời gian            | Khi có người xử lý các lỗi người dùng đã từng xuất hiện, họ muốn có danh sách thông tin các lỗi đó, để không phải hỏi lại hướng xử lý từ người khác | Support, BA, Developer, Tester | Số lỗi tương tự đã từng xuất hiện; thời gian tìm lại thông tin lỗi cũ                       |
| 8 | Cần đọc, tổng hợp nhiều thông tin | Khi cần đánh giá tiến độ một tính năng, tôi muốn nắm được trạng thái công việc từ BA, Developer và Tester, để biết tính năng đang ở giai đoạn nào.  | PM, BA, Developer, Tester      | Thời gian tổng hợp tiến độ từ các thành viên                                                |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Khi bắt đầu một sprint mới, tôi muốn xác định các ticket chưa được cập nhật trạng thái, để đảm bảo không bỏ sót công việc đang thực hiện. - Giữ lại vì đây cũng là công việc lặp lại mỗi khi bắt đầu sprint mới
- Khi gửi yêu cầu thay đổi tính năng, tôi muốn biết BA đã hiểu đúng mong muốn của mình chưa, để tránh việc sản phẩm triển khai không đúng kỳ vọng. - Bỏ đi do trùng vấn đề với #3

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn                                                                                                                                                        | Điều còn chưa chắc                                                                       |
|---:|---------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------|
| 1 | #3      | Ảnh hưởng trực tiếp đến tiến độ công việc của dự án và nhiều vị trí: BA, Dev, Tester                                                                               |                                                                                          |
| 2 | #1      | Đây là vấn đề trực tiếp ảnh hưởng đến việc đánh giá và ghi nhận hiệu suất làm việc.                                                                                | Thời gian thực tế log ticket mỗi sprint và tần suất bỏ sót ticket có thường xuyên không? |
| 3 | #7      | Một số lỗi người dùng có thể xuất hiện lặp lại trong quá trình vận hành phần mềm. Người xử lý mới thường không nắm được lịch sử và kinh nghiệm xử lý lỗi trước đó. | Các lỗi cũ có được ghi nhận đầy đủ thông tin nguyên nhân và hướng xử lý không ?          |

### Problem Card #1

| Trường | Nội dung                                                                                                                                                                                                                                                                                                                         |
|---|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Job Story | Khi nhận ticket từ BA, tôi muốn hiểu rõ điều kiện đầu vào, đầu ra và các trường hợp ngoại lệ, để không phải hỏi lại nhiều lần trước khi code.                                                                                                                                                                                    |
| Actor | Developer, Tester                                                                                                                                                                                                                                                                                                                |
| Thời điểm / bối cảnh | Khi BA chuyển ticket sang Developer để bắt đầu thực hiện một tính năng hoặc yêu cầu mới.                                                                                                                                                                                                                                         |
| Quy trình hiện tại (3–7 bước) | 1. Developer nhận ticket từ BA. 2. Đọc nội dung và phân tích yêu cầu. 3. Kiểm tra điều kiện đầu vào, đầu ra và các trường hợp ngoại lệ. 4. Phát hiện thông tin chưa rõ hoặc còn thiếu. 5. Liên hệ BA để hỏi và xác nhận lại yêu cầu. 6. Chờ BA phản hồi, cập nhật cách hiểu yêu cầu. 7. Bắt đầu code sau khi đã hiểu rõ yêu cầu. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước đọc và làm rõ ticket: Developer phải hỏi lại BA nhiều lần do thiếu thông tin hoặc yêu cầu chưa rõ. Thời gian chờ phản hồi và số lần hỏi lại cần được đo lường thực tế.                                                                                                                                                      |
| Impact (nếu không giải thì sao) | Làm gián đoạn quá trình code, kéo dài thời gian hoàn thành ticket; tăng trao đổi qua lại giữa BA và Developer; có nguy cơ hiểu sai yêu cầu và phải sửa lại code.                                                                                                                                                                 |
| Success metric (baseline → target) | - Số lần Developer phải hỏi lại BA trên mỗi ticket: Baseline chưa đo → Target giảm. - Thời gian từ lúc nhận ticket đến khi làm rõ yêu cầu: Baseline chưa đo → Target giảm. - Tỷ lệ ticket phải bổ sung thông tin sau khi chuyển cho Developer: Baseline chưa đo → Target giảm.                                                   |
| Phương án không dùng AI | Xây dựng checklist thông tin bắt buộc trong ticket; sử dụng template thống nhất cho BA; bổ sung bước review ticket trước khi chuyển cho Developer.                                                                                                                                                                               |
| Giả thuyết về AI (nếu có) | AI có thể phân tích nội dung ticket, phát hiện các thông tin còn thiếu như input, output, business rules và edge cases; từ đó gợi ý câu hỏi cần BA làm rõ.                                                                                                                                                                       |
| Cảm nhận nhanh | No AI, Ưu tiên chuẩn hóa quy trình và template trước; chỉ cân nhắc AI nếu cần phân tích nội dung ticket phức tạp.                                                                                                                                                                                                                                                                                                                          |

Quy trình nháp hiện tại:

```text
Developer nhận ticket → Đọc và phân tích yêu cầu → Phát hiện thông tin chưa rõ → Hỏi BA → Chờ phản hồi → Làm rõ yêu cầu → Bắt đầu code.
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi đến lịch chốt sprint công việc hàng tuần, tôi muốn hoàn thành log ticket công việc, để công sức làm việc của tôi được ghi nhận đầy đủ.|
| Actor |BA – người thực hiện và tổng hợp log ticket công việc của bản thân.|
| Thời điểm / bối cảnh | Khi đến thời điểm chốt sprint hoặc cuối tuần, cần tổng hợp các ticket đã tham gia xử lý để báo cáo công việc.|
| Quy trình hiện tại (3–7 bước) |1. Nhận thông báo hoặc đến lịch chốt log ticket cuối sprint. 2. Kiểm tra lại các công việc đã thực hiện trong tuần. 3. Truy cập Jira hoặc công cụ quản lý công việc để tìm ticket liên quan. 4. Đối chiếu trạng thái và lịch sử xử lý ticket. 5. Tổng hợp thông tin công việc vào file log hoặc biểu mẫu báo cáo. 6. Kiểm tra lại các ticket đã ghi nhận. 7. Gửi log ticket cho người phụ trách. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước tìm kiếm, đối chiếu và tổng hợp ticket đã thực hiện. Thời gian ước tính ban đầu: 40–60 phút mỗi lần log cuối tuần; cần xác minh bằng quan sát thực tế.|
| Impact (nếu không giải thì sao) |Tốn thời gian tổng hợp công việc; dễ bỏ sót ticket hoặc ghi nhận thiếu đóng góp; ảnh hưởng đến tính chính xác của báo cáo và việc ghi nhận công sức làm việc. |
| Success metric (baseline → target) |- Thời gian hoàn thành log ticket: Baseline 40–60 phút (ước tính ban đầu) → Target giảm. - Số ticket bị bỏ sót khi log: Baseline chưa đo → Target tiến tới 0. - Số lần phải chỉnh sửa log do thiếu hoặc sai thông tin: Baseline chưa đo → Target giảm. |
| Phương án không dùng AI |Sử dụng template log thống nhất; cập nhật ticket ngay sau khi hoàn thành công việc; tạo checklist hoặc bộ lọc Jira để tổng hợp ticket theo người thực hiện và thời gian. |
| Giả thuyết về AI (nếu có) | AI có thể hỗ trợ tổng hợp lịch sử ticket, phân loại công việc theo từng tuần và tạo bản nháp log để BA kiểm tra trước khi gửi.|
| Cảm nhận nhanh | Ưu tiên Rule / Workflow vì dữ liệu ticket đã có cấu trúc và có thể lọc, tổng hợp tự động mà không nhất thiết cần AI. |

Quy trình nháp hiện tại:

```text
Đến lịch chốt sprint → Kiểm tra công việc đã làm → Tìm ticket trên Jira → Đối chiếu lịch sử → Tổng hợp vào file log → Kiểm tra → Gửi báo cáo.
```

### Problem Card #3

| Trường | Nội dung                                                                                                                                                                                                                                                                                                                                                                                |
|---|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Job Story | Khi xử lý các lỗi đã từng xuất hiện, tôi muốn có danh sách thông tin các lỗi đó, để không phải hỏi lại hướng xử lý từ người khác.                                                                                                                                                                                                                                                       |
| Actor | Support, BA hoặc Developer                                                                                                                                                                                                                                                                                                                                                              |
| Thời điểm / bối cảnh | Khi tiếp nhận lỗi người dùng báo cáo và phát hiện lỗi có dấu hiệu tương tự những lỗi đã từng xảy ra trước đây.                                                                                                                                                                                                                                                                          |
| Quy trình hiện tại (3–7 bước) | 1. Tiếp nhận thông tin lỗi từ người dùng. 2. Kiểm tra mô tả, triệu chứng và bối cảnh phát sinh lỗi. 3. Nhận thấy lỗi có thể đã từng xuất hiện. 4. Tìm kiếm thông tin lỗi cũ trong ticket, tài liệu hoặc lịch sử trao đổi. 5. Nếu không tìm được thông tin, hỏi đồng nghiệp về nguyên nhân và hướng xử lý. 6. Thực hiện xử lý lỗi và kiểm tra kết quả. 7. Cập nhật trạng thái xử lý lỗi. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước tìm kiếm thông tin lỗi cũ và hỏi đồng nghiệp để xác định hướng xử lý. Thời gian tìm kiếm, thời gian chờ phản hồi và tần suất xảy ra chưa được đo lường.                                                                                                                                                                                                                            |
| Impact (nếu không giải thì sao) | Mất thời gian tìm kiếm và trao đổi với đồng nghiệp; phụ thuộc vào kinh nghiệm của người khác; có nguy cơ xử lý lại từ đầu hoặc áp dụng hướng xử lý không nhất quán giữa các nhân viên.                                                                                                                                                                                                  |
| Success metric (baseline → target) | - Thời gian tìm được thông tin lỗi tương tự: Baseline chưa đo → Target giảm. - Số lần phải hỏi đồng nghiệp về lỗi đã từng xuất hiện: Baseline chưa đo → Target giảm. - Tỷ lệ lỗi lặp lại có thể tìm được nguyên nhân và hướng xử lý cũ: Baseline chưa đo → Target tăng.                                                                                                                 |
| Phương án không dùng AI | Xây dựng danh mục lỗi đã biết (Known Error List); chuẩn hóa cách ghi nhận mã lỗi, triệu chứng, nguyên nhân, hướng xử lý và trạng thái; sử dụng bộ lọc hoặc từ khóa để tra cứu ticket cũ.                                                                                                                                                                                                |
| Giả thuyết về AI (nếu có) | AI có thể phân tích mô tả lỗi mới, tìm các lỗi cũ có nội dung hoặc triệu chứng tương tự, sau đó gợi ý nguyên nhân và hướng xử lý đã được ghi nhận.                                                                                                                                                                                                                                      |
| Cảm nhận nhanh | Workflow, Có thể bắt đầu bằng hệ thống tra cứu theo từ khóa; cân nhắc AI nếu cần tìm các lỗi tương tự dù cách mô tả khác nhau.                                                                                                                                                                                                                                                                                                                                                                              |

Quy trình nháp hiện tại:

```text
Tiếp nhận lỗi → Phân tích triệu chứng → Nhận diện lỗi có thể đã xuất hiện → Tìm ticket hoặc tài liệu cũ → Hỏi đồng nghiệp nếu không tìm thấy → Xử lý lỗi → Cập nhật kết quả.
```

### Card muốn pitch nhất

- Card số: 3
- Vì sao: Lỗi người dùng có thể xuất hiện lặp lại, khiến người xử lý phải tìm lại thông tin hoặc hỏi đồng nghiệp về hướng giải quyết.
- Câu hỏi muốn nhóm phản biện: Câu hỏi muốn nhóm phản biện: Khi gặp lỗi tương tự, người xử lý có thực sự phải hỏi đồng nghiệp hay đã có thể tự tìm được thông tin trong hệ thống?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
|Chưa xác định rõ ai là người trực tiếp gặp pain. | Có|Xác định Support, BA hoặc Developer là các vai trò có thể chịu ảnh hưởng; cần phỏng vấn để xác định actor chính.|

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì?                                                                                                | Kết quả / ảnh hưởng tới bài nhóm                                                                 |
|---|---------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
| Pitch Problem Card | Chuẩn bị 3 Card: Chốt ticket sprint, Xử lý lỗi đã xuất hiện, Ticket thiếu thông tin.                          | Vào shortlist và được chọn.                                                                      |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt:   Hỏi Huy: README đã chỉ dẫn các file cụ thể, chỗ nào khiến bạn vẫn phải dò thêm 15 phút? | Huy nhận định rằng chỉ dẫn README chưa đủ rõ ràng.                                               |
| Nhận phản biện | Câu hỏi tôi nhận được:     Lần gần nhất xử lý lại lỗi cũ, bạn đã tìm hướng xử lý ở đâu và mất bao lâu?        | Câu hỏi giúp nhóm thấy #6 còn thiếu một ca xử lý cụ thể và thời gian tìm.                        |
| Chọn candidate problem | Nhóm thống nhất chọn #6 — tìm lại thông tin và cách xử lý lỗi cũ.                                             | Nhóm chuyển sang phác thảo quy trình và tìm cách kiểm chứng; lựa chọn vẫn cần bằng chứng thực tế. |
| Kiểm chứng / research | Tìm và lựa chọn các phương án đã có.                                                                          | Bảng research của nhóm đã có nguồn, nhưng phần kiểm chứng với người thật còn hạn chế.            |
| Quyết định | Quyết định Not Yet với AI.                                                                                    | Cả nhóm bàn luận và đưa ra quyết định cuối cùng.                                                 |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì?                          | AI hữu ích ở đâu?                                                               | AI sai hoặc hời hợt ở đâu?                                  | Tôi sửa gì bằng nhận định của mình?                        |
|---|-------------------------------------------------|---------------------------------------------------------------------------------|-------------------------------------------------------------|------------------------------------------------------------|
| CP1 Scan | Gợi ý thêm problem theo vai trò BA              | Đưa ra thêm được problems                                                       | Một số problem có nội dung tương tự nhau                    | Bỏ đi 1 số problem không cần thiết                         |
| CP2 Problem Card | Nhờ AI đưa ra phản biệt cho các problem card    | Phát hiện những phần còn thiếu và gợi ý các chỉ số có thể dùng để đo lường pain | Một số nội dung còn chung chung, xác định chưa chính xác                                                            | Kiểm tra lại tình huống thực tế từ việc phỏng vấn          |
| CP4 Research | Tìm các giải pháp và công cụ                    | Gợi ý: Jira Cloud, GitHub Issues, Jira Rovo                                     |             Một số nhận định về giải pháp còn khái quát, chưa chỉ rõ giới hạn và điều kiện sử dụng             | Kiểm tra lại nguồn thông tin  về từng giải pháp            |
| CP6 Mức can thiệp / quyết định | Nhờ AI đưa ra phản biện đối với từng quyết định | Giúp đưa ra được mức độ đáp ứng của công cụ, giải pháp hiện tại                 | AI chưa có đủ dữ liệu thực tế để kết luận giải pháp phù hợp | Nhóm dựa vào phản biện của AI và chốt quyết định cuối cùng |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Sau khi nghe 3 problems của các bạn khác, tôi có thể mở rộng góc nhìn, học cách nhìn vấn đề từ trải nghiệm của người khác. Tôi nhận ra những công việc tưởng chừng đơn giản vẫn có thể gây lãng phí thời gian và ảnh hưởng đến nhiều người nếu xảy ra thường xuyên.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Có, khi phân tích vấn đề tra cứu lỗi cũ, nhóm từng nghĩ ngay đến việc xây dựng hệ thống lưu trữ lỗi hoặc sử dụng AI để tìm kiếm. Sau đó, nhóm nhận ra cần hiểu rõ pain thực tế và tìm hiểu các công cụ hiện có trước khi lựa chọn giải pháp.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Có, ban đầu tôi cho rằng vấn đề tra cứu lỗi cũ rất đáng ưu tiên vì người xử lý thường phải hỏi đồng nghiệp. Tuy nhiên, sau khi phản biện, tôi nhận ra nhóm chưa có đủ bằng chứng về tần suất lỗi lặp lại và thời gian tìm kiếm, nên cần kiểm chứng thêm trước khi quyết định.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Điều khiến tôi bất ngờ là thị trường đã có nhiều công cụ như Jira nhưng chưa thực sự có nhiều quy trình cụ thể với pain này.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Điều khó nhất đối với tôi là xác định đúng người thực sự gặp pain và phân biệt biểu hiện của vấn đề với nguyên nhân gốc rễ. Ngoài ra, việc viết Job Story ngắn gọn nhưng vẫn thể hiện đầy đủ bối cảnh, mong muốn và mục đích cũng khá khó khăn.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại, tôi sẽ phỏng vấn người dùng và thu thập bằng chứng thực tế sớm hơn, đồng thời nghiên cứu các giải pháp hiện có ngay từ đầu thay vì chỉ dựa vào cảm nhận cá nhân.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
Vấn đề nhóm tôi lựa chọn là người xử lý gặp khó khăn khi tra cứu các lỗi đã từng xuất hiện và thường phải hỏi đồng nghiệp về hướng xử lý. Quy trình hiện tại gồm tiếp nhận lỗi, phân tích triệu chứng, tìm kiếm ticket hoặc tài liệu cũ, hỏi đồng nghiệp nếu không tìm thấy thông tin, sau đó tiến hành xử lý lỗi. Nhóm sử dụng các metric như thời gian tìm được thông tin lỗi cũ, số lần phải hỏi đồng nghiệp và tỷ lệ lỗi lặp lại tìm được hướng xử lý. Phạm vi giải quyết chỉ tập trung vào việc tra cứu và tham khảo thông tin các lỗi đã được ghi nhận, không tự động kết luận nguyên nhân hoặc quyết định cách sửa lỗi. AI có thể được sử dụng để tìm kiếm các lỗi tương tự bằng ngữ nghĩa và tóm tắt hướng xử lý đã có, nhưng người xử lý vẫn phải kiểm tra và xác nhận. Nhóm ưu tiên cách tiếp cận kết hợp tìm kiếm thông thường với AI khi cần thiết, thay vì để AI tự động xử lý lỗi. Quyết định hiện tại là Not Yet, vì nhóm cần kiểm chứng thêm tần suất lỗi lặp lại, thời gian tra cứu và số người thực sự gặp vấn đề trước khi quyết định triển khai.
---

## 7. Tài liệu tham khảo

-
