# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: D2
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Người học mất thời gian tìm lại đúng thông báo và tài liệu trước buổi học, họp hoặc kiểm tra vì nội dung bị phân tán trong nhóm chat và nhiều file đính kèm.
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Nguyễn Như Duy An | Khi khách gửi yêu cầu bảo hành kèm mô tả/ảnh, cần trích seri, phân loại lỗi sơ bộ và gán người xử lý để hẹn khách trong 15 phút. | Điều phối viên dịch vụ | Diễn giải mô tả không chuyên môn thành nhóm lỗi: 4 phút/ca | Chờ ghi câu hỏi thực tế và người hỏi sau pitch |
| 2 | Nguyễn Như Duy An | Khi nhận hồ sơ hoàn ứng gồm ảnh hóa đơn/vé xe, cần đối soát ngày, mã số thuế và số tiền để duyệt trong ngày. | Kế toán thanh toán nội bộ | So khớp hóa đơn với bảng kê: 10 phút/bộ | Chờ ghi câu hỏi thực tế và người hỏi sau pitch |
| 3 | Nguyễn Như Duy An | Khi nhận file COD cuối ngày, cần đối chiếu mã vận đơn và tiền thực nhận để phát hiện đơn lệch cước/chưa thanh toán. | Kế toán đối soát công nợ | Rà nguyên nhân từng dòng lệch: 45 phút/ngày | Chờ ghi câu hỏi thực tế và người hỏi sau pitch |
| 4 | Mai Xuân Khang | Khi kết thúc buổi học, cần tổng hợp ý chính từ bài giảng/slide để ôn lại mà không đọc hoặc nghe lại toàn bộ. | Người học | Chọn và viết lại ý chính: khoảng 15 phút | Chờ ghi câu hỏi thực tế và người hỏi sau pitch |
| 5 | Mai Xuân Khang | Khi ôn thi từ nhiều nguồn, cần xác định kiến thức trọng tâm và nội dung thiếu để ưu tiên ôn hiệu quả. | Người học | Đối chiếu kiến thức giữa nhiều nguồn: khoảng 20 phút | Chờ ghi câu hỏi thực tế và người hỏi sau pitch |
| 6 | Mai Xuân Khang | Khi làm bài tập nhóm nhiều thành viên, cần theo dõi nhiệm vụ, tiến độ và thay đổi để tránh sót việc/trễ hạn. | Thành viên nhóm học tập | Đối chiếu thông báo, thay đổi và hạn mới nhất: khoảng 12 phút | Chờ ghi câu hỏi thực tế và người hỏi sau pitch |
| 7 | Nguyễn Minh Quân | Khi chuẩn bị học/họp/kiểm tra, cần tìm lại đúng thông báo và tài liệu để không bỏ sót yêu cầu. | Người học | Tìm và mở đúng tài liệu: 3–5 phút/lần | Chờ ghi câu hỏi thực tế và người hỏi sau pitch |
| 8 | Nguyễn Minh Quân | Khi nộp Lab AI thực chiến, cần kiểm tra yêu cầu, tên file và cấu trúc để tránh bị trừ điểm. | Người học làm lab | Đọc và đối chiếu rubric: phần lớn trong 10 phút/lab | Chờ ghi câu hỏi thực tế và người hỏi sau pitch |
| 9 | Nguyễn Minh Quân | Khi nhận lịch kiểm tra/deadline từ email và Zalo, cần tổng hợp ở một nơi để không quên hạn hoặc nhầm lịch thi. | Người học theo nhiều học phần | Tìm thông báo có lịch/deadline: phần lớn trong 10–15 phút/lần | Chờ ghi câu hỏi thực tế và người hỏi sau pitch |

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
- Các candidate tổng hợp/ôn tập của Mai Xuân Khang hiện dùng mốc "ước tính minh họa", chưa đủ bằng chứng hành vi thật để ưu tiên.
- Kiểm tra yêu cầu nộp Lab và tổng hợp deadline có scope gần với candidate được chọn, nhưng pain "tìm đúng thông báo/tài liệu" xảy ra ngay trước nhiều loại hoạt động hơn và có thể là nguyên nhân gốc.

**Xử lý bất đồng (nếu có):** Nhóm ưu tiên candidate dễ kiểm chứng với người học thật và ít rủi ro dữ liệu hơn các candidate vận hành. Các candidate COD/bảo hành được giữ ở hướng tiếp theo.

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
