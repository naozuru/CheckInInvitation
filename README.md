# 🎟️ School Event QR Check-In System

Sistem **Check-In Event Sekolah berbasis QR Code** yang terintegrasi dengan **Google Spreadsheet** menggunakan **Google Apps Script**.  
Dirancang untuk memudahkan proses absensi event sekolah dengan **real-time update**, **anti double check-in**, dan **counter kehadiran per jenjang**.

---

## ✨ Fitur Utama

- 📷 **Scan QR Code (Kamera)**
- 🚫 **Anti Double Check-In**
- 🔍 **Pencarian Nama (Search)**
- 📊 **Counter Kehadiran Real-Time**
  - SHS (Senior High School)
  - JHS (Junior High School)
  - ES (Elementary School)
- 📈 **Progress Bar Kehadiran**
- 🕒 **Timestamp Otomatis**
- 🔄 **Auto Refresh Data**
- 📱 **Mobile Friendly (Responsive)**
- 📄 **Log Kehadiran Lengkap**

---

## 🧠 Cara Kerja Sistem

1. QR Code dibuat dari **Full Name siswa**
2. Kamera melakukan scan QR
3. Website mengirim nama ke **Google Apps Script**
4. Apps Script:
   - mencari data di Spreadsheet
   - mengecek status check-in
   - menolak scan ganda
   - menyimpan waktu check-in
5. Website menampilkan hasil & update counter

---

## 🗂️ Struktur Spreadsheet

Gunakan **satu Spreadsheet** dengan beberapa Sheet:
DATA-SISWA-SHS
DATA-SISWA-JHS
DATA-SISWA-ES


### Format Kolom (WAJIB)

| Kolom | Keterangan |
|------|------------|
| A | Full Name |
| B | Class |
| C | Level (SHS / JHS / ES) |
| D | QR Code (opsional) |
| E | - |
| F | Status (Registered / Check In) |
| G | Check-In Time |

---

## 🌐 Struktur Website

```text
index.html
assets/
 └─ logo.png

```
---
## ⚙️ Teknologi yang Digunakan

- HTML5
- CSS3
- JavaScript (Vanilla)
- html5-qrcode
- Google Apps Script
- Google Spreadsheet
- GitHub Pages

## 🔐 Keamanan

- LockService untuk mencegah double scan bersamaan
- Validasi nama sebelum check-in
- Scan hanya bisa berhasil 1x per siswa

## 📸 Tampilan

- Dashboard modern
- Counter kehadiran visual
- Highlight peserta terbaru
- Progress bar dinamis

## 👨‍💻 Author

Mr Rayhan
School Event & Education Technology Project

## 📄 License

This project is licensed for educational and internal school use only.
Modification is allowed with proper credit.

## Demo
https://naozuru.github.io/CheckInInvitation/
