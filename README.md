# Flyme 10 for Xiaomi Mi MIX 3 (Perseus)

![Android Version](https://img.shields.io/badge/Android-13--33-green?style=for-the-badge&logo=android)
![ROM Status](https://img.shields.io/badge/Status-Beta--Port-orange?style=for-the-badge)
![Device](https://img.shields.io/badge/Device-Perseus-blue?style=for-the-badge)

Bản ROM Port mang giao diện mượt mà, độc quyền của **Flyme OS 10** lên chiếc **Xiaomi Mi MIX 3 (Perseus)** trên nền tảng Android 13. Dự án được tối ưu hóa cấu trúc phân quyền hệ thống để đảm bảo tính ổn định cao nhất khi sử dụng hàng ngày.

---

## 🚨 TUYÊN BỐ MIỄN TRỪ TRÁCH NHIỆM (Disclaimer)
> **Chú ý:** Việc vọc vạch, flash ROM có thể làm mất bảo hành hoặc gây brick thiết bị nếu làm sai bước. Tôi sẽ không chịu trách nhiệm nếu điện thoại của bạn biến thành "cục chặn giấy". Hãy chắc chắn rằng bạn đã đọc kỹ hướng dẫn và sao lưu dữ liệu quan trọng trước khi làm.

---

## 📱 Thông tin chi tiết bản ROM (Build Info)

| Thuộc tính | Thông tin chi tiết |
| :--- | :--- |
| **OS Base** | Flyme OS 10 (China Region) |
| **Android Version** | 13 (API 33) |
| **Build ID** | TQ3A.230901.001 |
| **Target Device** | Xiaomi Mi MIX 3 (Codename: `perseus`) |
| **Build Tool** | CRB Android Kitchen v3.4.0 |
| **Security Patch** | 2026-06 |

---

## 📸 Ảnh chụp màn hình (Screenshots)

<details>
<summary>📸 Nhấn vào đây để xem ảnh giao diện ROM</summary>

### Giao diện chính & Cài đặt
*Hiện tại chưa có*

### Trình quản lý ứng dụng (Flyme Apps)
*Hiện tại chưa có*

</details>

---

## ⚙️ Tình trạng hoạt động (Features Status)

### ✅ Hoạt động mượt mà (Working)
* **Kết nối:** Wi-Fi (2.4GHz/5GHz), Bluetooth, 4G/LTE (Nghe gọi, SMS, Data).
* **Hiển thị:** Tốc độ làm tươi, độ sáng tự động, chế độ tối (Dark Mode).
* **Âm thanh:** Loa thoại, loa ngoài, microphone, tai nghe Type-C.
* **Bảo mật:** Vân tay mặt lưng (Hoạt động nhạy).
* **Hệ thống:** Khung dịch vụ Core GApps (sau khi cài gói bổ sung).

### ❌ Lỗi đã biết (Bugs / Known Issues)
* **Cơ chế trượt (Slider):** Do Flyme không có framework gốc cho camera trượt của Xiaomi, âm thanh khi trượt vật lý chưa hoạt động.
* **Camera gốc:** App camera mặc định của Flyme có thể bị văng ở chế độ Chân dung (Portrait). 
  * *👉 Giải pháp tạm thời:* Sử dụng **Google Camera (GCam)** để thay thế.

---

## 🛠️ Hướng dẫn cài đặt chi tiết (Step-by-Step Installation)

### 📌 Điều kiện (Prerequisites)
1. Điện thoại đã được **Unlock Bootloader**.
2. Máy đã cài sẵn **TWRP Recovery** bản mới nhất hỗ trợ Android 13.
3. Máy tính đã cài đủ **Driver Xiaomi** và công cụ **ADB/Fastboot**.

### 🧼 Quy trình Clean Flash (Bắt buộc cho lần đầu từ MIUI sang)

<details>
<summary>🔄 Xem chi tiết các bước Flash qua TWRP</summary>

1. **Vào Recovery:** Tắt nguồn hoàn toàn. Nhấn giữ `Nguồn` + `Tăng âm lượng` để vào TWRP.
2. **Format bộ nhớ:** Vào `Wipe` -> Chọn `Format Data` -> Gõ `yes` và ấn dấu tick xanh.
3. **Khởi động lại TWRP:** Vào `Reboot` -> Chọn `Recovery` (Bước này giúp TWRP nhận diện lại phân vùng vừa format).
4. **Xóa phân vùng cũ:** Vào `Wipe` -> `Advanced Wipe` -> Tích chọn `Dalvik / ART Cache`, `Cache`, `System`, `Data` -> Kéo thanh trượt để Wipe.
5. **Chép file ROM:** Cắm cáp kết nối với máy tính, chép file `Flyme10_Perseus.zip` vào bộ nhớ máy (hoặc dùng USB OTG).
6. **Flash ROM:** Vào `Install` -> Chọn file ROM `.zip` -> Kéo thanh trượt để tiến hành nạp hệ thống.
7. **Cài đặt Google (Tùy chọn):** Nếu dùng gói Google rời, flash tiếp file `NikGApps-core-13.zip` ngay sau khi flash ROM.
8. **Khởi động:** Bấm `Reboot System` và kiên nhẫn chờ từ 10-15 phút.

</details>

---

## 📥 Tải về (Downloads)

* 🔴 [**Tải xuống file ROM ZIP (SourceForge)**](https://sourceforge.net/projects/flyme-10-for-mi-mix-3-perseus/files/Flyme10_Perseus.zip/download)
* 🟡 [**Tải xuống gói Google Core GApps (NikGApps)**](https://nikgapps.com)
* 🟢 [**Tải xuống bản GCam tối ưu cho Mi MIX 3**](https://www.celsoazevedo.com/files/android/google-camera/)

---

## 🐛 Hướng dẫn báo lỗi & Gửi Logcat (Bug Reporting)
Nếu bạn gặp tình trạng ứng dụng hệ thống bị văng hoặc treo máy, hãy giúp tôi cải thiện bản ROM bằng cách gửi Logcat:
1. Bật *Tùy chọn nhà phát triển* và kích hoạt *Gỡ lỗi USB (USB Debugging)* trên điện thoại.
2. Cắm cáp vào máy tính và chạy lệnh:
```bash
   adb logcat -d > error_log.txt
```
3. Tạo một **Issue** trên kho GitHub này và đính kèm file `error_log.txt` đó lên.
## 🤝 Lời cảm ơn (Credits & Acknowledgements)
* **Meizu OS Team** vì giao diện Flyme 10 tuyệt vời.
* **Xiaomi vì mã nguồn kernel nguồn mở của Mi MIX 3.
* **CRB Kitchen Team vì công cụ đóng gói phân vùng tuyệt vời giúp đơn giản hóa quy trình port.
```bash
   adb logcat -d > error_log.txt
