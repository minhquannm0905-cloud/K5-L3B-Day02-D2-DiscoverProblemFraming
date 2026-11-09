# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Như Duy An
- MSSV: 2A202603783
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: D2
- Link repo nhóm: https://github.com/minhquannm0905-cloud/K5-L3B-Day02-D2-DiscoverProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi nhận danh sách đối soát tiền thu hộ (COD) từ đơn vị vận chuyển vào cuối ngày, tôi muốn đối chiếu mã vận đơn và tiền thực nhận với đơn hàng trên hệ thống nội bộ, để phát hiện các đơn lệch cước hoặc chưa thanh toán. | Kế toán, chủ cửa hàng | Xử lý 120 đến 150 đơn mỗi ngày, mất 75 phút kiểm tra thủ công file Excel; tháng trước phát hiện trễ 3 đơn giao thành công nhưng bên vận chuyển chưa thanh toán 1,4 triệu đồng. |
| 2 | Tốn thời gian | Khi khách hàng gửi yêu cầu bảo hành kèm mô tả và ảnh chụp qua kênh nhắn tin, tôi muốn trích xuất số seri, phân loại mã lỗi phần cứng và gán người phụ trách, để phản hồi thời gian hẹn xử lý cho khách trong 15 phút. | Điều phối viên dịch vụ, kỹ thuật viên sửa chữa, khách hàng | Mỗi ngày tiếp nhận 25 đến 30 yêu cầu; điều phối viên mất 8 đến 10 phút nhập liệu từng ca vào bảng theo dõi; tuần trước có 4 trường hợp phân công nhầm thợ do mô tả sơ sài, làm trễ hẹn 1 ngày. |
| 3 | Cần tổng hợp thông tin | Khi nhận hồ sơ mời thầu thiết bị kỹ thuật dài 50 trang, tôi muốn bóc tách toàn bộ thông số bắt buộc và điều kiện loại trừ, để lập bảng dự toán chào giá mà không bỏ sót tiêu chuẩn kỹ thuật. | Kỹ sư dự toán, nhân viên báo giá | Một bộ hồ sơ thầu mất 3 đến 4 tiếng rà soát; đợt đấu thầu tháng trước sót yêu cầu tiêu chuẩn chống nước IP68 trong phụ lục, khiến công ty chịu phạt 18 triệu đồng để đổi lô vật tư tương đương. |
| 4 | Pain từ người khác | Khi tài xế giao hàng báo không gọi được người nhận, tôi muốn xác nhận nhanh địa chỉ và thời gian nhận mới từ khách mua hàng, để tài xế kịp giao lại đơn ngay trong ca làm việc. | Nhân viên CSKH, tài xế giao vận, người mua hàng | Tỷ lệ giao thất bại lần đầu chiếm 8% tổng lượng đơn (khoảng 35 đơn mỗi ca); tài xế mất trung bình 12 phút gọi điện xác minh từng đơn; bộ phận trực nhận 15 cuộc khiếu nại mỗi tuần về việc đơn bị hủy oan. |
| 5 | Lặp lại | Khi nhân viên gửi hồ sơ hoàn ứng chi phí công tác gồm 15 đến 20 ảnh chụp hóa đơn giấy và vé xe, tôi muốn đối soát tính hợp lệ của ngày xuất, mã số thuế và số tiền thanh toán, để duyệt phiếu chi trong ngày. | Kế toán thu chi, nhân viên thị trường | Mỗi tuần xử lý 18 bộ hồ sơ; kế toán mất 25 phút rà soát thủ công từng ảnh chụp mờ hoặc kiểm tra trùng số hóa đơn; tháng vừa rồi có 2 hóa đơn sai mã số thuế khiến thủ tục hoàn tiền bị trễ 5 ngày. |

**Nếu có dùng AI để gợi ý thêm:** 

Ý AI đề xuất: Tự động dự đoán tồn kho và đặt hàng nhà cung cấp bằng thuật toán thông minh.

Quyết định xử lý: Loại bỏ vì đây là giải pháp trá hình, không bắt đầu từ một bước nghẽn cụ thể mà nhân viên đang thao tác hàng ngày và dữ liệu chuỗi cung ứng quá phức tạp.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Phân loại yêu cầu bảo hành (#2) | Tần suất tiếp nhận cao, ảnh hưởng trực tiếp đến thời gian chờ của khách | Khách hàng chụp ảnh thiết bị quá mờ hoặc tem bị cào xước thì khả năng xử lí dữ liệu như nào? |
| 2 | Duyệt hóa đơn hoàn ứng công tác (#5) | Lặp lại cố định hàng tuần, tốn nhiều thời gian kiểm tra thủ công, dễ sót lỗi mã số thuế | Hóa đơn viết tay hoặc ảnh chụp nhàu nát có nhận diện được không |
| 3 | Đối soát tiền thu hộ COD (#1) | Quy trình lặp lại mỗi ngày, dữ liệu số rõ ràng, đo lường được ngay. | Các đơn vị vận chuyển có xuất file đúng chuẩn định dạng không |

### Problem Card #1 - Tiếp nhận và phân loại bảo hành thiết bị

| Trường | Nội dung |
|---|---|
| Job Story | Khi khách gửi yêu cầu bảo hành kèm mô tả và ảnh chụp qua tin nhắn, tôi muốn trích xuất số seri, phân loại mã lỗi phần cứng và gán thợ phụ trách, để phản hồi lịch hẹn xử lý cho khách trong 15 phút. |
| Actor | Điều phối viên dịch vụ khách hàng |
| Thời điểm / bối cảnh | Trong giờ hành chính khi khách gửi tin nhắn phản ánh sự cố kỹ thuật. |
| Quy trình hiện tại (3–7 bước) | 1. Đọc tin nhắn và xem ảnh khách gửi (2 phút) - 2. Gõ lại số seri vào hệ thống để tra cứu bảo hành (2 phút) - 3. Đọc mô tả để đoán linh kiện hỏng (4 phút) - 4. Nhập phiếu sửa chữa vào bảng theo dõi (2 phút) - 5. Nhắn tin gán việc cho kỹ thuật viên phù hợp (2 phút).    |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, phán đoán linh kiện hỏng từ mô tả của khách: mất 4 phút mỗi ca vì khách dùng từ ngữ không chuyên môn, điều phối viên phải hỏi lại nhiều lần. |
| Impact (nếu không giải thì sao) | 25 đến 30 ca mỗi ngày, tốn hơn 4 giờ nhập liệu; tuần trước có 4 ca chuyển nhầm thợ làm chậm tiến độ xử lý 1 ngày.  |
| Success metric (baseline → target) | Thời gian tạo một phiếu bảo hành giảm từ 12 phút xuống dưới 4 phút; tỷ lệ phân công đúng thợ kỹ thuật đạt trên 90%. |
| Phương án không dùng AI | Tạo form mẫu cố định có sẵn danh sách chọn lỗi phần cứng để khách tự tích trước khi gửi.    |
| Giả thuyết về AI (nếu có) | AI trích xuất số seri từ ảnh chụp phiếu bảo hành và phân loại mô tả lỗi thô của khách thành danh mục kỹ thuật. |
| Cảm nhận nhanh | Workflow. |

Quy trình nháp hiện tại:

HIỆN TẠI: 12 phút/ca (khoảng 300 phút/ngày)

[1. Đọc tin nhắn, xem ảnh: 2']
[2. Tra số seri hệ thống: 2']
[3. Đọc hiểu mô tả để phân loại lỗi: 4'] BOTTLENECK
[4. Nhập phiếu theo dõi: 2']
[5. Gán thợ phụ trách: 2']

### Problem Card #2 - Đối soát hóa đơn hoàn ứng công tác

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhân viên nộp hồ sơ hoàn ứng gồm 15 đến 20 ảnh chụp hóa đơn giấy và vé xe, tôi muốn đối soát tính hợp lệ của ngày xuất, mã số thuế và số tiền, để duyệt phiếu chi trong ngày. |
| Actor | Kế toán thanh toán nội bộ. |
| Thời điểm / bối cảnh | Chiều thứ Sáu hàng tuần khi các bộ phận gửi đề nghị thanh toán chi phí. |
| Quy trình hiện tại (3–7 bước) | 1. Mở từng ảnh hóa đơn đính kèm (3 phút) - 2. Gõ thủ công mã số thuế lên trang của Tổng cục Thuế để kiểm tra (7 phút) - 3. Đối chiếu số tiền trên hóa đơn với bảng kê nhân viên tự lập (10 phút) - 4. Ký duyệt và lập ủy nhiệm chi (5 phút). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, so khớp từng hóa đơn với bảng kê: mất 10 phút mỗi bộ vì hình chụp hóa đơn mờ hoặc thứ tự sắp xếp lộn xộn. |
| Impact (nếu không giải thì sao) | 18 bộ hồ sơ mỗi tuần, tốn khoảng 7,5 giờ làm việc; tháng trước có 2 hóa đơn sai mã số thuế làm chậm tiến độ thanh toán 5 ngày. |
| Success metric (baseline → target) | Thời gian duyệt 1 bộ hồ sơ giảm từ 25 phút xuống dưới 8 phút; không còn hóa đơn sai mã số thuế lọt qua bước duyệt. |
| Phương án không dùng AI | Bắt buộc nhân viên tự tra cứu mã số thuế và nộp file XML hóa đơn điện tử thay vì gửi ảnh chụp. |
| Giả thuyết về AI (nếu có) | Mô hình OCR kết hợp trích xuất thông tin tự động đọc số tiền, mã số thuế từ ảnh chụp và so sánh với bảng kê. |
| Cảm nhận nhanh | Workflow. |

Quy trình nháp hiện tại:

HIỆN TẠI: 25 phút/bộ hồ sơ

[1. Mở kiểm tra ảnh đính kèm: 3']
[2. Tra mã số thuế thủ công: 7']
[3. So khớp từng hóa đơn với bảng kê: 10'] BOTTLENECK
[4. Lập ủy nhiệm chi: 5']

### Problem Card #3 - Đối soát tiền thu hộ (COD)

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận danh sách đối soát COD từ đơn vị vận chuyển vào cuối ngày, tôi muốn đối chiếu mã vận đơn và tiền thực nhận với đơn hàng trên hệ thống nội bộ, để phát hiện các đơn lệch cước hoặc chưa thanh toán |
| Actor | Kế toán nội bộ đối soát công nợ. |
| Thời điểm / bối cảnh | Cuối giờ chiều mỗi ngày làm việc, sau khi đơn vị giao hàng gửi bảng kê thanh toán. |
| Quy trình hiện tại (3–7 bước) | 1. Tải file Excel từ bên vận chuyển (5 phút) - 2. Xuất dữ liệu đơn hoàn tất từ phần mềm bán hàng (5 phút) - 3. Dùng hàm VLOOKUP ghép 2 bảng (10 phút) - 4. Rà soát từng dòng lệch tiền hoặc sai trạng thái (45 phút) - 5. Lập danh sách đơn lệch gửi bộ phận vận hành kiểm tra (10 phút). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4, rà soát từng dòng lệch tiền: mất 45 phút vì phải mở chi tiết từng đơn tìm nguyên nhân do áp mã giảm giá hay tính sai phí lưu kho.|
| Impact (nếu không giải thì sao) | Trung bình 75 phút mỗi ngày cho 1 kế toán. Xử lí vấn đề chậm trễ, thiếu sót gây thất thoát |
| Success metric (baseline → target) | Tổng thời gian đối soát giảm từ 75 phút xuống dưới 20 phút mỗi ngày; tỷ lệ phát hiện đơn lệch tiền đạt 100%.  |
| Phương án không dùng AI | Viết macro Excel hoặc script Python tự động so khớp cột mã vận đơn và tiền cước; chỉ cảnh báo các dòng lệch. |
| Giả thuyết về AI (nếu có) | AI đọc lý do ghi chú từ đơn vị vận chuyển để tự phân loại nguyên nhân lệch cước vào nhóm cụ thể.    |
| Cảm nhận nhanh | Rule + Workflow |

Quy trình nháp hiện tại:

HIỆN TẠI: 75 phút/ngày

[1. Tải file bên vận chuyển: 5']
[2. Xuất dữ liệu bán hàng: 5'] 
[3. Ghép file VLOOKUP: 10']
[4. Rà soát từng dòng lệch cước: 45'] BOTTLENECK
[5. Lập bảng đơn lệch gửi vận hành: 10']

### Card muốn pitch nhất

- Card số: 1 - Đối soát tiền thu hộ COD
- Vì sao: Bài toán có quy trình lặp lại mỗi ngày, dữ liệu số rõ ràng, đo được thời gian thực tế (75 phút/ngày) và có thiệt hại tài chính cụ thể (tháng trước sót 3 đơn lệch 1,4 triệu đồng). Bài toán này cũng giúp phân định ranh giới rõ ràng giữa việc dùng Rule thuần túy và điểm can thiệp của AI.
- Câu hỏi muốn nhóm phản biện: Nếu viết script tự động so khớp mã vận đơn và tiền cước bằng Rule đã xử lý được 85% số đơn, thì chi phí đưa thêm một bước AI vào để đọc các đoạn ghi chú lệch cước có thực sự mang lại hiệu quả hơn việc để kế toán tự rà soát 15% còn lại không?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| So khớp mã vận đơn và đối chiếu số tiền là bài toán dữ liệu có cấu trúc, dùng AI ở bước này lãng phí tài nguyên và dễ gây sai lệch số liệu tài chính. | Đồng ý. | Giữ bước so khớp bằng Rule hoặc script; chỉ xem xét đưa AI vào bước đọc và phân loại các đoạn ghi chú tự do về nguyên nhân lệch cước từ đối tác giao vận. |
| Đưa ra giả định ngầm là mọi đối tác vận chuyển đều xuất file Excel theo cùng một cấu trúc cột giống nhau. | Đồng ý một phần. | GBổ sung giả định về sự không đồng nhất cấu trúc dữ liệu giữa các bên giao hàng vào danh sách cần kiểm chứng ở CP4. |
| Đề xuất AI tự động gửi email khiếu nại sang đối tác vận chuyển mà không cần con người rà soát. | Không đồng ý. | Giữ nguyên ranh giới kiểm soát: Kế toán bắt buộc phải duyệt danh sách đơn lệch trước khi chuyển tiếp thông tin ra bên ngoài. |
---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | | | | |
| CP2 Problem Card | | | | |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
