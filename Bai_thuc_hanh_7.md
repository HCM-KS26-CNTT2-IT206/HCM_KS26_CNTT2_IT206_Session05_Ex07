# BÀI THỰC HÀNH 7
## XÂY DỰNG KẾ HOẠCH TỔ CHỨC SỰ KIỆN CÔNG NGHỆ AI INNOVATION DAY

**Họ và tên:** ................................................  
**Lớp:** ................................................  
**Môn học:** ................................................  
**Ngày thực hiện:** 18/11/2026

---

## 1. Giới thiệu

Trong bài thực hành này, em sử dụng AI để hỗ trợ xây dựng kế hoạch tổ chức sự kiện **“AI Innovation Day”** dành cho sinh viên trong trường. Sự kiện hướng đến việc giúp sinh viên hiểu và trải nghiệm một số ứng dụng của trí tuệ nhân tạo (AI) trong học tập và công việc.

Để thực hiện bài tập, em kết hợp ba kỹ thuật:

- **Chain-of-Thought:** Yêu cầu AI phân tích vấn đề theo từng bước và trình bày các căn cứ, phép tính, kết luận chính. Trong bài, phần thể hiện là bản tóm tắt lập luận và kết quả kiểm tra, không phải toàn bộ suy nghĩ nội bộ của AI.
- **Prompt Chaining:** Chia công việc thành nhiều prompt, dùng kết quả của bước trước làm đầu vào cho bước sau.
- **Context Management:** Tạo bản tóm tắt thông tin quan trọng để có thể tiếp tục làm việc trong một cuộc hội thoại mới mà không mất các quyết định đã thống nhất.

### 1.1. Thông tin cố định của sự kiện

| Nội dung | Thông tin |
|---|---|
| Tên sự kiện | AI Innovation Day |
| Đối tượng | Sinh viên trong trường |
| Quy mô | 150 sinh viên |
| Thời gian | 1 ngày |
| Ngân sách tối đa | 15.000.000 đồng |
| Nhân sự tổ chức | 10 người |
| Mục tiêu | Giúp sinh viên hiểu và trải nghiệm ứng dụng AI trong học tập và công việc |

**Giả định để lập kế hoạch:** Sự kiện được tổ chức tại phòng hội trường hoặc không gian sinh hoạt của trường và được nhà trường/CLB hỗ trợ địa điểm, bàn ghế cơ bản. Thiết bị trình chiếu và âm thanh ưu tiên sử dụng thiết bị sẵn có. Đây là giả định lập kế hoạch, cần xác nhận trước khi triển khai; nếu phải thuê địa điểm hoặc thiết bị thì cần tính lại ngân sách.

---

## 2. Sơ đồ quy trình Prompt Chaining

```text
PROMPT 1 – PHÂN TÍCH TÍNH KHẢ THI
        |
        v
OUTPUT 1: Mục tiêu, điều kiện, giả định và rủi ro
        |
        v
PROMPT 2 – XÂY DỰNG LỊCH TRÌNH
        |
        v
OUTPUT 2: Chương trình sự kiện trong 1 ngày
        |
        v
PROMPT 3 – LẬP DỰ TOÁN NGÂN SÁCH
        |
        v
OUTPUT 3: Bảng chi phí và tổng ngân sách
        |
        v
PROMPT 4 – PHÂN CÔNG NHÂN SỰ
        |
        v
OUTPUT 4: Nhiệm vụ của 10 nhân sự
        |
        v
PROMPT 5 – LẬP KẾ HOẠCH TRUYỀN THÔNG
        |
        v
OUTPUT 5: Kế hoạch truyền thông trước sự kiện
        |
        v
PROMPT 6 – KIỂM TRA VÀ HIỆU CHỈNH
        |
        v
OUTPUT 6: Báo cáo kiểm tra, vấn đề và phương án chỉnh sửa
        |
        v
CONTEXT MANAGEMENT
Tóm tắt dự án để sử dụng ở cuộc hội thoại tiếp theo
```

Mỗi bước sử dụng thông tin đã thống nhất ở các bước trước. Nếu có thay đổi, cần cập nhật lại các phần liên quan thay vì chỉ sửa riêng một bảng.

---

## 3. Bộ prompt hoàn chỉnh

### 3.1. Prompt 1 – Phân tích tính khả thi

**Kỹ thuật sử dụng:** Chain-of-Thought theo dạng phân tích có cấu trúc, yêu cầu AI nêu căn cứ, phép tính và kết luận.

**Prompt:**

```text
Bạn là trợ lý lập kế hoạch tổ chức sự kiện sinh viên.

Hãy phân tích tính khả thi của sự kiện “AI Innovation Day” dựa trên
các thông tin cố định:
- Quy mô: 150 sinh viên.
- Thời gian: 1 ngày.
- Ngân sách tối đa: 15.000.000 đồng.
- Nhân sự tổ chức: 10 người.
- Mục tiêu: Giúp sinh viên hiểu và trải nghiệm ứng dụng AI
  trong học tập và công việc.

Hãy phân tích theo các bước:
1. Xác định mục tiêu và quy mô sự kiện.
2. Xác định các điều kiện cần có về địa điểm, thiết bị,
   nội dung, nhân sự và hậu cần.
3. Đánh giá ngân sách có phù hợp với quy mô 150 người không.
4. Liệt kê các rủi ro có thể xảy ra và mức độ ảnh hưởng.
5. Đề xuất cách hạn chế rủi ro.
6. Kết luận sự kiện có thể thực hiện hay không và nêu điều kiện.

Yêu cầu:
- Trình bày căn cứ và kết quả phân tích rõ ràng, không cần
  trình bày suy nghĩ nội bộ.
- Không thay đổi 150 sinh viên, 10 nhân sự và mức trần 15 triệu đồng.
- Nếu cần giả định, phải ghi rõ đó là giả định cần xác nhận.
- Chưa tự ý đưa ra khoản chi vượt ngân sách.

Xuất kết quả theo cấu trúc:
FEASIBILITY:
- Goals:
- Required_Conditions:
- Assumptions:
- Risks:
- Risk_Mitigation:
- Conclusion:
```

**Kết quả đầu ra – Output 1:**

#### A. Đánh giá mục tiêu và quy mô

Sự kiện có quy mô 150 sinh viên, tổ chức trong một ngày. Mục tiêu tập trung vào việc giới thiệu kiến thức và tạo cơ hội trải nghiệm AI, vì vậy chương trình nên có cả phần chia sẻ lý thuyết và hoạt động thực hành.

#### B. Điều kiện cần có

- Địa điểm đủ chỗ cho khoảng 150 sinh viên và 10 nhân sự tổ chức.
- Có máy chiếu, màn hình, micro và hệ thống âm thanh.
- Có kết nối Internet ổn định nếu hoạt động trải nghiệm cần truy cập công cụ trực tuyến.
- Có nội dung hướng dẫn dễ hiểu, phù hợp với sinh viên chưa có nhiều kiến thức về AI.
- Có khu vực check-in, hướng dẫn chỗ ngồi và hỗ trợ kỹ thuật.

#### C. Giả định

- Nhà trường hoặc CLB hỗ trợ địa điểm và bàn ghế.
- Có thể sử dụng thiết bị trình chiếu, âm thanh sẵn có.
- Người tham gia tự chuẩn bị điện thoại hoặc laptop nếu hoạt động thực hành cần thiết bị cá nhân.
- Không tổ chức ăn trưa cho toàn bộ người tham gia; ngân sách chỉ bố trí nước uống và vật dụng cần thiết.

#### D. Rủi ro và phương án hạn chế

| Rủi ro | Mức độ | Cách hạn chế |
|---|---|---|
| Internet không ổn định | Cao | Chuẩn bị hình ảnh, video hoặc ví dụ minh họa dự phòng |
| Người tham gia đến muộn | Trung bình | Gửi thông báo thời gian và mở check-in sớm |
| Thiếu thiết bị thực hành | Trung bình | Chuẩn bị hoạt động theo nhóm, trình diễn trên màn hình chung |
| Chi phí phát sinh | Cao | Có khoản dự phòng và phải xin duyệt trước khi chi |
| Diễn giả đến trễ hoặc vắng mặt | Trung bình | Có người điều phối nội dung và phương án thay thế |
| Số lượng đăng ký vượt sức chứa | Trung bình | Chốt danh sách theo quy mô 150 sinh viên |

#### E. Kết luận tính khả thi

Sự kiện có thể tổ chức trong điều kiện ngân sách 15 triệu đồng nếu được hỗ trợ địa điểm và thiết bị cơ bản. Ban tổ chức cần kiểm tra trước cơ sở vật chất, xác nhận người chia sẻ và kiểm soát các khoản chi phát sinh.

---

### 3.2. Prompt 2 – Xây dựng lịch trình sự kiện

**Đầu vào:** Output 1 – Phân tích tính khả thi, điều kiện và rủi ro.

**Prompt:**

```text
Dựa trên kết quả FEASIBILITY dưới đây:
[CHÈN TOÀN BỘ OUTPUT 1]

Hãy xây dựng lịch trình sự kiện AI Innovation Day trong 1 ngày
dành cho 150 sinh viên.

Yêu cầu:
- Có thời gian bắt đầu và kết thúc từng hoạt động.
- Có check-in, khai mạc, giới thiệu AI, chia sẻ ứng dụng,
  trải nghiệm thực tế, giải lao, hỏi đáp và tổng kết.
- Nội dung phù hợp với sinh viên, kể cả người mới tìm hiểu AI.
- Có thời gian chuyển tiếp giữa các hoạt động.
- Không đưa vào hoạt động cần thiết bị hoặc chi phí chưa được xác nhận.
- Lịch trình phải khả thi với 10 nhân sự tổ chức.

Xuất kết quả thành bảng:
Thời gian | Hoạt động | Nội dung | Người/bộ phận phụ trách.
```

**Kết quả đầu ra – Output 2: Lịch trình trong một ngày**

| Thời gian | Hoạt động | Nội dung | Phụ trách |
|---|---|---|---|
| 07:30–08:00 | Chuẩn bị | Kiểm tra hội trường, âm thanh, máy chiếu, bàn check-in | Nhóm hậu cần, kỹ thuật |
| 08:00–08:30 | Check-in | Đón sinh viên, xác nhận đăng ký, hướng dẫn chỗ ngồi | Nhóm check-in |
| 08:30–08:45 | Khai mạc | Giới thiệu chương trình và mục tiêu sự kiện | MC, trưởng BTC |
| 08:45–09:30 | Chuyên đề 1 | AI là gì? Một số ứng dụng phổ biến trong đời sống | Diễn giả, kỹ thuật |
| 09:30–10:15 | Chuyên đề 2 | Ứng dụng AI trong học tập và công việc | Diễn giả, điều phối |
| 10:15–10:30 | Giải lao | Nghỉ giải lao, giao lưu | Hậu cần |
| 10:30–11:30 | Trải nghiệm AI | Hướng dẫn thử một số công cụ AI qua ví dụ đơn giản | Nhóm nội dung, kỹ thuật |
| 11:30–12:00 | Hỏi đáp buổi sáng | Giải đáp thắc mắc của sinh viên | MC, diễn giả |
| 12:00–13:00 | Nghỉ trưa | Nghỉ trưa, BTC kiểm tra lại khu vực | Toàn bộ BTC |
| 13:00–13:15 | Ổn định | Đón sinh viên trở lại hội trường | Check-in, hậu cần |
| 13:15–14:15 | Hoạt động nhóm | Sinh viên thảo luận ý tưởng ứng dụng AI vào một tình huống học tập | Nhóm nội dung |
| 14:15–14:45 | Trình bày kết quả | Một số nhóm chia sẻ ý tưởng | MC, điều phối |
| 14:45–15:00 | Giải lao | Nghỉ giải lao | Hậu cần |
| 15:00–15:40 | Chuyên đề 3 | Lưu ý khi sử dụng AI có trách nhiệm, kiểm tra thông tin và bảo vệ dữ liệu | Diễn giả |
| 15:40–16:10 | Hỏi đáp | Giao lưu và giải đáp câu hỏi | MC, diễn giả |
| 16:10–16:30 | Tổng kết | Tổng kết chương trình, cảm ơn và chụp ảnh lưu niệm | Trưởng BTC, truyền thông |
| 16:30–17:00 | Thu dọn | Kiểm tra thiết bị, vệ sinh và bàn giao địa điểm | Hậu cần, kỹ thuật |

**Nhận xét:** Lịch trình kết hợp giữa nghe chia sẻ, trải nghiệm và hoạt động nhóm. Các khoảng giải lao và chuyển tiếp được bố trí để chương trình không quá dồn dập.

---

### 3.3. Prompt 3 – Lập dự toán ngân sách

**Đầu vào:** Output 1 và Output 2.

**Prompt:**

```text
Dựa trên:
1. Kết quả phân tích tính khả thi: [CHÈN OUTPUT 1]
2. Lịch trình sự kiện: [CHÈN OUTPUT 2]

Hãy lập dự toán ngân sách cho AI Innovation Day.

Thông tin cố định:
- 150 sinh viên.
- 1 ngày.
- 10 nhân sự tổ chức.
- Ngân sách tối đa: 15.000.000 đồng.

Yêu cầu:
- Liệt kê các hạng mục chi cần thiết.
- Ghi số lượng, đơn giá và thành tiền.
- Có khoản dự phòng phát sinh.
- Tổng ngân sách không vượt 15 triệu đồng.
- Ưu tiên tận dụng địa điểm và thiết bị nhà trường hỗ trợ.
- Không tính trùng các hạng mục.
- Nêu rõ đây là dự toán tham khảo, cần lấy báo giá thực tế.

Hãy tự kiểm tra phép tính:
Thành tiền = Số lượng x Đơn giá.
Tổng chi = Tổng các hạng mục.
Ngân sách còn lại = 15.000.000 - Tổng chi.

Nếu vượt ngân sách, hãy đề xuất điều chỉnh trước khi chốt.
```

**Kết quả đầu ra – Output 3: Dự toán ngân sách**

| STT | Hạng mục | Số lượng | Đơn giá (đồng) | Thành tiền (đồng) |
|---:|---|---:|---:|---:|
| 1 | Nước uống cho người tham gia và BTC | 170 | 8.000 | 1.360.000 |
| 2 | In bảng tên, tài liệu và phiếu hoạt động | 160 bộ | 5.000 | 800.000 |
| 3 | Backdrop và trang trí khu vực sân khấu | 1 gói | 1.500.000 | 1.500.000 |
| 4 | Hỗ trợ diễn giả/khách mời | 2 người | 1.000.000 | 2.000.000 |
| 5 | Ăn nhẹ cho BTC và khách mời | 15 suất | 40.000 | 600.000 |
| 6 | Vật dụng hoạt động trải nghiệm | 150 suất | 15.000 | 2.250.000 |
| 7 | Chụp ảnh và tư liệu truyền thông | 1 gói | 800.000 | 800.000 |
| 8 | In poster, standee hoặc vật phẩm truyền thông | 1 gói | 700.000 | 700.000 |
| 9 | Chi phí hậu cần và vệ sinh phát sinh | 1 gói | 500.000 | 500.000 |
|  | **Tổng chi dự kiến trước dự phòng** |  |  | **10.510.000** |
| 10 | Dự phòng phát sinh | 1 khoản | 1.500.000 | 1.500.000 |
|  | **TỔNG NGÂN SÁCH DỰ KIẾN** |  |  | **12.010.000** |

<box border radius="lg" padding={3} gap={2}>
  <text color="secondary" weight="medium" size="sm">Ngân sách tối đa</text>
  <title size="2xl" tabularNums>15.000.000đ</title>
  <divider color="subtle"/>
  <text color="secondary" size="sm">Tổng dự toán đã gồm dự phòng</text>
  <title size="xl" color="success" tabularNums>12.010.000đ</title>
  <row justify="between">
    **Ngân sách còn lại**
    **2.990.000đ**
  </row>
  <badge color="success">Không vượt ngân sách</badge>
</box>

**Kiểm tra phép tính:**

- Tổng 9 hạng mục: 10.510.000 đồng.
- Dự phòng: 1.500.000 đồng.
- Tổng ngân sách dự kiến: 10.510.000 + 1.500.000 = **12.010.000 đồng**.
- Ngân sách còn lại: 15.000.000 - 12.010.000 = **2.990.000 đồng**.

**Lưu ý:** Đây là số liệu giả định để lập kế hoạch học tập, không phải báo giá thực tế. Số lượng 170 nước uống gồm 150 sinh viên và 20 phần dự kiến cho BTC/khách mời; số lượng in 160 bộ dự kiến cho người tham gia và một phần dự phòng. Khoản hỗ trợ diễn giả cần được xác nhận theo quy định của CLB/nhà trường. Nếu địa điểm hoặc thiết bị phải thuê, cần lấy báo giá và điều chỉnh các hạng mục trước khi phê duyệt.

---

### 3.4. Prompt 4 – Phân công nhiệm vụ cho 10 nhân sự

**Đầu vào:** Output 1, Output 2 và Output 3.

**Prompt:**

```text
Dựa trên:
- Phân tích tính khả thi: [CHÈN OUTPUT 1]
- Lịch trình: [CHÈN OUTPUT 2]
- Dự toán ngân sách: [CHÈN OUTPUT 3]

Hãy phân công công việc cho đúng 10 nhân sự tổ chức AI Innovation Day.

Yêu cầu:
- Có 1 trưởng ban tổ chức.
- Phân chia rõ các nhóm nội dung, hậu cần, truyền thông,
  check-in và kỹ thuật.
- Mỗi người có nhiệm vụ chính và thời điểm phụ trách.
- Không tạo thêm nhân sự ngoài 10 người.
- Bố trí người phối hợp để tránh một người phải làm nhiều việc
  cùng lúc ở các khu vực khác nhau.

Xuất bảng:
Mã nhân sự | Vai trò | Nhiệm vụ | Thời gian phụ trách.
```

**Kết quả đầu ra – Output 4: Bảng phân công nhân sự**

| Nhân sự | Vai trò | Nhiệm vụ chính |
|---|---|---|
| NS01 | Trưởng BTC | Điều phối chung, làm việc với nhà trường, duyệt nội dung và chi phí |
| NS02 | Phó BTC – Nội dung | Xây dựng kịch bản, liên hệ diễn giả, chuẩn bị tài liệu |
| NS03 | MC – Điều phối sân khấu | Dẫn chương trình, giới thiệu diễn giả, điều phối hỏi đáp |
| NS04 | Phụ trách hậu cần | Chuẩn bị hội trường, bàn ghế, nước uống và vật dụng |
| NS05 | Hậu cần – Check-in | Chuẩn bị danh sách, bảng tên, hỗ trợ đón khách |
| NS06 | Phụ trách truyền thông | Lên nội dung, quản lý bài đăng và thông báo |
| NS07 | Thiết kế – Media | Thiết kế poster, chụp ảnh và lưu tư liệu |
| NS08 | Phụ trách kỹ thuật | Kiểm tra máy chiếu, âm thanh, micro và Internet |
| NS09 | Hỗ trợ trải nghiệm | Hướng dẫn hoạt động AI, hỗ trợ sinh viên trong phần thực hành |
| NS10 | Hỗ trợ điều phối | Theo dõi thời gian, hỗ trợ diễn giả, xử lý tình huống phát sinh |

**Phân chia nhóm:**

- Điều hành và nội dung: NS01, NS02, NS03.
- Hậu cần và check-in: NS04, NS05.
- Truyền thông: NS06, NS07.
- Kỹ thuật và trải nghiệm: NS08, NS09.
- Điều phối hỗ trợ: NS10.

**Nguyên tắc phối hợp:** NS01 là đầu mối xử lý quyết định chung. Các nhóm báo cáo tiến độ cho trưởng BTC. Trong thời gian check-in, NS05 phụ trách danh sách, NS04 hỗ trợ khu vực đón khách; NS08 kiểm tra kỹ thuật trước giờ khai mạc. Khi chương trình diễn ra, NS03 điều phối sân khấu, NS02 hỗ trợ nội dung và NS10 theo dõi thời gian.

---

### 3.5. Prompt 5 – Xây dựng kế hoạch truyền thông trước sự kiện

**Đầu vào:** Output 1 đến Output 4.

**Prompt:**

```text
Dựa trên các kết quả đã thống nhất:
- Tính khả thi: [CHÈN OUTPUT 1]
- Lịch trình: [CHÈN OUTPUT 2]
- Ngân sách: [CHÈN OUTPUT 3]
- Nhân sự: [CHÈN OUTPUT 4]

Hãy xây dựng kế hoạch truyền thông trước sự kiện AI Innovation Day.

Thông tin cố định:
- Đối tượng: Sinh viên trong trường.
- Quy mô tối đa: 150 sinh viên.
- Sự kiện diễn ra trong 1 ngày.
- Mục tiêu: Giúp sinh viên hiểu và trải nghiệm ứng dụng AI
  trong học tập và công việc.

Yêu cầu:
- Chia hoạt động theo mốc thời gian trước sự kiện.
- Có nội dung, kênh truyền thông và người phụ trách.
- Sử dụng các kênh phù hợp như Facebook, nhóm lớp,
  fanpage CLB và thông báo trong trường.
- Có bước mở đăng ký, nhắc lịch và xác nhận người tham gia.
- Không quảng bá số lượng vượt quá sức chứa 150 sinh viên.
- Ưu tiên tận dụng kênh truyền thông miễn phí để tiết kiệm ngân sách.
```

**Kết quả đầu ra – Output 5: Kế hoạch truyền thông**

| Thời gian | Hoạt động | Nội dung truyền thông | Kênh | Phụ trách |
|---|---|---|---|---|
| Trước 14 ngày | Công bố sự kiện | Giới thiệu tên, mục tiêu, đối tượng và nội dung chính | Fanpage CLB, Facebook | NS06, NS07 |
| Trước 12 ngày | Mở đăng ký | Đăng biểu mẫu đăng ký, thông tin thời gian và địa điểm sau khi được xác nhận | Facebook, nhóm lớp | NS06 |
| Trước 10 ngày | Bài viết giới thiệu | Chia sẻ các ứng dụng AI gần gũi trong học tập và công việc | Fanpage CLB | NS06, NS07 |
| Trước 7 ngày | Giới thiệu hoạt động | Đăng lịch trình tóm tắt và hoạt động trải nghiệm | Facebook, nhóm lớp | NS06, NS02 |
| Trước 5 ngày | Nhắc đăng ký | Nhắc sinh viên đăng ký, theo dõi số lượng đã ghi danh | Facebook, nhóm lớp | NS06 |
| Trước 3 ngày | Xác nhận tham gia | Gửi thông tin cho người đã đăng ký, kiểm tra danh sách | Email/nhóm liên hệ phù hợp | NS05, NS06 |
| Trước 1 ngày | Nhắc lịch | Nhắc giờ check-in, địa điểm, lưu ý chuẩn bị thiết bị cá nhân nếu cần | Facebook, nhóm lớp | NS06 |
| Trong ngày | Cập nhật sự kiện | Chụp ảnh, đăng một số hình ảnh hoạt động phù hợp | Fanpage CLB | NS07 |
| Sau sự kiện 1 ngày | Tổng kết | Đăng bài cảm ơn và hình ảnh chương trình | Fanpage CLB | NS06, NS07 |

**Nội dung thông điệp truyền thông gợi ý:**

> **AI INNOVATION DAY – CÙNG KHÁM PHÁ AI TRONG HỌC TẬP VÀ CÔNG VIỆC**
>
> Bạn đã từng sử dụng AI để tìm kiếm ý tưởng, hỗ trợ học tập hoặc xử lý công việc chưa? Hãy tham gia AI Innovation Day để tìm hiểu thêm về những ứng dụng của trí tuệ nhân tạo và trực tiếp trải nghiệm một số hoạt động thú vị.
>
> Chương trình dành cho sinh viên trong trường, với các nội dung chia sẻ, trải nghiệm và trao đổi về cách sử dụng AI phù hợp.
>
> Số lượng tiếp nhận dự kiến: 150 sinh viên. Đăng ký theo hướng dẫn của Ban tổ chức!

**Lưu ý:** Chỉ công bố thời gian, địa điểm, diễn giả và đường dẫn đăng ký sau khi đã được xác nhận chính thức.

---

### 3.6. Prompt 6 – Kiểm tra tính thống nhất và hiệu chỉnh

**Đầu vào:** Toàn bộ Output 1 đến Output 5.

**Prompt:**

```text
Bạn là trợ lý kiểm tra kế hoạch tổ chức sự kiện.

Hãy kiểm tra toàn bộ kế hoạch AI Innovation Day dựa trên:
1. Phân tích tính khả thi: [CHÈN OUTPUT 1]
2. Lịch trình: [CHÈN OUTPUT 2]
3. Dự toán ngân sách: [CHÈN OUTPUT 3]
4. Phân công nhân sự: [CHÈN OUTPUT 4]
5. Kế hoạch truyền thông: [CHÈN OUTPUT 5]

Kiểm tra các nội dung:
- Quy mô có đúng 150 sinh viên không?
- Số nhân sự có đúng 10 người không?
- Thời gian có đúng 1 ngày không?
- Tổng dự toán có thấp hơn hoặc bằng 15.000.000 đồng không?
- Các hoạt động có đủ người phụ trách không?
- Lịch trình có phù hợp với điều kiện thiết bị và địa điểm không?
- Truyền thông có quảng bá đúng nội dung và sức chứa không?
- Có rủi ro hoặc khoản chi nào bị bỏ sót không?

Hãy trình bày:
1. Bảng tiêu chí kiểm tra.
2. Các vấn đề phát hiện.
3. Phương án hiệu chỉnh cụ thể.
4. Kết luận kế hoạch sau hiệu chỉnh.

Không tự ý thay đổi các thông tin cố định.
Nếu đề xuất thay đổi một hạng mục, hãy kiểm tra ảnh hưởng
đến ngân sách, lịch trình và nhân sự.
```

---

## 4. Báo cáo kiểm tra và hiệu chỉnh kế hoạch

### 4.1. Bảng kiểm tra tính thống nhất

| Tiêu chí | Kết quả kiểm tra | Đánh giá |
|---|---|---|
| Quy mô người tham gia | 150 sinh viên | Đạt |
| Thời lượng | Một ngày, từ 08:00 đến 17:00 (chưa tính thời gian BTC chuẩn bị) | Đạt |
| Nhân sự | Đúng 10 người, mã NS01–NS10 | Đạt |
| Ngân sách | 12.010.000 đồng, đã gồm dự phòng | Đạt |
| Mục tiêu nội dung | Có chia sẻ, trải nghiệm, hỏi đáp và hoạt động nhóm về AI | Đạt |
| Lịch trình | Có thời gian chuẩn bị, check-in, giải lao và thu dọn | Đạt |
| Truyền thông | Có mở đăng ký, nhắc lịch và tổng kết | Đạt |
| Phân công | Các hoạt động chính có người phụ trách | Đạt có điều kiện |

### 4.2. Các vấn đề cần lưu ý

| Vấn đề | Nguyên nhân | Cách hiệu chỉnh |
|---|---|---|
| Chưa xác nhận địa điểm | Đề bài chưa cung cấp địa điểm cụ thể | Liên hệ nhà trường và xác nhận sức chứa trước khi công bố |
| Thiết bị có thể không đáp ứng | Phần trải nghiệm cần Internet và máy chiếu | Kiểm tra trước, chuẩn bị video hoặc hình ảnh dự phòng |
| Dự toán mới là số tham khảo | Chưa có báo giá thực tế | Xin báo giá và cập nhật trước khi trình duyệt |
| Sinh viên có thể không mang laptop | Không phải ai cũng có thiết bị cá nhân | Tổ chức theo nhóm hoặc trình diễn trên màn hình chung |
| Đăng ký có thể vượt sức chứa | Bài đăng được chia sẻ rộng | Theo dõi biểu mẫu và chốt tối đa 150 sinh viên |
| Diễn giả có thể thay đổi lịch | Chưa có xác nhận chính thức | Xác nhận trước và chuẩn bị nội dung thay thế |

### 4.3. Hiệu chỉnh sau kiểm tra

Sau khi rà soát, em giữ nguyên các thông tin bắt buộc: 150 sinh viên, 10 nhân sự, thời gian một ngày và ngân sách tối đa 15 triệu đồng.

Một số điều chỉnh về cách triển khai được đề xuất:

1. **Địa điểm:** Chỉ chốt kế hoạch khi có xác nhận địa điểm miễn phí hoặc được hỗ trợ. Nếu phát sinh tiền thuê, phải tính lại ngân sách.
2. **Hoạt động trải nghiệm:** Không yêu cầu tất cả sinh viên phải có laptop. Có thể chia nhóm và sử dụng một số thiết bị trình diễn chung.
3. **Ngân sách:** Giữ dự toán 12.010.000 đồng, trong đó 1.500.000 đồng là khoản dự phòng. Mọi khoản chi từ dự phòng cần được trưởng BTC đồng ý.
4. **Nhân sự:** NS10 hỗ trợ điều phối và theo dõi thời gian; NS01 xử lý các quyết định phát sinh. Không bổ sung người ngoài danh sách 10 nhân sự vào kế hoạch nhân sự chính.
5. **Truyền thông:** Chỉ nhận tối đa 150 sinh viên và xác nhận danh sách trước ngày tổ chức.

### 4.4. Kết luận sau kiểm tra

Kế hoạch hiện tại đáp ứng các ràng buộc cơ bản của đề bài. Tổng ngân sách dự kiến là **12.010.000 đồng**, thấp hơn mức tối đa 15.000.000 đồng. Chương trình có lịch trình trong một ngày, phân công đủ 10 nhân sự và có kế hoạch truyền thông trước sự kiện.

Tuy nhiên, tính khả thi khi triển khai thực tế còn phụ thuộc vào việc xác nhận địa điểm, thiết bị, diễn giả và báo giá. Ban tổ chức cần hoàn tất các nội dung này trước khi trình duyệt và công bố chính thức.

---

## 5. Bản tóm tắt ngữ cảnh dự án (Context Management)

Bản tóm tắt này được tạo để lưu lại những thông tin quan trọng. Khi chuyển sang một cuộc hội thoại mới, có thể sao chép toàn bộ nội dung bên dưới để AI tiếp tục hỗ trợ mà không phải xây dựng lại từ đầu.

### PROJECT_CONTEXT – AI INNOVATION DAY

```text
TÊN DỰ ÁN:
AI Innovation Day – Sự kiện công nghệ dành cho sinh viên.

1. THÔNG TIN CỐ ĐỊNH
- Đối tượng: Sinh viên trong trường.
- Quy mô: 150 sinh viên.
- Thời gian: 1 ngày.
- Ngân sách tối đa: 15.000.000 đồng.
- Nhân sự tổ chức: 10 người.
- Mục tiêu: Giúp sinh viên hiểu và trải nghiệm ứng dụng AI
  trong học tập và công việc.

2. GIẢ ĐỊNH ĐANG SỬ DỤNG
- Địa điểm và bàn ghế do trường/CLB hỗ trợ.
- Thiết bị trình chiếu và âm thanh ưu tiên dùng thiết bị sẵn có.
- Sinh viên có thể dùng thiết bị cá nhân hoặc tham gia theo nhóm.
- Các giả định này phải được xác nhận trước khi triển khai.

3. LỊCH TRÌNH CHÍNH
- 08:00–08:30: Check-in.
- 08:30–08:45: Khai mạc.
- 08:45–10:15: Chia sẻ về AI và ứng dụng.
- 10:30–11:30: Trải nghiệm AI.
- 11:30–12:00: Hỏi đáp.
- 13:00–14:45: Hoạt động nhóm và trình bày.
- 15:00–16:10: Chuyên đề sử dụng AI có trách nhiệm và hỏi đáp.
- 16:10–16:30: Tổng kết.
- 16:30–17:00: Thu dọn.

4. NGÂN SÁCH
- Tổng chi dự kiến trước dự phòng: 10.510.000 đồng.
- Dự phòng: 1.500.000 đồng.
- Tổng dự toán: 12.010.000 đồng.
- Ngân sách còn lại so với mức trần: 2.990.000 đồng.
- Đây là dự toán giả định, cần báo giá thực tế.
- Không được vượt 15.000.000 đồng.

5. NHÂN SỰ
- NS01: Trưởng BTC.
- NS02: Phó BTC – Nội dung.
- NS03: MC – Điều phối sân khấu.
- NS04: Hậu cần.
- NS05: Hậu cần – Check-in.
- NS06: Truyền thông.
- NS07: Thiết kế – Media.
- NS08: Kỹ thuật.
- NS09: Hỗ trợ trải nghiệm.
- NS10: Hỗ trợ điều phối.

6. TRUYỀN THÔNG
- Trước 14 ngày: Công bố sự kiện.
- Trước 12 ngày: Mở đăng ký.
- Trước 10 ngày: Bài viết giới thiệu AI.
- Trước 7 ngày: Giới thiệu hoạt động.
- Trước 5 ngày: Nhắc đăng ký.
- Trước 3 ngày: Xác nhận người tham gia.
- Trước 1 ngày: Nhắc lịch.
- Trong và sau sự kiện: Cập nhật hình ảnh, bài tổng kết.
- Kênh: Fanpage CLB, Facebook, nhóm lớp và kênh thông báo trong trường.

7. RỦI RO CẦN THEO DÕI
- Internet không ổn định.
- Thiếu thiết bị thực hành.
- Diễn giả thay đổi lịch.
- Chi phí phát sinh.
- Số lượng đăng ký vượt 150 người.
- Địa điểm chưa được xác nhận.

8. NGUYÊN TẮC KHÔNG ĐƯỢC THAY ĐỔI
- Không đổi quy mô 150 sinh viên.
- Không đổi số nhân sự 10 người.
- Không đổi thời lượng một ngày.
- Không vượt ngân sách 15.000.000 đồng.
- Nếu sửa lịch trình, phải kiểm tra lại nhân sự và thiết bị.
- Nếu sửa ngân sách, phải tính lại tổng chi và khoản dự phòng.
- Không tự tạo thông tin chưa được xác nhận.

9. PHONG CÁCH LÀM VIỆC
- Trình bày đơn giản, rõ ràng, phù hợp với sinh viên năm nhất.
- Giải thích các quyết định bằng căn cứ và kết quả kiểm tra.
- Không trình bày suy nghĩ nội bộ; chỉ đưa ra lập luận tóm tắt,
  phép tính, giả định và kết luận cần thiết.
```

### Prompt sử dụng khi chuyển sang hội thoại mới

```text
Bạn hãy tiếp tục hỗ trợ dự án AI Innovation Day dựa trên
bản PROJECT_CONTEXT dưới đây.

[ DÁN TOÀN BỘ PROJECT_CONTEXT ]

Trước khi thực hiện yêu cầu mới:
1. Đọc và xác nhận các thông tin cố định.
2. Không tự ý thay đổi quy mô, nhân sự, thời gian và ngân sách.
3. Nếu đề xuất chỉnh sửa, hãy kiểm tra ảnh hưởng đến các phần liên quan.
4. Giữ phong cách trình bày đơn giản, rõ ràng, phù hợp sinh viên năm nhất.
5. Tiếp tục từ kế hoạch hiện tại, không làm lại toàn bộ nếu không cần thiết.

Yêu cầu tiếp theo của tôi:
[ GHI CÔNG VIỆC MUỐN AI TIẾP TỤC ]
```

---

## 6. Tổng kết

Qua bài thực hành, em đã sử dụng kết hợp ba kỹ thuật AI để xây dựng kế hoạch tổ chức sự kiện AI Innovation Day.

- **Chain-of-Thought:** Được vận dụng dưới dạng phân tích có cấu trúc, kiểm tra căn cứ, phép tính ngân sách và rủi ro theo từng bước.
- **Prompt Chaining:** Chia công việc thành nhiều prompt, trong đó kết quả của bước trước được sử dụng cho bước sau.
- **Context Management:** Tạo bản tóm tắt dự án để lưu thông tin và tiếp tục làm việc trong cuộc hội thoại mới.

Qua bài tập, em hiểu rằng sử dụng AI để lập kế hoạch không chỉ là yêu cầu AI tạo ra nội dung mà còn cần kiểm tra tính hợp lý giữa lịch trình, ngân sách, nhân sự và truyền thông. Người sử dụng cần xem lại các giả định, xác nhận thông tin thực tế và điều chỉnh trước khi áp dụng.

---

**HẾT**
