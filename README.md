Ứng dụng Chuyển đổi Nhiệt độ

🌟 Giới thiệu
Dự án này gồm hai thành phần chính:

TemperatureServer: Dịch vụ web SOAP hỗ trợ chuyển đổi nhiệt độ giữa Fahrenheit và Celsius.
TemperatureClient: Ứng dụng Windows Forms giúp người dùng nhập và chuyển đổi nhiệt độ qua giao diện trực quan.
🗂️ Cấu trúc Dự án

plaintext
Sao chép
Chỉnh sửa
TemperatureWS/
├── TemperatureServer/
│   ├── WebService1.asmx       # Dịch vụ web chính
│   ├── WebService1.asmx.cs    # Mã nguồn xử lý dịch vụ
├── TemperatureClient/
│   ├── Form1.cs               # Form giao diện chính
│   ├── Program.cs             # Điểm bắt đầu của ứng dụng
│   ├── App.config             # Tệp cấu hình ứng dụng
⚙️ Yêu cầu Hệ thống

.NET Framework phiên bản 4.7 trở lên
Visual Studio 2019 hoặc các phiên bản mới hơn
🚀 Hướng dẫn Cài đặt

Bước 1: Clone repository

bash
Sao chép
Chỉnh sửa
git clone https://github.com/soa-ueh-thanhlam/Excersie1.git
Bước 2: Khởi động TemperatureServer

Cấu hình URL cho WebService trong tệp WebService1.asmx nếu cần thiết.
Mở Visual Studio, nhấn F5 để chạy dịch vụ.
Bước 3: Khởi động TemperatureClient

Đặt TemperatureClient làm dự án khởi chạy trong Visual Studio.
Nhấn F5 để chạy ứng dụng.
🌐 API Dịch vụ Web

Dịch vụ hỗ trợ hai phương thức chính:

FahrenheitToCelsius: Chuyển đổi nhiệt độ từ Fahrenheit sang Celsius.

Tham số: fahrenheit (double)
Trả về: Giá trị nhiệt độ tương ứng ở Celsius (double)
CelsiusToFahrenheit: Chuyển đổi nhiệt độ từ Celsius sang Fahrenheit.

Tham số: celsius (double)
Trả về: Giá trị nhiệt độ tương ứng ở Fahrenheit (double)
💡 Hướng dẫn Sử dụng

1. Thành phần
TemperatureServer: Dịch vụ web cung cấp các phương thức chuyển đổi.
TemperatureClient: Ứng dụng giao diện với các thành phần:
Textbox: Nhập nhiệt độ đầu vào.
Label: Hiển thị kết quả.
Button: Thực hiện chuyển đổi nhiệt độ.
2. Các bước thực hiện
Chạy TemperatureServer để khởi động dịch vụ web.
Mở ứng dụng TemperatureClient để nhập nhiệt độ cần chuyển đổi.
Kết quả sẽ hiển thị trực tiếp trên giao diện.
🔧 Hướng dẫn Kết nối Client với Server

Trong Visual Studio, nhấp chuột phải vào dự án TemperatureClient.
Chọn Add > Service Reference.
Nhấp vào Advanced, sau đó chọn Add Web Reference.
Nhập URL của dịch vụ web (ví dụ: http://localhost:port/WebService1.asmx).
Nhấn Go, chọn dịch vụ và nhấp Add Reference.
📋 Kiểm thử

Kiểm tra các phương thức API với các trường hợp phổ biến (ví dụ: 32°F = 0°C).
Sử dụng Visual Studio Unit Testing để đảm bảo tính chính xác của từng chức năng.
🛠️ Xử lý Lỗi

Ứng dụng sử dụng double.TryParse để xác minh dữ liệu nhập có hợp lệ không.
Hiển thị thông báo lỗi nếu phát sinh sự cố như nhập sai định dạng hoặc lỗi kết nối.
✅ Kết quả Đạt được

Ứng dụng hỗ trợ chuyển đổi chính xác giữa Fahrenheit và Celsius.
Dịch vụ web SOAP triển khai thành công và dễ dàng tích hợp.
Giao diện trực quan, thân thiện và hỗ trợ kiểm tra lỗi hiệu quả.
Củng cố kỹ năng xây dựng ứng dụng trên nền tảng .NET Framework.
📜 License
Dự án được phát hành theo giấy phép MIT License.

📧 Liên hệ
Nếu cần hỗ trợ thêm, bạn có thể liên hệ qua GitHub repository của dự án.
