




program mengurutkan data dari terkecil - terbesar .py

# 🧮 Program Mengurutkan Data dari Terkecil ke Terbesar

Program ini dibuat menggunakan bahasa **Python** untuk mengurutkan sejumlah data numerik yang dimasukkan oleh pengguna, kemudian menampilkan hasilnya secara **berurutan dari nilai terkecil hingga terbesar**.

---

## 📋 Fitur Program
- Meminta input jumlah data yang ingin dimasukkan oleh pengguna.
- Melakukan **validasi** agar jumlah data minimal 2.
- Menginput data satu per satu.
- Mengurutkan data menggunakan fungsi bawaan Python `sort()`.
- Menampilkan hasil pengurutan dengan rapi di layar.

---

## 💻 Cara Menjalankan Program

1. Pastikan kamu sudah menginstal **Python** (versi 3.x).
2. Simpan kode berikut dalam file bernama `urutkan_data.py`:
   ```python
   # Program Mengurutkan Data dari Terkecil ke Terbesar

   print("Program Mengurutkan Data dari Terkecil ke Terbesar")

   # Meminta jumlah data dari pengguna
   jumlah_data = int(input("Masukkan jumlah data (minimal 2): "))

   # Validasi jumlah data minimal 2
   if jumlah_data < 2:
       print("Jumlah data harus minimal 2!")
   else:
       data = []  # membuat list kosong untuk menyimpan data

       # Input data satu per satu
       for i in range(jumlah_data): 
           nilai = float(input(f"Masukkan data ke-{i+1}: "))
           data.append(nilai)

       # Mengurutkan data
       data.sort()

       # Menampilkan hasil
       print("\nData setelah diurutkan (dari terkecil ke terbesar):")
       for nilai in data:
           print(nilai)
