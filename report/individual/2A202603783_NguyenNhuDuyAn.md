# Báo cáo cá nhân — 2A202603783_NguyenNhuDuyAn

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
| Success metric (baseline → target) | Thời gian tạo một phiếu bảo hành giảm từ 12 phút xuống dưới 4 phút; tỷ lệ phân công đúng thợ kỹ thuật tăng cao. |
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
| Success metric (baseline → target) | Thời gian duyệt 1 bộ hồ sơ giảm từ 25 phút xuống dưới 8 phút; giảm bớt hóa đơn sai mã số thuế lọt qua bước duyệt. |
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
| Success metric (baseline → target) | Tổng thời gian đối soát giảm từ 75 phút xuống dưới 20 phút mỗi ngày; tỷ lệ phát hiện đơn lệch tiền tăng.  |
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
| Pitch Problem Card | Pitch Card số 1 về "Đối soát tiền thu hộ COD" cho kế toán bán hàng. | Nhóm ghi nhận đây là bài toán có số liệu tài chính rõ ràng nhưng quy trình thiên nhiều về logic cố định (Rule). |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: "Nếu lớp trưởng hoặc giảng viên ghim các thông báo quan trọng lên đầu nhóm chat và tạo sẵn thư mục Google Drive theo môn, liệu có giải quyết được vấn đề tìm kiếm mà không cần dùng công cụ nào không?" | Bạn phụ trách đề xuất đã làm rõ: Dù có ghim tin nhắn, số lượng thông báo dồn dập trong tuần thi vẫn làm trôi thông tin, và sinh viên vẫn mất thời gian mở từng file xem nội dung bên trong |
| Nhận phản biện | Câu hỏi tôi nhận được: "Bài đối soát COD có thực sự cần AI không hay chỉ cần viết hàm Excel là giải quyết được 90%?" | Tôi đã sửa gì: Thừa nhận bước so khớp mã đơn chỉ cần dùng Rule, và đồng thuận cùng nhóm chuyển hướng sang bài toán tìm kiếm thông tin môn học vì có mức độ mơ hồ cao hơn. |
| Gom cluster / cây OST | Cùng nhóm gom các đề xuất tìm tài liệu, tìm quyết định cũ vào nhóm "Tìm kiếm và truy xuất thông tin phân tán". | Xây dựng nhánh cơ hội (Opportunity) tập trung vào việc giảm thời gian đọc lướt nội dung trước giờ lên lớp. |
| Chọn candidate problem | Tham gia chấm điểm 7 tiêu chí cho 3 bài trong danh sách rút gọn. | Thống nhất chọn bài "Tìm lại thông báo và tài liệu môn học" vì tính gần gũi và dễ dàng khảo sát sinh viên trong lớp. |
| Kiểm chứng / research | Phỏng vấn trực tiếp 2 sinh viên trong lớp về thói quen tìm tài liệu trước giờ kiểm tra; hỗ trợ tìm kiếm tài liệu về các bot thông báo trên Discord/Telegram. | Xác nhận bước nghẽn lớn nhất không phải là tìm link, mà là đọc lướt để biết tài liệu đó có đúng yêu cầu cần nộp hay không. |
| Quy trình nhóm | Đóng góp ý kiến để vẽ quy trình trước và sau khi có giải pháp xử lý thông báo. | Bổ sung thêm bước sinh viên tự đối chiếu lại với file gốc, tránh việc phụ thuộc hoàn toàn vào tóm tắt tự động. |
| Problem Statement | Cùng nhóm hoàn thiện bản v0 và tinh chỉnh lên bản v1. | Bổ sung ranh giới an toàn (boundary): công cụ không được tự ý gửi tin nhắn thay sinh viên. |
| Mức can thiệp AI | Phân tích tính khả thi giữa Rule và Workflow. | Thống nhất chọn mức Workflow: Rule để lọc từ khóa và phân loại môn học, AI để trích xuất các mốc hạn chót từ văn bản dài. |
| Quyết định | Đánh giá 4 rủi ro sản phẩm (Value, Usability, Feasibility, Viability). | Đồng thuận ra quyết định Not Yet vì bài toán gặp rủi ro Feasibility và Viability cao (chưa có API trích xuất tin nhắn chat an toàn và vướng quyền riêng tư của sinh viên). |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Tìm thêm góc nhìn về các vấn đề vận hành lặp lại. | Gợi ý được tình huống rà soát hóa đơn công tác. | Gợi ý ý tưởng "tự động quản lý chuỗi cung ứng bằng AI", đây là giải pháp trá hình và quá rộng. | Loại bỏ hoàn toàn ý tưởng chuỗi cung ứng, giữ lại các việc thực tế đo được bằng phút. |
| CP2 Problem Card | Đưa ra gợi ý về kẽ hở trong card đối soát COD. | Chỉ ra việc so khớp số tiền là bài toán dữ liệu có cấu trúc, không nên lạm dụng AI. | Đề xuất để AI tự gửi khiếu nại sang hãng vận chuyển mà không cần người duyệt. | Bổ sung ranh giới bắt buộc: kế toán phải xác nhận danh sách lệch trước khi gửi khiếu nại. |
| CP4 Research | Tìm kiếm các giải pháp quản lý tài liệu học tập tự động cho sinh viên. | Liệt kê nhanh tính năng tìm kiếm của Notion AI và các bot Discord mã nguồn mở. | Đưa ra một số liên kết tài liệu đã cũ và không truy cập được. | Tự mở kiểm tra từng trang tài liệu, chỉ giữ lại các giải pháp có dẫn chứng thực tế. |
| CP5 Quy trình | Chuyển mô tả các bước thành khối mã sơ đồ trực quan. | Tạo khung sơ đồ nhanh chóng, đúng thứ tự các bước. | Gộp bước "mở đọc tài liệu" và "ghi lại yêu cầu" thành một bước duy nhất, làm mất bước nghẽn chính. | Tách riêng hai bước và gắn lại thời gian đo lường thực tế. |
| CP5–6 Problem Statement | Rà soát lỗi câu từ trong bản Problem Statement. | Phát hiện câu chữ bị dài dòng ở phần tác động (impact). | Đề xuất viết gộp giải pháp kỹ thuật vào phần mô tả vấn đề. | Giữ nguyên nguyên tắc mô tả vấn đề thuần túy, không đưa tên công cụ hay thuật toán vào. |
| CP6 Mức can thiệp / quyết định | So sánh ưu nhược điểm giữa Rule và Workflow. | Cung cấp góc nhìn về chi phí tính toán khi chạy mô hình ngôn ngữ lớn. | Khuyên dùng hệ thống tự hành (Agent) nhiều bước phức tạp. | Bác bỏ phương án Agent, chọn Workflow kết hợp Rule để tiết kiệm chi phí và giữ quyền kiểm soát cho người dùng. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Tôi nhận ra các vấn đề liên quan đến việc tìm kiếm thông tin phân tán xuất hiện rất phổ biến. Ban đầu tôi tập trung vào các bài toán kinh doanh như đối soát công nợ hay hóa đơn hoàn ứng vì nghĩ rằng thiệt hại tài chính mới là thước đo rõ ràng. Khi nghe bạn trình bày về việc mất từ 3 đến 5 phút trước mỗi buổi học chỉ để lục lại file thông báo trong nhóm chat, tôi thấy đây là một nỗi đau lặp lại hàng ngày với tần suất rất cao. Bài toán này có đối tượng chịu ảnh hưởng ngay quanh mình, giúp cả nhóm dễ dàng tiếp cận người thật để phỏng vấn và kiểm chứng thay vì phải phỏng đoán quy trình của các doanh nghiệp bên ngoài.
**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Nhóm tôi từng rơi vào bẫy này ngay khi bắt đầu thảo luận ở Checkpoint 3. Khi bạn phụ trách vừa trình bày xong bài toán tìm kiếm thông báo, cả nhóm lập tức bàn về việc tạo một con bot tự động đọc tin nhắn Telegram hay dùng mô hình ngôn ngữ lớn để trả lời câu hỏi tự động. Chúng tôi nhận ra mình đang nhảy thẳng vào giải pháp khi nhìn vào cây Opportunity Solution Tree: nhánh thảo luận toàn chứa tên phần mềm thay vì nỗi đau của người dùng. Nhóm đã dừng lại, gạch bỏ các từ khóa công nghệ và viết lại nhánh cây tập trung vào khó khăn thực sự: sinh viên bị quá tải bởi số lượng tin nhắn rác và không xác định được file nào là bản cập nhật mới nhất.
**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Tôi đã đổi ý hoàn toàn về việc bảo vệ bài toán đối soát COD của mình. Ban đầu tôi rất tự tin vì bài toán này có số liệu cụ thể. Khi các bạn trong nhóm đặt câu hỏi: "Nếu viết một đoạn code Python so khớp hai cột Excel đã giải quyết được 90% số đơn, thì tại sao phải đưa AI vào để làm phức tạp vấn đề?", tôi nhận thấy bản thân đang cố gượng ép công nghệ vào một quy trình vốn dĩ giải quyết tốt nhất bằng logic cố định (Rule). Tôi rút lui bài toán của mình và chuyển sang ủng hộ bài tìm kiếm thông tin môn học vì nhận thấy nó có sự mơ hồ thực sự trong việc đọc hiểu ngữ cảnh văn bản.
**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Điều làm tôi bất ngờ là khi phỏng vấn nhanh 3 bạn sinh viên trong lớp, cả 3 đều cho biết họ không hề thiếu nơi lưu trữ tài liệu. Giảng viên đã tải bài giảng lên hệ thống trường, nhưng sinh viên vẫn bị lỡ việc vì các thông báo thay đổi phòng học hoặc dời hạn nộp bài thường được gửi đột xuất qua tin nhắn trao đổi nhanh. Thêm vào đó, một bạn chia sẻ rằng bạn không cần công cụ đọc hộ toàn bộ bài giảng, bạn chỉ cần một dòng tóm tắt yêu cầu cần nộp trước khi bước vào cửa lớp. Điều này giúp nhóm tôi nhận ra giá trị cốt lõi nằm ở việc bóc tách hạn chót và việc cần làm, chứ không phải tóm tắt nội dung học thuật dài dòng.
**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Phần khó nhất là việc tách bạch hoàn toàn giải pháp ra khỏi phần phát biểu vấn đề và xác định ranh giới kiểm soát (boundary). Người viết rất dễ có xu hướng đưa chữ "hệ thống tự động" hoặc "công cụ hỗ trợ" vào phần quy trình. Nhóm tôi phải sửa đi sửa lại mục Success Metric để đảm bảo số liệu đo được bằng hành vi thực tế (giảm thời gian tìm kiếm từ 3 đến 5 phút xuống dưới 2 phút), thay vì dùng những từ ngữ chung chung như "giúp sinh viên tiện lợi hơn" hay "tìm kiếm nhanh chóng hơn".
**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Nếu được làm lại từ đầu, tôi sẽ yêu cầu nhóm thực hiện bấm giờ thực tế ngay trong buổi học thay vì sử dụng các con số ước tính. Tôi cũng sẽ phản biện mạnh hơn về rủi ro quyền riêng tư khi thu thập dữ liệu nhóm chat. Việc cho phép một công cụ đọc tin nhắn trong các nhóm trao đổi của sinh viên có thể gặp phải sự e ngại về bảo mật thông tin cá nhân. Nhóm cần đưa yếu tố này vào danh sách giả định cốt lõi ngay từ giai đoạn đầu để có phương án khoanh vùng phạm vi dữ liệu an toàn hơn.
**6.7. Hiểu bài:** 
Bài toán của nhóm xuất phát từ việc sinh viên mất từ 3 đến 5 phút trước mỗi buổi học để tìm lại đúng thông báo và tài liệu bài tập bị trôi trong các nhóm chat, dẫn đến nguy cơ bỏ sót yêu cầu quan trọng.
Quy trình hiện tại bao gồm việc mở nhóm chat, cuộn tìm tin nhắn, tải tài liệu đính kèm, đọc lướt nội dung và ghi lại đầu việc cần chuẩn bị.
Chỉ số thành công đo lường bằng việc giảm thời gian tìm đúng tài liệu từ mức 3 đến 5 phút xuống dưới 2 phút cho mỗi lần chuẩn bị, đồng thời tỷ lệ bỏ sót yêu cầu bài học giảm về 0%.
Ranh giới kiểm soát quy định công cụ chỉ được phép trích xuất thông tin từ các kênh thông báo công khai được chỉ định, không được tự động gửi tin nhắn hay nộp bài thay sinh viên, và sinh viên luôn phải đối chiếu lại với tệp gốc.
Mức can thiệp kỹ thuật được chọn là Workflow kết hợp Rule: áp dụng Rule để lọc từ khóa thông báo theo tên môn, kết hợp bước AI hỗ trợ bóc tách danh sách việc cần làm và hạn chót.
Quyết định cuối cùng là Not Yet, vì nhóm nhận diện rủi ro kỹ thuật và bảo mật quyền riêng tư ở mức cao khi chưa có cơ chế trích xuất tin nhắn hợp lệ từ các nền tảng chat. Nhóm đặt ngưỡng dừng kiểm chứng trong 1 tuần: nếu không thể kết nối API an toàn hoặc không được sinh viên đồng thuận chia sẻ dữ liệu nhóm, nhóm sẽ chuyển sang No-Go và quay về giải pháp No AI bằng cách ghim thông báo và chuẩn hóa cấu trúc thư mục lưu trữ bài giảng.

## 7. Tài liệu tham khảo

-
