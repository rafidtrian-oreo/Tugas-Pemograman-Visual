# 📦 README - Aplikasi Data Barang (Java NetBeans)

## 📌 Deskripsi Project

Project ini merupakan aplikasi desktop berbasis **Java Swing** yang digunakan untuk mengelola data barang dalam sebuah sistem penjualan sederhana. Aplikasi ini terhubung dengan database MySQL dan mendukung operasi CRUD (Create, Read, Update, Delete).

Aplikasi dibuat menggunakan **NetBeans IDE** dan menggunakan koneksi database melalui JDBC.

---

## 🧱 Struktur Project

```
Tugas-Pemograman-Visual/
│
├── src/
│   ├── Pelanggan/
│   │   ├── barang.java       → Form utama data barang
│   │   ├── barang.form       → Desain GUI (NetBeans)
│   │   ├── Pelanggan.java    → (kemungkinan form lain)
│   │   └── Pelanggan.form
│   │
│   └── koneksi/
│       └── koneksi.java      → Koneksi ke database MySQL
│
├── nbproject/                → Konfigurasi project NetBeans
├── build.xml                 → File build (Ant)
└── manifest.mf              → Konfigurasi manifest
```

---

## ⚙️ Teknologi yang Digunakan

* Java (Swing GUI)
* MySQL Database
* JDBC (Java Database Connectivity)
* NetBeans IDE
* Apache Ant (build tool)

---

## 🗄️ Konfigurasi Database

### 1. Nama Database

```
penjualan
```

### 2. Tabel yang Digunakan

Tabel: `barang`

### 3. Struktur Tabel (SQL)

```sql
CREATE TABLE barang (
    id_barang VARCHAR(10) PRIMARY KEY,
    nama_barang VARCHAR(100),
    jenis VARCHAR(50),
    harga_beli INT,
    harga_jual INT
);
```

---

## 🔌 Konfigurasi Koneksi Database

File: `koneksi/koneksi.java`

```java
String url = "jdbc:mysql://localhost:3306/penjualan";
Connection conn = DriverManager.getConnection(url, "root", "");
```

📌 Catatan:

* Username: `root`
* Password: kosong (default XAMPP)
* Driver: `com.mysql.jdbc.Driver` (versi lama, bisa diganti ke `com.mysql.cj.jdbc.Driver` jika error)

---

## 🚀 Fitur Aplikasi

### ✅ 1. Tambah Data Barang

* Input ID Barang
* Nama Barang
* Jenis (Makanan / Minuman)
* Harga Beli
* Harga Jual
* Simpan ke database

---

### 🔍 2. Tampilkan Data

* Semua data barang ditampilkan dalam tabel
* Data diambil dari database

---

### 🔎 3. Pencarian Data

* Berdasarkan:

  * Nama Barang
  * Jenis Barang

---

### ✏️ 4. Update Data

* Klik data pada tabel
* Edit data
* Klik tombol **Ubah**

---

### ❌ 5. Hapus Data

* Pilih data
* Klik tombol **Hapus**
* Konfirmasi penghapusan

---

### 🔄 6. Reset Form

* Tombol **Batal** untuk mengosongkan form

---

### 🚪 7. Keluar Aplikasi

* Tombol **Keluar**

---

## 🖥️ Tampilan UI

Form utama berisi:

* Input field (ID, Nama, Jenis, Harga)
* ComboBox jenis barang
* Tombol aksi:

  * Simpan
  * Ubah
  * Hapus
  * Batal
  * Keluar
* Tabel data barang
* Fitur pencarian

---

## 🔁 Alur Program

1. Aplikasi dijalankan
2. Koneksi ke database dibuat
3. Data ditampilkan di tabel (`datatable()`)
4. User dapat:

   * Menambah data
   * Mengedit data
   * Menghapus data
   * Mencari data

---

## 🛠️ Cara Menjalankan Project

### 1. Import Project ke NetBeans

* File → Open Project
* Pilih folder project

### 2. Setup Database

* Jalankan MySQL (XAMPP)
* Import / buat database `penjualan`
* Buat tabel `barang`

### 3. Jalankan Program

* Klik Run (F6)

---

## 👨‍💻 Author

Project ini dibuat oleh rafidtrian

---
