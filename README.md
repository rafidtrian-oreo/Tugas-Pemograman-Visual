# 🛒 Aplikasi Penjualan Toko (Tugas Pemrograman Visual)

Aplikasi desktop berbasis Java Swing untuk mengelola data transaksi penjualan, pelanggan, barang, dan nota secara terintegrasi dengan database MySQL.

---

## 👤 Identitas Mahasiswa
* **Nama:** Rafid Trian Rifadi
* **NPM:** 202343500988
* **Kelas:** X6G
* **Mata Kuliah:** Pemrograman Visual

---

## 🚀 Fitur Utama Aplikasi
* **Sistem Login Multi-user:** Mengamankan akses aplikasi berdasarkan akun kasir/admin.
* **Manajemen Data Barang & Pelanggan:** Fitur CRUD (Create, Read, Update, Delete) data master.
* **Form Transaksi Nota:** Menghitung total belanja, quantity, kembalian, dan cetak detail nota otomatis.
* **Auto-Number ID Nota:** Generator kode nota otomatis (`IN0001`, `IN0002`, dst.) agar data tidak bentrok.

---

## 🛠️ Teknologi & Tools yang Digunakan
* **Bahasa Pemrograman:** Java (JDK 8)
* **IDE:** NetBeans IDE
* **Database:** MySQL (XAMPP / phpMyAdmin)
* **Driver:** MySQL JDBC Connector

---

## 📦 Struktur Database (`pelanggan`)
Aplikasi ini menggunakan database bernama **`pelanggan`** dengan beberapa tabel utama:
1. `nota` - Menyimpan data utama ringkasan nota transaksi.
2. `detail_nota` - Menyimpan rincian barang, harga, dan QTY yang dibeli pada setiap nota.
3. `barang` - Menyimpan master data barang/produk.
4. `pelanggan` - Menyimpan data master pelanggan.

---

## 🏃 Menjalankan Project di Lokal

1. **Clone Repositori Ini:**
   ```bash
   git clone [https://github.com/rafidtrian-oreo/Tugas-Pemograman-Visual.git](https://github.com/rafidtrian-oreo/Tugas-Pemograman-Visual.git)
