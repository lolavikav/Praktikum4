# Praktikum4

# BIODATA
## Nama  : Lola Seftyliani
## Kelas : TI.24.A.4
## Nim   : 312410339

# input dan output dari praktikum5

# input 

![code](https://github.com/user-attachments/assets/5a2c2a26-4369-41e1-9fb5-b27855d94f24)

# output

![Screenshot 2024-11-14 160427](https://github.com/user-attachments/assets/911fd121-1920-44d3-b805-dbd5c6269046)

# flowchart

![WhatsApp Image 2024-11-14 at 16 05 40_bd0785b0](https://github.com/user-attachments/assets/ce45982a-3c11-4158-8399-6c8f62c33ea9)

# 1.Fungsi `Hitung_nilai_akhir (tugas, uts, uas):`

```python
def hitung_nilai_akhir(tugas, uts, uas):
    return (tugas * 0.30) + (uts * 0.35) + (uas * 0.35)
```

# 2. Fungsi `tampilkan_daftar (daftar_mahasiswa):`

```python
def tampilkan_daftar(daftar_mahasiswa):
    print("=" * 70)  # Membuat garis pembatas
    print("| No |     Nama      |    NIM    | Tugas | UTS | UAS | Akhir |")
    print("=" * 70)  # Membuat garis pembatas
```

- Menerima parameter berupa list yang berisi data mahasiswa
- Membuat tampilan tabel dengan header
- Menggunakan perulangan untuk menampilkan setiap data mahasiswa
- Format output menggunakan string formatting untuk merapikan tampilan
- enumerate(daftar_mahasiswa, 1) digunakan untuk membuat penomoran mulai dari 1

# 3. Fungsi `main():`

```python
def main():
    daftar_mahasiswa = []  # Inisialisasi list kosong
```

- Fungsi utama program
- Membuat list kosong untuk menyimpan data mahasiswa

# 4. Input Data dan Validasi

```python
while True:
    print("\nMasukkan data mahasiswa")
    nama = input("Nama : ")
    nim = input("NIM : ")
    
    while True:
        try:
            tugas = float(input("Nilai Tugas : "))
            if 0 <= tugas <= 100:
                break
            print("Nilai harus antara 0-100!")
        except ValueError:
            print("Masukkan nilai yang valid!")
```

- Menggunakan nested while loop untuk input dan validasi
- Try-except untuk menangani input nilai yang tidak valid
- Validasi rentang nilai (0-100)
- Proses yang sama dilakukan untuk nilai UTS dan UAS

# 5. Menyimpan Data:

```python
# Hitung nilai akhir
nilai_akhir = hitung_nilai_akhir(tugas, uts, uas)

# Tambahkan ke daftar
mahasiswa = {
    'nama': nama,
    'nim': nim,
    'tugas': tugas,
    'uts': uts,
    'uas': uas,
    'nilai_akhir': nilai_akhir
}
daftar_mahasiswa.append(mahasiswa)
```

- Memanggil fungsi hitung_nilai_akhir
- Membuat dictionary untuk menyimpan data satu mahasiswa
- Menambahkan dictionary ke dalam list daftar_mahasiswa

# 6. Konfirmasi Tambah Data:

```python
tambah = input("\nTambah data (y/t)? ")
if tambah.lower() != 'y':
    break
```

- Meminta konfirmasi untuk menambah data lagi
- Jika input bukan 'y', keluar dari loop

# 7. Menampilkan Hasil:

```python
print("\nDaftar Nilai Mahasiswa:")
tampilkan_daftar(daftar_mahasiswa)
```

- Memanggil fungsi tampilkan_daftar untuk menampilkan semua data

# 8. Entry Point Program:

```python
if _name_ == "_main_":
    main()
```

- Memastikan fungsi main() hanya dijalankan jika file dijalankan langsung
- Tidak akan dijalankan jika file di-import sebagai modul

Fitur-fitur Program:

1. Dapat menambahkan data mahasiswa secara dinamis
2. Validasi input untuk nilai (harus numerik dan 0-100)
3. Perhitungan nilai akhir otomatis dengan bobot yang ditentukan
4. Tampilan output dalam bentuk tabel yang rapi
5. Penanganan error untuk input yang tidak valid
6. Konfirmasi untuk menambah data baru

Program ini dibuat untuk memudahkan pengelolaan data nilai mahasiswa dengan interface yang user-friendly dan penanganan error yang baik.




