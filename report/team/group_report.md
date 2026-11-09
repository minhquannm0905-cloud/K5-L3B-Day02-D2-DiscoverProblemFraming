# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: D2
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Người học mất thời gian tìm lại đúng thông báo và tài liệu trước buổi học, họp hoặc kiểm tra vì nội dung bị phân tán trong nhóm chat và nhiều file đính kèm.
- Quyết định cuối: - Quyết định cuối: Go, phạm vi nhỏ — pilot Rule trong 2 tuần

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Nguyễn Như Duy An | Khi khách gửi yêu cầu bảo hành kèm mô tả/ảnh, cần trích seri, phân loại lỗi sơ bộ và gán người xử lý để hẹn khách trong 15 phút. | Điều phối viên dịch vụ | Diễn giải mô tả không chuyên môn thành nhóm lỗi: 4 phút/ca | "Khách hàng mô tả bằng từ ngữ lộn xộn hoặc chụp tem vỡ mờ, nhóm lấy dữ liệu thực tế ở đâu trong buổi lab để kiểm chứng mô hình phân loại lỗi mà không vi phạm thông tin khách hàng?" (Nguyễn Minh Quân) |
| 2 | Nguyễn Như Duy An | Khi nhận hồ sơ hoàn ứng gồm ảnh hóa đơn/vé xe, cần đối soát ngày, mã số thuế và số tiền để duyệt trong ngày. | Kế toán thanh toán nội bộ | So khớp hóa đơn với bảng kê: 10 phút/bộ | "Hóa đơn giấy bị nhàu, chụp mờ hoặc viết tay thì OCR nhận diện sai số tiền/mã số thuế, kế toán vẫn phải mở từng ảnh đối soát thủ công thì có thực sự cắt giảm được 10 phút không?" (Mai Xuân Khang) |
| 3 | Nguyễn Như Duy An | Khi nhận file COD cuối ngày, cần đối chiếu mã vận đơn và tiền thực nhận để phát hiện đơn lệch cước/chưa thanh toán. | Kế toán đối soát công nợ | Rà nguyên nhân từng dòng lệch: 45 phút/ngày | "Viết script Python hoặc dùng hàm Excel so khớp hai cột mã đơn và tiền cước đã giải quyết được 85% trường hợp, tại sao phải dùng AI để tăng chi phí và rủi ro tính toán sai lệch?" (Nguyễn Minh Quân) |
| 4 | Mai Xuân Khang | Khi kết thúc buổi học, cần tổng hợp ý chính từ bài giảng/slide để ôn lại mà không đọc hoặc nghe lại toàn bộ. | Người học | Chọn và viết lại ý chính | "Mốc 15 phút là ước tính hay bạn đã bấm giờ thật? Nếu học viên không tự chọn lọc và viết lại ý chính mà để máy tóm tắt hộ thì lúc thi có thực sự hiểu bài không?" (Nguyễn Như Duy An) |
| 5 | Mai Xuân Khang | Khi ôn thi từ nhiều nguồn, cần xác định kiến thức trọng tâm và nội dung thiếu để ưu tiên ôn hiệu quả. | Người học | Đối chiếu kiến thức giữa nhiều nguồn | "Mỗi môn học có cấu trúc đề và đề cương riêng, làm sao công cụ biết tài liệu nào là chuẩn để so sánh đối chiếu mà không bịa ra thông tin sai lệch?" (Nguyễn Minh Quân) |
| 6 | Mai Xuân Khang | Khi làm bài tập nhóm nhiều thành viên, cần theo dõi nhiệm vụ, tiến độ và thay đổi để tránh sót việc/trễ hạn. | Thành viên nhóm học tập | Đối chiếu thông báo, thay đổi và hạn mới nhất | "Bước nghẽn 12 phút là do thiếu công cụ hay do nhóm thiếu kỷ luật cập nhật? Nếu chỉ cần lập một bảng Google Sheets chung và quy ước ai đổi việc phải tự vào sửa thì có giải quyết triệt để mà không cần phần mềm không?" (Mai Xuân Khang) |
| 7 | Nguyễn Minh Quân | Khi chuẩn bị học/họp/kiểm tra, cần tìm lại đúng thông báo và tài liệu để không bỏ sót yêu cầu. | Người học | Tìm và mở đúng tài liệu: 3–5 phút/lần | "Nếu nhóm trưởng ghim thông báo quan trọng lên đầu nhóm chat và tạo sẵn thư mục Google Drive theo từng môn, liệu sinh viên có tìm được ngay mà không cần xây dựng công cụ mới không?" (Mai Xuân Khang) |
| 8 | Nguyễn Minh Quân | Khi nộp Lab AI thực chiến, cần kiểm tra yêu cầu, tên file và cấu trúc để tránh bị trừ điểm. | Người học làm lab | Đọc và đối chiếu rubric: phần lớn trong 10 phút/lab | "Mỗi lab chỉ nộp 1 lần/tuần, việc tự đọc checklist rubric mất 10 phút là trách nhiệm tự kiểm tra của sinh viên. Tần suất này có đủ dày đặc để xem là một bottleneck đáng đầu tư giải pháp không?" (Mai Xuân Khang) |
| 9 | Nguyễn Minh Quân | Khi nhận lịch kiểm tra/deadline từ email và Zalo, cần tổng hợp ở một nơi để không quên hạn hoặc nhầm lịch thi. | Người học theo nhiều học phần | Tìm thông báo có lịch/deadline: phần lớn trong 10–15 phút/lần | "Lịch thi và hạn nộp gửi qua email trường và Zalo cá nhân, giải pháp nào trích xuất tự động được hai nguồn này mà không vi phạm chính sách bảo mật tài khoản và quyền riêng tư?" (Nguyễn Như Duy An) |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Đối soát vận hành/tài chính | #2 Hoàn ứng; #3 COD | Đối chiếu dữ liệu, phát hiện sai lệch và giảm xử lý thủ công. |
| B — Tiếp nhận yêu cầu dịch vụ | #1 Bảo hành | Chuẩn hóa thông tin đầu vào mơ hồ trước khi chuyển cho người xử lý. |
| C — Quản lý thông tin học tập | #4–#5 Tổng hợp/ôn tập; #7–#9 Thông báo, lab, lịch | Thông tin rải rác làm người học mất thời gian tìm, đọc, đối chiếu và theo dõi. |
| D — Phối hợp nhóm | #6 Theo dõi tiến độ nhóm | Thay đổi phân tán khiến thành viên hỏi lại, sót việc hoặc trễ hạn. |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian và sai sót khi xử lý thông tin rải rác trong các quy trình lặp lại
├── Opportunity A: Dữ liệu vận hành/tài chính nằm ở nhiều file, cần đối soát để tìm sai lệch
├── Opportunity B: Thông tin đầu vào của khách không chuẩn hóa, dẫn đến phân loại hoặc phân công sai
├── Opportunity C: Thông báo, tài liệu và rubric học tập nằm ở nhiều nơi, dễ bị bỏ sót
└── Opportunity D: Nhiệm vụ và thay đổi trong nhóm không được cập nhật ở một nơi
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- "AI tự chẩn đoán linh kiện hỏng".
- "Chatbot tóm tắt mọi tài liệu học tập".
- "Agent tự gửi email khiếu nại cho đơn vị giao vận".
- "Một app quản lý toàn bộ deadline".

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Đối soát tiền thu hộ COD (#3) | 5 | 5 | 5 | 5 | 5 | 5 | 3 | **33** |
| Tiếp nhận và phân loại bảo hành (#1) | 5 | 5 | 5 | 5 | 5 | 5 | 3 | **33** |
| Tìm lại thông báo và tài liệu môn học (#7) | 5 | 5 | 4 | 3 | 5 | 5 | 5 | **32** |

> Các điểm trên tổng hợp từ báo cáo cá nhân; nhóm đã chốt candidate #7 sau pitch. Nhóm vẫn cần ghi lại câu hỏi phản biện thật của từng thành viên vào bảng pitch.

**Candidate được chọn:** Tìm lại thông báo và tài liệu trước buổi học, họp hoặc kiểm tra (#7 — Nguyễn Minh Quân).

**Vì sao chọn:** Actor và quy trình rõ; nhóm hiểu domain người học và có thể kiểm chứng nhanh với người học thật mà không cần truy cập dữ liệu tài chính, bảo hành hoặc khách hàng nội bộ. Bottleneck có phạm vi nhỏ (tìm và mở đúng tài liệu), thời gian baseline đã có (3–5 phút/lần), đồng thời nhóm so sánh được các mức No AI / Rule / Workflow trước khi kết luận có cần AI hay không.

**Vì sao loại các candidate còn lại:**

- Đối soát COD và hoàn ứng có impact tài chính rõ nhưng cần file vận hành thật, quyền truy cập và xác minh từ kế toán; nhóm khó kiểm chứng an toàn trong thời gian lab.
- Tiếp nhận bảo hành có rủi ro phân công/kỹ thuật sai và cần dữ liệu khách hàng, ảnh thiết bị; nhóm chưa đủ domain để đánh giá đầu ra.
- Nhóm chưa có đủ bằng chứng hành vi để ưu tiên các đề xuất tổng hợp kiến thức và ôn tập của Mai Xuân Khang.
- Kiểm tra yêu cầu nộp Lab và tổng hợp deadline có scope gần với candidate được chọn, nhưng pain "tìm đúng thông báo/tài liệu" xảy ra ngay trước nhiều loại hoạt động hơn và có thể là nguyên nhân gốc.

**Xử lý bất đồng (nếu có):** Nhóm ưu tiên candidate dễ kiểm chứng với người học thật và ít rủi ro dữ liệu hơn các candidate vận hành. Các candidate COD/bảo hành được giữ ở hướng tiếp theo.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Người học thường phải tìm lại thông báo, deadline, quyết định đã chốt hoặc link tài liệu trong nhóm chat. | Value | 5 | 4 | ✅ |
| 2 | Việc tìm lại thông tin thường lặp lại ít nhất 3 lần trong một tuần học/làm nhóm. | Value | 5 | 4 | ✅ |
| 3 | Người học mất từ 5 phút trở lên mới tìm được thông tin cần thiết. | Value | 5 | 4 | ✅ |
| 4 | Ghim tin nhắn/bảng phân công hiện tại chưa giải quyết triệt để vì thông tin vẫn cần được cập nhật. | Usability | 4 | 4 | ✅ |
| 5 | Một mục lục chung có định dạng cố định sẽ giúp người học tìm đúng thông tin nhanh hơn. | Usability | 5 | 1 | ✅ |
| 6 | Nhóm có thể duy trì một nguồn thông tin chuẩn mà không cần tích hợp AI hay truy cập dữ liệu riêng tư. | Feasibility | 4 | 3 | — |

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này: 1–4 bằng micro survey; giả định 5 sẽ được kiểm chứng bằng pilot 2 tuần ở CP6.

### 3.2. Kiểm chứng

Cách đã dùng: **Micro survey ẩn danh, 11 người trả lời**, về hành vi tìm lại thông tin trong 7 ngày gần nhất. Ảnh kết quả survey cần được giữ trong `report/assets/` để các link dưới đây hiển thị.

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Không áp dụng — nhóm dùng survey ẩn danh thay cho phỏng vấn. |
| Câu nói đáng nhớ nhất (nguyên văn) | Không thu thập câu trả lời mở; không bịa trích dẫn. |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Survey hỏi hành vi trong 7 ngày gần nhất: 9/11 người phải tìm lại hoặc hỏi lại thông tin đã chốt từ 3 lần trở lên. |
| Hiện đang xử lý bằng cách nào (workaround)? | Tìm kiếm trong chat (9/11), hỏi lại nhóm/nhắn riêng (8/11), cuộn lịch sử chat và xem tin ghim (mỗi cách 7/11), mở biên bản/bảng phân công (6/11). |
| Mất bao lâu, bao lần? | 8/11 mất từ 5 phút trở lên trong lần tìm gần nhất; 9/11 phải tìm lại ít nhất 3 lần trong 7 ngày. |
| Insight / opportunity rút ra | Vấn đề không chỉ là thiếu công cụ tìm kiếm: các cách hiện tại đã được dùng nhưng 7/11 nói vẫn phải cập nhật; cần một nguồn chuẩn có người chịu trách nhiệm cập nhật. |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Micro survey ẩn danh | 11 người | Deadline/mốc thời gian là thông tin được tìm lại nhiều nhất (10/11); tiếp theo là người phụ trách và quyết định/phương án đã chốt (mỗi loại 8/11), link tài liệu/file (7/11). Mức độ phiền trung bình là 4/5. | 2/11 cho biết chưa từng gặp hậu quả làm trùng, làm sai hoặc trễ việc trong tháng qua; vì vậy problem không xảy ra giống nhau với mọi người. |

Evidence survey: [nhóm/kênh trao đổi](../assets/cp4_survey_result.png) · [tần suất và loại thông tin](../assets/cp4-survey-result2.png) · [thời gian và cách tìm](../assets/cp4-survey-result3.png) · [hậu quả](../assets/cp4-survey-result4.png) · [workaround](../assets/cp4-survey-result5.png) · [mức độ phiền](../assets/cp4-survey-result6.png).

**Nhóm đã sửa problem thế nào sau kiểm chứng:** Thu hẹp từ “tìm thông báo và tài liệu” thành “tìm lại thông tin đã chốt có ảnh hưởng đến hành động: deadline, người phụ trách, quyết định và link tài liệu chính thức”. Không giả định mọi người đều gặp hậu quả nặng; pilot chỉ nhắm vào nhóm học/làm việc qua chat có nhu cầu cập nhật thường xuyên.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Google Drive — tìm file trong Drive | https://support.google.com/drive/answer/2375114 | Tìm link/tài liệu khi file đã nằm trong một Drive có quyền truy cập phù hợp | Có tìm kiếm và bộ lọc theo loại/chủ sở hữu/thời gian | Không giải quyết việc deadline hoặc quyết định nằm trong chat; cần người biết nơi lưu file | Lưu file đúng nơi chỉ giải quyết một phần; mục lục phải giữ link nguồn chuẩn |
| Slack — tabs/bookmarks trong kênh | https://slack.com/help/articles/32562841868307-Add-and-manage-tabs-in-channels-and-direct-messages | Ghim tài liệu/liên kết tham chiếu trong một kênh | Tạo nơi truy cập nhanh, không cần AI | Phụ thuộc người dùng cập nhật; survey cho thấy 7/11 người vẫn phải cập nhật workaround hiện tại | Cần quy ước rõ ai cập nhật, khi nào cập nhật và thông tin nào bắt buộc ghi |
| Discord — pinned messages | https://support.discord.com/hc/en-us/articles/221421867-Pin-Messages-FAQ | Đánh dấu thông báo quan trọng trong chat | Đơn giản, có sẵn trong công cụ chat | Tin ghim vẫn có thể nhiều và thiếu ngữ cảnh như deadline/owner/phiên bản tài liệu | Pin chỉ là lớp lưu trữ; nhóm cần mẫu record cố định để truy hồi nhanh |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
[1. Nhận thông báo hoặc file qua chat/email/LMS: 0.5']
→ [2. Nhớ từ khóa hoặc đoán nơi đã gửi: 1']
→ [3. Tìm kiếm/cuộn chat và mở các link liên quan: 3–8'] ← BOTTLENECK
→ [4. Kiểm tra đúng phiên bản, deadline hoặc người phụ trách: 1–3']
→ [5. Ghi lại việc cần làm hoặc hỏi lại nhóm: 1–2']
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Người học | Thông báo/file mới từ chat, email hoặc LMS | Tin nhắn/link cần lưu ý | Mỗi khi có cập nhật | Nguồn thông tin phân tán |
| 2 | Người học | Từ khóa, trí nhớ về nơi gửi | Câu truy vấn hoặc vị trí cần tìm | Khoảng 1 phút/lần | Có thể không nhớ đúng kênh/từ khóa |
| 3 | Người học | Lịch sử chat, email, Drive, LMS | Thông báo hoặc tài liệu ứng viên | 3–8 phút/lần | Dễ mở nhầm file hoặc bỏ sót tin cũ |
| 4 | Người học | Thông báo/tài liệu đã mở | Xác nhận deadline, người phụ trách, phiên bản đúng | 1–3 phút/lần | Có thể hỏi lại nếu chưa chắc |
| 5 | Người học | Thông tin đã xác nhận | Việc cần chuẩn bị/cập nhật cá nhân | 1–2 phút/lần | Có thể phát sinh hỏi lại nhóm |

**Bottleneck chính:** Bước 3 — tìm kiếm/cuộn nhiều nguồn và mở đúng thông báo/tài liệu. Survey cho thấy 8/11 người mất từ 5 phút trở lên trong lần tìm gần nhất.

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
[1. Người gửi thông báo theo mẫu cố định: môn/nhóm, loại thông tin, ngày, link nguồn] ← RULE
→ [2. Người phụ trách cập nhật một mục lục chung trong 10 phút] ← CON NGƯỜI
→ [3. Người học tìm theo loại thông tin/môn/ngày trong mục lục] ← RULE
→ [4. Người học mở link nguồn và tự xác nhận nội dung] ← CON NGƯỜI
→ [5. Nếu không có record hoặc link lỗi, quay về chat/email/LMS gốc và báo người phụ trách] ← FALLBACK
```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 5 | 5 | Thêm bước cập nhật mục lục nhưng giảm tìm kiếm phân tán |
| Tổng thời gian | 5–10 phút hoặc lâu hơn (8/11 survey) | Mục tiêu dưới 2 phút để tìm và mở đúng nguồn | Đo trên các lần tìm trong pilot |
| Số bước thủ công | 5/5 | 3/5 | Người phụ trách cập nhật; người học xác nhận nguồn |
| Bottleneck chính | Tìm kiếm/cuộn nhiều nguồn | Kỷ luật cập nhật mục lục | Nếu record đầy đủ, việc tìm giảm đáng kể |
| Rủi ro mới phát sinh | — | Mục lục cũ, link sai hoặc thiếu record | Có owner, mốc cập nhật và fallback về nguồn gốc |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Người học làm việc qua chat, email, LMS và file đính kèm cho một học phần hoặc nhóm học tập. |
| **Quy trình** | Nhận thông báo/file → nhớ hoặc đoán nơi gửi → tìm/cuộn nhiều nguồn → mở và kiểm tra đúng nội dung → ghi lại việc cần làm hoặc hỏi lại. |
| **Bottleneck** | Tìm và mở đúng thông báo/tài liệu trong các nguồn phân tán; 8/11 người khảo sát mất từ 5 phút trở lên ở lần tìm gần nhất. |
| **Impact** | Deadline là thông tin bị tìm lại nhiều nhất (10/11). Trong tháng gần nhất, 5/11 người cho biết việc không tìm lại được thông tin từng làm họ hoặc nhóm làm trùng, làm sai hoặc trễ việc. |
| **Success Metric** (baseline → target, cách đo) | Baseline: 8/11 mất từ 5 phút trở lên; target pilot: ít nhất 70% lượt tìm dưới 2 phút và không có lần dùng nhầm link/phiên bản trong 2 tuần. Đo bằng log 10–15 lượt tìm và đối chiếu với nguồn gốc. |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | Không dùng AI để suy đoán deadline/quyết định từ chat. Người gửi hoặc người phụ trách phải xác nhận record; người học mở link nguồn trước khi hành động. |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

- Phản biện cần kiểm tra thêm: baseline survey là nhóm nhỏ, chọn mẫu thuận tiện; nhóm không được suy rộng cho toàn bộ người học. Vì vậy pilot 2 tuần là bước kiểm chứng tiếp theo.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **Độ mơ hồ thấp–trung bình × độ phức tạp thấp.**

Vì sao: Người học biết mình cần loại thông tin nào (deadline, người phụ trách, quyết định, link tài liệu), nhưng các nguồn đang phân tán. Các bước cần làm có thể dự đoán trước; không cần hệ thống tự chọn mục tiêu hoặc hành động tiếp theo.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Ghim tin quan trọng, lưu link theo thư mục hoặc bảng chung | Nhóm có ít thông báo và người gửi luôn cập nhật | Dễ thành nhiều nơi lưu, thiếu owner | Dùng làm nền |
| **Rule** | Mỗi record bắt buộc có: môn/nhóm, loại thông tin, deadline hoặc ngày cập nhật, link nguồn, người cập nhật | Nguồn thông tin có cấu trúc cố định; người học chỉ cần lọc/tìm record | Record có thể cũ hoặc thiếu | **Chọn** |
| **Workflow** | Thu thập tin từ chat/email/LMS → AI tóm tắt/gắn nhãn → người phụ trách duyệt → đăng mục lục | Khi có quyền truy cập các nguồn và Rule không đủ | Sai ngữ cảnh, quyền truy cập, chi phí tích hợp | Không chọn ở pilot |
| **Agent** | Tự đọc mọi nguồn, tự quyết thông tin nào quan trọng và tự gửi nhắc việc | Chỉ phù hợp khi bước tiếp theo không cố định | Bỏ sót/suy đoán sai deadline hoặc quyết định; khó kiểm soát | Không chọn |

**Mức chọn:** Rule, trên nền sửa quy trình No AI.

**Vì sao không chọn mức đơn giản hơn:** Chỉ ghim tin hoặc để bảng chung không đủ vì survey cho thấy chúng đã được dùng (7/11 ghim tin, 7/11 dùng bảng phân công) nhưng 7/11 vẫn phải cập nhật cách xử lý. Rule bổ sung trường thông tin bắt buộc và owner cập nhật, giúp mọi người tìm theo cùng một cấu trúc.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Không áp dụng: nhóm chọn Rule, không dùng AI ở pilot. |
| **Judgment** — con người cân nhắc, quyết định gì? | Người gửi/người phụ trách xác nhận record có đúng và đủ trước khi công bố. |
| **Action** — hành động cuối cùng là gì, ai làm? | Người phụ trách cập nhật mục lục; người học tự mở nguồn gốc và hành động theo thông tin đã xác nhận. |
| **Outcome** — đo kết quả bằng gì? | Tỷ lệ lượt tìm dưới 2 phút, số record đúng/đủ, số lần dùng nhầm link/phiên bản. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Không áp dụng cho pilot Rule. |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Log lượt tìm, record bị thiếu/sai, và phản hồi của người học cuối pilot. |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Không áp dụng trực tiếp vì pilot không dùng AI. Thiết kế chỉ chuẩn hóa nơi ghi và cách tìm, còn con người xác nhận nguồn gốc.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Nếu sau này dùng AI, bỏ sót hoặc suy đoán nhầm deadline/quyết định đều nghiêm trọng. Vì vậy pilot giữ nguồn gốc và người xác nhận làm boundary.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Người học làm việc qua chat, email, LMS và file đính kèm cho một học phần hoặc nhóm học tập. |
| **Quy trình** | Người gửi đăng thông báo theo mẫu → người phụ trách cập nhật record chuẩn → người học lọc/tìm record → mở link nguồn → thực hiện việc cần làm. |
| **Bottleneck** | Không có nguồn chuẩn; người học phải tìm/cuộn nhiều nguồn để mở đúng thông báo/tài liệu. |
| **Impact** | 8/11 mất từ 5 phút trở lên; 5/11 từng báo hậu quả làm trùng, làm sai hoặc trễ việc trong tháng gần nhất. |
| **Success Metric** (baseline → target, cách đo) | Từ 8/11 lượt tìm mất từ 5 phút trở lên xuống ít nhất 70% lượt tìm dưới 2 phút; 0 lần dùng nhầm link/phiên bản trong pilot 2 tuần. Đo bằng log 10–15 lượt tìm và kiểm tra nguồn gốc. |
| **Boundary** | Record chỉ là chỉ mục, không thay thế thông báo gốc. Người học không được hành động chỉ dựa vào tóm tắt; người phụ trách xác nhận record trước khi công bố. |
| **AI intervention point** | Không có trong pilot. |
| **Mức chọn** | Rule, trên nền No AI. |
| **Rủi ro & người kiểm tra** | Record thiếu/cũ, link lỗi hoặc gắn sai loại thông tin → người phụ trách cập nhật kiểm tra; người học đối chiếu link nguồn trước khi hành động. |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Quy trình | Tìm trực tiếp trong chat/email/LMS | Thêm mục lục record chuẩn trước khi tìm | Survey cho thấy các workaround hiện tại vẫn cần cập nhật |
| Mức can thiệp | Chưa xác định | Rule trên nền No AI | Các bước cố định, không cần AI/Agent tự quyết |
| Success Metric | Chỉ có thời gian cá nhân 3–5 phút | Dùng baseline survey và đo tỷ lệ tìm dưới 2 phút + link/phiên bản đúng | Bổ sung chất lượng, không chỉ đo nhanh |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Record đầy đủ | Có môn/nhóm, loại thông tin, ngày hoặc deadline, link nguồn và người cập nhật | Thiếu một trường bắt buộc |
| 2 | Record đúng nguồn | Link mở được và khớp thông báo/tài liệu gốc | Link lỗi, link sai hoặc phiên bản cũ |
| 3 | Record kịp thời | Được cập nhật trong 10 phút từ khi có quyết định/thông báo cuối | Cập nhật muộn khiến người học phải tìm lại chat |
| 4 | Tìm được nhanh | Người học tìm và mở đúng nguồn dưới 2 phút | Mất từ 5 phút trở lên hoặc phải hỏi lại nhóm |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | Trung bình | Survey 11 người cho thấy pain lặp lại và 8/11 mất từ 5 phút trở lên, nhưng mẫu nhỏ và không đại diện toàn bộ người học. |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | Trung bình | Rule đơn giản nhưng cần hình thành thói quen: 7/11 nói workaround hiện tại vẫn phải cập nhật. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | Thấp | Có thể dùng bảng chung/Drive/LMS hiện có; không yêu cầu tích hợp AI hoặc dữ liệu riêng tư. |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | Thấp | Không phát sinh chi phí AI; chỉ cần một người phụ trách cập nhật theo quy ước nhóm. |

### 8.2. Kết luận

**Quyết định:** Go, phạm vi nhỏ — pilot Rule trong 2 tuần.

**Lý do:** Pain đã có evidence survey, không có rủi ro Cao, và phương án Rule đơn giản hơn AI. Pilot nhằm kiểm chứng giả định quan trọng nhất: nhóm có thực sự cập nhật mục lục đúng hạn và người học có tìm nhanh hơn không.

**Nếu Go — pilot nhỏ nhất:** Một nhóm học/làm việc dùng một bảng mục lục chung trong 2 tuần. Mỗi thông báo/điều chỉnh quan trọng phải có 5 trường: môn/nhóm, loại thông tin, deadline/ngày, link nguồn, người cập nhật. Ghi log ít nhất 10 lượt tìm để đo thời gian và độ đúng.

**Nếu Not Yet — cần kiểm chứng gì trước:** Không áp dụng cho quyết định Go hiện tại; nếu pilot không đạt ngưỡng, cần kiểm chứng mức độ tuân thủ cập nhật record và lý do người học không dùng mục lục.

**Nếu No-Go — nên làm gì thay AI:** Không áp dụng cho quyết định Go hiện tại; phương án quay về là ghim tin và thư mục theo môn, không triển khai tự động hóa.

**Ngưỡng dừng** (nếu sau 2 tuần mà dưới 70% record được cập nhật trong 10 phút, hoặc vẫn có hơn 2 lần dùng nhầm link/phiên bản, thì quay về quy trình ghim tin + thư mục theo môn và xem lại owner/mẫu record trước khi cân nhắc bất kỳ tự động hóa nào):

---

## 9. Hạn chế và hướng tiếp theo

- Survey chỉ có 11 người trả lời và là mẫu thuận tiện, nên không đại diện cho toàn bộ người học.
- Survey không có câu trả lời mở/phỏng vấn sâu; nhóm chưa biết đầy đủ nguyên nhân của từng lần tìm không thành công.
- Một số người đã dùng ghim tin hoặc bảng chung; pilot cần phân biệt lỗi do công cụ, do cập nhật muộn hay do không tuân thủ quy ước.
- Hướng tiếp theo: sau pilot, xem log các record bị thiếu/sai để quyết định Rule có đủ không. Chỉ cân nhắc Workflow có AI khi có bằng chứng rằng record chuẩn vẫn không giúp tìm đúng thông tin.

## 10. Tài liệu tham khảo

- Micro survey ẩn danh 11 người, kết quả lưu trong `report/assets/cp4_survey_result.png` và `report/assets/cp4-survey-result2.png` đến `cp4-survey-result6.png`.
- [Google Drive Help — Search for your files](https://support.google.com/drive/answer/2375114)
- [Slack Help — Add and manage tabs in channels and direct messages](https://slack.com/help/articles/32562841868307-Add-and-manage-tabs-in-channels-and-direct-messages)
- [Discord Support — Pin Messages FAQ](https://support.discord.com/hc/en-us/articles/221421867-Pin-Messages-FAQ)

## 10. Tài liệu tham khảo

-
