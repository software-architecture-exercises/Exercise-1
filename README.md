# Ứng dụng Chuyển đổi Nhiệt độ

🌟 **Mô tả**  
Dự án này gồm hai thành phần chính:  

1. **TemperatureServer**: Dịch vụ web SOAP hỗ trợ chuyển đổi nhiệt độ giữa Fahrenheit và Celsius.  
2. **TemperatureClient**: Ứng dụng Windows Forms giúp người dùng nhập và chuyển đổi nhiệt độ qua giao diện trực quan.  

---

## 🗂️ Cấu trúc Dự án
```plaintext
TemperatureWS/
├── TemperatureServer/
│   ├── WebService1.asmx       # Dịch vụ web chính
│   ├── WebService1.asmx.cs    # Mã nguồn xử lý dịch vụ
├── TemperatureClient/
│   ├── Form1.cs               # Form giao diện chính
│   ├── Program.cs             # Điểm bắt đầu của ứng dụng
│   ├── App.config             # Tệp cấu hình ứng dụng
