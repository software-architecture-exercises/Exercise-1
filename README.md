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

⚙️ Yêu cầu Hệ thống
.NET Framework >= 4.7
Visual Studio 2019 hoặc mới hơn
🚀 Hướng dẫn Cài đặt
Bước 1: Clone Repository
Sử dụng lệnh sau để clone dự án:

bash
Sao chép
Chỉnh sửa
git clone https://github.com/soa-ueh-thanhlam/Excersie1.git
Bước 2: Chạy TemperatureServer
Cài đặt URL cho WebService trong tệp WebService1.asmx nếu cần thiết.
Mở Visual Studio, nhấn F5 để khởi động dịch vụ.
Bước 3: Chạy TemperatureClient
Đặt dự án TemperatureClient làm dự án khởi chạy trong Visual Studio.
Nhấn F5 để chạy ứng dụng.
🌐 API Dịch vụ Web
Dịch vụ web hỗ trợ hai phương thức chuyển đổi nhiệt độ:

Chuyển đổi từ Fahrenheit sang Celsius

Phương thức: FahrenheitToCelsius
Tham số:
fahrenheit (double): Nhiệt độ đầu vào bằng Fahrenheit
Trả về:
Nhiệt độ tương ứng bằng Celsius (double)
Chuyển đổi từ Celsius sang Fahrenheit

Phương thức: CelsiusToFahrenheit
Tham số:
celsius (double): Nhiệt độ đầu vào bằng Celsius
Trả về:
Nhiệt độ tương ứng bằng Fahrenheit (double)
💡 Hướng dẫn Sử dụng
1. Thành phần
TemperatureServer: Dịch vụ web cung cấp các phương thức chuyển đổi nhiệt độ.
TemperatureClient: Ứng dụng giao diện người dùng với các thành phần:
Textbox: Nhập nhiệt độ đầu vào.
Label: Hiển thị kết quả chuyển đổi.
Button: Thực hiện chuyển đổi giữa Fahrenheit và Celsius.
2. Các bước sử dụng
Chạy TemperatureServer để khởi động dịch vụ web.
Mở ứng dụng TemperatureClient để nhập nhiệt độ cần chuyển đổi.
Kết quả sẽ hiển thị trực tiếp trên giao diện.
🔧 Hướng dẫn Kết nối Client với Server
Trong Visual Studio, nhấp chuột phải vào dự án TemperatureClient.
Chọn Add > Service Reference.
Trong cửa sổ Add Service Reference, chọn Advanced.
Nhấp vào Add Web Reference.
Nhập URL của dịch vụ web (ví dụ: http://localhost:port/WebService1.asmx).
Nhấn Go để tải thông tin dịch vụ.
Chọn dịch vụ và nhấn Add Reference.
📋 Kiểm thử
Sử dụng các bài kiểm thử có sẵn trong Visual Studio để kiểm tra từng phương thức API.
Đảm bảo kết quả trả về đúng với các trường hợp thử nghiệm (ví dụ: 32°F = 0°C).
🛠️ Xử lý Lỗi
Ứng dụng sử dụng double.TryParse để kiểm tra dữ liệu nhập có hợp lệ hay không.
Hiển thị thông báo lỗi nếu nhập sai định dạng hoặc xảy ra lỗi kết nối với dịch vụ web.
✅ Kết quả Đạt được
Ứng dụng hoàn thiện: Chuyển đổi chính xác giữa Fahrenheit và Celsius.
Dịch vụ web SOAP: Được triển khai thành công, tương thích với nhiều nền tảng.
Giao diện người dùng: Trực quan, thân thiện, hỗ trợ kiểm tra và xử lý lỗi hiệu quả.
Kỹ năng thực tiễn: Tăng cường kỹ năng phát triển ứng dụng .NET Framework.
📜 License
Dự án này được phát hành dưới giấy phép MIT License.

📧 Thông tin Liên hệ
