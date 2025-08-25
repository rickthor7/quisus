# 🚀 Kuis Interaktif Luar Angkasa

Selamat datang di Kuis Interaktif Luar Angkasa! Sebuah aplikasi kuis berbasis web yang dirancang agar seru dan menarik bagi siswa. Proyek ini menggunakan Google Sheets sebagai database _real-time_ yang dikelola melalui Google Apps Script, membuatnya menjadi solusi yang hemat biaya dan mudah diimplementasikan.

[**➡️ Lihat Live Demo**](https://ricktho7.github.io/quisus/)

## ✨ Fitur Utama

- **📝 Input Data Siswa**: Form sederhana untuk memasukkan nama dan kelas sebelum memulai kuis.
- **🎮 Kuis Pilihan Ganda**: Soal-soal interaktif dengan batas waktu per pertanyaan.
- **📊 Papan Skor Real-Time**: Halaman leaderboard yang menampilkan peringkat, nama, kelas, dan skor tertinggi, diurutkan secara otomatis.
- **🚀 Tema Luar Angkasa**: Desain visual yang ceria dan interaktif dengan animasi untuk meningkatkan engagement siswa.
- **☁️ Database Gratis**: Menggunakan Google Sheets sebagai backend, tidak memerlukan biaya hosting database.
- **📱 Desain Responsif**: Tampilan yang optimal di berbagai perangkat, baik desktop maupun mobile.

## 🛠️ Teknologi yang Digunakan

- **Frontend**:
  - HTML5
  - [Tailwind CSS](https://tailwindcss.com/)
  - JavaScript (ES6)
- **Backend & Database**:
  - [Google Sheets](https://www.google.com/sheets/about/)
  - [Google Apps Script](https://developers.google.com/apps-script)

## 📂 Struktur Proyek

.  
├── index.html // Halaman utama untuk input data & pengerjaan kuis.  
├── papan-skor.html // Halaman untuk menampilkan papan skor.  
├── Code.gs // (Opsional) Kode Google Apps Script untuk backend.  
└── README.md // Dokumentasi proyek ini.  

## ⚙️ Cara Instalasi & Setup

Ikuti langkah-langkah ini untuk menjalankan versi Anda sendiri dari proyek ini.

### 1\. Siapkan Google Sheet

1. Buat [Google Sheet](https://sheets.new) baru.
2. Ganti nama sheet (tab di bawah) menjadi skor_kuis.
3. Buat 4 kolom di baris pertama dengan judul: timestamp, nama, kelas, skor.

### 2\. Konfigurasi Google Apps Script

1. Buka Google Sheet Anda, lalu klik **Ekstensi** > **Apps Script**.
2. Hapus semua kode contoh dan tempel kode dari file Code.gs.
3. Cari baris const SHEET_ID = "..." dan ganti dengan **ID Google Sheet** Anda (ID bisa ditemukan di URL sheet).
4. Simpan proyek script tersebut.

### 3\. Deploy Script sebagai Web App

1. Di editor Apps Script, klik tombol biru **Deploy** > **Deployment baru**.
2. Klik ikon gerigi (⚙️) dan pilih **Aplikasi Web**.
3. Pada bagian "Siapa yang memiliki akses", ubah menjadi **"Siapa saja"**.
4. Klik **Deploy**.
5. Otorisasi akses jika diminta.
6. **Salin URL Aplikasi Web** yang muncul. Ini adalah kunci untuk menghubungkan website Anda.

### 4\. Hubungkan URL ke File HTML

1. Buka file index.html dan papan-skor.html.
2. Cari baris const SCRIPT_URL = "...".
3. Tempel **URL Aplikasi Web** yang sudah Anda salin ke dalam tanda kutip di kedua file tersebut.
4. Simpan perubahan.

Proyek Anda sekarang siap untuk di-hosting di platform seperti GitHub Pages!

## 🕹️ Cara Menggunakan

1. Buka halaman utama (index.html).
2. Masukkan nama dan kelas Anda.
3. Klik "Mulai Petualangan!" dan jawab semua pertanyaan sebelum waktu habis.
4. Setelah selesai, klik "Kirim Skor".
5. Anda akan otomatis diarahkan ke halaman Papan Skor untuk melihat peringkat Anda.

## 🤝 Kontribusi

Kontribusi, isu, dan permintaan fitur sangat diterima! Jangan ragu untuk membuat _issue_ atau _pull request_.

## 📄 Lisensi

Proyek ini dilisensikan di bawah **MIT License**. Lihat file LICENSE untuk detailnya.
