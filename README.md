# Temperature Application

## 🌟 Giới thiệu
Dự án **Temperature Application** bao gồm hai thành phần chính:

1. **TemperatureServer**: Một dịch vụ web SOAP hỗ trợ chuyển đổi nhiệt độ giữa Fahrenheit và Celsius.
2. **TemperatureClient**: Ứng dụng Windows Forms với giao diện trực quan để người dùng thực hiện các phép chuyển đổi nhiệt độ.

---

## 🗂️ Cấu trúc dự án

```
TemperatureWS/
├── TemperatureServer/
│   ├── WebService1.asmx       # Dịch vụ web chính
│   ├── WebService1.asmx.cs    # Code-behind của WebService1
├── TemperatureClient/
│   ├── Form1.cs               # Form chính của ứng dụng WinForm
│   ├── Program.cs             # Điểm bắt đầu của ứng dụng
│   ├── App.config             # Tệp cấu hình ứng dụng
```

---

## ⚙️ Yêu cầu hệ thống

- **.NET Framework** >= 4.7
- **Visual Studio** 2019 hoặc mới hơn

---

## 🚀 Hướng dẫn cài đặt

### Bước 1: Clone repository
```bash
git clone https://github.com/soa-ueh-thanhlam/Excersie1.git
```

### Bước 2: Chạy TemperatureServer
1. Cấu hình URL cho WebService trong `WebService1.asmx` nếu cần.
2. Mở dự án trong Visual Studio và nhấn **F5** để chạy dịch vụ.

### Bước 3: Chạy TemperatureClient
1. Trong Visual Studio, chọn **TemperatureClient** làm dự án khởi chạy.
2. Nhấn **F5** để chạy ứng dụng.

---

## 🌐 API Dịch vụ Web

Dịch vụ web cung cấp hai phương thức chính:

### 1. Chuyển đổi từ Fahrenheit sang Celsius
- **Phương thức**: `FahrenheitToCelsius`
- **Tham số**: 
  - `fahrenheit` (double): Nhiệt độ đầu vào bằng Fahrenheit
- **Trả về**: Nhiệt độ tương ứng bằng Celsius (double)

### 2. Chuyển đổi từ Celsius sang Fahrenheit
- **Phương thức**: `CelsiusToFahrenheit`
- **Tham số**: 
  - `celsius` (double): Nhiệt độ đầu vào bằng Celsius
- **Trả về**: Nhiệt độ tương ứng bằng Fahrenheit (double)

---

## 💡 Hướng dẫn sử dụng

### Thành phần

#### 1. TemperatureServer
- **Tệp**: `WebService1.asmx`
- **Namespace**: `http://tempuri.org/`
- Chức năng: Cung cấp các phương thức chuyển đổi nhiệt độ.

#### 2. TemperatureClient
- **Giao diện**: 
  - **Textbox**: Nhập nhiệt độ đầu vào
  - **Label**: Hiển thị kết quả chuyển đổi
  - **Button**: Thực hiện chuyển đổi giữa Fahrenheit và Celsius

### Các bước sử dụng
1. Chạy **TemperatureServer** để khởi động dịch vụ.
2. Mở ứng dụng **TemperatureClient** để nhập nhiệt độ và chọn phép chuyển đổi.
3. Kết quả sẽ được hiển thị trong giao diện ứng dụng.

---

## 🔧 Hướng dẫn kết nối Client với Server

1. Trong Visual Studio, nhấp chuột phải vào dự án **TemperatureClient**.
2. Chọn **Add > Service Reference**.
3. Trong cửa sổ **Add Service Reference**, nhấp **Advanced**.
4. Chọn **Add Web Reference**.
5. Nhập URL của `WebService1.asmx` (ví dụ: `http://localhost:port/WebService1.asmx`).
6. Nhấn **Go** để tải thông tin dịch vụ.
7. Chọn dịch vụ và nhấn **Add Reference**.

---

## 📋 Kiểm thử

- Sử dụng các bài kiểm thử có sẵn trong Visual Studio để đảm bảo tính chính xác của các phương thức API.
- Ví dụ kiểm thử:
  - 32°F = 0°C
  - 100°C = 212°F

---

## 🛠️ Xử lý lỗi

- Ứng dụng sử dụng `double.TryParse` để kiểm tra tính hợp lệ của đầu vào.
- Thông báo lỗi hiển thị nếu:
  - Dữ liệu nhập không hợp lệ.
  - Không thể kết nối với dịch vụ web.

---

## ✅ Kết quả đạt được

- **Hoàn thiện ứng dụng**: Cung cấp khả năng chuyển đổi nhiệt độ chính xác giữa Fahrenheit và Celsius.
- **Dịch vụ web SOAP**: Được triển khai thành công, đảm bảo tính tương thích đa nền tảng.
- **Giao diện người dùng**: Trực quan, dễ sử dụng, hỗ trợ kiểm tra và xử lý lỗi đầu vào hiệu quả.
- **Kiến thức thực tiễn**: Xây dựng ứng dụng dựa trên .NET Framework một cách chuyên sâu.

---

## 📜 License

Dự án này được phát hành dưới giấy phép **MIT License**.
