# 📋 SIRA — Sistem Informasi Razia
### *Platform Digital Pencatatan & Pemantauan Pelanggaran Siswa SMKN 1 Malteng*

<div align="center">

![Version](https://img.shields.io/badge/versi-6.1--ENTERPRISE-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/status-aktif-brightgreen?style=for-the-badge)
![License](https://img.shields.io/badge/lisensi-MIT-orange?style=for-the-badge)
![Platform](https://img.shields.io/badge/platform-Web%20Browser-lightgrey?style=for-the-badge)
![No Backend](https://img.shields.io/badge/backend-tidak%20perlu-red?style=for-the-badge)

**Satu platform. Semua pelanggaran. Nol kertas.**  
SIRA adalah sistem informasi terpadu untuk mencatat, memantau, dan mengelola seluruh bentuk pelanggaran siswa — dari razia harian hingga kasus tata tertib berat — langsung dari browser, tanpa server, tanpa instalasi.

[🚀 Cara Menjalankan](#-cara-menjalankan) · [📖 Fitur Lengkap](#-fitur-lengkap) · [🐛 Laporkan Bug](#-kontribusi) · [💡 Saran Fitur](#-kontribusi)

</div>

---

## 📑 Daftar Isi

- [Tentang SIRA](#-tentang-sira)
- [Latar Belakang](#-latar-belakang)
- [Cakupan Pelanggaran](#-cakupan-pelanggaran)
- [Fitur Lengkap](#-fitur-lengkap)
- [Teknologi yang Digunakan](#-teknologi-yang-digunakan)
- [Struktur Aplikasi](#-struktur-aplikasi)
- [Cara Menjalankan](#-cara-menjalankan)
- [Panduan Penggunaan](#-panduan-penggunaan)
- [Konfigurasi Admin](#-konfigurasi-admin)
- [Arsitektur Kode](#-arsitektur-kode)
- [Penyimpanan Data](#-penyimpanan-data)
- [Keamanan & Privasi](#-keamanan--privasi)
- [Keterbatasan](#-keterbatasan)
- [Rencana Pengembangan](#-rencana-pengembangan)
- [Kontribusi](#-kontribusi)
- [Lisensi](#-lisensi)
- [Kredit & Penghargaan](#-kredit--penghargaan)

---

## 🏫 Tentang SIRA

**SIRA** adalah singkatan dari **Sistem Informasi Razia** — sebuah aplikasi web satu halaman (*single-page application*) yang dirancang sebagai platform terpadu untuk mencatat dan memantau **seluruh bentuk pelanggaran tata tertib siswa** di **SMKN 1 Malteng**.

Kata "Razia" dalam nama SIRA bukan berarti aplikasi ini hanya digunakan saat razia rutin. SIRA dirancang lebih luas dari itu: mencakup **razia barang terlarang, pelanggaran seragam, kasus kedisiplinan, pelanggaran atribut, kenakalan siswa, kasus perundungan, ketidakhadiran, dan berbagai bentuk pelanggaran tata tertib lainnya** yang terjadi sehari-hari di lingkungan sekolah.

Aplikasi ini dibangun sebagai satu file HTML tunggal yang dapat dijalankan langsung di browser mana pun — tidak memerlukan instalasi, tidak memerlukan koneksi internet aktif, dan tidak memerlukan server backend sama sekali. Seluruh data tersimpan secara lokal di perangkat pengguna menggunakan `localStorage`.

### Filosofi SIRA

> *"Satu siswa. Satu rekam jejak. Semua pelanggaran tercatat."*

SIRA dibangun di atas keyakinan bahwa **setiap pelanggaran perlu didokumentasikan secara konsisten** — bukan hanya untuk keperluan hukuman, tetapi untuk membantu guru BK, wali kelas, dan pihak sekolah memahami pola perilaku siswa secara menyeluruh dan mengambil tindakan pembinaan yang tepat.

---

## 📌 Latar Belakang

Di banyak sekolah menengah kejuruan, penanganan pelanggaran siswa masih dilakukan secara terpisah dan tidak terstruktur. Guru tatib mencatat di buku besar, guru BK menyimpan di file berbeda, wali kelas memiliki catatannya sendiri — tidak ada satu sumber data yang bisa dijadikan acuan bersama.

Masalah konkret yang kerap terjadi:

- 📂 **Data tersebar** — catatan pelanggaran ada di buku, kertas, grup WA, dan memori masing-masing guru
- 🔍 **Sulit ditelusuri** — riwayat lengkap seorang siswa tidak bisa diakses dalam hitungan detik
- 📉 **Tidak ada pola** — tidak terlihat apakah seorang siswa semakin membaik atau semakin bermasalah
- 📵 **Tidak ada alarm otomatis** — siswa yang sudah berkali-kali melanggar tidak langsung terdeteksi
- 🗑️ **Rentan hilang** — buku catatan bisa rusak, tertinggal, atau terbakar
- 🤝 **Tidak ada koordinasi** — tatib, BK, dan wali kelas tidak selalu berbagi informasi yang sama
- ⏱️ **Lambat** — proses mencatat manual saat razia di lapangan membuang waktu

SIRA lahir untuk menjawab semua masalah ini dengan satu solusi ringan yang bisa langsung digunakan tanpa birokrasi teknis.

---

## 📚 Cakupan Pelanggaran

SIRA **tidak terbatas** pada razia HP semata. Sistem ini dirancang untuk mencatat **semua jenis pelanggaran tata tertib** yang terjadi di sekolah, antara lain:

### 📵 Razia Barang Terlarang
- Membawa dan menggunakan HP saat KBM
- Membawa rokok, vape, atau zat terlarang
- Membawa senjata tajam atau benda berbahaya
- Membawa barang yang tidak berkaitan dengan pembelajaran

### 👔 Pelanggaran Seragam & Atribut
- Tidak memakai seragam sesuai ketentuan
- Tidak menggunakan dasi, ikat pinggang, atau atribut wajib
- Memakai seragam tidak rapi atau dimodifikasi
- Memakai sepatu yang tidak sesuai aturan
- Rambut tidak sesuai ketentuan sekolah

### ⏰ Kedisiplinan & Kehadiran
- Terlambat masuk sekolah atau kelas
- Membolos sebagian atau seluruh hari
- Keluar kelas tanpa izin saat KBM berlangsung
- Tidak mengikuti upacara atau kegiatan wajib sekolah

### 🤝 Perilaku & Etika
- Bersikap tidak sopan kepada guru atau staf
- Melakukan perundungan (*bullying*) terhadap sesama siswa
- Terlibat perkelahian atau kekerasan fisik
- Melakukan tindakan vandalisme terhadap fasilitas sekolah
- Menyontek atau berlaku curang saat ujian
- Membuat keributan dan mengganggu ketertiban kelas

### 🌐 Pelanggaran Digital
- Mengakses konten tidak pantas menggunakan perangkat sekolah
- Menyebarkan konten negatif di media sosial yang mencemarkan nama sekolah
- Penyalahgunaan akun atau sistem informasi sekolah

### 📋 Pelanggaran Administrasi
- Tidak mengumpulkan tugas atau laporan tepat waktu berulang kali
- Memalsukan tanda tangan orang tua atau dokumen sekolah
- Tidak memenuhi persyaratan praktik atau PKL

> ℹ️ **Catatan:** Kolom "Kronologi" pada form SIRA bersifat bebas teks, sehingga petugas dapat mencatat jenis pelanggaran apapun secara deskriptif sesuai situasi di lapangan.

---

## ✨ Fitur Lengkap

### 🗂️ Manajemen Pelanggaran

| Fitur | Deskripsi |
|---|---|
| **Registrasi Pelanggaran Baru** | Form lengkap dengan validasi: nama siswa, kelas, jurusan, nomor HP siswa & orang tua, serta kronologi pelanggaran secara detail |
| **Deteksi Siswa Duplikat** | Jika nama dan kelas siswa sudah terdaftar, sistem otomatis menambahkan pelanggaran ke riwayat yang sudah ada — tidak membuat data ganda |
| **Tambah Pelanggaran Cepat** | Tombol ⚡ TAMBAH di kartu siswa untuk mencatat pelanggaran berikutnya tanpa mengisi ulang seluruh form |
| **Dua Kategori Tindakan** | Setiap pencatatan pelanggaran dikategorikan: **SITA** (barang atau bukti disita) atau **CATAT SAJA** (hanya dicatat tanpa penyitaan) |
| **Riwayat Lengkap Per Siswa** | Setiap siswa memiliki timeline riwayat pelanggaran dengan tanggal, deskripsi, dan kategori tindakan |
| **Edit Data Siswa** | Klik nama siswa untuk membuka modal edit dan memperbarui semua informasi |
| **Hapus Data Siswa** | Hapus data siswa secara permanen dengan dialog konfirmasi |

### 📊 Dashboard & Statistik

| Fitur | Deskripsi |
|---|---|
| **Quick Stats Real-time** | 3 kartu statistik yang selalu diperbarui: Total Siswa Tercatat, Jumlah Barang Disita, Jumlah Kasus Selesai |
| **3 Status Penanganan** | `TIADA` — tidak ada sitaan, `BELUM` — barang masih ditahan (kartu berborder merah menyala), `SELESAI` — barang sudah dikembalikan |
| **Toggle Status Cepat** | Tombol 🔄 STATUS untuk merotasi status penanganan siswa secara instan |

### 🔔 Sistem Peringatan & Eskalasi

| Fitur | Deskripsi |
|---|---|
| **Deteksi Pelanggaran 3x+** | Sistem otomatis menandai siswa yang telah tercatat melanggar sebanyak 3 kali atau lebih |
| **Panel Notifikasi Khusus** | Panel tersendiri yang menampilkan daftar siswa yang wajib mendapat panggilan orang tua |
| **Badge Penanda di Header** | Indikator merah yang menampilkan jumlah siswa bermasalah secara real-time |
| **Navigasi Cepat ke Kartu** | Klik nama siswa di panel notifikasi untuk langsung menuju kartu siswa tersebut di halaman utama |

### 🔍 Filter & Pencarian

| Fitur | Deskripsi |
|---|---|
| **Pencarian Real-time** | Cari siswa berdasarkan nama, kelas, atau jurusan dengan debounce 150ms agar tidak memberatkan browser |
| **Filter per Kelas** | Dropdown untuk menampilkan hanya siswa dari kelas tertentu |
| **Filter per Jurusan** | Dropdown untuk menampilkan hanya siswa dari jurusan tertentu |
| **Tombol Hapus Cepat** | Tombol ✕ pada kolom pencarian untuk mengosongkan filter seketika |
| **Filter Kombinasi** | Pencarian teks, filter kelas, dan filter jurusan dapat digunakan secara bersamaan |

### ⚙️ Panel Admin

| Fitur | Deskripsi |
|---|---|
| **Kelola Kelas Dinamis** | Tambah, edit, dan hapus opsi kelas tanpa menyentuh kode |
| **Kelola Jurusan Dinamis** | Tambah, edit, dan hapus opsi jurusan tanpa menyentuh kode |
| **Sinkronisasi Instan** | Setiap perubahan konfigurasi langsung diterapkan ke seluruh form, filter, dan tampilan tanpa perlu reload |
| **Persistensi Konfigurasi** | Pengaturan kelas dan jurusan tersimpan di `localStorage` secara terpisah dari data siswa |

### 💬 Integrasi WhatsApp

| Fitur | Deskripsi |
|---|---|
| **Pesan Otomatis ke Orang Tua** | Generate link WhatsApp dengan pesan terformat otomatis berisi nama siswa, kelas, jurusan, jumlah pelanggaran, dan kronologi terakhir |
| **Normalisasi Nomor HP** | Otomatis mengkonversi format `08xx` menjadi `628xx` yang valid untuk WhatsApp |
| **Penguncian Otomatis** | Tombol WA hanya aktif untuk siswa yang sudah melanggar 3x atau lebih — mencegah kontak orang tua sebelum diperlukan |
| **Maintenance Mode** | Flag bawaan untuk menonaktifkan sementara fitur WA dengan modal informasi yang ramah pengguna |

### 📱 UI & UX

| Fitur | Deskripsi |
|---|---|
| **Dark Mode Penuh** | Tema gelap konsisten dengan palet `slate-900` / `slate-950` yang nyaman di mata saat digunakan lama |
| **Mobile-First Responsive** | Dirancang untuk layar HP terlebih dahulu, dengan bottom navigation bar khusus perangkat mobile |
| **Custom Select Dropdown** | Komponen dropdown kustom yang lebih estetis dan konsisten dibanding `<select>` bawaan browser |
| **Shimmer Skeleton Loading** | Animasi placeholder saat aplikasi pertama kali memuat data |
| **Infinite Scroll** | Kartu siswa dimuat secara bertahap (10 per batch) menggunakan `IntersectionObserver` agar halaman tetap ringan |
| **Toast Notification** | Notifikasi pop-up ringan di pojok bawah layar untuk setiap aksi yang dilakukan |
| **Animasi Modal Halus** | Efek masuk dan keluar yang natural pada semua dialog modal |
| **Error Boundary Global** | Tampilan fallback yang informatif jika terjadi error kritis, dengan tombol muat ulang |

---

## 🛠️ Teknologi yang Digunakan

```
SIRA dibangun hanya dengan teknologi web standar —
tanpa framework berat, tanpa proses build, tanpa dependensi eksternal yang rumit.
```

| Teknologi | Keterangan |
|---|---|
| **HTML5** | Struktur dan semantik halaman |
| **Tailwind CSS (CDN)** | Utility-first styling, dimuat via `cdn.tailwindcss.com` |
| **Vanilla JavaScript (ES2020+)** | Seluruh logika aplikasi, tanpa framework |
| **localStorage API** | Penyimpanan data lokal di browser |
| **IntersectionObserver API** | Implementasi infinite scroll yang efisien |
| **Custom Events API** | Komunikasi antar komponen internal aplikasi |
| **Google Fonts (CDN)** | Font `Inter` untuk tipografi |

> ⚠️ **Catatan:** Tailwind CSS dimuat via CDN untuk mempertahankan sifat *single-file* dari aplikasi ini. Untuk deployment skala besar, disarankan beralih ke Tailwind CLI dengan proses purge CSS agar ukuran file lebih kecil.

---

## 🗂️ Struktur Aplikasi

Meskipun SIRA adalah satu file HTML, kode JavaScript di dalamnya terstruktur rapi menggunakan paradigma **Object-Oriented Programming berbasis kelas**:

```
SIRA.html
│
├── 🎨 Struktur HTML
│   ├── Header (Logo + Tombol Notifikasi + Tombol Admin)
│   ├── Konten Utama
│   │   ├── Quick Stats Cards
│   │   ├── Form Registrasi Pelanggaran
│   │   ├── Filter Kelas, Filter Jurusan & Search Bar
│   │   └── Container Kartu Siswa (Infinite Scroll)
│   ├── Panel Notifikasi (Pelanggaran 3x+)
│   ├── Modal Tindakan (SITA / CATAT)
│   ├── Modal Edit Data Siswa
│   ├── Modal Reset Database
│   ├── Modal Maintenance WhatsApp
│   ├── Toast Notification
│   ├── Bottom Navigation Bar (Mobile)
│   └── Admin Panel (Kelas & Jurusan)
│
└── ⚙️ Kelas JavaScript
    ├── ConfigManager       → Kelola & simpan konfigurasi kelas dan jurusan
    ├── StorageService      → Abstraksi CRUD ke localStorage
    ├── ToastSystem         → Tampilkan notifikasi toast
    ├── Validator           → Validasi input form & skema data
    ├── StudentModel        → Model data dan behavior siswa
    ├── DOMInjector         → Isi opsi ke elemen <select>
    ├── CustomSelect        → Bangun komponen dropdown kustom
    ├── DOMRenderer         → Render kartu, statistik, dan notifikasi
    └── AppController       → Orkestrator utama seluruh aplikasi
```

---

## 🚀 Cara Menjalankan

SIRA tidak memerlukan proses instalasi apapun. Langsung buka dan pakai.

### Metode 1: Clone & Buka

```bash
# Clone repositori
git clone https://github.com/username/SIRA.git

# Masuk ke folder
cd SIRA

# Buka di browser
# Windows:
start index.html

# macOS:
open index.html

# Linux:
xdg-open index.html
```

### Metode 2: Download ZIP

1. Klik tombol **Code → Download ZIP** di halaman repositori ini
2. Ekstrak file ZIP ke folder mana saja
3. Buka file `index.html` langsung dengan browser

### Metode 3: Local Server (Opsional)

Jika ingin menjalankan melalui server lokal:

```bash
# Python 3
python -m http.server 8000

# Node.js
npx serve .

# PHP
php -S localhost:8000
```

Buka `http://localhost:8000` di browser.

### Kompatibilitas Browser

| Browser | Versi Minimum | Status |
|---|---|---|
| Google Chrome | 80+ | ✅ Didukung Penuh |
| Mozilla Firefox | 75+ | ✅ Didukung Penuh |
| Microsoft Edge | 80+ | ✅ Didukung Penuh |
| Safari | 13+ | ✅ Didukung Penuh |
| Opera | 67+ | ✅ Didukung Penuh |
| Internet Explorer | Semua | ❌ Tidak Didukung |

> 💡 **Rekomendasi:** Gunakan Google Chrome versi terbaru untuk pengalaman terbaik.

---

## 📖 Panduan Penggunaan

### 1. Mencatat Pelanggaran Baru

1. Isi **Nama Lengkap** siswa (minimal 3 karakter)
2. Pilih **Kelas** dari dropdown
3. Pilih **Jurusan** dari dropdown
4. Isi **HP Siswa** — opsional, hanya angka
5. Isi **HP Orang Tua (WA)** — opsional, dibutuhkan untuk fitur notifikasi WhatsApp
6. Isi kolom **Kronologi** dengan deskripsi lengkap pelanggaran (minimal 5 karakter)
7. Klik tombol **Simpan Data**
8. Di modal tindakan, pilih salah satu:
   - **SITA HP** → Barang disita, status siswa menjadi `BELUM`
   - **CATAT SAJA** → Hanya dicatat tanpa penyitaan

> ℹ️ **Deteksi Duplikat:** Jika nama dan kelas siswa sudah pernah terdaftar sebelumnya, sistem akan otomatis menambahkan pelanggaran baru ke riwayat siswa tersebut tanpa membuat entri baru. Kartu siswa juga akan dipindahkan ke urutan paling atas.

### 2. Menambah Pelanggaran pada Siswa yang Sudah Terdaftar

1. Temukan kartu siswa di daftar
2. Klik tombol ⚡ **TAMBAH** pada kartu
3. Isi deskripsi pelanggaran baru di kotak dialog
4. Pilih tindakan: **SITA** atau **CATAT SAJA**
5. Riwayat siswa akan langsung diperbarui

### 3. Mengubah Status Penanganan

Klik tombol 🔄 **STATUS** di kartu siswa untuk merotasi status:

```
TIADA  →  BELUM  →  SELESAI  →  TIADA  → ...
```

| Status | Arti | Tampilan Kartu |
|---|---|---|
| `TIADA` | Tidak ada barang yang disita | Border normal |
| `BELUM` | Barang disita, belum dikembalikan | Border merah menyala + badge animasi |
| `SELESAI` | Barang sudah dikembalikan | Badge hijau |

### 4. Mengedit Data Siswa

1. Klik langsung pada **nama siswa** di kartu
2. Modal edit terbuka dengan data yang sudah terisi
3. Ubah informasi yang diperlukan
4. Klik **Simpan**

### 5. Menghapus Data Siswa

1. Klik ikon 🗑️ di pojok kanan atas kartu siswa
2. Konfirmasi penghapusan pada dialog
3. Data dihapus permanen dari sistem

### 6. Mencari dan Memfilter Data

- Ketik di **kolom pencarian** untuk mencari berdasarkan nama, kelas, atau jurusan
- Pilih kelas di dropdown **Semua Kelas** untuk memfilter per tingkat
- Pilih jurusan di dropdown **Semua Jurusan** untuk memfilter per program studi
- Ketiga filter dapat digunakan secara bersamaan dan saling melengkapi

### 7. Menggunakan Panel Notifikasi

1. Klik ikon 🔔 di header — badge merah menunjukkan jumlah siswa bermasalah
2. Panel menampilkan daftar siswa dengan 3 pelanggaran atau lebih
3. Klik nama siswa untuk langsung menavigasi ke kartunya
4. Klik ikon 💬 untuk langsung membuka WhatsApp orang tua siswa tersebut

### 8. Menghubungi Orang Tua via WhatsApp

1. Pastikan nomor HP orang tua sudah terisi di data siswa
2. Klik tombol **WHATSAPP** di kartu siswa
3. Browser akan membuka WhatsApp Web atau aplikasi WhatsApp dengan pesan yang sudah otomatis terformat

Contoh pesan yang digenerate:
```
Halo, saya dari SMKN 1 Malteng. Menginfokan bahwa siswa atas nama *Budi Santoso*
(Kelas: *X - TJKT 1*) telah melakukan pelanggaran ke-3.

Kronologi terakhir: Kedapatan membawa HP saat KBM dan menolak dikumpulkan
```

> ⚠️ Tombol WhatsApp hanya aktif jika siswa sudah memiliki **minimal 3 pelanggaran** dan fitur tidak sedang dalam mode maintenance.

### 9. Reset Seluruh Database

1. Klik tombol **Reset** di bottom navigation bar (perangkat mobile)
2. Pada modal konfirmasi, **ketik `HAPUS`** (huruf kapital) untuk verifikasi
3. Seluruh data dihapus permanen

> ⛔ **Peringatan Keras:** Tindakan ini tidak dapat dibatalkan dan tidak bisa dipulihkan. Pastikan data sudah dibackup sebelum melakukan reset.

---

## ⚙️ Konfigurasi Admin

Panel admin memungkinkan penyesuaian daftar kelas dan jurusan secara dinamis tanpa perlu mengubah kode satu baris pun.

### Membuka Panel Admin

Klik ikon **⚙️ (sliders)** di pojok kanan atas header aplikasi.

### Mengelola Kelas

| Aksi | Langkah |
|---|---|
| **Tambah Kelas** | Klik `+ Tambah` → Masukkan kode kelas (contoh: `XIII`) → Konfirmasi |
| **Edit Kelas** | Klik `✏️ Edit` di samping kelas → Masukkan nama baru → Konfirmasi |
| **Hapus Kelas** | Klik `🗑️ Hapus` di samping kelas → Konfirmasi penghapusan |

### Mengelola Jurusan

Prosedur identik dengan pengelolaan kelas, namun di kolom Jurusan.

> ⚠️ **Penting:** Menghapus kelas atau jurusan dari konfigurasi **tidak** menghapus data siswa yang sudah tercatat menggunakan kelas/jurusan tersebut. Hanya menghapus opsi dari form registrasi dan filter.

### Data Konfigurasi Bawaan

**Kelas Default:**
```
X  |  XI  |  XII
```

**Jurusan Default:**
```
TJKT 1  |  TJKT 2  |  TK 1  |  TK 2  |  MPLB  |  AKL  |  Pemasaran  |  ULP
```

---

## 🏗️ Arsitektur Kode

### Alur Data Aplikasi

```
Aksi Pengguna
      │
      ▼
AppController  ←─── attachGlobalListeners() (Event Delegation + Custom Events)
      │
      ├──► Submit Form Baru
      │         └── Validator.validateStudent()
      │                  └── StudentModel (baru atau existing)
      │                           └── StudentModel.addViolation()
      │                                    └── StorageService.save()
      │                                             └── DOMRenderer.refreshUI()
      │
      ├──► Quick Add (Tambah Cepat)
      │         └── prompt() → StudentModel.addViolation() → StorageService.save()
      │
      ├──► Filter / Search
      │         └── AppController.refreshUI(reset=true)
      │                  └── DOMRenderer.clearList() + DOMRenderer.appendCards()
      │
      ├──► Toggle Status
      │         └── StudentModel.toggleStatus() → StorageService.save()
      │
      └──► Perubahan Konfigurasi Admin
                └── ConfigManager.addItem / editItem / removeItem
                         └── AppController.instantSync()
                                  └── DOMInjector → CustomSelect → refreshUI()
```

### Penjelasan Tiap Kelas

#### `ConfigManager` — Manajer Konfigurasi
Mengelola daftar kelas dan jurusan yang tersimpan di `localStorage` dengan key `app_config`. Jika tidak ada data tersimpan, otomatis menggunakan konfigurasi default. Bersifat statik (semua method adalah `static`).

```javascript
// Contoh penggunaan
ConfigManager.addItem('kelas', 'XIII', 'XIII')
ConfigManager.editItem('jurusan', 'TJKT 1', 'TJKT 3', 'TJKT 3')
ConfigManager.removeItem('kelas', 'XIII')
ConfigManager.loadConfig()  // → { KELAS_OPTIONS: [...], JURUSAN_OPTIONS: [...] }
```

#### `StorageService` — Layanan Penyimpanan
Abstraksi lengkap atas `localStorage` untuk data siswa. Menangani error `QuotaExceededError` dan memvalidasi bahwa data yang disimpan selalu berupa array.

```javascript
StorageService.save(arrayOfStudents)   // → true / throw Error
StorageService.load()                  // → array of raw objects
StorageService.clear()                 // → true
```

#### `StudentModel` — Model Data Siswa
Merepresentasikan satu siswa beserta seluruh riwayat pelanggarannya. Menyediakan method untuk menambah pelanggaran dan mengubah status sitaan.

```javascript
const siswa = new StudentModel({ nama: 'Budi', kelas: 'X', jurusan: 'TJKT 1', ... })
siswa.addViolation('Membawa HP saat ujian', 'SITA')
siswa.toggleStatus()  // TIADA → BELUM → SELESAI → TIADA
```

#### `Validator` — Validator Input
Memvalidasi data form sebelum disimpan. Mengembalikan objek `{ valid: boolean, errors: {} }`.

Aturan validasi:
| Field | Aturan |
|---|---|
| Nama | Wajib, 3–100 karakter |
| Kelas | Wajib diisi |
| Jurusan | Wajib diisi |
| Kronologi | Wajib, minimal 5 karakter |
| HP Siswa | Opsional, hanya angka jika diisi |
| HP Orang Tua | Opsional, hanya angka jika diisi |

#### `DOMRenderer` — Renderer Tampilan
Mengelola semua operasi DOM: render kartu siswa, statistik, dan panel notifikasi. Menggunakan `DocumentFragment` untuk batch insert yang efisien dan `IntersectionObserver` untuk infinite scroll.

#### `AppController` — Kontroler Utama
Bertindak sebagai orkestrator yang menghubungkan semua komponen. Menggunakan pola *event delegation* untuk satu event listener global dan *Custom Events* untuk komunikasi antar komponen secara loosely coupled.

---

## 💾 Penyimpanan Data

### Skema Data Siswa

```json
{
  "id": "ID-1710000000000-abc123xyz",
  "nama": "Budi Santoso",
  "kelas": "X",
  "jurusan": "TJKT 1",
  "telpSiswa": "081234567890",
  "telpOrtu": "081298765432",
  "statusSitaan": "BELUM",
  "history": [
    {
      "timestamp": "2024-03-15T08:30:00.000Z",
      "reason": "Membawa dan menggunakan HP saat ujian semester",
      "mode": "SITA"
    },
    {
      "timestamp": "2024-02-10T10:15:00.000Z",
      "reason": "Terlambat masuk sekolah lebih dari 30 menit tanpa keterangan",
      "mode": "CATAT"
    }
  ]
}
```

### Skema Data Konfigurasi

```json
{
  "KELAS_OPTIONS": [
    { "value": "X", "label": "X" },
    { "value": "XI", "label": "XI" },
    { "value": "XII", "label": "XII" }
  ],
  "JURUSAN_OPTIONS": [
    { "value": "TJKT 1", "label": "TJKT 1" },
    { "value": "AKL", "label": "AKL" }
  ]
}
```

### Kunci localStorage

| Key | Berisi | Ukuran Estimasi |
|---|---|---|
| `RAZIA_APP_V6` | Array seluruh data siswa | ~500 byte per siswa |
| `app_config` | Konfigurasi kelas dan jurusan | < 5 KB |

### Estimasi Kapasitas

`localStorage` memiliki batas **~5 MB** per domain/file. Dengan ukuran rata-rata ~500 byte per siswa (termasuk riwayat pelanggaran), SIRA dapat menampung hingga sekitar **10.000 entri siswa** sebelum mendekati batas penyimpanan.

---

## 🔐 Keamanan & Privasi

### Perlindungan XSS

Seluruh input pengguna disanitasi menggunakan fungsi `Utils.sanitize()` sebelum dirender ke dalam DOM, sehingga mencegah serangan *Cross-Site Scripting (XSS)*:

```javascript
sanitize: (str) => {
    const t = document.createElement('div');
    t.textContent = str;   // Karakter berbahaya di-escape otomatis
    return t.innerHTML;
}
```

### Privasi Data

- ✅ Seluruh data **hanya ada di perangkat lokal** pengguna
- ✅ Tidak ada transfer data ke server manapun
- ✅ Tidak ada tracking, analytics, atau telemetri tersembunyi
- ✅ Tidak ada cookies yang dibuat
- ✅ Tidak memerlukan akun, login, atau autentikasi
- ✅ Tidak ada ketergantungan pada layanan pihak ketiga untuk fungsionalitas inti

### Catatan Keamanan Tambahan

> ⚠️ Karena SIRA berjalan sebagai file lokal tanpa autentikasi, **siapapun yang memiliki akses ke perangkat** dapat membaca dan memodifikasi data. Untuk lingkungan dengan kebutuhan keamanan tinggi, pertimbangkan untuk menambahkan fitur PIN (ada di roadmap v7.0).

---

## ⚠️ Keterbatasan

| Keterbatasan | Penjelasan |
|---|---|
| **Satu Perangkat** | Data tidak tersinkronisasi antar perangkat. Setiap perangkat menyimpan datanya masing-masing |
| **Tidak Ada Backup Otomatis** | Data hilang permanen jika pengguna menghapus cache atau data browser |
| **Tanpa Autentikasi** | Tidak ada perlindungan akses — siapapun yang membuka file bisa melihat dan mengubah data |
| **Kapasitas Terbatas** | localStorage dibatasi ~5 MB per domain |
| **Belum Ada Ekspor** | Belum tersedia fitur ekspor ke Excel atau PDF (masuk roadmap) |
| **WA dalam Maintenance** | Fitur kirim WhatsApp saat ini dinonaktifkan sementara via flag internal |
| **Tidak Ada Multi-User** | Tidak ada sistem peran (tatib, BK, wali kelas) — semua pengguna memiliki akses penuh |

---

## 🗺️ Rencana Pengembangan

### v6.2 — Ekspor & Laporan
- [ ] Ekspor seluruh data ke format Excel (.xlsx)
- [ ] Cetak kartu pelanggaran individual sebagai PDF
- [ ] Laporan rekap per kelas dan per jurusan

### v6.3 — WhatsApp Aktif
- [ ] Aktifkan penuh fitur pengiriman pesan WhatsApp ke orang tua
- [ ] Template pesan yang dapat dikustomisasi dari admin panel

### v7.0 — Keamanan & Multi-Device
- [ ] Perlindungan PIN / password sederhana
- [ ] Sinkronisasi data melalui Google Sheets sebagai backend gratis
- [ ] Import / Export data via file JSON untuk backup manual

### v7.5 — Analitik & Laporan Lanjutan
- [ ] Grafik tren pelanggaran per bulan
- [ ] Peringkat siswa dengan pelanggaran terbanyak
- [ ] Laporan rekap otomatis mingguan dan bulanan
- [ ] Filter berdasarkan jenis pelanggaran / kategori

### v8.0 — Progressive Web App (PWA)
- [ ] Service Worker untuk dukungan offline penuh
- [ ] Instalasi ke home screen perangkat
- [ ] Push notification pengingat tindak lanjut

### v9.0 — Multi-Role & Kolaborasi
- [ ] Sistem peran: Tatib, Guru BK, Wali Kelas, Kepala Sekolah
- [ ] Catatan dan anotasi per pelanggaran oleh beberapa guru
- [ ] Alur persetujuan tindakan untuk kasus berat

---

## 🤝 Kontribusi

Kontribusi dalam bentuk apapun sangat diterima dan diapresiasi!

### Melaporkan Bug

1. Buka tab [Issues](https://github.com/username/SIRA/issues)
2. Klik **New Issue** dan pilih template **Bug Report**
3. Sertakan informasi berikut:
   - Browser dan versinya
   - Langkah-langkah untuk mereproduksi bug
   - Apa yang diharapkan vs apa yang terjadi
   - Screenshot atau rekaman layar jika memungkinkan

### Mengajukan Fitur Baru

1. Buka tab [Issues](https://github.com/username/SIRA/issues)
2. Klik **New Issue** dan pilih template **Feature Request**
3. Jelaskan fitur yang diinginkan, kasus penggunaannya, dan manfaatnya

### Mengajukan Pull Request

```bash
# 1. Fork repositori ini ke akun GitHub Anda

# 2. Clone hasil fork
git clone https://github.com/USERNAME_ANDA/SIRA.git

# 3. Buat branch baru dari main
git checkout -b fitur/nama-fitur-anda

# 4. Lakukan perubahan pada kode

# 5. Commit dengan pesan yang deskriptif
git commit -m "feat: tambah fitur ekspor data ke Excel"

# 6. Push branch ke fork Anda
git push origin fitur/nama-fitur-anda

# 7. Buka Pull Request ke repositori utama melalui GitHub
```

### Konvensi Pesan Commit

Gunakan format [Conventional Commits](https://www.conventionalcommits.org/):

| Prefix | Digunakan untuk |
|---|---|
| `feat:` | Penambahan fitur baru |
| `fix:` | Perbaikan bug |
| `docs:` | Perubahan dokumentasi saja |
| `style:` | Perubahan tampilan / CSS |
| `refactor:` | Refaktor kode tanpa perubahan fungsionalitas |
| `perf:` | Optimasi performa |
| `chore:` | Perubahan konfigurasi, tooling, atau build |

---

## 📄 Lisensi

```
MIT License

Copyright (c) 2024 SMKN 1 Malteng

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```

Lihat file [LICENSE](LICENSE) untuk teks lengkap.

---

## 🙏 Kredit & Penghargaan

- **[Tailwind CSS](https://tailwindcss.com/)** — Framework CSS utility-first yang digunakan untuk seluruh tampilan
- **[Google Fonts](https://fonts.google.com/)** — Font `Inter` untuk tipografi yang bersih dan mudah dibaca
- **[Heroicons](https://heroicons.com/)** — Koleksi ikon SVG yang digunakan di seluruh antarmuka
- Seluruh **guru, staf tata tertib, dan tim BK SMKN 1 Malteng** — atas masukan nyata dari lapangan yang menjadi fondasi desain SIRA

---

<div align="center">

Dibuat dengan ❤️ untuk SMKN 1 Malteng

*"Satu rekam jejak yang jelas adalah awal dari pembinaan yang benar."*

**[⬆ Kembali ke Atas](#-sira--sistem-informasi-razia)**

</div>
