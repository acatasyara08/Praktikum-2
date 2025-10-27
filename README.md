program mencari bilangan terbesar 

# 🧮 Program Mencari Bilangan Terbesar

Program ini dibuat menggunakan bahasa **Python** untuk menentukan **bilangan terbesar** dari empat buah bilangan yang dimasukkan oleh pengguna.  
Program menggunakan **percabangan `if`** untuk melakukan perbandingan antar bilangan tanpa menggunakan fungsi bawaan seperti `max()`.

---

## 📋 Fitur Program
- Menerima input **4 buah bilangan** dari pengguna.
- Menentukan bilangan yang paling **besar** menggunakan logika perbandingan manual.
- Menampilkan semua bilangan yang dimasukkan serta hasil bilangan terbesar.

---

## 💻 Kode Program

```python
print("=== Program Mencari Bilangan Terbesar ===")
print("Masukkan 4 buah bilangan:")

# Input 4 bilangan
bil1 = float(input("Bilangan 1: "))
bil2 = float(input("Bilangan 2: "))
bil3 = float(input("Bilangan 3: "))
bil4 = float(input("Bilangan 4: "))

# Mencari bilangan terbesar menggunakan statement if
terbesar = bil1

if bil2 > terbesar:
    terbesar = bil2

if bil3 > terbesar:
    terbesar = bil3

if bil4 > terbesar:
    terbesar = bil4

# Menampilkan hasil
print("\n=== HASIL ===")
print(f"Bilangan yang dimasukkan: {bil1}, {bil2}, {bil3}, {bil4}")
print(f"Bilangan terbesar adalah: {terbesar}")





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
