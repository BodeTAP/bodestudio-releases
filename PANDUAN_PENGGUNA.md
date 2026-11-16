# BodeStudio Pro 3.0 — Panduan Pengguna Resmi & Quick-Start Guide
### *Universal YouTube Ambience Video Automation Engine*

Selamat datang di **BodeStudio Pro 3.0**! Software ini dirancang khusus untuk kreator konten YouTube, produser musik lofi/ambience, dan pemilik agensi video automation yang ingin memproduksi video ambience berdurasi panjang (1 hingga 3+ jam) berkualitas broadcast dengan efisiensi maksimal dan proteksi monetisasi terbaik.

---

## DAFTAR ISI

1. [Bab 1: Persyaratan Sistem & Instalasi](#bab-1-persyaratan-sistem--instalasi)
2. [Bab 2: Panduan Aktivasi Lisensi](#bab-2-panduan-aktivasi-lisensi)
3. [Bab 3: Pengenalan Ruang Kerja (Studio Workspace)](#bab-3-pengenalan-ruang-kerja-studio-workspace)
4. [Bab 4: Alur Kerja Pembuatan Video Ambience (Langkah demi Langkah)](#bab-4-alur-kerja-pembuatan-video-ambience-langkah-demi-langkah)
5. [Bab 5: Fitur Unggulan & Standar Emas Industri](#bab-5-fitur-unggulan--standar-emas-industri)
6. [Bab 6: Otomasi YouTube Studio (Upload, SEO, & Chapters)](#bab-6-otomasi-youtube-studio-upload-seo--chapters)
7. [Bab 7: Pembaruan Software (In-App Auto-Updater)](#bab-7-pembaruan-software-in-app-auto-updater)
8. [Bab 8: Tanya Jawab & Solusi Kendala (FAQ & Troubleshooting)](#bab-8-tanya-jawab--solusi-kendala-faq--troubleshooting)

---

## BAB 1: PERSYARATAN SISTEM & INSTALASI

### 1.1. Spesifikasi Perangkat Keras yang Disarankan
* **Sistem Operasi**: Windows 10 (64-bit) Build 19041 atau lebih baru / Windows 11.
* **Prosesor (CPU)**: Intel Core i5 / AMD Ryzen 5 generasi ke-8 atau lebih baru.
* **Memori (RAM)**: Minimal 8 GB RAM (Direkomendasikan 16 GB untuk rendering 1080p 60fps / 4K).
* **Kartu Grafis (GPU)**:
  * NVIDIA: GeForce GTX 1050 atau lebih baru (Mendukung NVENC).
  * Intel: Intel UHD Graphics 620 atau lebih baru (Mendukung QuickSync / QSV).
  * AMD: Radeon RX 500 series atau lebih baru (Mendukung AMF).
* **Penyimpanan**: Ruang kosong minimal 1 GB untuk instalasi dan ruang kerja video.

### 1.2. Langkah-Langkah Instalasi
1. Unduh installer resmi: `BodeStudioPro_v3.0_Setup.exe`.
2. Klik dua kali pada file installer untuk memulai wizard pemasangan.
3. **Catatan Windows SmartScreen**:
   Jika muncul jendela biru *"Windows protected your PC"* (hal yang wajar pada software independen baru):
   * Klik tombol tulisan kecil **"More info"** (*Informasi selengkapnya*).
   * Klik tombol **"Run anyway"** (*Tetap jalankan*).
4. Pilih folder instalasi (Standar: `C:\Program Files\BodeStudio Pro`).
5. Centang opsi *"Create a desktop shortcut"* jika ingin membuat ikon di Desktop.
6. Klik **Install**. Proses kompresi ultra akan mengekstrak runtime mandiri dalam beberapa detik.
7. Klik **Finish** untuk langsung meluncurkan BodeStudio Pro.

---

## BAB 2: PANDUAN AKTIVASI LISENSI

BodeStudio Pro menggunakan sistem lisensi kriptografis berbasis **Machine ID (Hardware ID)** yang mengunci lisensi pada perangkat keras komputer Anda.

### 2.1. Cara Mengaktifkan Lisensi Anda
1. Buka aplikasi BodeStudio Pro.
2. Di bilah menu atas (Header Bar), klik tombol status lisensi (misal: `TRIAL` atau ikon kunci).
3. Jendela **Aktivasi Lisensi Software** akan terbuka.
4. Anda akan melihat **Machine ID** Anda (Format: `XXXX-XXXX-XXXX-XXXX`).
5. Klik tombol **Salin** di samping Machine ID, lalu kirimkan kode tersebut ke admin / penjual lisensi Anda.
6. Admin akan menerbitkan **Serial Key Resmi** Anda (Format: `BODE-TIER-HWID-SIGNATURE`).
7. Tempelkan Serial Key tersebut ke dalam kolom input *"Serial Key Lisensi"*, lalu klik **Aktivasi Lisensi Sekarang**.
8. Setelah terverifikasi, status akan berubah menjadi **LIFETIME ACTIVE** dengan tier lisensi Anda (`PERSONAL` atau `AGENCY`).

> **PENTING**: File lisensi Anda tersimpan dengan aman di folder sistem `%APPDATA%\BodeStudioPro\license.dat`. Melakukan instalasi ulang atau memperbarui software **tidak akan pernah menghapus lisensi Anda**.

---

## BAB 3: PENGENALAN RUANG KERJA (STUDIO WORKSPACE)

Antarmuka BodeStudio Pro mengusung filosofi desain modern ala software editing profesional papan atas (CapCut Style) dengan 3 panel utama yang terintegrasi rapi:

```
+-----------------------------------------------------------------------------------------+
| [B] BodeStudio Pro  [Preset: Nocturnal Cruise v]   [QSV Active] [PERSONAL] [Update] [-][#][X] |
+-----------------------+---------------------------------+-------------------------------+
| PANEL 1: MEDIA BIN    | PANEL 2: MONITOR PREVIEW        | PANEL 3: INSPECTOR & MASTERING|
|                       |                                 |                               |
| * Antrean Video Mentah| * Real-time Video Canvas        | * Durasi Video (~1 Jam, dsb)  |
| * Pool Koleksi Musik  | * Safe Guides & Shorts 9:16     | * Resolusi & Kualitas Render  |
| * Tombol Tambah File  | * Loop Indicator (No Reverse)   | * EBU R128 (-14 LUFS) Master  |
|                       | * Play, Seek, Mute, Volume      | * Watermark / Channel Logo    |
|                       |                                 | * YouTube Metadata & Upload   |
+-----------------------+---------------------------------+-------------------------------+
```

### 1. Panel Kiri (Media Bin & Asset Pool)
* **Antrean Video**: Menampilkan klip video mentah pendek yang akan digabungkan menjadi loop tanpa putus.
* **Koleksi Musik**: Menampilkan pool track audio yang akan diacak oleh algoritma Smart Shuffle.

### 2. Panel Tengah (Monitor Player Adaptif)
* **Layar Pemutar Real-Time**: Memutar preview video 16:9 secara instan.
* **Safe Guides**: Menampilkan garis pandu area aman YouTube agar teks tidak tertutup elemen antarmuka.
* **Shorts 9:16 Framer**: Memotong dan menampilkan bingkai vertikal 9:16 untuk mengecek komposisi Shorts.
* **Desain Responsif**: Jika jendela dikecilkan, kontrol secara pintar meringkas diri menjadi ikon tanpa ada teks yang bertabrakan.

### 3. Panel Kanan (Inspector & Mastering Settings)
* Tempat mengatur durasi, resolusi, mastering volume -14 LUFS, lapisan suara alam (SFX), logo watermark, dan otomatisasi upload.

---

## BAB 4: ALUR KERJA PEMBUATAN VIDEO AMBIENCE (LANGKAH DEMI LANGKAH)

### Langkah 1: Pilih atau Buat Preset Channel
1. Di bilah atas, pilih profil channel Anda melalui menu dropdown (misal: `Nocturnal Cruise`).
2. Jika memiliki channel baru, klik ikon **Slider Preset** untuk membuka modal manajemen channel:
   * Masukkan ID channel (huruf kecil tanpa spasi, misal: `rainy_lofi`).
   * Tentukan nama channel, judul template, dan folder output.
   * Tetapkan logo watermark default jika ada.

### Langkah 2: Masukkan Video Mentah
1. Di Panel Kiri bagian *Antrean Video*, klik tombol **Tambah**.
2. Pilih 1 atau beberapa file video mentah pendek Anda (format `.mp4`, `.mov`, `.mkv`).
3. Video Anda akan otomatis dianalisis (durasi, resolusi, framerate).

### Langkah 3: Masukkan Lagu ke Pool Musik
1. Di Panel Kiri bagian *Koleksi Musik*, klik tombol **Tambah Lagu** atau **Folder**.
2. Masukkan file audio musik lofi / santai Anda (format `.mp3`, `.wav`, `.flac`, `.aac`).
3. Algoritma Smart Shuffle akan otomatis mengelola urutan pemutaran.

### Langkah 4: Tentukan Durasi & Mastering Audio
1. Di Panel Kanan (Card 1):
   * Pilih **Target Durasi**:
     * `~1 Jam Organik` (~1:05:00 - 1:20:00) — *Sangat direkomendasikan untuk YouTube Ambience!*
     * `~2 Jam Organik` (~2:05:00 - 2:30:00)
     * `~3 Jam Organik` (~3:05:00 - 3:30:00)
     * `15 Menit Cepat` (Untuk pengujian cepat)
2. Aktifkan sakelar **Standar Broadcast -14 LUFS** (EBU R128) agar volume musik stabil, nyaman didengar, dan tidak diturunkan secara paksa oleh YouTube.
3. *(Opsional)* Aktifkan **Lapisan Suara Ambience (SFX)**:
   * Masukkan file suara hujan, ombak pantai, atau gemertak api unggun.
   * Atur slider volume SFX (Standar terbaik: 15% - 25%).

### Langkah 5: Watermark & Proteksi Konten
1. Di Panel Kanan (Card 2):
   * Aktifkan **Watermark / Logo Channel**.
   * Pilih file gambar PNG transparan logo channel Anda.
   * Tentukan posisi sudut (misal: *Kanan Atas* atau *Kiri Bawah*).
   * Atur transparansi (misal: 70%) dan ukuran lebar logo.
2. Centang **Pembersih Metadata AI** untuk memastikan tag tersembunyi C2PA dan AI dihapus.

### Langkah 6: Thumbnail & Shorts Otomatis
1. Centang **Auto Thumbnail 1080p** untuk mengambil frame terbaik beresolusi tinggi otomatis.
2. Centang **Generate YouTube Shorts (9:16)**:
   * Tentukan durasi Shorts (misal: 45 detik).
   * Klik tombol **Preview Frame Shorts** di player untuk menggeser framing horizontal (fokus ke objek utama, misal: perapian atau jendela mobil).

### Langkah 7: Ekspor Video
1. Klik tombol oranye besar **Export Video** di pojok kanan atas Header.
2. Jendela progres ekspor akan muncul menampilkan:
   * Status encoder GPU (NVENC / QuickSync QSV).
   * Persentase perenderan real-time.
   * Kecepatan render (misal: `3.5x realtime`) dan sisa waktu (ETA).
   * Log proses teknis.
3. Setelah selesai, suara notifikasi chime dua nada yang merdu akan berbunyi, dan tombol **Buka Folder Output** siap dibuka.

---

## BAB 5: FITUR UNGGULAN & STANDAR EMAS INDUSTRI

BodeStudio Pro dibangun berlandaskan 5 prinsip rekayasa video broadcast internasional:

### 1. 100% Forward Seamless Crossfade Loop (Bebas Efek Reverse)
Sebagian besar software gratisan membuat video loop dengan cara membalik video mundur (*reverse / ping-pong*), yang menyebabkan asap perapian atau tetesan hujan terlihat bergerak mundur secara aneh.
BodeStudio Pro **100% memutar video maju** menggunakan teknik *forward-only crossfade dissolve* pada titik potong presisi, sehingga loop tidak kasat mata dan terlihat sangat alami.

### 2. Smart Audio Shuffle Engine (Cooldown Minimal 60%)
Dalam video 2–3 jam dengan 10–15 lagu, pemutaran acak konvensional sering memutar lagu yang sama hanya berselang 1–2 lagu.
Smart Shuffle Engine menjamin adanya **jarak cooldown minimal 60% dari jumlah total pool musik** (minimal 6–7 lagu lain di antaranya). Penonton tidak akan pernah merasa bosan mendengar lagu yang sama berulang kali dalam jarak pendek.

### 3. Pembersih Tag AI Metadata (-map_metadata -1 -bitexact)
Algoritma YouTube kini memindai metadata EXIF/C2PA yang disematkan oleh generator video/gambar AI (seperti Midjourney, Runway, Kling, Sora).
BodeStudio Pro secara otomatis membuang seluruh tag metadata AI tersebut sehingga video Anda diperlakukan sebagai konten video organik berstandar tinggi.

### 4. Ekspor Super Cepat Berkat Fast Stream-Copy Architecture
Logo watermark dan loop dibakar pada tahap klip loop 10–30 detik. Saat merakit video final 1 hingga 3 jam, engine menggunakan teknik `-c:v copy` (Fast Stream-Copy) sehingga proses rendering video 1 jam dapat selesai hanya dalam ~45 detik!

---

## BAB 6: OTOMASI YOUTUBE STUDIO (UPLOAD, SEO, & CHAPTERS)

Anda tidak perlu membuka browser dan mengunggah video secara manual satu per satu.

### 6.1. Menghubungkan Akun YouTube Channel
1. Klik tombol **YouTube** di Header Bar.
2. Masukkan kredensial Google API OAuth 2.0 (Client ID & Client Secret) atau impor file `client_secrets.json`.
3. Klik **Otorisasi Channel**. Browser Anda akan terbuka untuk memberikan izin unggah ke channel YouTube Anda.
4. Token akan tersimpan secara otomatis dan aman per-preset channel.

### 6.2. Fitur Otomasi Upload
* **Daftar Bab & Timestamp Otomatis**: Deskripsi video langsung terisi daftar lagu dan menit pemutarannya (`00:00 - Track A`, `03:45 - Track B`) dari file `_chapters.txt` yang dibuat otomatis saat render.
* **Smart SEO Title & Tags Generator**: Menyusun judul menarik dan 500 karakter kata kunci (Tags) relevan tanpa memerlukan API key eksternal (100% gratis & offline).
* **Opsi Status Privasi**:
  * `Private / Draft`: Video masuk sebagai draft, siap ditinjau ulang sebelum tayang.
  * `Unlisted`: Hanya yang memiliki link yang bisa menonton.
  * `Public`: Langsung tayang ke publik.
  * `Scheduled (Terjadwal)`: Menentukan tanggal dan jam tayang otomatis.
* **Auto-Upload Pasca Render**: Jika sakelar *Auto-Upload YouTube* diaktifkan di panel utama, video akan langsung diunggah otomatis segera setelah render selesai!

---

## BAB 7: PEMBARUAN SOFTWARE (IN-APP AUTO-UPDATER)

BodeStudio Pro dilengkapi dengan fitur pembaruan otomatis di dalam aplikasi (*In-App Auto-Updater*).

### 7.1. Bagaimana Cara Mengetahui Jika Ada Versi Baru?
1. Setiap kali aplikasi dibuka, sistem secara senyap memeriksa server rilis resmi di latar belakang.
2. Jika ada pembaruan baru, tombol **Update** di bilah atas akan otomatis berubah warna menjadi **Flame Orange** dengan efek animasi denyut halus (*animate-pulse*).
3. Klik tombol **Update** untuk membuka jendela pembaruan.

### 7.2. Proses Pembaruan Sekali Klik
1. Di jendela pembaruan, Anda dapat membaca daftar fitur baru (*Changelog*).
2. Klik tombol **Unduh Pembaruan**.
3. Sistem akan mengunduh paket installer resmi langsung dengan indikator persentase, total megabyte, dan kecepatan transfer real-time (MB/s).
4. Setelah unduhan selesai, tombol akan berubah menjadi hijau: **Pasang & Mulai Ulang**.
5. Klik tombol tersebut. Aplikasi akan menutup diri secara teratur dan installer akan memperbarui sistem secara mulus (*in-place upgrade*).
6. **Seluruh lisensi, channel preset, dan riwayat Anda tetap tersimpan utuh!**

---

## BAB 8: TANYA JAWAB & SOLUSI KENDALA (FAQ & TROUBLESHOOTING)

### Q1: Apakah aman jika Windows Defender SmartScreen memunculkan peringatan saat instalasi?
> **Jawaban**: Sangat aman. Ini adalah perilaku standar Windows untuk software baru independen yang belum mengumpulkan reputasi unduhan global Microsoft. Cukup klik **More info** lalu pilih **Run anyway**.

### Q2: Mengapa status GPU saya menampilkan "CPU (libx264)" bukannya "NVENC" atau "QSV"?
> **Jawaban**: Pastikan driver kartu grafis Anda (NVIDIA GeForce Experience atau Intel Graphics Driver) dalam kondisi terinstal versi terbaru. BodeStudio Pro secara otomatis mendeteksi hardware encoder terbaik yang aktif di komputer Anda.

### Q3: Apakah saya bisa memindahkan lisensi ke laptop/komputer lain?
> **Jawaban**: Lisensi Serial Key dikunci ke Machine ID fisik satu komputer. Jika Anda mengganti komputer atau meng-upgrade motherboard, silakan hubungi tim dukungan kami dengan menyertakan bukti pembelian untuk penerbitan ulang lisensi baru.

### Q4: Apakah video hasil render bebas dari klaim hak cipta musik?
> **Jawaban**: Pastikan track musik yang Anda masukkan ke dalam folder *Koleksi Musik* adalah musik bebas royalti (Royalty-Free / No Copyright), atau musik yang Anda beli/ciptakan sendiri. BodeStudio Pro mengatur mixing dan mastering volume, tetapi hak cipta audio ditentukan oleh sumber musik yang Anda gunakan.

---

### PUSAT DUKUNGAN & INFORMASI KOMERSIAL

* **Portal Rilis & Unduhan**: [https://github.com/BodeTAP/bodestudio-releases](https://github.com/BodeTAP/bodestudio-releases)
* **Kompilasi Versi**: BodeStudio Pro 3.0 (Official Flame Orange Workstation)
* **Pengembang**: BodeStudio Engineering Team

*Selamat berkarya dan sukses membangun jaringan channel YouTube Ambience Anda!*
