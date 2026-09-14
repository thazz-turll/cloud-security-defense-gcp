# Multi-Layer Cloud Defense & Security Monitoring on GCP

Giải pháp kiến trúc phòng thủ đa lớp (Multi-Layer Cloud Defense) và giám sát an ninh tập trung được triển khai trên nền tảng **Google Cloud Platform (GCP)**, nhằm bảo vệ hạ tầng đám mây trước các mối đe dọa tinh vi và kiểm soát chặt chẽ luồng truy cập dữ liệu.

---

## 🎯 1. Tổng quan Dự án
Trong bối cảnh chuyển đổi số, việc bảo vệ các tài nguyên trên Cloud đòi hỏi một chiến lược phòng thủ nhiều tầng (Defense-in-Depth). Dự án tập trung xây dựng hệ thống bảo mật toàn diện trên GCP với các mục tiêu cốt lõi:
* **Phòng thủ Đa lớp (Multi-Layer Security):** Thiết lập các vành đai bảo vệ từ tầng biên mạng, tầng quản trị IAM, đến tầng dịch vụ ứng dụng và lưu trữ.
* **Giám sát & Cảnh báo Thời gian thực:** Thu thập nhật ký hoạt động (Cloud Audit Logs, VPC Flow Logs) để phát hiện kịp thời các hành vi xâm nhập hoặc cấu hình sai lầm (Misconfigurations).
* **Tự động hóa phản ứng:** Giảm thiểu thời gian phát hiện và xử lý sự cố (MTTD / MTTR) thông qua các công cụ phân tích hiện đại trên hạ tầng Google Cloud.

---

## 🏗️ 2. Kiến trúc Bảo mật Đa lớp trên GCP
Hệ thống được phân chia thành các lớp phòng thủ chuyên biệt:
1. **Lớp Biên Mạng & Tường lửa (Network & Perimeter Layer):** Sử dụng VPC Service Controls, Cloud Firewall Rules và Cloud Armor để ngăn chặn các cuộc tấn công DDoS và kiểm soát luồng traffic ra vào.
2. **Lớp Định danh & Phân quyền (IAM & Access Control Layer):** Áp dụng nguyên tắcặc quyền tối thiểu (Principle of Least Privilege), quản lý Service Accounts và kiểm soát chặt chẽ lịch sử gọi API.
3. **Lớp Giám sát & Kiểm toán (Monitoring & Logging Layer):** Tích hợp Google Cloud Logging và Cloud Monitoring để gom nhóm, phân tích log tập trung.
4. **Lớp Bảo vệ Dữ liệu & Tài nguyên (Data & Compute Protection):** Bảo mật cácBucket Cloud Storage, mã hóa dữ liệu và thiết lập các chính sách ngăn chặn rò rỉ thông tin.

---

## 🛠️ 3. Công nghệ & Dịch vụ GCP Sử dụng (Tech Stack)
* **Cloud Platform:** Google Cloud Platform (GCP)
* **Identity & Access:** GCP IAM, Service Accounts, Resource Manager
* **Network Security:** Google Cloud VPC, Firewall Rules, Cloud NAT, Cloud Load Balancing
* **Monitoring & Logging:** Cloud Audit Logs, VPC Flow Logs, Cloud Monitoring & Logging
* **Security Analytics:** Security Command Center (tùy chọn tích hợp)

---

