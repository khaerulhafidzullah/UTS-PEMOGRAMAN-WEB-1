# 📚 StoryVerse - Modern Online Book Store

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)

**StoryVerse** adalah prototipe aplikasi *e-commerce* toko buku online berbasis antarmuka web (Front-End) yang dirancang dengan konsep **Modern Creative, Playful, dan Estetik**. 

Project ini dibuat untuk memenuhi tugas **UTS Pemrograman Web 1**, dibangun **100% menggunakan Vanilla HTML, CSS, dan JavaScript murni** (tanpa framework seperti React, Bootstrap, atau Tailwind) serta menggunakan `localStorage` sebagai simulasi database (*State Management*).

## ✨ Fitur Utama

Aplikasi ini dibagi menjadi dua sisi: **Sisi Pengunjung (Publik)** dan **Sisi Admin**.

### 🛒 Sisi Pengunjung (Publik)
- **Katalog Interaktif:** Menampilkan grid buku dengan desain *card* modern. Buku yang kehabisan stok akan otomatis berubah menjadi *grayscale* (abu-abu) dengan tombol dinonaktifkan.
- **Sistem Keranjang (Cart):** Pengunjung dapat menambahkan buku ke keranjang. Terdapat validasi stok real-time (tidak bisa menambah barang melebihi stok yang ada).
- **Checkout & Generate Resi:** Proses checkout otomatis menghitung subtotal, memotong stok dari database, dan membuat Nomor Resi/Delivery Order (DO) unik.
- **Pelacakan Pesanan (Tracking):** Halaman pelacakan paket menggunakan UI *Timeline* visual yang dinamis. Status akan berubah (*Diproses* -> *Dikirim*) sesuai dengan update dari sisi Admin.

### ⚙️ Sisi Admin (Dashboard)
- **Otentikasi Login:** Halaman login dengan *split-screen layout* dan animasi CSS.
- **Dashboard Statistik:** Ringkasan total buku, total pesanan masuk, dan estimasi pendapatan secara real-time.
- **Manajemen Inventaris (CRUD):** 
  - Tambah, Edit, dan Hapus buku melalui Modal interaktif.
  - Tampilan inventaris menggunakan *Card List* dengan *badge* status stok dinamis.
- **History Pesanan (Order Management):** Admin dapat melihat daftar pesanan yang masuk dan memperbarui status pengiriman (*Kirim Paket*), yang otomatis terhubung ke halaman Tracking publik.
- **Toast Notification:** Notifikasi interaktif (berhasil/gagal) pada setiap aksi.

## 📁 Struktur Folder

```text
book-store/
├── login.html           # Halaman Login Admin
├── dashboard.html