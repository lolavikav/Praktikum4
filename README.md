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

# 1.Fungsi
```
Hitung_nilai_akhir (tugas, uts, uas):
```

```python
def hitung_nilai_akhir(tugas, uts, uas):
    return (tugas * 0.30) + (uts * 0.35) + (uas * 0.35)
```

# 2. Fungsi
tampilkan_daftar (daftar_mahasiswa):

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



