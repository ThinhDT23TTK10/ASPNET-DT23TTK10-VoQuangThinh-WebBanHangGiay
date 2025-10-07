# ASP.NET MVC — Web Bán Hàng Giày

**Repository:** [github.com/ThinhDT23TTK10/ASPNET-DT23TTK10-VoQuangThinh-WebBanHangGiay](https://github.com/ThinhDT23TTK10/ASPNET-DT23TTK10-VoQuangThinh-WebBanHangGiay)

---

## Thông tin liên hệ
- **Tác giả:** Võ Quang Thịnh  
- **Email:** thinhvq201294@sv-onuni.edu.vn  
- **SĐT:** 0838666236  

---

## Công nghệ sử dụng
- ASP.NET MVC 5 (.NET Framework 4.8)  
- Entity Framework 6  
- SQL Server LocalDB  
- VNPAY Sandbox Integration  

---

## Hướng dẫn cài đặt

### 1️ Clone dự án
```bash
git clone https://github.com/ThinhDT23TTK10/ASPNET-DT23TTK10-VoQuangThinh-WebBanHangGiay.git
```
### 2 Mở dự án
Mở file .sln trong Visual Studio 2019 hoặc 2022
Visual Studio sẽ tự động restore NuGet packages

---
### 3 Khôi phục database từ file .bak
Mở SQL Server Management Studio (SSMS)
Chuột phải Databases → Restore Database...
Chọn file .bak trong thư mục /Database/
Đặt tên database trùng với connection string trong web.config

---
### 4 Cấu hình web config và build
```bash
<connectionStrings>
  <add name="DefaultConnection"
       connectionString="Data Source=(localdb)\\MSSQLLocalDB;Initial Catalog=BanHangThoiTrangMVC;Integrated Security=True;MultipleActiveResultSets=True"
       providerName="System.Data.SqlClient" />
</connectionStrings>
```
Nhấn Ctrl + F5 hoặc chọn IIS Express để chạy web
Truy cập: https://localhost:44367/
