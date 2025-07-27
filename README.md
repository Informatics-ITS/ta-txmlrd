# 🏁 Tugas Akhir (TA) - Final Project

**Nama Mahasiswa**: I Gusti Agung Ngurah Adhi Sanjaya  
**NRP**: 5025211056  
**Judul TA**: Rancang Bangun Modul Otentikasi dan Otorisasi Berbasis Rekognisi Wajah dengan Arsitektur Microservices dan API Gateway pada LMS Bahasa Inggris  
**Dosen Pembimbing**: Bintang Nuralamsyah S. Kom., M. Kom.  
**Dosen Ko-pembimbing**: Ratih Nur Esti Anggraini, S.Kom., M.Sc., Ph.D.  

---

## 📺 Demo Aplikasi  
[![Demo Aplikasi](https://sevima.com/wp-content/uploads/2021/06/lms-untuk-perguruan-tinggi.png)](https://www.youtube.com/watch?v=VIDEO_ID)  
*Klik gambar di atas untuk menonton demo*

---


## 🛠 Panduan Instalasi & Menjalankan Software  

### Prasyarat  
- Daftar syarat :
  - Memiliki docker yang terinstall pada device.


### Langkah-langkah  
1. **Clone Repository**  
   ```bash
   git clone https://github.com/Informatics-ITS/ta-txmlrd
   ```
2. **Pisahkan 4 Layanan**
- Setelah clone repo, pisahkan setiap layanan yang terdiri dari user management service, auth & security service, role management service dan api gateway
- Lalu masuk ke direktori masing-masing layanan untuk melanjutkan menjalankan docker setiap layanan

3. **Konfigurasi**
- Konfigurasi mengharuskan file .env yang tepat, dikarenakan file env yang ter-config pada repo ini menyangkut data sensitif, dapat menghubungi penulis untuk mendapatkan data valid.

4. **Instalasi Pada Setiap Layanan**
- Untuk build pertama kali dapat menjalankan kode ini
   ```bash
   cd [setiap-layanan]
   docker-compose up --build
   ```
- Jika ingin, stop docker dapat menjalankan kode berikut
   ```bash
   docker-compose down
   ```
- Jika ingin start lagi tanpa build dapat menjalankan kode berikut
   ```bash
   docker-compose up
   ```

5. Buka postman untuk testing backend setiap layanan dengan list port:
- `http://localhost:5000` untuk port auth & security service
- `http://localhost:5001` untuk port user management service
- `http://localhost:5002` untuk port api gateway
- `http://localhost:5003` untuk port role management service

---

## ⁉️ Pertanyaan?

Hubungi:
- Penulis: gungadhisanjaya@gmail.com
- Pembimbing Utama: bintang@its.ac.id
