# Trinity Project

Trinity adalah aplikasi berbasis Python yang menggunakan **computer vision** dan **gesture recognition** untuk mendeteksi serta memproses perintah berbasis gerakan tangan.

---

## 📦 Instalasi

1. **Clone repository Trinity**
   ```bash
   git clone https://github.com/username/trinity.git
   cd trinity
   ```

2. **Install semua dependencies**  
   Pastikan Anda sudah memiliki Python 3.8+ dan pip. Lalu jalankan:
   ```bash
   pip install -r requirements.txt
   ```

   Jika file `requirements.txt` belum tersedia, Anda bisa menginstall manual:
   ```bash
   pip install opencv-python numpy mediapipe easyocr
   ```

3. **Jalankan aplikasi**
   ```bash
   python run.py
   ```

---

## ✋ Kontrol Gesture

Gunakan gesture tangan berikut untuk mengontrol aplikasi:

| Gesture Tangan         | Fungsi                                                |
|------------------------|-------------------------------------------------------|
| **Telunjuk Diangkat**  | Menggambar di layar                                   |
| **Tangan Menggenggam** | Menghapus seluruh gambar                              |
| **Lima Jari Merapat**  | Masuk ke mode idle, menunggu hasil selama 7 detik     |
| **ESC (keyboard)**     | Menutup aplikasi setelah proses scan selesai          |

---

## ⏳ Mode Idle

Setelah pengguna melakukan gesture **lima jari merapat**, aplikasi akan masuk ke **mode idle selama 7 detik** sebelum melanjutkan proses lebih lanjut (misalnya menampilkan hasil scan).

Selama mode ini:
- Jangan melakukan gesture lain.
- Kamera akan tetap aktif dan menunggu.
- Hasil akhir akan diproses setelah 7 detik.

---

## 📝 Catatan

- Gunakan pencahayaan yang cukup agar kamera dapat mengenali gesture dengan akurat.
- Pastikan webcam Anda aktif sebelum menjalankan `run.py`.
- Jika aplikasi tidak merespons gesture:
  - Periksa apakah semua dependensi sudah terinstall.
  - Coba jalankan ulang aplikasi dan pastikan tidak ada error di terminal.
