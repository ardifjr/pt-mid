# PT Multyartha Indo Daya - Web Company Profile & Showcase

Repositori ini berisi *source code* untuk pengembangan situs web *Company Profile* resmi **PT Multyartha Indo Daya (PT MID)**, sebuah perusahaan kontraktor terkemuka, sekaligus menjadi etalase digital untuk **Apartment Bandung Technoplex Living**.

Proyek ini bertujuan untuk mendigitalisasi profil perusahaan dengan mengutamakan **keamanan maksimal (Anti-Deface)**, performa muat yang sangat cepat, serta kemudahan pemeliharaan melalui arsitektur modern *Static Site Generation* (SSG).

---

## 🏢 Tinjauan Proyek (Non-Teknis)

Situs web ini dirancang untuk memenuhi kebutuhan informasi publik dan *marketing*, dengan cakupan fitur operasional sebagai berikut:
1. **Profil Perusahaan:** Memuat Identitas, Visi & Misi, Struktur Organisasi, serta Legalitas PT MID.
2. **Layanan Utama:** Informasi mendetail terkait jasa *Building Design*, *Mechanical*, dan *Electrical*.
3. **Portofolio Proyek:** Galeri dokumentasi (foto dan video) untuk proyek yang sedang berjalan (*On Going*) dan yang sudah selesai (*Completed*).
4. **Showcase Apartemen:** Etalase unit Apartment Bandung Technoplex Living yang interaktif (ketersediaan unit, spesifikasi material, dan denah tipe kamar).
5. **Pusat Edukasi:** Referensi artikel industri, seperti inovasi "Smart Building".
6. **Kontak & Lokasi:** Informasi *Contact Person* dan integrasi peta interaktif dengan alamat resmi kantor: `Jl. Telekomunikasi No.1, Sukapura, Kec. Dayeuhkolot, Kabupaten Bandung, Jawa Barat 40267`.

---

## 💻 Spesifikasi Teknis (Tech Stack)

Situs ini dibangun menggunakan pendekatan **Jamstack** (JavaScript, API, Markup) untuk memastikan tidak ada celah keamanan komputasi server (seperti *SQL Injection*):
* **Core Framework:** [Astro.js](https://astro.build/) (SSG - *Zero JavaScript by default*)
* **Styling:** [Tailwind CSS](https://tailwindcss.com/)
* **Konten & Artikel:** Markdown (`.md`) / JSON Data
* **Manajemen Versi:** Git & GitHub
* **Deployment (Rencana):** Vercel / Cloudflare Pages

---

## 📂 Struktur Direktori

```text
📁 pt-mid-company-profile
├── 📁 public           # Aset statis yang dapat diakses publik (Logo, Gambar PDF, Favicon)
├── 📁 src
│   ├── 📁 components   # Komponen UI modular (Navbar, Footer, ProjectCard)
│   ├── 📁 data         # Dummy data / JSON spesifikasi unit apartemen
│   ├── 📁 layouts      # Kerangka utama HTML (BaseLayout)
│   ├── 📁 pages        # Rute halaman (index.astro, about.astro, dll)
│   └── 📁 styles       # Konfigurasi CSS global / Tailwind
├── 📄 .gitignore       # Daftar file yang diabaikan Git
├── 📄 astro.config.mjs # File konfigurasi utama Astro
├── 📄 package.json     # Daftar dependensi proyek
└── 📄 README.md        # Dokumentasi proyek
```
---

## 🚀 Panduan Instalasi & Pengembangan Lokal

Bagi tim developer yang ingin menjalankan proyek ini di mesin lokal, silakan ikuti langkah-langkah berikut:
1. Clone Repositori:
```git clone [https://github.com/username-kamu/pt-mid-company-profile.git](https://github.com/username-kamu/pt-mid-company-profile.git)```
2. Masuk ke Direktori Proyek:
```cd pt-mid-company-profile```
3. Instalasi Dependensi:
Pastikan Anda telah menginstal Node.js versi LTS.
```npm install```
4. Jalankan Server Development:
```npm run dev```
5. Akses http://localhost:4321 melalui peramban web Anda.

---

## 🤝 Alur Kolaborasi (Git Flow)
Untuk menjaga kerapian kode antara developer, ikuti aturan branching berikut:
1. main : Branch utama, khusus untuk kode yang sudah final dan siap deploy ke produksi.
2. dev : Branch pengembangan utama. Semua fitur baru digabungkan ke sini terlebih dahulu.
3. Fitur Branch : Buat branch baru dari dev saat mengerjakan fitur spesifik.
4. Format penamaan: feature/nama-fitur (Contoh: feature/navbar, feature/portfolio).

Cara membuat branch fitur baru:
```git checkout dev
git pull origin dev
git checkout -b feature/nama-fitur
```

© 2026 PT Multyartha Indo Daya. All rights reserved. Dikembangkan secara internal oleh tim Web Developer Intern.
