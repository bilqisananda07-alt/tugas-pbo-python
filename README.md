# 🛒 Sistem Manajemen Stok Warung (Python OOP)

Program sederhana berbasis Python yang menerapkan konsep dasar Object-Oriented Programming (OOP), khususnya Enkapsulasi, penggunaan Getter & Setter, serta validasi data.

---

## 📌 Fitur Utama & Konsep OOP
- Enkapsulasi Atribut Private: Menggunakan `__harga` dan `__stok` untuk mencegah akses atau perubahan data secara langsung dari luar class.
- Getter: Method `get_harga()` dan `get_stok()` untuk mengambil/membaca nilai atribut private dengan aman.
- Setter dengan Validasi: Method `set_harga()` dan `set_stok()` untuk mengubah nilai atribut dengan pengujian input (mencegah nilai negatif).

---

## 💻 Cara Menjalankan Program

1. Pastikan Python sudah terinstal di komputer/laptop kamu.
2. Clone repository ini:
   ```bash
   git clone [https://github.com/bilqisananda07/tugas-pbo-python.git](https://github.com/bilqisananda07/tugas-pbo-python.git)
3. Jalankan file warung.py:

python warung.py

Analisis Masalah & Solusi (Enkapsulasi)
​Masalah (Tanpa Enkapsulasi): 
Jika atribut harga dan stok bersifat publik, data bisa diubah sembarangan dari luar (misal: item.harga = -5000). Hal ini dapat merusak logika program dan menyebabkan kerugian transaksi.
​Solusi (Dengan Setter): Dengan menggunakan metode Setter, setiap perubahan nilai disaring menggunakan logika kondisi if. Perubahan hanya diproses jika data valid (harga > 0 dan stok >= 0). Jika input bernilai negatif, sistem akan menolak perubahan data secara otomatis.