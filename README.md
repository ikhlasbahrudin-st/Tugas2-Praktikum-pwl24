<p align="center">
  <a href="https://laravel.com" target="_blank">
    <img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="420" alt="Laravel Logo">
  </a>
</p>

<p align="center">
  <img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status">
  <img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads">
  <img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Version">
  <img src="https://img.shields.io/packagist/l/laravel/framework" alt="License">
</p>

---

# 📚 Sistem Informasi Perpustakaan

## 📌 Tentang Project
Sistem Informasi Perpustakaan ini adalah aplikasi berbasis web yang dibangun menggunakan **Laravel Framework** untuk mengelola data perpustakaan seperti buku, rak buku, kategori, peminjaman, dan pengembalian secara terstruktur.

Project ini dibuat untuk kebutuhan **tugas praktikum Pemrograman Web Lanjut (PWL)**.

---

## ⚙️ Fitur Utama

### 📘 Manajemen Buku
- Tambah, edit, hapus data buku
- Upload cover buku
- Relasi dengan rak buku

### 📚 Manajemen Rak Buku
- Pengelompokan buku berdasarkan rak
- Kode rak unik

### 🏷 Kategori Buku
- Pengelompokan kategori buku

### 📦 Peminjaman Buku
- Transaksi peminjaman
- Multi buku dalam 1 transaksi
- Tracking status peminjaman

### 🔁 Pengembalian Buku
- Proses pengembalian
- Update status otomatis
- Sistem denda (charge & amount)

### 👤 Manajemen User
- Data pengguna / peminjam

---

## 🧠 Relasi Database
- Book → Bookshelf (Many to One)
- Book → Category (Optional pengembangan)
- Loan → User (Many to One)
- Loan → LoanDetail (One to Many)
- LoanDetail → Book (Many to One)
- Return → LoanDetail (One to One)

---

## 🛠️ Teknologi yang Digunakan
- Laravel Framework
- PHP 8+
- MySQL
- Composer
- Node.js (Vite)
- Git & GitHub

---

## 🚀 Cara Instalasi

```bash
git clone https://github.com/ikhlasbahrudin-st/Tugas3-praktikum-PWL24.git
cd Tugas3-praktikum-PWL24
composer install
npm install
cp .env.example .env
php artisan key:generate
