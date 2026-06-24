# Smart Traffic Light System (STLS) – Modular PCB Design

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live%20Demo-brightgreen?style=for-the-badge&logo=github)](https://VuTheHuyHDES.github.io/TrafficLight-PCB/)
[![Altium 365](https://img.shields.io/badge/Altium%20365-Interactive%203D-blue?style=for-the-badge&logo=altium)](https://365.altium.com/)
[![Embedded System](https://img.shields.io/badge/Hardware-Modular-cyan?style=for-the-badge&logo=microchip)](https://365.altium.com/)

Dự án thiết kế phần cứng cho **Hệ thống Đèn giao thông thông minh (Smart Traffic Light System - STLS)** phục vụ điều phối giao thông đô thị thời gian thực. Hệ thống được thiết kế theo cấu trúc modular gồm 4 bo mạch PCB riêng biệt, tối ưu hóa theo các tiêu chuẩn công nghiệp (DFM/DFA/DFT).

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

### 4. STLS Sensor & Interface Node (Bo mạch giao tiếp cảm biến)
*   **Chức năng**: Giao tiếp cảm biến vòng từ dò xe (loop detector), cảm biến radar đo tốc độ, và nút bấm ưu tiên cho người đi bộ.
*   **Xem mạch 3D**: [Altium 365 Viewer - Sensor Node](https://365.altium.com/files/C8D35E16-98AD-496C-89E0-EC4160A98B60)

---

## 🛠️ Điểm nhấn thiết kế kỹ thuật (DFM / DFA / DFT)
*   **Chống sét và nhiễu (ESD/Surge)**: Đạt tiêu chuẩn IEC 61000-4-2 với điốt TVS bảo vệ các cổng giao tiếp và các linh kiện chống sét MOV trên nguồn AC.
*   **Thiết kế dễ lắp ráp (DFA)**: Linh kiện SMT tập trung ở một mặt của PCB, sử dụng kích thước chân linh kiện tiêu chuẩn để giảm tối đa chi phí sản xuất.
*   **Thiết kế dễ kiểm thử (DFT)**: Bố trí các điểm đo (Test Points) đồng bộ trên tất cả các đường nguồn và bus tín hiệu chính để sử dụng với JIG kiểm thử tự động.

---

## 🖥️ Xem Portfolio PCB tương tác

Trang web GitHub Pages đã tích hợp trực quan cả 4 bo mạch dưới dạng 3D xoay lật trực tuyến:
👉 **[https://VuTheHuyHDES.github.io/TrafficLight-PCB/](https://VuTheHuyHDES.github.io/TrafficLight-PCB/)**

---

## 👨‍💻 Thông tin tác giả
*   **Họ và tên**: Vũ Thế Huy
*   **Chuyên ngành**: Kỹ thuật Điện tử & Tin học Công nghiệp 1, Khóa 62
*   **Đề tài**: Thiết kế phần cứng Hệ thống Đèn giao thông thông minh (STLS)
