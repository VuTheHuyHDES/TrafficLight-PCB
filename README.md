# Smart Traffic Light System (STLS) – Modular PCB Design

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live%20Demo-brightgreen?style=for-the-badge&logo=github)](https://VuTheHuyHDES.github.io/TrafficLight-PCB/)
[![Altium 365](https://img.shields.io/badge/Altium%20365-Interactive%203D-blue?style=for-the-badge&logo=altium)](https://365.altium.com/)
[![Embedded System](https://img.shields.io/badge/Hardware-Modular-cyan?style=for-the-badge&logo=microchip)](https://365.altium.com/)

Dự án thiết kế phần cứng cho **Hệ thống Đèn giao thông thông minh (Smart Traffic Light System - STLS)** phục vụ điều phối giao thông đô thị thời gian thực. Hệ thống được thiết kế theo cấu trúc modular gồm 7 bo mạch PCB riêng biệt, tối ưu hóa theo các tiêu chuẩn công nghiệp (DFM/DFA/DFT).

---

## 🚀 Các bo mạch thành phần trong hệ thống

### 1. STLS Master Controller (Bo mạch điều khiển trung tâm)
*   **Chức năng**: Bộ não của hệ thống, lập trình thời gian chu kỳ đèn, thu thập dữ liệu cảm biến và giao tiếp điều khiển không dây ghi đè khẩn cấp.
*   **Xem mạch 3D**: [Altium 365 Viewer - Master Controller](https://365.altium.com/files/653198E5-79FD-4426-84B0-B41E053BF8AF)

### 2. STLS Power Distribution & Charging (Bo mạch quản lý nguồn & sạc)
*   **Chức năng**: Quản lý và phân phối nguồn điện ổn định từ lưới điện AC hoặc hệ thống pin năng lượng mặt trời dự phòng (UPS).
*   **Xem mạch 3D**: [Altium 365 Viewer - Power Board](https://365.altium.com/files/1436E06B-F6CC-4C17-849A-14EEDF96343A)

### 3. STLS Light Driver Board (Bo mạch điều khiển đèn LED)
*   **Chức năng**: Sử dụng các IC điều khiển dòng không đổi (Constant Current LED Driver) để đảm bảo độ sáng đồng đều của hệ thống đèn LED Đỏ-Vàng-Xanh công suất lớn.
*   **Xem mạch 3D**: [Altium 365 Viewer - Light Driver Board](https://365.altium.com/files/5CA444A1-6D06-4D42-AD1B-D9A25DB2741F)

### 4. STLS Sensor Interface Gateway (Bo mạch giao tiếp cảm biến)
*   **Chức năng**: Giao tiếp cảm biến vòng từ dò xe (loop detector), cảm biến radar đo tốc độ, và cảm biến microwave phát hiện vật cản.
*   **Xem mạch 3D**: [Altium 365 Viewer - Sensor Node](https://365.altium.com/files/C8D35E16-98AD-496C-89E0-EC4160A98B60)

### 5. STLS Pedestrian Console (Giao diện người đi bộ qua đường)
*   **Chức năng**: Nút bấm yêu cầu qua đường của người đi bộ tích hợp màn hình hiển thị OLED, còi cảnh báo và âm thanh hướng dẫn.
*   **Xem mạch 3D**: [Altium 365 Viewer - Pedestrian Console](https://365.altium.com/files/3410839A-B567-4C9B-BBD0-DC1A358AC494)

### 6. STLS Wireless V2X Gateway (Bo mạch giao tiếp không dây V2X)
*   **Chức năng**: Bo mạch tích hợp module 4G/LTE và LoRa WAN truyền dữ liệu về Cloud thông minh của thành phố và đồng bộ hóa pha đèn.
*   **Xem mạch 3D**: [Altium 365 Viewer - V2X Gateway](https://365.altium.com/files/26EAEF4B-C7EA-430A-A702-1F8874A07770)

### 7. STLS Emergency Override Module (Bộ nhận tín hiệu ưu tiên khẩn cấp)
*   **Chức năng**: Nhận tín hiệu sóng radio (RF) phát ra từ xe ưu tiên (Cứu thương, Cảnh sát, Cứu hỏa) để tự động chuyển toàn bộ pha đèn sang màu xanh giải phóng ngã tư.
*   **Xem mạch 3D**: [Altium 365 Viewer - Emergency Module](https://365.altium.com/files/112B2122-BF28-4B17-B8AC-0FC441B9653D)

---

## 🛠️ Điểm nhấn thiết kế kỹ thuật (DFM / DFA / DFT)
*   **Chống sét và nhiễu (ESD/Surge)**: Đạt tiêu chuẩn IEC 61000-4-2 với điốt TVS bảo vệ các cổng giao tiếp và các linh kiện chống sét MOV trên nguồn AC.
*   **Thiết kế dễ lắp ráp (DFA)**: Linh kiện SMT tập trung ở một mặt của PCB, sử dụng kích thước chân linh kiện tiêu chuẩn để giảm tối đa chi phí sản xuất.
*   **Thiết kế dễ kiểm thử (DFT)**: Bố trí các điểm đo (Test Points) đồng bộ trên tất cả các đường nguồn và bus tín hiệu chính để sử dụng với JIG kiểm thử tự động.

---

## 🖥️ Xem Portfolio PCB tương tác

Trang web GitHub Pages đã tích hợp trực quan cả 7 bo mạch dưới dạng 3D xoay lật trực tuyến:
👉 **[https://VuTheHuyHDES.github.io/TrafficLight-PCB/](https://VuTheHuyHDES.github.io/TrafficLight-PCB/)**

---

## 👨‍💻 Thông tin tác giả
*   **Họ và tên**: Vũ Thế Huy
*   **Chuyên ngành**: Kỹ thuật Điện tử & Tin học Công nghiệp 1, Khóa 62
*   **Đề tài**: Thiết kế phần cứng Hệ thống Đèn giao thông thông minh (STLS)
