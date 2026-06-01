# 🌴 Sawit Tracker — Aplikasi Pencatat Hasil Panen Sawit

Aplikasi web ringan berbasis browser untuk mencatat, memantau, dan menganalisis hasil panen kelapa sawit secara pribadi. Tidak memerlukan server, instalasi, maupun koneksi internet untuk digunakan.

---

## ✨ Fitur Utama

### 📊 Dashboard
- Ringkasan statistik bulan ini: total berat panen, pendapatan kotor, total upah, dan pendapatan bersih
- 4 grafik interaktif: tren berat panen bulanan, tren pendapatan bersih, distribusi panen per lokasi, dan pergerakan harga sawit
- Banner pengingat jadwal panen otomatis berdasarkan interval yang dikonfigurasi
- Tabel 5 panen terakhir

### ✏️ Catat Panen
Form input lengkap meliputi:
- Tanggal panen
- Lokasi kebun (dari daftar yang dikonfigurasi)
- Harga sawit (Rp/kg) dari pengepul
- Berat hasil panen (kg)
- Nama tukang panen
- Biaya upah panen (Rp/kg)
- **Total upah, pendapatan kotor, dan pendapatan bersih dihitung otomatis**
- Catatan tambahan (opsional)

### 📋 Riwayat Panen
- Tabel semua catatan panen
- Filter berdasarkan lokasi, bulan, dan nama tukang
- Fitur edit dan hapus per data

### 📄 Laporan & Export
- Filter laporan berdasarkan rentang tanggal dan lokasi
- **Export ke PDF** — laporan berformat tabel siap cetak
- **Export ke Excel (.xlsx)** — untuk analisis lanjutan atau backup data

### ⚙️ Pengaturan
- Konfigurasi interval jadwal panen (mis. setiap 20 hari)
- Kelola daftar lokasi kebun (tambah / hapus)

---

## 🚀 Cara Penggunaan

### Opsi 1: Langsung dari File (Lokal)
1. Download file `index.html`
2. Buka di browser Chrome atau Firefox
3. Aplikasi siap digunakan — data tersimpan di browser

### Opsi 2: GitHub Pages (Direkomendasikan)
Agar bisa diakses dari HP dan laptop manapun:

1. Daftar akun di [github.com](https://github.com) (gratis)
2. Buat repository baru, beri nama mis. `sawit-tracker`, pilih **Public**
3. Upload file `index.html`, rename menjadi `index.html`, lalu klik **Commit**
4. Buka **Settings → Pages → Source**, pilih branch `main` → **Save**
5. Aplikasi tersedia di: `https://username.github.io/sawit-tracker`

### Opsi 3: Netlify Drop
1. Buka [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag & drop file `index.html` ke halaman tersebut
3. Aplikasi langsung online dengan URL otomatis

---

## ⚠️ Catatan Penting tentang Data

Aplikasi ini menggunakan **IndexedDB** — storage bawaan browser. Data tersimpan **per perangkat per browser**, artinya:

| Kondisi | Hasil |
|---|---|
| Buka di HP yang sama, browser sama | ✅ Data tetap ada |
| Buka di browser berbeda (HP sama) | ❌ Data kosong |
| Buka di perangkat lain | ❌ Data kosong |

**Rekomendasi:** Gunakan satu perangkat utama sebagai tempat input data, dan lakukan **export ke Excel secara rutin** sebagai backup.

---

## 🛠️ Teknologi

| Komponen | Teknologi |
|---|---|
| Frontend | HTML5, CSS3, Vanilla JavaScript |
| Database | IndexedDB (browser built-in) |
| Grafik | Chart.js 4.4 |
| Export PDF | jsPDF + jsPDF-AutoTable |
| Export Excel | SheetJS (xlsx) |
| Font | Plus Jakarta Sans, DM Mono |
| Hosting | GitHub Pages / Netlify (opsional) |

Tidak ada framework, tidak ada server, tidak ada biaya — cukup satu file HTML.

---

## 📁 Struktur File

```
sawit-tracker/
└── index.html     ← Seluruh aplikasi dalam satu file
```

---

## 🔄 Update Aplikasi

Jika ada versi baru:
1. Download file `index.html` terbaru
2. **Export data lama ke Excel terlebih dahulu** (sebagai backup)
3. Ganti file lama dengan yang baru
4. Data di IndexedDB tetap aman selama nama domain/file tidak berubah

---

## 📝 Lisensi

Dibuat untuk penggunaan pribadi. Bebas dimodifikasi sesuai kebutuhan.

---

*Dikembangkan dengan bantuan Claude (Anthropic) · 2025*
