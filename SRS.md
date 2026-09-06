## 3. Stakeholder Identification

### 3.1. Danh sách Stakeholder

| STT | Stakeholder                         | Vai trò                                                                                                                                                                  |
| --- | ----------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1   | Khách hàng                          | Người sử dụng hệ thống để đăng ký, đặt xe, theo dõi chuyến đi, thanh toán, xem lịch sử và đánh giá tài xế.                                                               |
| 2   | Tài xế                              | Người nhận và thực hiện chuyến xe; cập nhật trạng thái chuyến đi, thông tin phương tiện và trạng thái hoạt động.                                                         |
| 3   | Nhân viên vận hành                  | Quản lý khách hàng, tài xế, phương tiện và chuyến đi; theo dõi chuyến đang diễn ra và hỗ trợ xử lý các trường hợp phát sinh.                                             |
| 4   | Ban lãnh đạo / Quản lý doanh nghiệp | Định hướng hoạt động của hệ thống, theo dõi báo cáo về số lượng chuyến, doanh thu, tỷ lệ hoàn thành, tỷ lệ hủy và hiệu quả tài xế.                                       |
| 5   | Nhà cung cấp thanh toán bên ngoài   | Cung cấp dịch vụ xử lý thanh toán điện tử cho hệ thống CAB.                                                                                                              |
| 6   | Nhà cung cấp dịch vụ thông báo      | Cung cấp các kênh gửi thông báo cho khách hàng và tài xế; có thể được mở rộng hoặc thay thế trong tương lai.                                                             |
| 7   | Business Analyst (BA)               | Làm rõ các yêu cầu chưa được chốt với các bên liên quan và xác định phạm vi, tác nhân, quy trình nghiệp vụ, yêu cầu chức năng, phi chức năng và các trường hợp ngoại lệ. |
| 8   | Nhóm phát triển hệ thống            | Phân tích, thiết kế, xây dựng và triển khai nền tảng CAB dựa trên các yêu cầu đã được xác định.                                                                          |

### 3.2. Vai trò và mức độ quan tâm của Stakeholder

| Stakeholder                         | Quyền lực (Power) | Mức độ quan tâm (Interest) | Mức độ ưu tiên | Chiến lược quản lý                                                   |
| ----------------------------------- | ----------------- | -------------------------- | -------------- | -------------------------------------------------------------------- |
| Ban lãnh đạo / Quản lý doanh nghiệp | Cao               | Cao                        | Rất cao        | Quản lý chặt chẽ, thường xuyên cập nhật và lấy ý kiến                |
| Nhân viên vận hành                  | Cao               | Cao                        | Rất cao        | Tham gia thường xuyên, lấy phản hồi trong quá trình phân tích        |
| Khách hàng                          | Thấp              | Cao                        | Cao            | Theo dõi nhu cầu và đảm bảo hệ thống đáp ứng trải nghiệm sử dụng     |
| Tài xế                              | Thấp              | Cao                        | Cao            | Thường xuyên thu thập phản hồi về quy trình nhận và thực hiện chuyến |
| Nhà cung cấp thanh toán bên ngoài   | Trung bình        | Trung bình                 | Trung bình     | Phối hợp và theo dõi việc tích hợp                                   |
| Nhà cung cấp dịch vụ thông báo      | Trung bình        | Trung bình                 | Trung bình     | Phối hợp về giao tiếp và khả năng mở rộng kênh thông báo             |
| Business Analyst (BA)               | Cao               | Cao                        | Rất cao        | Phối hợp chặt chẽ với các stakeholder để làm rõ yêu cầu              |
| Nhóm phát triển hệ thống            | Cao               | Cao                        | Rất cao        | Phối hợp chặt chẽ trong quá trình thiết kế và triển khai             |

---

## 3.3. Stakeholder Matrix

Stakeholder Matrix được phân loại dựa trên hai tiêu chí: **Power (Quyền lực)** và **Interest (Mức độ quan tâm)**.

|                | **Interest thấp**                                                 | **Interest cao**                                                                                    |
| -------------- | ----------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| **Power cao**  | Nhà cung cấp thanh toán bên ngoài, Nhà cung cấp dịch vụ thông báo | Ban lãnh đạo / Quản lý doanh nghiệp, Nhân viên vận hành, Business Analyst, Nhóm phát triển hệ thống |
| **Power thấp** | —                                                                 | Khách hàng, Tài xế                                                                                  |

### Chiến lược theo Stakeholder Matrix

* **Power cao – Interest cao:** Quản lý chặt chẽ. Đây là nhóm cần được tham gia thường xuyên vì có khả năng quyết định hoặc ảnh hưởng lớn đến hệ thống.
* **Power cao – Interest thấp:** Duy trì sự hài lòng và phối hợp khi cần thiết, đặc biệt đối với các bên cung cấp dịch vụ bên ngoài.
* **Power thấp – Interest cao:** Theo dõi và thu thập phản hồi thường xuyên vì đây là những người trực tiếp sử dụng hoặc chịu ảnh hưởng bởi hệ thống.
* **Power thấp – Interest thấp:** Không có stakeholder chính thuộc nhóm này trong phạm vi yêu cầu hiện tại.

---

## 3.4. Mermaid – Stakeholder Matrix

```mermaid
quadrantChart
    title Stakeholder Matrix - CAB System
    x-axis "Interest thấp" --> "Interest cao"
    y-axis "Power thấp" --> "Power cao"
    
    quadrant-1 "Quản lý chặt chẽ"
    quadrant-2 "Duy trì sự hài lòng"
    quadrant-3 "Theo dõi"
    quadrant-4 "Theo dõi và thu thập phản hồi"

    "Ban lãnh đạo": [0.85, 0.90]
    "Nhân viên vận hành": [0.90, 0.85]
    "Business Analyst": [0.88, 0.88]
    "Nhóm phát triển": [0.90, 0.82]
    "Nhà cung cấp thanh toán": [0.45, 0.65]
    "Nhà cung cấp thông báo": [0.40, 0.60]
    "Khách hàng": [0.85, 0.30]
    "Tài xế": [0.80, 0.35]
```

## 3.5. Mermaid – Sơ đồ Stakeholder và CAB System

```mermaid
flowchart LR
    CAB["CAB System<br/>Nền tảng đặt xe"]

    KH["Khách hàng"]
    TX["Tài xế"]
    NV["Nhân viên vận hành"]
    LD["Ban lãnh đạo /<br/>Quản lý doanh nghiệp"]
    PAY["Nhà cung cấp<br/>thanh toán bên ngoài"]
    NOTI["Nhà cung cấp<br/>dịch vụ thông báo"]
    BA["Business Analyst"]
    DEV["Nhóm phát triển"]

    KH -->|"Đăng ký, đặt xe,<br/>theo dõi, thanh toán,<br/>đánh giá"| CAB
    CAB -->|"Thông báo trạng thái<br/>chuyến đi và thanh toán"| KH

    TX -->|"Nhận/từ chối chuyến,<br/>cập nhật trạng thái,<br/>vị trí"| CAB
    CAB -->|"Thông báo chuyến mới<br/>và thay đổi chuyến"| TX

    NV -->|"Quản lý và hỗ trợ<br/>khách hàng, tài xế,<br/>phương tiện, chuyến đi"| CAB
    CAB -->|"Trạng thái và<br/>thông tin vận hành"| NV

    LD -->|"Định hướng,<br/>yêu cầu báo cáo"| CAB
    CAB -->|"Báo cáo hoạt động,<br/>doanh thu, chuyến đi"| LD

    CAB -->|"Yêu cầu thanh toán"| PAY
    PAY -->|"Kết quả giao dịch"| CAB

    CAB -->|"Gửi yêu cầu thông báo"| NOTI
    NOTI -->|"Kết quả gửi thông báo"| CAB

    BA -->|"Phân tích và làm rõ<br/>yêu cầu"| CAB
    DEV -->|"Thiết kế, xây dựng<br/>và triển khai"| CAB
```
## 4. Business Goals

### BG-01 – Nâng cao chất lượng dịch vụ đặt xe

**Business Goal:**
Xây dựng một nền tảng CAB giúp khách hàng thực hiện toàn bộ quy trình đặt xe thuận tiện, từ tạo yêu cầu, tìm tài xế, theo dõi chuyến đi, thanh toán đến đánh giá sau chuyến.

**Mục tiêu:**

* Giảm những hạn chế của hệ thống đặt xe hiện tại.
* Cải thiện trải nghiệm của khách hàng trong quá trình đặt và sử dụng dịch vụ.
* Cung cấp thông tin rõ ràng về trạng thái chuyến đi cho khách hàng.

---

### BG-02 – Nâng cao hiệu quả phân công tài xế

**Business Goal:**
Tự động hóa và cải thiện quá trình tìm kiếm, lựa chọn và phân công tài xế phù hợp cho mỗi yêu cầu đặt xe.

**Mục tiêu:**

* Ưu tiên tài xế phù hợp và ở gần khách hàng.
* Giảm sự phụ thuộc vào việc phân công thủ công.
* Có khả năng tiếp tục tìm tài xế khác khi tài xế được đề xuất không phản hồi hoặc từ chối chuyến.
* Hạn chế trường hợp khách hàng phải tạo lại yêu cầu khi việc phân công tài xế thất bại.

### BG-03 – Nâng cao hiệu quả quản lý và vận hành

**Business Goal:**
Tập trung hóa hoạt động quản lý khách hàng, tài xế, phương tiện và chuyến đi nhằm giúp bộ phận vận hành theo dõi và xử lý hoạt động kinh doanh hiệu quả hơn.

**Mục tiêu:**

* Hỗ trợ nhân viên vận hành theo dõi các chuyến đang diễn ra.
* Kiểm tra trạng thái hoạt động của tài xế.
* Hỗ trợ xử lý các trường hợp chuyến đi bị lỗi.
* Tra cứu lịch sử giao dịch.
* Phân quyền các thao tác quản trị theo vai trò.

---

### BG-04 – Quản lý doanh thu và thanh toán hiệu quả

**Business Goal:**
Xây dựng quy trình tính cước và thanh toán tập trung, chính xác và có khả năng tích hợp với các dịch vụ thanh toán điện tử bên ngoài.

**Mục tiêu:**

* Xác định chính xác số tiền khách hàng cần thanh toán sau chuyến đi.
* Hỗ trợ cả thanh toán tiền mặt và thanh toán điện tử.
* Giảm rủi ro khi quản lý thông tin thanh toán nhạy cảm.
* Có khả năng xử lý lại giao dịch khi thanh toán điện tử thất bại.
* Cung cấp dữ liệu phục vụ theo dõi doanh thu.

Tài liệu yêu cầu doanh nghiệp tích hợp nhà cung cấp thanh toán bên ngoài nhưng không lưu trực tiếp thông tin nhạy cảm của thẻ hoặc tài khoản thanh toán trong hệ thống CAB.

---

### BG-05 – Cải thiện khả năng theo dõi và giao tiếp với khách hàng, tài xế

**Business Goal:**
Cung cấp thông tin kịp thời cho khách hàng và tài xế trong suốt quá trình sử dụng dịch vụ.

**Mục tiêu:**

* Thông báo cho khách hàng về trạng thái yêu cầu và chuyến đi.
* Thông báo khi tài xế nhận chuyến và khi tài xế đến điểm đón.
* Thông báo kết quả thanh toán.
* Thông báo cho tài xế về chuyến mới và các thay đổi liên quan đến chuyến đang thực hiện.
* Cho phép mở rộng thêm các kênh thông báo trong tương lai.

---

### BG-06 – Đảm bảo hệ thống hoạt động ổn định và có khả năng mở rộng

**Business Goal:**
Xây dựng nền tảng CAB có khả năng đáp ứng nhu cầu tăng cao và phát triển lâu dài mà không ảnh hưởng lớn đến các chức năng đang hoạt động.

**Mục tiêu:**

* Duy trì hoạt động ổn định khi nhu cầu sử dụng tăng cao.
* Cho phép các thành phần của hệ thống mở rộng độc lập khi tải tăng.
* Cho phép triển khai từng phần các chức năng mới.
* Hạn chế ảnh hưởng của lỗi ở một thành phần đến toàn bộ hệ thống.
* Tạo nền tảng có thể phục vụ số lượng lớn khách hàng và tài xế.

Đây là một trong những kỳ vọng quan trọng của doanh nghiệp đối với nền tảng CAB mới.

---

### BG-07 – Đảm bảo an toàn và bảo mật dữ liệu

**Business Goal:**
Bảo vệ thông tin người dùng, dữ liệu vận hành và dữ liệu giao dịch trong quá trình hệ thống hoạt động.

**Mục tiêu:**

* Đảm bảo khách hàng và tài xế được xác thực trước khi sử dụng các chức năng yêu cầu tài khoản.
* Kiểm soát quyền truy cập đối với các thao tác quản trị.
* Bảo vệ thông tin cá nhân, thông tin phương tiện, dữ liệu vị trí và dữ liệu giao dịch.
* Lưu vết các thao tác quan trọng để hỗ trợ kiểm tra và xử lý sự cố.

Các mục tiêu này được xác định trực tiếp từ yêu cầu bảo mật của doanh nghiệp.

---

### BG-08 – Hỗ trợ ra quyết định và đánh giá hiệu quả kinh doanh

**Business Goal:**
Cung cấp dữ liệu và báo cáo cần thiết để ban lãnh đạo theo dõi tình hình hoạt động và đánh giá hiệu quả kinh doanh của dịch vụ đặt xe.

**Mục tiêu:**

* Theo dõi số lượng chuyến.
* Theo dõi doanh thu.
* Theo dõi tỷ lệ chuyến hoàn thành.
* Theo dõi tỷ lệ hủy chuyến.
* Đánh giá hiệu quả hoạt động của tài xế.

Ban lãnh đạo được kỳ vọng có báo cáo về các chỉ số hoạt động này.

---

## 4.1. Business Goals Summary

| ID    | Business Goal                             | Mục đích chính                           |
| ----- | ----------------------------------------- | ---------------------------------------- |
| BG-01 | Nâng cao chất lượng dịch vụ đặt xe        | Cải thiện trải nghiệm khách hàng         |
| BG-02 | Nâng cao hiệu quả phân công tài xế        | Tìm và phân công tài xế phù hợp          |
| BG-03 | Nâng cao hiệu quả quản lý và vận hành     | Hỗ trợ bộ phận vận hành quản lý hệ thống |
| BG-04 | Quản lý doanh thu và thanh toán hiệu quả  | Quản lý cước và thanh toán               |
| BG-05 | Cải thiện khả năng theo dõi và giao tiếp  | Cung cấp thông tin kịp thời              |
| BG-06 | Đảm bảo ổn định và khả năng mở rộng       | Đáp ứng nhu cầu tăng trưởng              |
| BG-07 | Đảm bảo an toàn và bảo mật dữ liệu        | Bảo vệ dữ liệu và kiểm soát truy cập     |
| BG-08 | Hỗ trợ ra quyết định và đánh giá hiệu quả | Cung cấp báo cáo cho quản lý             |
| BG-09 | Tạo nền tảng linh hoạt cho tương lai      | Hỗ trợ mở rộng dịch vụ và công nghệ      |

## 5. Project Scope – Xác định phạm vi phát triển

Dựa trên các Business Goals đã xác định, sẽ giới hạn phạm vi phát triển trong giai đoạn đầu để phù hợp với thời gian xây dựng và triển khai sản phẩm là **7 tuần**.

Các chức năng được ưu tiên là những chức năng **cốt lõi để hệ thống CAB có thể thực hiện được quy trình đặt xe hoàn chỉnh**: khách hàng tạo yêu cầu → tìm tài xế → thực hiện chuyến → tính cước → thanh toán → thông báo → đánh giá.

### Các module nằm trong phạm vi phát triển

| STT | Module                                | Business Goal liên quan | Phạm vi chính                                                                                               | Mức độ          |
| --- | ------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------- | --------------- |
| 1   | **User & Account Management**         | BG-01, BG-07            | Đăng ký, đăng nhập, cập nhật thông tin khách hàng và tài xế; xác thực người dùng                            | **Must Have**   |
| 2   | **Driver Management**                 | BG-02, BG-03            | Quản lý hồ sơ tài xế, phương tiện và trạng thái sẵn sàng nhận chuyến                                        | **Must Have**   |
| 3   | **Booking Management**                | BG-01, BG-02            | Nhập điểm đón/điểm đến, lựa chọn loại xe, tạo và quản lý yêu cầu đặt xe                                     | **Must Have**   |
| 4   | **Driver Matching & Trip Management** | BG-02, BG-03            | Tìm tài xế phù hợp, gửi yêu cầu nhận chuyến, xử lý từ chối/không phản hồi, cập nhật trạng thái chuyến       | **Must Have**   |
| 5   | **Fare & Payment Management**         | BG-04                   | Tính cước, hỗ trợ tiền mặt và thanh toán điện tử thông qua nhà cung cấp bên ngoài, xử lý kết quả thanh toán | **Must Have**   |
| 6   | **Notification Management**           | BG-05                   | Gửi thông báo về đặt xe, tài xế nhận chuyến, tài xế đến, hoàn thành chuyến và thanh toán                    | **Must Have**   |
| 7   | **Rating & Trip History**             | BG-01                   | Xem lịch sử chuyến đi, số tiền phải trả và đánh giá tài xế sau chuyến                                       | **Should Have** |
| 8   | **Operation Management**              | BG-03                   | Quản lý khách hàng, tài xế, phương tiện, chuyến đi; theo dõi chuyến đang diễn ra và xử lý trường hợp lỗi    | **Must Have**   |
| 9   | **Report & Dashboard**                | BG-08                   | Báo cáo số lượng chuyến, doanh thu, tỷ lệ hoàn thành, tỷ lệ hủy và hiệu quả tài xế                          | **Should Have** |
| 10  | **Security & Access Control**         | BG-07                   | Phân quyền quản trị, kiểm soát truy cập và lưu vết các thao tác quan trọng                                  | **Must Have**   |

# 6. Business Requirements

### BG01 – Quản lý và đặt xe

Hệ thống phải hỗ trợ khách hàng quản lý tài khoản, tạo yêu cầu đặt xe, theo dõi chuyến đi, xem lịch sử chuyến đi và đánh giá tài xế.

### BG02 – Quản lý và phân công tài xế

Hệ thống phải hỗ trợ quản lý thông tin, trạng thái hoạt động của tài xế và tự động tìm kiếm, phân công tài xế phù hợp cho từng yêu cầu đặt xe.

### BG03 – Quản lý chuyến đi và vận hành

Hệ thống phải hỗ trợ nhân viên vận hành quản lý khách hàng, tài xế, phương tiện và chuyến đi; đồng thời theo dõi các chuyến đang diễn ra và xử lý các trường hợp phát sinh.

### BG04 – Quản lý cước phí và thanh toán

Hệ thống phải hỗ trợ tính cước chuyến đi, thanh toán bằng tiền mặt hoặc phương thức điện tử, tích hợp với nhà cung cấp thanh toán bên ngoài và xử lý trường hợp thanh toán thất bại.

### BG05 – Quản lý thông báo

Hệ thống phải cung cấp thông báo cho khách hàng và tài xế về các sự kiện liên quan đến quá trình đặt xe, phân công tài xế, chuyến đi và thanh toán.

### BG06 – Đảm bảo tính ổn định và khả năng mở rộng

Hệ thống phải hoạt động ổn định trong thời gian cao điểm, hạn chế ảnh hưởng khi một thành phần gặp lỗi và cho phép các thành phần được mở rộng hoặc triển khai độc lập.

### BG07 – Đảm bảo an toàn và bảo mật

Hệ thống phải xác thực người dùng, kiểm soát quyền truy cập quản trị, bảo vệ dữ liệu cá nhân, thông tin phương tiện, vị trí và giao dịch, đồng thời lưu vết các thao tác quan trọng.

### BG08 – Báo cáo và đánh giá hiệu quả kinh doanh

Hệ thống phải cung cấp các báo cáo phục vụ quản lý và ra quyết định, bao gồm số lượng chuyến, doanh thu, tỷ lệ hoàn thành, tỷ lệ hủy và hiệu quả hoạt động của tài xế.

### BG09 – Hỗ trợ mở rộng trong tương lai

Hệ thống phải có kiến trúc linh hoạt để có thể bổ sung loại hình dịch vụ, phương thức thanh toán, nhà cung cấp thông báo và các thành phần kỹ thuật mới mà không cần xây dựng lại toàn bộ hệ thống.

# 7. Business Process Modeling

## 7.1. Tổng quan quy trình nghiệp vụ

Hệ thống quản lý và đặt xe bao gồm các quy trình nghiệp vụ chính từ khi khách hàng tạo yêu cầu đặt xe, hệ thống tìm kiếm và phân công tài xế, thực hiện chuyến đi, thanh toán cho đến khi hoàn tất chuyến và đánh giá tài xế.

Các quy trình chính gồm:

1. Đặt xe và phân công tài xế.
2. Thực hiện và theo dõi chuyến đi.
3. Thanh toán và xử lý thanh toán thất bại.
4. Đánh giá chuyến đi và tài xế.
5. Quản lý và vận hành tài xế, phương tiện và chuyến đi.
6. Quản lý thông báo.
7. Báo cáo và đánh giá hiệu quả kinh doanh.

---

## 7.2. Quy trình đặt xe và phân công tài xế

### 7.2.1. Mục tiêu

Quy trình cho phép khách hàng tạo yêu cầu đặt xe và hệ thống tự động tìm kiếm, phân công tài xế phù hợp.

### 7.2.2. Tác nhân tham gia

* **Khách hàng**
* **Hệ thống**
* **Tài xế**
* **Nhân viên vận hành**

### 7.2.3. Quy trình

1. Khách hàng đăng nhập vào hệ thống.
2. Khách hàng nhập thông tin chuyến đi gồm điểm đón, điểm đến và các thông tin cần thiết.
3. Hệ thống kiểm tra tính hợp lệ của yêu cầu.
4. Nếu thông tin không hợp lệ, hệ thống yêu cầu khách hàng điều chỉnh.
5. Nếu thông tin hợp lệ, hệ thống tạo yêu cầu đặt xe.
6. Hệ thống tính cước dự kiến cho chuyến đi.
7. Hệ thống tìm kiếm các tài xế phù hợp dựa trên trạng thái hoạt động, vị trí và khả năng đáp ứng.
8. Hệ thống gửi yêu cầu nhận chuyến đến tài xế phù hợp.
9. Tài xế chấp nhận hoặc từ chối yêu cầu.
10. Nếu tài xế từ chối hoặc không phản hồi, hệ thống tiếp tục tìm kiếm tài xế khác.
11. Nếu có tài xế nhận chuyến, hệ thống xác nhận chuyến đi.
12. Hệ thống gửi thông báo cho khách hàng và tài xế.
13. Quy trình kết thúc.

### 7.2.4. Sơ đồ quy trình

```mermaid
flowchart TD
    A([Bắt đầu]) --> B[Khách hàng đăng nhập]
    B --> C[Nhập thông tin đặt xe]
    C --> D{Thông tin hợp lệ?}

    D -- Không --> E[Thông báo lỗi]
    E --> C

    D -- Có --> F[Tạo yêu cầu đặt xe]
    F --> G[Tính cước dự kiến]
    G --> H[Tìm kiếm tài xế phù hợp]
    H --> I[Gửi yêu cầu nhận chuyến]

    I --> J{Tài xế chấp nhận?}

    J -- Không --> K{Còn tài xế phù hợp?}
    K -- Có --> H
    K -- Không --> L[Thông báo không tìm được tài xế]
    L --> M([Kết thúc])

    J -- Có --> N[Xác nhận chuyến đi]
    N --> O[Gửi thông báo cho khách hàng và tài xế]
    O --> M([Kết thúc])
```

---

## 7.3. Quy trình thực hiện và theo dõi chuyến đi

### 7.3.1. Mục tiêu

Quy trình quản lý chuyến đi từ khi tài xế được phân công đến khi chuyến đi hoàn tất hoặc phát sinh vấn đề cần xử lý.

### 7.3.2. Tác nhân tham gia

* **Khách hàng**
* **Tài xế**
* **Hệ thống**
* **Nhân viên vận hành**

### 7.3.3. Quy trình

1. Sau khi chuyến đi được xác nhận, tài xế nhận thông tin chuyến.
2. Tài xế di chuyển đến điểm đón.
3. Hệ thống cập nhật trạng thái chuyến đi.
4. Khách hàng theo dõi trạng thái và thông tin chuyến đi.
5. Tài xế đón khách.
6. Tài xế bắt đầu chuyến đi.
7. Hệ thống cập nhật và lưu thông tin chuyến đi trong quá trình di chuyển.
8. Nếu phát sinh sự cố, tài xế hoặc khách hàng gửi thông tin đến hệ thống.
9. Nhân viên vận hành tiếp nhận và xử lý trường hợp phát sinh.
10. Tài xế đưa khách đến điểm đến.
11. Tài xế kết thúc chuyến đi.
12. Hệ thống cập nhật trạng thái chuyến thành hoàn thành.
13. Hệ thống chuyển sang quy trình thanh toán.
14. Quy trình kết thúc.

### 7.3.4. Sơ đồ quy trình

```mermaid
flowchart TD
    A([Bắt đầu]) --> B[Chuyến đi được xác nhận]
    B --> C[Tài xế nhận thông tin chuyến]
    C --> D[Di chuyển đến điểm đón]
    D --> E[Cập nhật trạng thái]
    E --> F[Khách hàng theo dõi chuyến đi]
    F --> G[Đón khách]
    G --> H[Bắt đầu chuyến đi]
    H --> I[Cập nhật thông tin chuyến đi]

    I --> J{Có phát sinh sự cố?}

    J -- Có --> K[Gửi thông tin sự cố]
    K --> L[Nhân viên vận hành xử lý]
    L --> I

    J -- Không --> M[Di chuyển đến điểm đến]
    M --> N[Kết thúc chuyến đi]
    N --> O[Cập nhật trạng thái hoàn thành]
    O --> P[Chuyển sang thanh toán]
    P --> Q([Kết thúc])
```

---

## 7.4. Quy trình thanh toán

### 7.4.1. Mục tiêu

Quy trình thực hiện thanh toán cước chuyến đi bằng tiền mặt hoặc phương thức thanh toán điện tử.

### 7.4.2. Tác nhân tham gia

* **Khách hàng**
* **Hệ thống**
* **Nhà cung cấp dịch vụ thanh toán**
* **Tài xế**

### 7.4.3. Quy trình

1. Chuyến đi được hoàn thành.
2. Hệ thống xác định cước phí cuối cùng.
3. Hệ thống xác định phương thức thanh toán của khách hàng.
4. Nếu khách hàng thanh toán bằng tiền mặt, khách hàng thanh toán trực tiếp cho tài xế.
5. Tài xế xác nhận đã nhận tiền.
6. Hệ thống cập nhật trạng thái thanh toán thành công.
7. Nếu khách hàng thanh toán điện tử, hệ thống gửi yêu cầu thanh toán đến nhà cung cấp dịch vụ thanh toán.
8. Nhà cung cấp thanh toán xử lý giao dịch.
9. Hệ thống nhận kết quả giao dịch.
10. Nếu giao dịch thành công, hệ thống cập nhật trạng thái thanh toán.
11. Nếu giao dịch thất bại, hệ thống thông báo cho khách hàng và cho phép thực hiện lại hoặc lựa chọn phương thức thanh toán khác.
12. Hệ thống gửi thông báo kết quả thanh toán.
13. Quy trình kết thúc.

### 7.4.4. Sơ đồ quy trình

```mermaid
flowchart TD
    A([Bắt đầu]) --> B[Chuyến đi hoàn thành]
    B --> C[Xác định cước phí cuối cùng]
    C --> D{Phương thức thanh toán?}

    D -- Tiền mặt --> E[Khách hàng thanh toán cho tài xế]
    E --> F[Tài xế xác nhận thanh toán]
    F --> G[Cập nhật thanh toán thành công]

    D -- Điện tử --> H[Gửi yêu cầu đến nhà cung cấp thanh toán]
    H --> I[Nhà cung cấp xử lý giao dịch]
    I --> J{Thanh toán thành công?}

    J -- Có --> G
    J -- Không --> K[Thông báo thanh toán thất bại]
    K --> L{Thực hiện lại hoặc đổi phương thức?}
    L -- Có --> D
    L -- Không --> M[Ghi nhận thanh toán chưa hoàn tất]
    
    G --> N[Gửi thông báo kết quả]
    M --> N
    N --> O([Kết thúc])
```

---

## 7.5. Quy trình đánh giá chuyến đi và tài xế

### 7.5.1. Mục tiêu

Cho phép khách hàng đánh giá chất lượng chuyến đi và tài xế sau khi chuyến đi hoàn tất.

### 7.5.2. Quy trình

1. Chuyến đi được hoàn thành.
2. Hệ thống gửi yêu cầu đánh giá đến khách hàng.
3. Khách hàng lựa chọn mức đánh giá và nhập nhận xét nếu cần.
4. Hệ thống kiểm tra dữ liệu đánh giá.
5. Hệ thống lưu đánh giá.
6. Hệ thống cập nhật dữ liệu đánh giá của tài xế.
7. Dữ liệu đánh giá được sử dụng cho việc theo dõi và đánh giá hiệu quả tài xế.
8. Quy trình kết thúc.

### 7.5.3. Sơ đồ quy trình

```mermaid
flowchart TD
    A([Bắt đầu]) --> B[Chuyến đi hoàn thành]
    B --> C[Gửi yêu cầu đánh giá]
    C --> D[Khách hàng đánh giá tài xế]
    D --> E{Dữ liệu hợp lệ?}
    E -- Không --> F[Thông báo lỗi]
    F --> D
    E -- Có --> G[Lưu đánh giá]
    G --> H[Cập nhật dữ liệu đánh giá tài xế]
    H --> I([Kết thúc])
```

---

## 7.6. Quy trình quản lý và vận hành

### 7.6.1. Mục tiêu

Hỗ trợ nhân viên vận hành quản lý khách hàng, tài xế, phương tiện và các chuyến đi đang diễn ra.

### 7.6.2. Tác nhân tham gia

* **Nhân viên vận hành**
* **Hệ thống**
* **Khách hàng**
* **Tài xế**

### 7.6.3. Quy trình

1. Nhân viên vận hành đăng nhập hệ thống.
2. Hệ thống xác thực tài khoản và quyền truy cập.
3. Nhân viên lựa chọn chức năng cần quản lý.
4. Hệ thống cung cấp thông tin tương ứng về khách hàng, tài xế, phương tiện hoặc chuyến đi.
5. Nhân viên theo dõi trạng thái hoạt động của tài xế và chuyến đi.
6. Khi phát hiện vấn đề, nhân viên tiếp nhận và xử lý.
7. Hệ thống cập nhật kết quả xử lý.
8. Hệ thống lưu vết các thao tác quản trị quan trọng.
9. Quy trình kết thúc.

### 7.6.4. Sơ đồ quy trình

```mermaid
flowchart TD
    A([Bắt đầu]) --> B[Nhân viên vận hành đăng nhập]
    B --> C{Xác thực và phân quyền}
    C -- Không hợp lệ --> D[Từ chối truy cập]
    D --> E([Kết thúc])

    C -- Hợp lệ --> F[Truy cập chức năng quản lý]
    F --> G{Đối tượng quản lý?}

    G -- Khách hàng --> H[Quản lý thông tin khách hàng]
    G -- Tài xế --> I[Quản lý tài xế và trạng thái hoạt động]
    G -- Phương tiện --> J[Quản lý phương tiện]
    G -- Chuyến đi --> K[Theo dõi và quản lý chuyến đi]

    H --> L{Có vấn đề cần xử lý?}
    I --> L
    J --> L
    K --> L

    L -- Có --> M[Xử lý trường hợp phát sinh]
    M --> N[Cập nhật kết quả]
    N --> O[Lưu vết thao tác]

    L -- Không --> O
    O --> E([Kết thúc])
```

---

## 7.7. Quy trình quản lý thông báo

### 7.7.1. Mục tiêu

Đảm bảo khách hàng và tài xế nhận được thông tin kịp thời về các sự kiện liên quan đến đặt xe, phân công tài xế, chuyến đi và thanh toán.

### 7.7.2. Quy trình

1. Hệ thống phát sinh một sự kiện nghiệp vụ.
2. Hệ thống xác định đối tượng cần nhận thông báo.
3. Hệ thống xác định loại thông báo và kênh gửi.
4. Hệ thống gửi thông báo.
5. Hệ thống kiểm tra kết quả gửi.
6. Nếu gửi thành công, hệ thống ghi nhận trạng thái thông báo.
7. Nếu gửi thất bại, hệ thống ghi nhận lỗi và thực hiện cơ chế gửi lại theo cấu hình.
8. Quy trình kết thúc.

### 7.7.3. Sơ đồ quy trình

```mermaid
flowchart TD
    A([Bắt đầu]) --> B[Phát sinh sự kiện nghiệp vụ]
    B --> C[Xác định đối tượng nhận]
    C --> D[Xác định loại và kênh thông báo]
    D --> E[Gửi thông báo]
    E --> F{Gửi thành công?}

    F -- Có --> G[Ghi nhận trạng thái đã gửi]
    F -- Không --> H[Ghi nhận lỗi]
    H --> I{Có thể gửi lại?}
    I -- Có --> E
    I -- Không --> J[Ghi nhận thông báo thất bại]

    G --> K([Kết thúc])
    J --> K
```

---

## 7.8. Quy trình báo cáo và đánh giá hiệu quả kinh doanh

### 7.8.1. Mục tiêu

Cung cấp thông tin phục vụ quản lý, theo dõi hoạt động kinh doanh và đánh giá hiệu quả vận hành.

### 7.8.2. Quy trình

1. Nhân viên quản lý truy cập chức năng báo cáo.
2. Nhân viên lựa chọn loại báo cáo và khoảng thời gian.
3. Hệ thống truy xuất dữ liệu liên quan.
4. Hệ thống tổng hợp và tính toán các chỉ số.
5. Hệ thống tạo báo cáo.
6. Nhân viên xem báo cáo.
7. Báo cáo có thể bao gồm:

   * Số lượng chuyến đi.
   * Doanh thu.
   * Tỷ lệ hoàn thành chuyến.
   * Tỷ lệ hủy chuyến.
   * Hiệu quả hoạt động của tài xế.
8. Nhân viên sử dụng báo cáo để theo dõi và ra quyết định.
9. Quy trình kết thúc.

### 7.8.3. Sơ đồ quy trình

```mermaid
flowchart TD
    A([Bắt đầu]) --> B[Truy cập chức năng báo cáo]
    B --> C[Chọn loại báo cáo và khoảng thời gian]
    C --> D[Truy xuất dữ liệu]
    D --> E[Tổng hợp và tính toán chỉ số]
    E --> F[Tạo báo cáo]
    F --> G[Hiển thị báo cáo]
    G --> H[Phân tích và đánh giá hiệu quả]
    H --> I([Kết thúc])
```

---

## 7.9. Mối quan hệ giữa Business Requirements và Business Processes

| Business Requirement                                | Business Process liên quan                                                                          |
| --------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| **BG01 – Quản lý và đặt xe**                        | Quy trình đặt xe và phân công tài xế; Quy trình thực hiện và theo dõi chuyến đi; Quy trình đánh giá |
| **BG02 – Quản lý và phân công tài xế**              | Quy trình đặt xe và phân công tài xế; Quy trình quản lý và vận hành                                 |
| **BG03 – Quản lý chuyến đi và vận hành**            | Quy trình thực hiện và theo dõi chuyến đi; Quy trình quản lý và vận hành                            |
| **BG04 – Quản lý cước phí và thanh toán**           | Quy trình thanh toán                                                                                |
| **BG05 – Quản lý thông báo**                        | Quy trình quản lý thông báo                                                                         |
| **BG06 – Đảm bảo tính ổn định và khả năng mở rộng** | Áp dụng xuyên suốt các quy trình nghiệp vụ                                                          |
| **BG07 – Đảm bảo an toàn và bảo mật**               | Quy trình đăng nhập, xác thực, phân quyền và lưu vết trong các quy trình                            |
| **BG08 – Báo cáo và đánh giá hiệu quả kinh doanh**  | Quy trình báo cáo và đánh giá hiệu quả kinh doanh                                                   |
                                            |

# 8. Business Functions

Các chức năng nghiệp vụ được phân rã từ các quy trình nghiệp vụ tại mục 7. Mỗi chức năng nghiệp vụ thể hiện một khả năng mà hệ thống phải cung cấp để hỗ trợ thực hiện nghiệp vụ.

## 8.1. Nhóm chức năng quản lý tài khoản và đặt xe

| Mã SR    | Chức năng nghiệp vụ       | Mô tả                                                                              |
| -------- | ------------------------- | ---------------------------------------------------------------------------------- |
| **SR01** | Đăng ký tài khoản         | Cho phép khách hàng tạo tài khoản để sử dụng dịch vụ.                              |
| **SR02** | Đăng nhập và xác thực     | Cho phép khách hàng, tài xế và nhân viên vận hành đăng nhập và xác thực danh tính. |
| **SR03** | Quản lý thông tin cá nhân | Cho phép người dùng xem và cập nhật thông tin tài khoản cá nhân.                   |
| **SR04** | Tạo yêu cầu đặt xe        | Cho phép khách hàng nhập thông tin và tạo yêu cầu đặt xe.                          |
| **SR05** | Kiểm tra yêu cầu đặt xe   | Cho phép hệ thống kiểm tra tính hợp lệ của thông tin đặt xe.                       |
| **SR06** | Tính cước dự kiến         | Cho phép hệ thống tính và hiển thị cước phí dự kiến cho chuyến đi.                 |
| **SR07** | Hủy yêu cầu đặt xe        | Cho phép khách hàng hủy yêu cầu đặt xe theo điều kiện nghiệp vụ.                   |
| **SR08** | Xem lịch sử chuyến đi     | Cho phép khách hàng xem các chuyến đi đã thực hiện.                                |

---

## 8.2. Nhóm chức năng quản lý và phân công tài xế

| Mã SR    | Chức năng nghiệp vụ       | Mô tả                                                                                                          |
| -------- | ------------------------- | -------------------------------------------------------------------------------------------------------------- |
| **SR09** | Quản lý thông tin tài xế  | Cho phép nhân viên vận hành quản lý thông tin tài xế.                                                          |
| **SR10** | Quản lý trạng thái tài xế | Cho phép hệ thống cập nhật và theo dõi trạng thái hoạt động của tài xế.                                        |
| **SR11** | Xác định tài xế phù hợp   | Cho phép hệ thống tìm kiếm tài xế phù hợp với yêu cầu đặt xe.                                                  |
| **SR12** | Phân công tài xế          | Cho phép hệ thống gửi và phân công yêu cầu chuyến đi cho tài xế phù hợp.                                       |
| **SR13** | Tiếp nhận yêu cầu chuyến  | Cho phép tài xế xem và chấp nhận hoặc từ chối yêu cầu nhận chuyến.                                             |
| **SR14** | Phân công lại tài xế      | Cho phép hệ thống tiếp tục tìm kiếm và phân công tài xế khác khi tài xế được chọn từ chối hoặc không phản hồi. |

---

## 8.3. Nhóm chức năng quản lý và theo dõi chuyến đi

| Mã SR    | Chức năng nghiệp vụ                 | Mô tả                                                                                            |
| -------- | ----------------------------------- | ------------------------------------------------------------------------------------------------ |
| **SR15** | Xác nhận chuyến đi                  | Cho phép hệ thống xác nhận chuyến sau khi tài xế nhận yêu cầu.                                   |
| **SR16** | Cập nhật trạng thái chuyến đi       | Cho phép hệ thống cập nhật trạng thái của chuyến theo từng giai đoạn.                            |
| **SR17** | Theo dõi chuyến đi                  | Cho phép khách hàng và nhân viên vận hành theo dõi trạng thái chuyến đi.                         |
| **SR18** | Cập nhật thông tin vị trí chuyến đi | Cho phép hệ thống cập nhật thông tin vị trí của tài xế trong quá trình thực hiện chuyến.         |
| **SR19** | Bắt đầu chuyến đi                   | Cho phép tài xế xác nhận bắt đầu thực hiện chuyến.                                               |
| **SR20** | Kết thúc chuyến đi                  | Cho phép tài xế xác nhận hoàn thành chuyến khi đến điểm đến.                                     |
| **SR21** | Quản lý trường hợp phát sinh        | Cho phép tài xế, khách hàng hoặc nhân viên vận hành ghi nhận và xử lý các sự cố trong chuyến đi. |

---

## 8.4. Nhóm chức năng quản lý phương tiện

| Mã SR    | Chức năng nghiệp vụ            | Mô tả                                                                           |
| -------- | ------------------------------ | ------------------------------------------------------------------------------- |
| **SR22** | Quản lý thông tin phương tiện  | Cho phép nhân viên vận hành quản lý thông tin các phương tiện tham gia dịch vụ. |
| **SR23** | Quản lý trạng thái phương tiện | Cho phép theo dõi và cập nhật trạng thái hoạt động của phương tiện.             |
| **SR24** | Gán phương tiện cho tài xế     | Cho phép quản lý mối quan hệ giữa tài xế và phương tiện được sử dụng.           |

---

## 8.5. Nhóm chức năng quản lý cước phí và thanh toán

| Mã SR    | Chức năng nghiệp vụ       | Mô tả                                                                                                |
| -------- | ------------------------- | ---------------------------------------------------------------------------------------------------- |
| **SR25** | Tính cước cuối chuyến     | Cho phép hệ thống xác định cước phí cuối cùng dựa trên thông tin thực tế của chuyến đi.              |
| **SR26** | Thanh toán tiền mặt       | Cho phép khách hàng thanh toán trực tiếp bằng tiền mặt và tài xế xác nhận thanh toán.                |
| **SR27** | Thanh toán điện tử        | Cho phép khách hàng thực hiện thanh toán thông qua nhà cung cấp dịch vụ thanh toán bên ngoài.        |
| **SR28** | Xử lý kết quả thanh toán  | Cho phép hệ thống tiếp nhận và cập nhật trạng thái giao dịch thanh toán.                             |
| **SR29** | Xử lý thanh toán thất bại | Cho phép hệ thống thông báo và hỗ trợ khách hàng thực hiện lại hoặc thay đổi phương thức thanh toán. |
| **SR30** | Xem thông tin thanh toán  | Cho phép người dùng xem thông tin và trạng thái thanh toán của chuyến đi.                            |

---

## 8.6. Nhóm chức năng thông báo

| Mã SR    | Chức năng nghiệp vụ             | Mô tả                                                                               |
| -------- | ------------------------------- | ----------------------------------------------------------------------------------- |
| **SR31** | Gửi thông báo đặt xe            | Cho phép hệ thống thông báo kết quả tạo yêu cầu đặt xe cho khách hàng.              |
| **SR32** | Gửi thông báo phân công tài xế  | Cho phép hệ thống thông báo thông tin phân công chuyến cho khách hàng và tài xế.    |
| **SR33** | Gửi thông báo trạng thái chuyến | Cho phép hệ thống thông báo các thay đổi quan trọng của chuyến đi.                  |
| **SR34** | Gửi thông báo thanh toán        | Cho phép hệ thống thông báo kết quả thanh toán cho khách hàng và các bên liên quan. |
| **SR35** | Quản lý trạng thái thông báo    | Cho phép hệ thống ghi nhận trạng thái gửi và xử lý trường hợp thông báo thất bại.   |

---

## 8.7. Nhóm chức năng đánh giá

| Mã SR    | Chức năng nghiệp vụ     | Mô tả                                                                 |
| -------- | ----------------------- | --------------------------------------------------------------------- |
| **SR36** | Đánh giá chuyến đi      | Cho phép khách hàng đánh giá chất lượng chuyến đi sau khi hoàn thành. |
| **SR37** | Đánh giá tài xế         | Cho phép khách hàng đánh giá tài xế dựa trên trải nghiệm chuyến đi.   |
| **SR38** | Quản lý đánh giá tài xế | Cho phép hệ thống lưu trữ và tổng hợp dữ liệu đánh giá của tài xế.    |

---

## 8.8. Nhóm chức năng quản lý và vận hành

| Mã SR    | Chức năng nghiệp vụ          | Mô tả                                                                                         |
| -------- | ---------------------------- | --------------------------------------------------------------------------------------------- |
| **SR39** | Quản lý khách hàng           | Cho phép nhân viên vận hành xem và quản lý thông tin khách hàng.                              |
| **SR40** | Theo dõi hoạt động tài xế    | Cho phép nhân viên vận hành theo dõi trạng thái và hoạt động của tài xế.                      |
| **SR41** | Theo dõi chuyến đang diễn ra | Cho phép nhân viên vận hành theo dõi các chuyến đi đang thực hiện.                            |
| **SR42** | Xử lý trường hợp phát sinh   | Cho phép nhân viên vận hành tiếp nhận và xử lý các vấn đề phát sinh trong quá trình vận hành. |
| **SR43** | Quản lý tài khoản nhân viên  | Cho phép quản lý hệ thống quản lý tài khoản và quyền của nhân viên vận hành.                  |

---

## 8.9. Nhóm chức năng báo cáo và đánh giá hiệu quả

| Mã SR    | Chức năng nghiệp vụ             | Mô tả                                                                                      |
| -------- | ------------------------------- | ------------------------------------------------------------------------------------------ |
| **SR44** | Báo cáo số lượng chuyến         | Cho phép nhân viên quản lý xem số lượng chuyến theo khoảng thời gian và tiêu chí lựa chọn. |
| **SR45** | Báo cáo doanh thu               | Cho phép nhân viên quản lý theo dõi doanh thu từ các chuyến đi.                            |
| **SR46** | Báo cáo tỷ lệ hoàn thành chuyến | Cho phép hệ thống tính toán và cung cấp tỷ lệ chuyến hoàn thành.                           |
| **SR47** | Báo cáo tỷ lệ hủy chuyến        | Cho phép hệ thống tính toán và cung cấp tỷ lệ hủy chuyến.                                  |
| **SR48** | Báo cáo hiệu quả tài xế         | Cho phép quản lý đánh giá hiệu quả hoạt động của tài xế dựa trên các chỉ số liên quan.     |

---

## 8.10. Nhóm chức năng an toàn và bảo mật

| Mã SR    | Chức năng nghiệp vụ        | Mô tả                                                                          |
| -------- | -------------------------- | ------------------------------------------------------------------------------ |
| **SR49** | Phân quyền người dùng      | Cho phép hệ thống kiểm soát quyền truy cập dựa trên vai trò của người dùng.    |
| **SR50** | Bảo vệ dữ liệu             | Cho phép hệ thống bảo vệ thông tin cá nhân, phương tiện, vị trí và giao dịch.  |
| **SR51** | Ghi nhận nhật ký hoạt động | Cho phép hệ thống lưu vết các thao tác quan trọng của người dùng và nhân viên. |

---

## 8.11. Ma trận truy xuất Business Process – System Requirement

| Business Process                                   | Các System Requirements                                                            |
| -------------------------------------------------- | ---------------------------------------------------------------------------------- |
| **BP01 – Đặt xe và phân công tài xế**              | SR01, SR02, SR03, SR04, SR05, SR06, SR07, SR09, SR10, SR11, SR12, SR13, SR14, SR15 |
| **BP02 – Thực hiện và theo dõi chuyến đi**         | SR16, SR17, SR18, SR19, SR20, SR21, SR31, SR32, SR33                               |
| **BP03 – Thanh toán**                              | SR25, SR26, SR27, SR28, SR29, SR30, SR34                                           |
| **BP04 – Đánh giá chuyến đi và tài xế**            | SR36, SR37, SR38                                                                   |
| **BP05 – Quản lý và vận hành**                     | SR09, SR10, SR22, SR23, SR24, SR39, SR40, SR41, SR42, SR43                         |
| **BP06 – Quản lý thông báo**                       | SR31, SR32, SR33, SR34, SR35                                                       |
| **BP07 – Báo cáo và đánh giá hiệu quả kinh doanh** | SR44, SR45, SR46, SR47, SR48                                                       |
| **Xuyên suốt hệ thống – An toàn và bảo mật**       | SR02, SR43, SR49, SR50, SR51                                                       |

# 9. Business Rules and Exceptions

## 9.1. Business Rules

Các Business Rule quy định các điều kiện và ràng buộc mà hệ thống phải tuân thủ trong quá trình thực hiện các nghiệp vụ đặt xe, phân công tài xế, thực hiện chuyến đi, thanh toán và vận hành.

### BR01 – Quy định về tài khoản

* Mỗi khách hàng phải có một tài khoản hợp lệ để sử dụng chức năng đặt xe.
* Mỗi tài khoản phải được xác thực trước khi sử dụng các chức năng yêu cầu đăng nhập.
* Người dùng chỉ được truy cập các chức năng tương ứng với vai trò được cấp.
* Thông tin tài khoản phải được bảo vệ và không được cung cấp cho người không có quyền truy cập.

### BR02 – Quy định về yêu cầu đặt xe

* Khách hàng phải cung cấp đầy đủ thông tin bắt buộc trước khi tạo yêu cầu đặt xe.
* Điểm đón và điểm đến phải là các địa điểm hợp lệ.
* Một yêu cầu đặt xe chỉ được tạo khi thông tin yêu cầu hợp lệ.
* Yêu cầu đặt xe phải được gắn với một khách hàng cụ thể.
* Khách hàng chỉ được hủy yêu cầu khi yêu cầu vẫn đang ở trạng thái cho phép hủy.

### BR03 – Quy định về phân công tài xế

* Chỉ tài xế đang ở trạng thái có thể nhận chuyến mới được xem xét phân công.
* Tài xế được lựa chọn phải đáp ứng các điều kiện phù hợp với yêu cầu chuyến đi.
* Hệ thống ưu tiên tài xế phù hợp theo vị trí và khả năng đáp ứng.
* Một yêu cầu đặt xe chỉ được phân công cho một tài xế tại một thời điểm.
* Khi tài xế từ chối hoặc không phản hồi, hệ thống phải có khả năng tìm tài xế khác.
* Khi không còn tài xế phù hợp, yêu cầu đặt xe phải được chuyển sang trạng thái không tìm được tài xế.

### BR04 – Quy định về trạng thái chuyến đi

* Chuyến đi phải được xác nhận trước khi tài xế bắt đầu thực hiện.
* Chuyến đi phải tuân thủ trình tự trạng thái nghiệp vụ.
* Tài xế chỉ được bắt đầu chuyến khi đã được phân công.
* Chuyến đi chỉ được chuyển sang trạng thái hoàn thành sau khi tài xế xác nhận kết thúc chuyến.
* Không được thực hiện các thao tác trái với trạng thái hiện tại của chuyến đi.

### BR05 – Quy định về phương tiện

* Mỗi phương tiện tham gia cung cấp dịch vụ phải có thông tin được quản lý trong hệ thống.
* Phương tiện phải ở trạng thái hợp lệ để được sử dụng cho chuyến đi.
* Phương tiện không hoạt động hoặc không hợp lệ không được sử dụng để thực hiện chuyến.
* Mối quan hệ giữa tài xế và phương tiện phải được quản lý và cập nhật trong hệ thống.

### BR06 – Quy định về cước phí

* Hệ thống phải tính cước dự kiến trước khi khách hàng xác nhận đặt xe nếu thông tin cần thiết đã đầy đủ.
* Cước cuối cùng được xác định dựa trên thông tin thực tế của chuyến đi.
* Cước phí phải được lưu cùng với thông tin chuyến đi.
* Cước phí phải được hiển thị rõ ràng cho khách hàng trước hoặc trong quá trình thanh toán.

### BR07 – Quy định về thanh toán

* Khách hàng có thể thanh toán bằng tiền mặt hoặc phương thức thanh toán điện tử được hệ thống hỗ trợ.
* Với thanh toán tiền mặt, tài xế phải xác nhận đã nhận tiền.
* Với thanh toán điện tử, hệ thống phải gửi yêu cầu đến nhà cung cấp dịch vụ thanh toán.
* Chỉ giao dịch được nhà cung cấp xác nhận thành công mới được ghi nhận là thanh toán thành công.
* Giao dịch thất bại không được ghi nhận là thanh toán thành công.
* Khi thanh toán thất bại, khách hàng phải được thông báo và có thể thực hiện lại hoặc lựa chọn phương thức thanh toán khác.

### BR08 – Quy định về đánh giá

* Khách hàng chỉ được đánh giá sau khi chuyến đi hoàn thành.
* Mỗi chuyến đi chỉ được đánh giá theo quy định của hệ thống.
* Nội dung đánh giá phải đáp ứng các điều kiện về dữ liệu mà hệ thống quy định.
* Đánh giá phải được lưu và liên kết với chuyến đi và tài xế tương ứng.

### BR09 – Quy định về thông báo

* Hệ thống phải gửi thông báo khi xảy ra các sự kiện nghiệp vụ quan trọng.
* Thông báo phải được gửi đến đúng đối tượng liên quan.
* Hệ thống phải ghi nhận trạng thái gửi thông báo.
* Khi gửi thông báo thất bại, hệ thống phải xử lý theo cơ chế gửi lại được cấu hình.

### BR10 – Quy định về quản lý vận hành

* Nhân viên vận hành chỉ được truy cập các chức năng phù hợp với quyền được cấp.
* Nhân viên vận hành được phép theo dõi các chuyến đang diễn ra.
* Các trường hợp phát sinh phải được ghi nhận và xử lý bởi nhân viên có quyền phù hợp.
* Các thao tác quản trị quan trọng phải được lưu vết.

### BR11 – Quy định về báo cáo

* Báo cáo phải được tổng hợp từ dữ liệu nghiệp vụ đã được lưu trong hệ thống.
* Các chỉ số báo cáo phải được tính toán thống nhất theo quy tắc nghiệp vụ.
* Báo cáo phải hỗ trợ lọc theo khoảng thời gian hoặc tiêu chí được hệ thống cung cấp.
* Chỉ người dùng có quyền phù hợp mới được xem các báo cáo quản lý.

### BR12 – Quy định về bảo mật

* Người dùng phải được xác thực trước khi truy cập các chức năng yêu cầu quyền truy cập.
* Hệ thống phải kiểm soát quyền dựa trên vai trò người dùng.
* Thông tin cá nhân, thông tin vị trí và thông tin giao dịch phải được bảo vệ.
* Các thao tác quan trọng phải được ghi nhận để phục vụ kiểm tra và truy vết.

---

## 9.2. Các ngoại lệ (Exceptions)

Các ngoại lệ mô tả những trường hợp quy trình nghiệp vụ không thể thực hiện theo luồng chính và cách hệ thống xử lý.

| Mã       | Ngoại lệ                               | Điều kiện xảy ra                                                      | Cách xử lý                                                                                             |
| -------- | -------------------------------------- | --------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| **EX01** | Thông tin đặt xe không hợp lệ          | Khách hàng nhập thiếu hoặc sai thông tin                              | Hệ thống thông báo lỗi và yêu cầu nhập lại.                                                            |
| **EX02** | Không tìm được tài xế                  | Không có tài xế phù hợp hoặc tất cả tài xế đều từ chối                | Hệ thống thông báo cho khách hàng và cập nhật trạng thái yêu cầu.                                      |
| **EX03** | Tài xế không phản hồi                  | Tài xế được gửi yêu cầu nhưng không phản hồi trong thời gian quy định | Hệ thống chuyển sang tìm kiếm tài xế khác.                                                             |
| **EX04** | Tài xế từ chối chuyến                  | Tài xế không chấp nhận yêu cầu                                        | Hệ thống tiếp tục tìm tài xế phù hợp khác.                                                             |
| **EX05** | Chuyến đi phát sinh sự cố              | Có vấn đề trong quá trình thực hiện chuyến                            | Hệ thống ghi nhận sự cố và chuyển cho nhân viên vận hành xử lý.                                        |
| **EX06** | Thanh toán điện tử thất bại            | Nhà cung cấp thanh toán trả về kết quả thất bại                       | Hệ thống thông báo cho khách hàng và cho phép thanh toán lại hoặc đổi phương thức.                     |
| **EX07** | Nhà cung cấp thanh toán không phản hồi | Không nhận được kết quả từ dịch vụ thanh toán                         | Hệ thống ghi nhận giao dịch chưa hoàn tất và xử lý theo cơ chế kiểm tra lại.                           |
| **EX08** | Gửi thông báo thất bại                 | Kênh thông báo không thể gửi thông báo                                | Hệ thống ghi nhận lỗi và thực hiện gửi lại theo cấu hình.                                              |
| **EX09** | Người dùng không có quyền              | Người dùng truy cập chức năng không thuộc quyền được cấp              | Hệ thống từ chối truy cập và ghi nhận sự kiện nếu cần.                                                 |
| **EX10** | Phương tiện không hợp lệ               | Phương tiện không ở trạng thái được phép hoạt động                    | Hệ thống không cho phép phương tiện được sử dụng cho chuyến đi.                                        |
| **EX11** | Không thể cập nhật vị trí              | Hệ thống không nhận được thông tin vị trí của tài xế                  | Hệ thống ghi nhận lỗi và thông báo cho bên liên quan hoặc nhân viên vận hành.                          |
| **EX12** | Dữ liệu hệ thống không khả dụng        | Một thành phần xử lý dữ liệu gặp lỗi                                  | Hệ thống thông báo lỗi, hạn chế ảnh hưởng đến các chức năng khác và thực hiện cơ chế phục hồi phù hợp. |

---

## 9.3. Mối quan hệ giữa Business Rules và Business Requirements

| Business Requirement                                | Business Rules liên quan                                           |
| --------------------------------------------------- | ------------------------------------------------------------------ |
| **BG01 – Quản lý và đặt xe**                        | BR01, BR02, BR04, BR08                                             |
| **BG02 – Quản lý và phân công tài xế**              | BR03, BR05                                                         |
| **BG03 – Quản lý chuyến đi và vận hành**            | BR04, BR05, BR10                                                   |
| **BG04 – Quản lý cước phí và thanh toán**           | BR06, BR07                                                         |
| **BG05 – Quản lý thông báo**                        | BR09                                                               |
| **BG06 – Đảm bảo tính ổn định và khả năng mở rộng** | BR09, BR12 và các cơ chế xử lý EX05, EX08, EX12                    |
| **BG07 – Đảm bảo an toàn và bảo mật**               | BR01, BR10, BR12                                                   |
| **BG08 – Báo cáo và đánh giá hiệu quả kinh doanh**  | BR11                                                               |
| **BG09 – Hỗ trợ mở rộng trong tương lai**           | Các quy tắc nghiệp vụ được thiết kế độc lập và có khả năng mở rộng |

# 10. Non-Functional Requirements

Các yêu cầu phi chức năng xác định các tiêu chí về chất lượng, hiệu năng, bảo mật, khả năng mở rộng và độ ổn định mà hệ thống phải đáp ứng trong quá trình vận hành.

## 10.1. Hiệu năng (Performance)

| Mã NFR    | Yêu cầu                                                                                                                                 |
| --------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| **NFR01** | Hệ thống phải phản hồi các thao tác thông thường của người dùng trong thời gian phù hợp với điều kiện vận hành.                         |
| **NFR02** | Hệ thống phải có khả năng xử lý đồng thời nhiều yêu cầu đặt xe trong thời gian cao điểm.                                                |
| **NFR03** | Việc tìm kiếm và phân công tài xế phải được thực hiện tự động và trong thời gian phù hợp để không gây ảnh hưởng đến trải nghiệm đặt xe. |
| **NFR04** | Thời gian xử lý thanh toán phải được tối ưu và không làm ảnh hưởng đến các chức năng khác của hệ thống.                                 |

## 10.2. Tính khả dụng và ổn định (Availability & Reliability)

| Mã NFR    | Yêu cầu                                                                                                        |
| --------- | -------------------------------------------------------------------------------------------------------------- |
| **NFR05** | Hệ thống phải duy trì hoạt động ổn định trong thời gian vận hành.                                              |
| **NFR06** | Khi một thành phần của hệ thống gặp lỗi, lỗi đó phải được cô lập để hạn chế ảnh hưởng đến các thành phần khác. |
| **NFR07** | Hệ thống phải có cơ chế xử lý và phục hồi phù hợp khi xảy ra lỗi trong quá trình vận hành.                     |
| **NFR08** | Dữ liệu giao dịch và chuyến đi phải được đảm bảo tính toàn vẹn, tránh mất mát hoặc ghi nhận sai trạng thái.    |

## 10.3. Bảo mật (Security)

| Mã NFR    | Yêu cầu                                                                                                  |
| --------- | -------------------------------------------------------------------------------------------------------- |
| **NFR09** | Hệ thống phải xác thực người dùng trước khi cho phép truy cập các chức năng yêu cầu đăng nhập.           |
| **NFR10** | Hệ thống phải áp dụng cơ chế phân quyền dựa trên vai trò của người dùng.                                 |
| **NFR11** | Thông tin cá nhân của khách hàng và tài xế phải được bảo vệ khỏi truy cập trái phép.                     |
| **NFR12** | Thông tin phương tiện, vị trí và giao dịch phải được bảo vệ trong quá trình lưu trữ và trao đổi dữ liệu. |
| **NFR13** | Hệ thống phải ghi nhận nhật ký đối với các thao tác quan trọng để phục vụ kiểm tra và truy vết.          |

## 10.4. Khả năng mở rộng (Scalability)

| Mã NFR    | Yêu cầu                                                                                                          |
| --------- | ---------------------------------------------------------------------------------------------------------------- |
| **NFR14** | Hệ thống phải có khả năng mở rộng để đáp ứng số lượng người dùng và yêu cầu đặt xe tăng lên.                     |
| **NFR15** | Các thành phần của hệ thống phải có khả năng mở rộng hoặc triển khai độc lập khi cần thiết.                      |
| **NFR16** | Việc bổ sung loại hình dịch vụ mới không được yêu cầu xây dựng lại toàn bộ hệ thống.                             |
| **NFR17** | Hệ thống phải cho phép tích hợp thêm phương thức thanh toán hoặc nhà cung cấp dịch vụ bên ngoài trong tương lai. |

## 10.5. Khả năng bảo trì (Maintainability)

| Mã NFR    | Yêu cầu                                                                                                     |
| --------- | ----------------------------------------------------------------------------------------------------------- |
| **NFR18** | Hệ thống phải được thiết kế theo các thành phần có trách nhiệm rõ ràng để thuận tiện cho việc bảo trì.      |
| **NFR19** | Việc thay đổi hoặc nâng cấp một thành phần không nên gây ảnh hưởng không cần thiết đến các thành phần khác. |
| **NFR20** | Hệ thống phải cung cấp nhật ký và thông tin lỗi cần thiết để hỗ trợ việc phát hiện và xử lý sự cố.          |

## 10.6. Khả năng sử dụng (Usability)

| Mã NFR    | Yêu cầu                                                                                                       |
| --------- | ------------------------------------------------------------------------------------------------------------- |
| **NFR21** | Giao diện phải rõ ràng và dễ sử dụng đối với khách hàng, tài xế và nhân viên vận hành.                        |
| **NFR22** | Các thông tin quan trọng như trạng thái chuyến đi, cước phí và kết quả thanh toán phải được hiển thị rõ ràng. |
| **NFR23** | Hệ thống phải cung cấp thông báo và hướng dẫn phù hợp khi người dùng thực hiện thao tác không hợp lệ.         |

---

# 11. Entity Identification and ERD

## 11.1. Xác định các thực thể

Dựa trên các Business Process, Business Rules và System Requirements đã xác định, hệ thống cần quản lý các thực thể dữ liệu chính sau:

| Mã      | Thực thể                            | Mô tả                                                                        |
| ------- | ----------------------------------- | ---------------------------------------------------------------------------- |
| **E01** | **Khách hàng (Customer)**           | Lưu thông tin khách hàng sử dụng dịch vụ đặt xe.                             |
| **E02** | **Tài xế (Driver)**                 | Lưu thông tin tài xế và trạng thái hoạt động.                                |
| **E03** | **Nhân viên vận hành (Operator)**   | Lưu thông tin nhân viên thực hiện công tác quản lý và vận hành.              |
| **E04** | **Tài khoản (Account)**             | Lưu thông tin đăng nhập và trạng thái tài khoản người dùng.                  |
| **E05** | **Phương tiện (Vehicle)**           | Lưu thông tin phương tiện được sử dụng để thực hiện chuyến đi.               |
| **E06** | **Yêu cầu đặt xe (Booking)**        | Lưu thông tin yêu cầu đặt xe do khách hàng tạo.                              |
| **E07** | **Chuyến đi (Trip)**                | Lưu thông tin chuyến đi được thực hiện sau khi yêu cầu đặt xe được xác nhận. |
| **E08** | **Cước phí (Fare)**                 | Lưu thông tin cước phí dự kiến và cước phí cuối cùng của chuyến đi.          |
| **E09** | **Thanh toán (Payment)**            | Lưu thông tin giao dịch và trạng thái thanh toán.                            |
| **E10** | **Đánh giá (Review)**               | Lưu đánh giá của khách hàng đối với chuyến đi và tài xế.                     |
| **E11** | **Thông báo (Notification)**        | Lưu thông tin các thông báo được gửi đến người dùng.                         |
| **E12** | **Sự cố (Incident)**                | Lưu thông tin các trường hợp phát sinh trong quá trình thực hiện chuyến đi.  |
| **E13** | **Nhật ký hoạt động (ActivityLog)** | Lưu vết các thao tác quan trọng của người dùng và nhân viên.                 |

---

## 11.2. Các thuộc tính chính của thực thể

### 11.2.1. Customer

* `CustomerID` – Khóa chính
* `FullName`
* `Phone`
* `Email`
* `Address`
* `CreatedAt`
* `Status`

### 11.2.2. Driver

* `DriverID` – Khóa chính
* `FullName`
* `Phone`
* `Email`
* `LicenseNumber`
* `Status`
* `Rating`

### 11.2.3. Operator

* `OperatorID` – Khóa chính
* `FullName`
* `Phone`
* `Email`
* `Status`

### 11.2.4. Account

* `AccountID` – Khóa chính
* `Username`
* `PasswordHash`
* `Role`
* `Status`
* `CreatedAt`

### 11.2.5. Vehicle

* `VehicleID` – Khóa chính
* `LicensePlate`
* `VehicleType`
* `Brand`
* `Model`
* `Status`
* `DriverID` – Khóa ngoại

### 11.2.6. Booking

* `BookingID` – Khóa chính
* `CustomerID` – Khóa ngoại
* `PickupLocation`
* `Destination`
* `BookingTime`
* `Status`
* `EstimatedFare`
* `PreferredPaymentMethod`

### 11.2.7. Trip

* `TripID` – Khóa chính
* `BookingID` – Khóa ngoại
* `DriverID` – Khóa ngoại
* `VehicleID` – Khóa ngoại
* `StartTime`
* `EndTime`
* `Status`
* `ActualPickupLocation`
* `ActualDestination`

### 11.2.8. Fare

* `FareID` – Khóa chính
* `TripID` – Khóa ngoại
* `EstimatedAmount`
* `FinalAmount`
* `CalculatedAt`

### 11.2.9. Payment

* `PaymentID` – Khóa chính
* `TripID` – Khóa ngoại
* `PaymentMethod`
* `Amount`
* `PaymentTime`
* `Status`
* `TransactionCode`

### 11.2.10. Review

* `ReviewID` – Khóa chính
* `TripID` – Khóa ngoại
* `CustomerID` – Khóa ngoại
* `DriverID` – Khóa ngoại
* `Rating`
* `Comment`
* `CreatedAt`

### 11.2.11. Notification

* `NotificationID` – Khóa chính
* `AccountID` – Khóa ngoại
* `Type`
* `Title`
* `Content`
* `SentAt`
* `Status`

### 11.2.12. Incident

* `IncidentID` – Khóa chính
* `TripID` – Khóa ngoại
* `ReportedBy`
* `IncidentType`
* `Description`
* `ReportedAt`
* `Status`
* `ResolvedAt`
* `ResolvedBy`

### 11.2.13. ActivityLog

* `LogID` – Khóa chính
* `AccountID` – Khóa ngoại
* `Action`
* `EntityType`
* `EntityID`
* `CreatedAt`
* `IPAddress`

---

## 11.3. Mối quan hệ giữa các thực thể

| Quan hệ                | Bội số | Ý nghĩa                                                                      |
| ---------------------- | ------ | ---------------------------------------------------------------------------- |
| Customer – Booking     | 1:N    | Một khách hàng có thể tạo nhiều yêu cầu đặt xe.                              |
| Booking – Trip         | 1:0..1 | Một yêu cầu đặt xe có thể chưa có hoặc có một chuyến đi được xác nhận.       |
| Driver – Trip          | 1:N    | Một tài xế có thể thực hiện nhiều chuyến đi.                                 |
| Vehicle – Trip         | 1:N    | Một phương tiện có thể được sử dụng cho nhiều chuyến đi.                     |
| Driver – Vehicle       | 1:N    | Một tài xế có thể được gán một hoặc nhiều phương tiện theo cấu hình quản lý. |
| Trip – Fare            | 1:1    | Mỗi chuyến đi có một thông tin cước phí.                                     |
| Trip – Payment         | 1:0..1 | Một chuyến đi có thể chưa thanh toán hoặc có một giao dịch thanh toán.       |
| Trip – Review          | 1:0..1 | Một chuyến đi có thể chưa được đánh giá hoặc có một đánh giá.                |
| Customer – Review      | 1:N    | Một khách hàng có thể tạo nhiều đánh giá.                                    |
| Driver – Review        | 1:N    | Một tài xế có thể nhận nhiều đánh giá.                                       |
| Account – Notification | 1:N    | Một tài khoản có thể nhận nhiều thông báo.                                   |
| Trip – Incident        | 1:N    | Một chuyến đi có thể phát sinh nhiều sự cố.                                  |
| Account – ActivityLog  | 1:N    | Một tài khoản có thể tạo nhiều bản ghi nhật ký hoạt động.                    |

---

## 11.4. ERD tổng quát

```mermaid
erDiagram

    ACCOUNT ||--o{ NOTIFICATION : receives
    ACCOUNT ||--o{ ACTIVITY_LOG : creates

    CUSTOMER ||--o{ BOOKING : creates
    BOOKING ||--o| TRIP : generates

    DRIVER ||--o{ TRIP : performs
    VEHICLE ||--o{ TRIP : used_for
    DRIVER ||--o{ VEHICLE : assigned

    TRIP ||--|| FARE : has
    TRIP ||--o| PAYMENT : has
    TRIP ||--o| REVIEW : receives
    TRIP ||--o{ INCIDENT : has

    CUSTOMER ||--o{ REVIEW : writes
    DRIVER ||--o{ REVIEW : receives

    CUSTOMER {
        int CustomerID PK
        string FullName
        string Phone
        string Email
        string Address
        datetime CreatedAt
        string Status
    }

    DRIVER {
        int DriverID PK
        string FullName
        string Phone
        string Email
        string LicenseNumber
        string Status
        decimal Rating
    }

    OPERATOR {
        int OperatorID PK
        string FullName
        string Phone
        string Email
        string Status
    }

    ACCOUNT {
        int AccountID PK
        string Username
        string PasswordHash
        string Role
        string Status
        datetime CreatedAt
    }

    VEHICLE {
        int VehicleID PK
        string LicensePlate
        string VehicleType
        string Brand
        string Model
        string Status
        int DriverID FK
    }

    BOOKING {
        int BookingID PK
        int CustomerID FK
        string PickupLocation
        string Destination
        datetime BookingTime
        string Status
        decimal EstimatedFare
        string PreferredPaymentMethod
    }

    TRIP {
        int TripID PK
        int BookingID FK
        int DriverID FK
        int VehicleID FK
        datetime StartTime
        datetime EndTime
        string Status
        string ActualPickupLocation
        string ActualDestination
    }

    FARE {
        int FareID PK
        int TripID FK
        decimal EstimatedAmount
        decimal FinalAmount
        datetime CalculatedAt
    }

    PAYMENT {
        int PaymentID PK
        int TripID FK
        string PaymentMethod
        decimal Amount
        datetime PaymentTime
        string Status
        string TransactionCode
    }

    REVIEW {
        int ReviewID PK
        int TripID FK
        int CustomerID FK
        int DriverID FK
        int Rating
        string Comment
        datetime CreatedAt
    }

    NOTIFICATION {
        int NotificationID PK
        int AccountID FK
        string Type
        string Title
        string Content
        datetime SentAt
        string Status
    }

    INCIDENT {
        int IncidentID PK
        int TripID FK
        string ReportedBy
        string IncidentType
        string Description
        datetime ReportedAt
        string Status
        datetime ResolvedAt
        int ResolvedBy
    }

    ACTIVITY_LOG {
        int LogID PK
        int AccountID FK
        string Action
        string EntityType
        int EntityID
        datetime CreatedAt
        string IPAddress
    }
```

## 11.5. Truy xuất từ nghiệp vụ đến thực thể dữ liệu

| Business Process                           | Các thực thể chính                                           |
| ------------------------------------------ | ------------------------------------------------------------ |
| **BP01 – Đặt xe và phân công tài xế**      | Customer, Account, Booking, Driver, Vehicle, Trip            |
| **BP02 – Thực hiện và theo dõi chuyến đi** | Trip, Driver, Vehicle, Incident, Notification                |
| **BP03 – Thanh toán**                      | Trip, Fare, Payment, Notification                            |
| **BP04 – Đánh giá chuyến đi và tài xế**    | Trip, Customer, Driver, Review                               |
| **BP05 – Quản lý và vận hành**             | Customer, Driver, Vehicle, Trip, Incident, Operator, Account |
| **BP06 – Quản lý thông báo**               | Account, Notification                                        |
| **BP07 – Báo cáo và đánh giá hiệu quả**    | Trip, Fare, Payment, Driver, Review                          |
| **An toàn và bảo mật**                     | Account, ActivityLog                                         |

```
# 12. Use Case Design

## 12.1. Actors

| Actor                  | Vai trò                                                                                        |
| ---------------------- | ---------------------------------------------------------------------------------------------- |
| **Khách hàng**         | Sử dụng hệ thống để quản lý tài khoản, đặt xe, theo dõi chuyến, thanh toán và đánh giá tài xế. |
| **Tài xế**             | Nhận yêu cầu chuyến, thực hiện chuyến, cập nhật trạng thái và xử lý các trường hợp phát sinh.  |
| **Nhân viên vận hành** | Theo dõi và quản lý khách hàng, tài xế, phương tiện và các chuyến đang diễn ra.                |
| **Quản trị viên**      | Quản lý tài khoản, phân quyền và theo dõi hoạt động quản trị hệ thống.                         |
| **Cổng thanh toán**    | Hệ thống bên ngoài thực hiện và trả kết quả giao dịch thanh toán điện tử.                      |

---

## 12.2. Danh sách Use Case

### Nhóm 1 – Quản lý tài khoản

| Mã       | Use Case                  |
| -------- | ------------------------- |
| **UC01** | Đăng ký tài khoản         |
| **UC02** | Đăng nhập                 |
| **UC03** | Quản lý thông tin cá nhân |

### Nhóm 2 – Đặt xe

| Mã       | Use Case              |
| -------- | --------------------- |
| **UC04** | Đặt xe                |
| **UC05** | Hủy yêu cầu đặt xe    |
| **UC06** | Xem lịch sử chuyến đi |

### Nhóm 3 – Phân công và thực hiện chuyến

| Mã       | Use Case                   |
| -------- | -------------------------- |
| **UC07** | Phân công tài xế           |
| **UC08** | Tiếp nhận yêu cầu chuyến   |
| **UC09** | Theo dõi chuyến đi         |
| **UC10** | Thực hiện chuyến đi        |
| **UC11** | Xử lý trường hợp phát sinh |

### Nhóm 4 – Thanh toán

| Mã       | Use Case                  |
| -------- | ------------------------- |
| **UC12** | Tính cước chuyến đi       |
| **UC13** | Thanh toán                |
| **UC14** | Xử lý thanh toán thất bại |

### Nhóm 5 – Đánh giá và thông báo

| Mã       | Use Case           |
| -------- | ------------------ |
| **UC15** | Đánh giá chuyến đi |
| **UC16** | Gửi thông báo      |

### Nhóm 6 – Quản lý vận hành

| Mã       | Use Case                     |
| -------- | ---------------------------- |
| **UC17** | Quản lý khách hàng           |
| **UC18** | Quản lý tài xế               |
| **UC19** | Quản lý phương tiện          |
| **UC20** | Theo dõi chuyến đang diễn ra |
| **UC21** | Xử lý sự cố                  |

### Nhóm 7 – Báo cáo và quản trị

| Mã       | Use Case                        |
| -------- | ------------------------------- |
| **UC22** | Xem báo cáo                     |
| **UC23** | Quản lý tài khoản và phân quyền |
| **UC24** | Xem nhật ký hoạt động           |

---

## 12.3. Quan hệ giữa các Use Case

### Quan hệ `<<include>>`

* **UC04 Đặt xe**

  * `<<include>>` UC02 Đăng nhập
  * `<<include>>` UC12 Tính cước chuyến đi
  * `<<include>>` UC07 Phân công tài xế

* **UC10 Thực hiện chuyến đi**

  * `<<include>>` UC09 Theo dõi chuyến đi

* **UC13 Thanh toán**

  * `<<include>>` UC12 Tính cước chuyến đi

* **UC15 Đánh giá chuyến đi**

  * `<<include>>` UC02 Đăng nhập

* **UC17–UC21**

  * `<<include>>` UC02 Đăng nhập

### Quan hệ `<<extend>>`

* **UC14 Xử lý thanh toán thất bại**

  * `<<extend>>` UC13 Thanh toán

* **UC11 Xử lý trường hợp phát sinh**

  * `<<extend>>` UC10 Thực hiện chuyến đi

* **UC05 Hủy yêu cầu đặt xe**

  * `<<extend>>` UC04 Đặt xe

* **UC16 Gửi thông báo**

  * được kích hoạt khi xảy ra các sự kiện liên quan đến đặt xe, phân công, chuyến đi hoặc thanh toán.

---

## 12.4. Use Case Diagram

```mermaid
flowchart LR

    KH["👤 Khách hàng"]
    TX["👤 Tài xế"]
    NV["👤 Nhân viên vận hành"]
    QTV["👤 Quản trị viên"]
    PAY["💳 Cổng thanh toán"]

    subgraph SYS["HỆ THỐNG QUẢN LÝ VÀ ĐẶT XE"]

        UC01(("UC01\nĐăng ký tài khoản"))
        UC02(("UC02\nĐăng nhập"))
        UC03(("UC03\nQuản lý thông tin cá nhân"))

        UC04(("UC04\nĐặt xe"))
        UC05(("UC05\nHủy yêu cầu đặt xe"))
        UC06(("UC06\nXem lịch sử chuyến đi"))

        UC07(("UC07\nPhân công tài xế"))
        UC08(("UC08\nTiếp nhận yêu cầu chuyến"))
        UC09(("UC09\nTheo dõi chuyến đi"))
        UC10(("UC10\nThực hiện chuyến đi"))
        UC11(("UC11\nXử lý trường hợp phát sinh"))

        UC12(("UC12\nTính cước chuyến đi"))
        UC13(("UC13\nThanh toán"))
        UC14(("UC14\nXử lý thanh toán thất bại"))

        UC15(("UC15\nĐánh giá chuyến đi"))
        UC16(("UC16\nGửi thông báo"))

        UC17(("UC17\nQuản lý khách hàng"))
        UC18(("UC18\nQuản lý tài xế"))
        UC19(("UC19\nQuản lý phương tiện"))
        UC20(("UC20\nTheo dõi chuyến đang diễn ra"))
        UC21(("UC21\nXử lý sự cố"))

        UC22(("UC22\nXem báo cáo"))
        UC23(("UC23\nQuản lý tài khoản\nvà phân quyền"))
        UC24(("UC24\nXem nhật ký hoạt động"))
    end

    KH --- UC01
    KH --- UC02
    KH --- UC03
    KH --- UC04
    KH --- UC05
    KH --- UC06
    KH --- UC09
    KH --- UC13
    KH --- UC15

    TX --- UC02
    TX --- UC08
    TX --- UC09
    TX --- UC10
    TX --- UC11
    TX --- UC16

    NV --- UC02
    NV --- UC17
    NV --- UC18
    NV --- UC19
    NV --- UC20
    NV --- UC21
    NV --- UC22

    QTV --- UC02
    QTV --- UC23
    QTV --- UC24
    QTV --- UC22

    PAY --- UC13

    UC04 -. "«include»" .-> UC02
    UC04 -. "«include»" .-> UC12
    UC04 -. "«include»" .-> UC07

    UC05 -. "«extend»" .-> UC04

    UC10 -. "«include»" .-> UC09
    UC11 -. "«extend»" .-> UC10

    UC13 -. "«include»" .-> UC12
    UC14 -. "«extend»" .-> UC13

    UC15 -. "«include»" .-> UC02
```

---

## 12.5. Phân rã Use Case theo Actor

### Khách hàng

* UC01 – Đăng ký tài khoản
* UC02 – Đăng nhập
* UC03 – Quản lý thông tin cá nhân
* UC04 – Đặt xe
* UC05 – Hủy yêu cầu đặt xe
* UC06 – Xem lịch sử chuyến đi
* UC09 – Theo dõi chuyến đi
* UC13 – Thanh toán
* UC15 – Đánh giá chuyến đi

### Tài xế

* UC02 – Đăng nhập
* UC08 – Tiếp nhận yêu cầu chuyến
* UC09 – Theo dõi chuyến đi
* UC10 – Thực hiện chuyến đi
* UC11 – Xử lý trường hợp phát sinh
* UC16 – Gửi thông báo

### Nhân viên vận hành

* UC02 – Đăng nhập
* UC17 – Quản lý khách hàng
* UC18 – Quản lý tài xế
* UC19 – Quản lý phương tiện
* UC20 – Theo dõi chuyến đang diễn ra
* UC21 – Xử lý sự cố
* UC22 – Xem báo cáo

### Quản trị viên

* UC02 – Đăng nhập
* UC22 – Xem báo cáo
* UC23 – Quản lý tài khoản và phân quyền
* UC24 – Xem nhật ký hoạt động

### Cổng thanh toán

* UC13 – Thanh toán

# 13. Acceptance Criteria

Acceptance Criteria (AC) là các tiêu chí nghiệm thu được sử dụng để xác định một chức năng đã được triển khai hoàn chỉnh và đáp ứng đúng yêu cầu nghiệp vụ hay chưa.

Một chức năng được xem là **đạt** khi tất cả các Acceptance Criteria tương ứng đều được đáp ứng.

## 13.1. Acceptance Criteria cho quản lý tài khoản

| Mã AC    | Use Case                         | SR liên quan | Acceptance Criteria                                                                       |
| -------- | -------------------------------- | ------------ | ----------------------------------------------------------------------------------------- |
| **AC01** | UC01 – Đăng ký tài khoản         | SR01         | Người dùng có thể đăng ký tài khoản khi cung cấp đầy đủ thông tin hợp lệ.                 |
| **AC02** | UC01 – Đăng ký tài khoản         | SR01         | Hệ thống không cho phép đăng ký khi thông tin bắt buộc bị thiếu hoặc không hợp lệ.        |
| **AC03** | UC01 – Đăng ký tài khoản         | SR01         | Hệ thống không cho phép tạo tài khoản trùng thông tin định danh đã tồn tại theo quy định. |
| **AC04** | UC02 – Đăng nhập                 | SR02         | Người dùng đăng nhập thành công khi cung cấp thông tin xác thực hợp lệ.                   |
| **AC05** | UC02 – Đăng nhập                 | SR02         | Hệ thống từ chối đăng nhập khi thông tin xác thực không hợp lệ.                           |
| **AC06** | UC03 – Quản lý thông tin cá nhân | SR03         | Người dùng có thể xem thông tin cá nhân của tài khoản.                                    |
| **AC07** | UC03 – Quản lý thông tin cá nhân | SR03         | Người dùng có thể cập nhật thông tin khi dữ liệu mới hợp lệ.                              |
| **AC08** | UC03 – Quản lý thông tin cá nhân | SR03         | Hệ thống không lưu thông tin khi dữ liệu cập nhật không hợp lệ.                           |

---

## 13.2. Acceptance Criteria cho đặt xe

| Mã AC    | Use Case                     | SR liên quan | Acceptance Criteria                                                                     |
| -------- | ---------------------------- | ------------ | --------------------------------------------------------------------------------------- |
| **AC09** | UC04 – Đặt xe                | SR04, SR05   | Khách hàng có thể tạo yêu cầu đặt xe khi cung cấp đầy đủ thông tin hợp lệ.              |
| **AC10** | UC04 – Đặt xe                | SR05         | Hệ thống từ chối yêu cầu khi điểm đón hoặc điểm đến không hợp lệ.                       |
| **AC11** | UC04 – Đặt xe                | SR06         | Hệ thống tính và hiển thị cước phí dự kiến trước khi khách hàng xác nhận đặt xe.        |
| **AC12** | UC04 – Đặt xe                | SR07         | Sau khi tạo yêu cầu, hệ thống ghi nhận yêu cầu với trạng thái phù hợp.                  |
| **AC13** | UC05 – Hủy yêu cầu đặt xe    | SR07         | Khách hàng có thể hủy yêu cầu khi yêu cầu đang ở trạng thái được phép hủy.              |
| **AC14** | UC05 – Hủy yêu cầu đặt xe    | SR07         | Hệ thống không cho phép hủy yêu cầu khi trạng thái chuyến không còn cho phép hủy.       |
| **AC15** | UC06 – Xem lịch sử chuyến đi | SR08         | Khách hàng có thể xem danh sách các chuyến đi thuộc tài khoản của mình.                 |
| **AC16** | UC06 – Xem lịch sử chuyến đi | SR08         | Thông tin lịch sử phải thể hiện tối thiểu trạng thái, thời gian và thông tin chuyến đi. |

---

## 13.3. Acceptance Criteria cho phân công tài xế

| Mã AC    | Use Case                        | SR liên quan | Acceptance Criteria                                                                             |
| -------- | ------------------------------- | ------------ | ----------------------------------------------------------------------------------------------- |
| **AC17** | UC07 – Phân công tài xế         | SR11, SR12   | Hệ thống có thể tìm kiếm và lựa chọn tài xế đáp ứng điều kiện phân công.                        |
| **AC18** | UC07 – Phân công tài xế         | SR12         | Hệ thống gửi yêu cầu nhận chuyến đến tài xế được lựa chọn.                                      |
| **AC19** | UC07 – Phân công tài xế         | SR14         | Khi tài xế từ chối hoặc không phản hồi, hệ thống có thể tiếp tục tìm tài xế khác.               |
| **AC20** | UC07 – Phân công tài xế         | SR14         | Khi không còn tài xế phù hợp, hệ thống thông báo cho khách hàng và cập nhật trạng thái yêu cầu. |
| **AC21** | UC08 – Tiếp nhận yêu cầu chuyến | SR13         | Tài xế có thể xem thông tin yêu cầu được phân công.                                             |
| **AC22** | UC08 – Tiếp nhận yêu cầu chuyến | SR13         | Tài xế có thể chấp nhận hoặc từ chối yêu cầu.                                                   |
| **AC23** | UC08 – Tiếp nhận yêu cầu chuyến | SR13         | Khi tài xế chấp nhận, hệ thống cập nhật tài xế được phân công cho chuyến.                       |

---

## 13.4. Acceptance Criteria cho thực hiện và theo dõi chuyến đi

| Mã AC    | Use Case                          | SR liên quan | Acceptance Criteria                                                                                   |
| -------- | --------------------------------- | ------------ | ----------------------------------------------------------------------------------------------------- |
| **AC24** | UC09 – Theo dõi chuyến đi         | SR17, SR18   | Khách hàng có thể xem trạng thái hiện tại của chuyến đi.                                              |
| **AC25** | UC09 – Theo dõi chuyến đi         | SR18         | Hệ thống cập nhật thông tin vị trí của tài xế trong quá trình thực hiện chuyến khi có dữ liệu hợp lệ. |
| **AC26** | UC10 – Thực hiện chuyến đi        | SR19         | Tài xế chỉ có thể bắt đầu chuyến khi đã được phân công cho chuyến đó.                                 |
| **AC27** | UC10 – Thực hiện chuyến đi        | SR19         | Khi tài xế bắt đầu chuyến, trạng thái chuyến được cập nhật tương ứng.                                 |
| **AC28** | UC10 – Thực hiện chuyến đi        | SR20         | Tài xế có thể xác nhận kết thúc chuyến khi đáp ứng điều kiện hoàn thành.                              |
| **AC29** | UC10 – Thực hiện chuyến đi        | SR20         | Khi kết thúc chuyến, hệ thống cập nhật chuyến sang trạng thái hoàn thành.                             |
| **AC30** | UC11 – Xử lý trường hợp phát sinh | SR21         | Người dùng hoặc tài xế có thể ghi nhận trường hợp phát sinh trong chuyến đi.                          |
| **AC31** | UC11 – Xử lý trường hợp phát sinh | SR21         | Nhân viên vận hành có thể tiếp nhận và cập nhật kết quả xử lý trường hợp phát sinh.                   |

---

## 13.5. Acceptance Criteria cho thanh toán

| Mã AC    | Use Case                         | SR liên quan | Acceptance Criteria                                                                   |
| -------- | -------------------------------- | ------------ | ------------------------------------------------------------------------------------- |
| **AC32** | UC12 – Tính cước chuyến đi       | SR25         | Hệ thống có thể xác định cước phí cuối cùng sau khi chuyến đi hoàn thành.             |
| **AC33** | UC12 – Tính cước chuyến đi       | SR25         | Cước phí cuối cùng được lưu và liên kết với chuyến đi tương ứng.                      |
| **AC34** | UC13 – Thanh toán                | SR26         | Khách hàng có thể thanh toán bằng tiền mặt theo quy trình nghiệp vụ.                  |
| **AC35** | UC13 – Thanh toán                | SR27         | Khách hàng có thể thực hiện thanh toán điện tử thông qua cổng thanh toán được hỗ trợ. |
| **AC36** | UC13 – Thanh toán                | SR28         | Khi giao dịch thành công, hệ thống cập nhật trạng thái thanh toán thành công.         |
| **AC37** | UC13 – Thanh toán                | SR28         | Khi giao dịch chưa có kết quả, hệ thống không được ghi nhận là thanh toán thành công. |
| **AC38** | UC14 – Xử lý thanh toán thất bại | SR29         | Khi thanh toán thất bại, hệ thống thông báo kết quả cho khách hàng.                   |
| **AC39** | UC14 – Xử lý thanh toán thất bại | SR29         | Khách hàng có thể thực hiện lại thanh toán hoặc lựa chọn phương thức thanh toán khác. |

---

## 13.6. Acceptance Criteria cho đánh giá và thông báo

| Mã AC    | Use Case                  | SR liên quan           | Acceptance Criteria                                                                  |
| -------- | ------------------------- | ---------------------- | ------------------------------------------------------------------------------------ |
| **AC40** | UC15 – Đánh giá chuyến đi | SR36, SR37             | Khách hàng có thể đánh giá sau khi chuyến đi hoàn thành.                             |
| **AC41** | UC15 – Đánh giá chuyến đi | SR36, SR37             | Hệ thống không cho phép đánh giá đối với chuyến chưa hoàn thành.                     |
| **AC42** | UC15 – Đánh giá chuyến đi | SR38                   | Đánh giá được lưu và liên kết với chuyến đi, khách hàng và tài xế tương ứng.         |
| **AC43** | UC16 – Gửi thông báo      | SR31, SR32, SR33, SR34 | Hệ thống gửi thông báo đến đúng đối tượng khi phát sinh sự kiện nghiệp vụ tương ứng. |
| **AC44** | UC16 – Gửi thông báo      | SR35                   | Hệ thống ghi nhận trạng thái gửi thông báo.                                          |
| **AC45** | UC16 – Gửi thông báo      | SR35                   | Khi gửi thất bại, hệ thống ghi nhận lỗi và xử lý gửi lại theo quy định.              |

---

## 13.7. Acceptance Criteria cho quản lý vận hành

| Mã AC    | Use Case                            | SR liên quan | Acceptance Criteria                                                                |
| -------- | ----------------------------------- | ------------ | ---------------------------------------------------------------------------------- |
| **AC46** | UC17 – Quản lý khách hàng           | SR39         | Nhân viên vận hành có thể xem và quản lý thông tin khách hàng theo quyền được cấp. |
| **AC47** | UC18 – Quản lý tài xế               | SR09, SR40   | Nhân viên vận hành có thể xem và quản lý thông tin tài xế.                         |
| **AC48** | UC18 – Quản lý tài xế               | SR10         | Hệ thống thể hiện được trạng thái hoạt động hiện tại của tài xế.                   |
| **AC49** | UC19 – Quản lý phương tiện          | SR22, SR23   | Nhân viên vận hành có thể quản lý thông tin và trạng thái phương tiện.             |
| **AC50** | UC19 – Quản lý phương tiện          | SR24         | Hệ thống quản lý được thông tin phương tiện được gán cho tài xế.                   |
| **AC51** | UC20 – Theo dõi chuyến đang diễn ra | SR41         | Nhân viên vận hành có thể xem danh sách và trạng thái các chuyến đang diễn ra.     |
| **AC52** | UC21 – Xử lý sự cố                  | SR42         | Nhân viên vận hành có thể tiếp nhận, cập nhật và hoàn tất xử lý sự cố.             |

---

## 13.8. Acceptance Criteria cho báo cáo và quản trị

| Mã AC    | Use Case                               | SR liên quan | Acceptance Criteria                                                                |
| -------- | -------------------------------------- | ------------ | ---------------------------------------------------------------------------------- |
| **AC53** | UC22 – Xem báo cáo                     | SR44         | Người có quyền có thể xem báo cáo số lượng chuyến theo khoảng thời gian được chọn. |
| **AC54** | UC22 – Xem báo cáo                     | SR45         | Người có quyền có thể xem báo cáo doanh thu.                                       |
| **AC55** | UC22 – Xem báo cáo                     | SR46, SR47   | Hệ thống cung cấp tỷ lệ hoàn thành và tỷ lệ hủy chuyến dựa trên dữ liệu nghiệp vụ. |
| **AC56** | UC22 – Xem báo cáo                     | SR48         | Hệ thống cung cấp các chỉ số phục vụ đánh giá hiệu quả tài xế.                     |
| **AC57** | UC23 – Quản lý tài khoản và phân quyền | SR43, SR49   | Quản trị viên có thể quản lý tài khoản và quyền truy cập của người dùng.           |
| **AC58** | UC23 – Quản lý tài khoản và phân quyền | SR49         | Người dùng không thể truy cập chức năng ngoài quyền được cấp.                      |
| **AC59** | UC24 – Xem nhật ký hoạt động           | SR51         | Hệ thống ghi nhận các thao tác quan trọng kèm thông tin cần thiết để truy vết.     |
| **AC60** | UC24 – Xem nhật ký hoạt động           | SR51         | Quản trị viên có quyền có thể xem và tra cứu nhật ký hoạt động.                    |

---

## 13.9. Acceptance Criteria cho yêu cầu phi chức năng

Ngoài các tiêu chí nghiệm thu chức năng, hệ thống phải đáp ứng các tiêu chí chất lượng sau:

| Mã AC    | NFR liên quan | Acceptance Criteria                                                                                                         |
| -------- | ------------- | --------------------------------------------------------------------------------------------------------------------------- |
| **AC61** | NFR01–NFR04   | Các chức năng chính phải đáp ứng mức thời gian phản hồi được quy định trong đặc tả hệ thống.                                |
| **AC62** | NFR05–NFR08   | Hệ thống phải duy trì hoạt động ổn định và đảm bảo tính toàn vẹn dữ liệu khi xảy ra lỗi.                                    |
| **AC63** | NFR09–NFR13   | Người dùng chỉ có thể truy cập dữ liệu và chức năng phù hợp với quyền được cấp; các thao tác quan trọng phải được ghi nhận. |
| **AC64** | NFR14–NFR17   | Hệ thống có khả năng mở rộng người dùng, dịch vụ và phương thức thanh toán mà không phải xây dựng lại toàn bộ hệ thống.     |
| **AC65** | NFR18–NFR20   | Các thành phần hệ thống có thể được bảo trì, thay đổi và kiểm tra mà hạn chế ảnh hưởng đến các thành phần khác.             |
| **AC66** | NFR21–NFR23   | Giao diện và thông báo phải rõ ràng, dễ sử dụng và hỗ trợ người dùng xử lý các thao tác không hợp lệ.                       |

---

## 13.10. Ma trận truy xuất SR – AC

| SR            | Acceptance Criteria                                                 |
| ------------- | ------------------------------------------------------------------- |
| **SR01**      | AC01, AC02, AC03                                                    |
| **SR02**      | AC04, AC05                                                          |
| **SR03**      | AC06, AC07, AC08                                                    |
| **SR04**      | AC09                                                                |
| **SR05**      | AC09, AC10                                                          |
| **SR06**      | AC11                                                                |
| **SR07**      | AC12, AC13, AC14                                                    |
| **SR08**      | AC15, AC16                                                          |
| **SR09**      | AC47                                                                |
| **SR10**      | AC48                                                                |
| **SR11**      | AC17                                                                |
| **SR12**      | AC17, AC18                                                          |
| **SR13**      | AC21, AC22, AC23                                                    |
| **SR14**      | AC19, AC20                                                          |
| **SR15**      | AC23                                                                |
| **SR16**      | AC27, AC29                                                          |
| **SR17**      | AC24                                                                |
| **SR18**      | AC25                                                                |
| **SR19**      | AC26, AC27                                                          |
| **SR20**      | AC28, AC29                                                          |
| **SR21**      | AC30, AC31                                                          |
| **SR22**      | AC49                                                                |
| **SR23**      | AC49                                                                |
| **SR24**      | AC50                                                                |
| **SR25**      | AC32, AC33                                                          |
| **SR26**      | AC34                                                                |
| **SR27**      | AC35                                                                |
| **SR28**      | AC36, AC37                                                          |
| **SR29**      | AC38, AC39                                                          |
| **SR30**      | *(cần bổ sung Use Case xem thông tin thanh toán nếu nhóm giữ SR30)* |
| **SR31–SR35** | AC43–AC45                                                           |
| **SR36–SR38** | AC40–AC42                                                           |
| **SR39**      | AC46                                                                |
| **SR40**      | AC47, AC48                                                          |
| **SR41**      | AC51                                                                |
| **SR42**      | AC52                                                                |
| **SR43**      | AC57                                                                |
| **SR44–SR48** | AC53–AC56                                                           |
| **SR49**      | AC57, AC58                                                          |
| **SR50**      | AC62, AC63                                                          |
| **SR51**      | AC59, AC60                                                          |
