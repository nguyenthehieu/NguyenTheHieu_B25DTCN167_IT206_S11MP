**Hạng mục 1\. Phân rã Epic – Feature**

| Mã | Epic / Feature | Giá trị nghiệp vụ |
| ----- | ----- | ----- |
| E-01 | Tìm và đặt xe | Giúp khách tìm được xe phù hợp và đặt xe nhanh chóng. |
| F-01.1 | Tìm xe theo nhu cầu | Giúp khách lọc xe theo địa điểm, thời gian và tình trạng còn trống. FR-01, FR-02 |
| F-01.2 | Đặt giữ chỗ | Giúp khách giữ xe trong thời gian thanh toán. FR-03, FR-04 |
| E-02 | Vận hành cửa hàng cho thuê | Giúp cửa hàng xử lý đơn và tránh cho thuê trùng xe. |
| F-02.1 | Xử lý đơn thuê | Giúp nhân viên xem và xác nhận đơn đặt xe. FR-05, FR-06 |
| F-02.2 | Quản lý lịch xe | Giúp cửa hàng theo dõi lịch thuê và tình trạng xe. FR-07, BR-01 |
| E-03 | Giao nhận xe minh bạch | Giúp hai bên có bằng chứng rõ ràng về tình trạng xe khi giao nhận. |
| F-03.1 | Lập biên bản giao xe | Ghi nhận tình trạng xe khi bàn giao cho khách. FR-08, FR-09 |
| F-03.2 | Xác nhận hoàn trả xe | Ghi nhận tình trạng xe khi khách trả xe. FR-10, FR-11 |

## **Hạng mục 2\. Danh sách User Story**

### **2.1. Danh sách tóm tắt**

| Mã | User Story | Feature cha | Truy vết | Ưu tiên | SP |
| ----- | ----- | ----- | ----- | ----- | ----- |
| US-01 | Là khách thuê, tôi muốn tìm xe theo địa điểm và thời gian để chọn xe phù hợp. | F-01.1 | FR-01, FR-02 | Must | 5 |
| US-02 | Là khách thuê, tôi muốn xem chi tiết xe để quyết định có đặt xe hay không. | F-01.1 | FR-02 | Should | 3 |
| US-03 | Là khách thuê, tôi muốn đặt giữ chỗ xe còn trống để tránh bị người khác đặt mất. | F-01.2 | FR-03, BR-02 | Must | 5 |
| US-04 | Là khách thuê, tôi muốn biết trạng thái đơn để chủ động theo dõi việc thuê xe. | F-01.2 | FR-04 | Should | 2 |
| US-05 | Là nhân viên cửa hàng, tôi muốn xem các đơn mới để xử lý yêu cầu thuê xe. | F-02.1 | FR-05 | Must | 3 |
| US-06 | Là nhân viên cửa hàng, tôi muốn xác nhận hoặc từ chối đơn để phản hồi khách kịp thời. | F-02.1 | FR-06, BR-01 | Must | 3 |
| US-07 | Là chủ cửa hàng, tôi muốn cập nhật tình trạng và lịch xe để tránh cho thuê trùng lịch. | F-02.2 | FR-07, BR-01 | Should | 5 |
| US-08 | Là nhân viên cửa hàng, tôi muốn chụp ảnh tình trạng xe khi giao để làm bằng chứng bàn giao. | F-03.1 | FR-08, FR-09 | Could | 5 |
| US-09 | Là khách thuê, tôi muốn xác nhận tình trạng xe khi trả để hai bên có căn cứ đối chiếu. | F-03.2 | FR-10, FR-11 | Could | 3 |
| US-10 | Là khách thuê, tôi muốn tích điểm sau mỗi chuyến đi để nhận ưu đãi cho lần thuê sau. | F-01.2 | FR-12 | Won't | 5 |

US-10 là hạng mục dự kiến cân nhắc cho phiên bản sau, không phải chức năng đã xác nhận trong SRS. Chỉ giữ story này nếu FR-12 thuộc phạm vi được phép; nếu SRS mục 6 loại trừ tính năng tích điểm, hãy thay bằng một yêu cầu hợp lệ khác hoặc bỏ story khỏi danh sách.

### **2.2. Kiểm tra số lượng và phạm vi**

* Có 3 Epic, mỗi Epic có 2 Feature.  
* Có 10 User Story thuộc 3 nhóm nghiệp vụ.  
* Có 2 story dành cho nhân viên cửa hàng và 1 story dành cho chủ cửa hàng.  
* Must: 4/10 story \= 40%, không vượt quá 50%.  
* Mỗi story có mã truy vết giả định về FR/BR.

## **Hạng mục 3\. Bảng tự đánh giá INVEST**

### **3.1. Đánh giá ba User Story**

| Tiêu chí | US-01: Tìm xe | US-03: Đặt giữ chỗ | US-06: Xử lý đơn |
| ----- | ----- | ----- | ----- |
| I – Independent | Đạt – Có thể phát triển tìm kiếm riêng. | Chưa đạt – Phụ thuộc dữ liệu xe và lịch trống. | Chưa đạt – Phụ thuộc đơn đặt xe. |
| N – Negotiable | Đạt – Có thể điều chỉnh bộ lọc. | Đạt – Thời hạn giữ chỗ có thể thương lượng. | Đạt – Có thể điều chỉnh quy tắc xử lý đơn. |
| V – Valuable | Đạt – Giúp khách tìm xe phù hợp. | Đạt – Giảm nguy cơ mất xe đã chọn. | Đạt – Giúp cửa hàng phản hồi khách. |
| E – Estimable | Đạt – Phạm vi tìm kiếm tương đối rõ. | Đạt – Có thể ước lượng khi rõ quy tắc giữ chỗ. | Đạt – Có thể ước lượng thao tác xác nhận đơn. |
| S – Small | Đạt – Phạm vi giới hạn ở tìm kiếm. | Đạt – Phạm vi một quy trình giữ chỗ. | Đạt – Phạm vi xác nhận hoặc từ chối đơn. |
| T – Testable | Đạt – Kiểm tra được kết quả tìm kiếm. | Đạt – Kiểm tra được trạng thái giữ chỗ. | Đạt – Kiểm tra được trạng thái đơn. |

### **3.2. Viết lại User Story US-03**

Bản trước:

Là khách thuê, tôi muốn đặt xe để thuê xe dễ dàng và sử dụng các dịch vụ liên quan.

Bản sau:

Là khách thuê, tôi muốn giữ chỗ một xe còn trống trong 30 phút để có thời gian hoàn tất thanh toán cọc.

Giải thích: Bản mới giới hạn vào một giá trị cụ thể, xác định được thời hạn giữ chỗ và dễ kiểm thử hơn. Story vẫn cần phối hợp với chức năng tìm xe và quản lý lịch xe để tránh trùng lịch.

## **Hạng mục 4\. Acceptance Criteria**

Ba story có mức ưu tiên cao nhất được chọn là US-01, US-03 và US-05. Mỗi story có ít nhất 3 tiêu chí, bao gồm trường hợp ngoại lệ.

### **US-01 – Tìm xe theo nhu cầu**

Mã story: US-01

User Story: Là khách thuê, tôi muốn tìm xe theo địa điểm và thời gian để chọn xe phù hợp.

Truy vết: FR-01, FR-02

Mức ưu tiên: Must

Story Point: 5

Acceptance Criteria:

* AC-01 (Luồng chính): Given khách đã chọn Vũng Tàu và thời gian thuê hợp lệ, When khách tìm xe, Then hệ thống hiển thị các xe còn trống phù hợp.  
* AC-02 (Ngoại lệ): Given không có xe phù hợp, When khách thực hiện tìm kiếm, Then hệ thống thông báo không tìm thấy xe.  
* AC-03 (Quy tắc nghiệp vụ BR-01): Given xe đã được đặt trong toàn bộ khoảng thời gian yêu cầu, When khách tìm xe trong khoảng đó, Then hệ thống không hiển thị xe là còn trống.

### **US-03 – Đặt giữ chỗ**

Mã story: US-03

User Story: Là khách thuê, tôi muốn giữ chỗ một xe còn trống trong 30 phút để có thời gian hoàn tất thanh toán cọc.

Truy vết: FR-03, BR-02

Mức ưu tiên: Must

Story Point: 5

Acceptance Criteria:

* AC-01 (Luồng chính): Given khách chọn xe còn trống, When khách đặt giữ chỗ thành công, Then hệ thống tạo đơn ở trạng thái chờ thanh toán.  
* AC-02 (Quy tắc nghiệp vụ BR-02): Given đơn đang chờ thanh toán, When chưa hết 30 phút giữ chỗ, Then hệ thống duy trì trạng thái giữ chỗ cho đơn đó.  
* AC-03 (Ngoại lệ): Given đơn chưa thanh toán cọc, When thời hạn giữ chỗ 30 phút kết thúc, Then hệ thống hủy đơn và giải phóng xe nếu không có điều kiện nghiệp vụ khác ngăn việc giải phóng.

### **US-05 – Xem đơn mới**

Mã story: US-05

User Story: Là nhân viên cửa hàng, tôi muốn xem các đơn mới để xử lý yêu cầu thuê xe.

Truy vết: FR-05

Mức ưu tiên: Must

Story Point: 3

Acceptance Criteria:

* AC-01 (Luồng chính): Given nhân viên đã đăng nhập đúng cửa hàng, When nhân viên mở danh sách đơn mới, Then hệ thống hiển thị các đơn thuộc cửa hàng đó đang chờ xử lý.  
* AC-02 (Ngoại lệ): Given cửa hàng chưa có đơn mới, When nhân viên mở danh sách, Then hệ thống hiển thị thông báo chưa có đơn.  
* AC-03 (Phân quyền): Given người dùng không thuộc cửa hàng, When người dùng truy cập danh sách đơn của cửa hàng đó, Then hệ thống từ chối truy cập.

Lưu ý: BR-01 và BR-02 là quy tắc nghiệp vụ giả định, cần thay bằng mã và nội dung chính xác trong SRS chính thức.

## **Hạng mục 5\. Definition of Done**

### **5.1. Bộ DoD chung**

| STT | Điều kiện hoàn thành | Kiểm chứng |
| ----- | ----- | ----- |
| 1 | Mã nguồn của story đã được đưa vào nhánh tích hợp theo quy trình nhóm. | Có/Không |
| 2 | Các kiểm thử đơn vị liên quan đã chạy và đạt yêu cầu của nhóm. | Có/Không |
| 3 | Tất cả Acceptance Criteria của story đã được kiểm thử và đạt. | Có/Không |
| 4 | Không còn lỗi nghiêm trọng hoặc lỗi chặn phát hành chưa được xử lý. | Có/Không |
| 5 | Code đã được thành viên khác review và tài liệu cần thiết đã cập nhật. | Có/Không |

### **5.2. Phân biệt DoD và Acceptance Criteria**

* Acceptance Criteria (AC): Điều kiện cụ thể để xác định một User Story đáp ứng yêu cầu nghiệp vụ.  
* Definition of Done (DoD): Tiêu chuẩn hoàn thành chung áp dụng cho mọi User Story trong nhóm.

Ví dụ: US-03 có AC yêu cầu đơn được hủy sau 30 phút nếu chưa thanh toán cọc. DoD yêu cầu các AC của US-03 đã được kiểm thử và đạt, đồng thời code đã review và không còn lỗi nghiêm trọng chưa xử lý.

## **Hạng mục 6\. Prioritized Product Backlog**

### **6.1. Thứ tự ưu tiên**

| STT | Story | MoSCoW | Lý do ưu tiên |
| :---: | ----- | :---: | ----- |
| 1 | US-01 – Tìm xe | Must | Là bước đầu tiên để khách tìm được xe phù hợp. |
| 2 | US-03 – Giữ chỗ | Must | Giúp khách tránh mất xe khi đang hoàn tất đặt thuê. |
| 3 | US-05 – Xem đơn mới | Must | Giúp cửa hàng tiếp nhận yêu cầu thuê xe. |
| 4 | US-06 – Xử lý đơn | Must | Giúp cửa hàng phản hồi yêu cầu đặt xe. |
| 5 | US-07 – Quản lý lịch xe | Should | Hỗ trợ cửa hàng quản lý lịch thuê và giảm nguy cơ trùng lịch; cần phối hợp với cơ chế giữ chỗ. |
| 6 | US-02 – Xem chi tiết xe | Should | Giúp khách có thêm thông tin trước khi quyết định. |
| 7 | US-04 – Theo dõi trạng thái đơn | Should | Giúp khách chủ động theo dõi yêu cầu thuê. |
| 8 | US-08 – Biên bản giao xe | Could | Bổ sung bằng chứng tình trạng xe khi giao nhận. |
| 9 | US-09 – Xác nhận trả xe | Could | Hỗ trợ đối chiếu tình trạng xe khi hoàn trả. |
| 10 | US-10 – Tích điểm | Won't | Chưa ưu tiên trong phiên bản đầu, tập trung trước vào quy trình thuê xe cốt lõi; chỉ giữ nếu được SRS cho phép. |

### **6.2. Giải trình theo mục tiêu kinh doanh**

Ba mục tiêu được giả định từ mô tả nghiệp vụ: (1) giúp khách tìm và đặt xe; (2) giúp cửa hàng xác nhận đơn, tránh trùng lịch; (3) minh bạch tình trạng xe khi giao nhận.

* US-01 – Must: Phục vụ mục tiêu 1, vì khách cần tìm được xe phù hợp trước khi đặt.  
* US-03 – Must: Phục vụ mục tiêu 1 và 2, vì giữ chỗ phải đồng bộ với tình trạng xe.  
* US-06 – Must: Phục vụ mục tiêu 2, giúp cửa hàng xử lý yêu cầu đặt xe.  
* US-08 – Could: Phục vụ mục tiêu 3, nhưng có thể triển khai sau khi quy trình tìm và đặt xe hoạt động ổn định.  
* US-10 – Won't: Chưa đóng góp trực tiếp vào ba mục tiêu cốt lõi bằng các chức năng đặt xe và vận hành cửa hàng.

## **Hạng mục 7\. Bảng ước lượng Story Point**

### **7.1. Story chuẩn**

Chọn US-05 – Xem đơn mới làm story chuẩn, gán 3 Story Point vì phạm vi tương đối rõ, chủ yếu gồm truy vấn danh sách đơn và kiểm tra quyền truy cập cửa hàng.

### **7.2. Bảng ước lượng theo Fibonacci**

| Story | SP | Căn cứ so sánh |
| :---: | :---: | ----- |
| US-01 | 5 | Phức tạp hơn US-05 do cần lọc theo địa điểm, thời gian và tình trạng xe. |
| US-02 | 3 | Tương đương story chuẩn về mức độ triển khai và kiểm thử. |
| US-03 | 5 | Phức tạp hơn US-05 vì cần giữ chỗ và xử lý thời hạn. |
| US-04 | 2 | Nhỏ hơn US-05 vì chủ yếu hiển thị trạng thái đơn. |
| US-05 | 3 | Story chuẩn, dùng làm mốc so sánh. |
| US-06 | 3 | Tương đương US-05, thêm thao tác cập nhật trạng thái đơn. |
| US-07 | 5 | Phức tạp hơn story chuẩn vì cần cập nhật và kiểm soát lịch xe. |
| US-08 | 5 | Cần ghi nhận thông tin giao xe và xử lý hình ảnh bằng chứng. |
| US-09 | 3 | Nhỏ hơn US-08 vì tập trung xác nhận tình trạng hoàn trả. |
| US-10 | 5 | Cần thêm quy tắc tích điểm và kiểm thử; chưa đưa vào Sprint 1\. |

Các giá trị sử dụng trong bảng thuộc thang Fibonacci cho phép: 1, 2, 3, 5, 8, 13\. Không có story nào vượt 13 điểm nên chưa cần tách nhỏ theo ngưỡng này.

## **Hạng mục 8\. Kế hoạch Sprint 1**

### **8.1. Sprint Goal**

Giúp khách thuê tìm và giữ chỗ xe, đồng thời giúp cửa hàng tiếp nhận và xử lý các yêu cầu thuê xe để quá trình đặt xe ban đầu diễn ra thuận tiện hơn.

### **8.2. Sprint Backlog**

Velocity giả định của nhóm là 20 Story Point/Sprint.

| Thứ tự | Story | SP | Lý do chọn |
| :---: | ----- | :---: | ----- |
| 1 | US-01 – Tìm xe | 5 | Nền tảng của quy trình đặt xe. |
| 2 | US-03 – Giữ chỗ | 5 | Hoàn thiện bước đặt xe ban đầu. |
| 3 | US-05 – Xem đơn mới | 3 | Giúp cửa hàng nhận yêu cầu. |
| 4 | US-06 – Xử lý đơn | 3 | Giúp cửa hàng phản hồi khách. |
| 5 | US-04 – Theo dõi trạng thái đơn | 2 | Giúp khách biết tiến độ xử lý. |
|  | Tổng cộng | 18 | Không vượt velocity 20 SP. |

### **8.3. Phân rã Task cho US-03**

| Task | Nội dung công việc | Giờ dự kiến |
| ----- | ----- | :---: |
| T1 | Phân tích quy tắc giữ chỗ và trạng thái đơn | 2 |
| T2 | Thiết kế giao diện đặt giữ chỗ | 2 |
| T3 | Xây dựng API tạo đơn giữ chỗ | 4 |
| T4 | Kiểm tra tình trạng xe và thời hạn giữ chỗ | 3 |
| T5 | Viết và chạy kiểm thử | 2 |
| T6 | Review code và sửa lỗi | 1 |
|  | ***Tổng*** | ***14 giờ*** |

### **8.4. Bảng Capacity cá nhân**

Giả định Sprint có 10 ngày làm việc; mỗi thành viên dành 6 giờ/ngày cho công việc dự án và dự phòng 10% thời gian.

| Thành viên | Vai trò | Giờ/ngày | Ngày | Tổng giờ | Dự phòng 10% | Capacity thực tế |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Thành viên 1 | PO | 6 | 10 | 60 | 6 | 54 |
| Thành viên 2 | Scrum Master | 6 | 10 | 60 | 6 | 54 |
| Thành viên 3 | Developer | 6 | 10 | 60 | 6 | 54 |
| Thành viên 4 | Developer/Tester | 6 | 10 | 60 | 6 | 54 |
|  | Tổng |  |  | 240 | 24 | 216 giờ |

Capacity dành cho công việc dự án là 216 giờ sau dự phòng. Đây là giả định lập kế hoạch; nhóm cần điều chỉnh theo lịch học, lịch nghỉ và khả năng thực tế của từng thành viên. Story Point không được quy đổi trực tiếp thành số giờ.

# **Phụ lục A. Nhật ký vai trò**

| Quyết định | Vai trò | Căn cứ |
| ----- | ----- | ----- |
| Ưu tiên tìm xe và giữ chỗ trong Sprint đầu. | Product Owner | Đây là bước đầu của hành trình thuê xe. |
| Giới hạn Sprint 1 ở 18 SP. | Scrum Master | Không vượt velocity giả định 20 SP. |
| Kiểm thử trường hợp trùng lịch và hết hạn giữ chỗ. | Development Team | Giảm nguy cơ đặt xe không hợp lệ. |

# **Phụ lục B. Câu hỏi và giả định**

| Câu hỏi cho khách hàng | Câu trả lời/giả định thay thế | Ảnh hưởng nếu giả định sai |
| ----- | ----- | ----- |
| Thời gian giữ chỗ tối đa là bao lâu? | Giả định là 30 phút. | Nếu thời hạn khác, phải sửa quy tắc xử lý đơn và kiểm thử. |
| Cửa hàng có được xác nhận đơn khi xe đã có lịch thuê trùng không? | Giả định hệ thống không cho phép xác nhận nếu lịch bị trùng. | Nếu quy tắc khác, cần điều chỉnh cơ chế kiểm tra lịch xe. |

