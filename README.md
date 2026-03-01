# KuisPintar

**KuisPintar** adalah sebuah aplikasi web interaktif berbasis kuis yang dirancang untuk memberikan pengalaman belajar dan menguji pengetahuan pengguna melalui berbagai kuis. Aplikasi ini memiliki dua peran utama, yaitu **User** (Pengguna) dan **Admin** (Administrator).

## 🚀 Fitur Utama

### 👨‍💻 Fitur Pengguna (User)
- **Otentikasi**: Login dan Register untuk pengguna baru.
- **Beranda (Landing Page)**: Halaman utama yang menampilkan ringkasan aplikasi.
- **Kuis**: Modul untuk mengerjakan kuis secara interaktif.
- **Leaderboard**: Papan peringkat untuk melihat skor tertinggi antar pengguna.
- **Papan Hasil (Result Page)**: Menampilkan hasil dan evaluasi setelah mengerjakan kuis.
- **Pembelajaran Saya (My Learning)**: Riwayat pembelajaran dan kuis yang telah diambil oleh pengguna.

### 🔐 Fitur Administrator (Admin)
- **Manajemen Pengguna (User Management)**: Mengelola data pengguna yang terdaftar di sistem.
- **Manajemen Peran (Role Management)**: Mengatur peran dan hak akses untuk pengguna.
- **Manajemen Kuis (Quiz Management)**: Menambah, mengedit, dan menghapus kuis beserta pertanyaannya.

## 🛠️ Teknologi yang Digunakan

Proyek ini dibangun menggunakan teknologi web modern berbasis ekosistem React:

- **[React](https://react.dev/) (v19)**: Library antarmuka pengguna (UI) utama berbasis komponen.
- **[Vite](https://vitejs.dev/)**: *Build tool* dan *development server* yang sangat cepat.
- **[React Router DOM](https://reactrouter.com/) (v7)**: Manajemen rute (routing) untuk navigasi Single Page Application (termasuk penerapan *Route Guards* untuk proteksi halaman).
- **[Tailwind CSS](https://tailwindcss.com/) (v4)**: *Utility-first CSS framework* untuk mempercepat proses *styling* dan membuat desain responsif.
- **[Framer Motion](https://www.framer.com/motion/)**: Library animasi untuk memberikan efek transisi visual web yang dinamis dan interaktif.
- **[Axios](https://axios-http.com/)**: HTTP client untuk kemudahan dalam mengonsumsi layanan API dari backend.
- **[React Icons](https://react-icons.github.io/react-icons/) & [@iconify/react](https://iconify.design/)**: Kumpulan dan pengelola ikon berbasis komponen React.
- **[ESLint](https://eslint.org/)**: Linter untuk menjaga standar dan konsistensi kualitas kode JavaScript/React.

## 📂 Struktur Direktori Proyek

Berikut adalah penjelasan fungsi direktori di dalam `src/`:

```
src/
├── assets/       # Tempat menyimpan aset statis seperti gambar (logo, ilustrasi).
├── Components/   # Komponen UI independen dan reusable (seperti Tombol, Input, Kartu), termasuk Route Guards.
├── context/      # React Context untuk manajemen state global secara efisien (contoh: Auth state).
├── Layouts/      # Layout kerangka halaman persisten (seperti MainLayout dan AdminLayout).
├── lib/          # File utilitas pembantu, helper, atau konfigurasi pihak ketiga.
├── Pages/        # Halaman-halaman penuh sesuai dengan routing aplikasi (seperti LoginPage, QuizPage, dll).
├── Sections/     # Kelompok potongan komponen besar pembentuk suatu halaman (seperti HeroSection).
├── services/     # Pusat layanan API untuk berkomunikasi ke backend agar kode komponen lebih bersih.
├── App.jsx       # Registrasi utama routing (menghubungkan komponen Route atau Guards ke Pages).
├── main.jsx      # Titik masukan utama (entry point) me-render React App ke DOM.
└── index.css     # File CSS dasar untuk reset gaya awal dan import Tailwind.
```

## 💻 Panduan Menjalankan Proyek Secara Lokal

Ikuti langkah-langkah di bawah ini untuk memulai pengembangan secara lokal:

1. **Persiapan**: Pastikan sistem Anda telah terinstal [Node.js](https://nodejs.org/).
2. **Kloning Repositori**:
   ```bash
   git clone <URL_REPOSITORY>
   cd KuisPintar
   ```
3. **Instalasi Dependensi**:
   Jalankan perintah ini untuk mengunduh semua library yang diperlukan:
   ```bash
   npm install
   ```
4. **Jalankan *Development Server***:
   Memulai aplikasi mode pengembangan dengan HMR:
   ```bash
   npm run dev
   ```
5. Akses url lokal yang disediakan di terminal (secara umum di `http://localhost:5173`) menggunakan *browser* favorit Anda.

## 📦 Skrip NPM

Anda dapat mengeksekusi skrip ini dari terminal:
- `npm run dev` : Menjalankan server lokal pengembangan.
- `npm run build` : Membuat bundel aplikasi siap edar untuk *production*.
- `npm run lint` : Mengaudit dan mencari kemungkinan masalah di kode (Linting).
- `npm run preview` : Mensimulasikan aplikasi *production build* di server lokal.
