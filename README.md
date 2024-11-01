# latihan praktikum 1
 Latihan 3: Buat program python untuk kasus berikut:

Kasus 1: Program Pemesanan Tiket Bioskop

Buat program yang menghitung harga tiket bioskop. Tiket reguler berharga Rp50.000, sedangkan tiket VIP berharga Rp100.000. Jika user memiliki kartu member, mereka mendapatkan diskon 20% dari harga tiket. Program ini harus meminta tipe tiket dan status member dari user, lalu menghitung total harga yang harus dibayar.

Petunjuk:

Gunakan if else dan operator ternary.

## cara kerja program
- Program meminta pengguna untuk memasukkan tipe tiket (reguler atau VIP) dan status keanggotaan (ya atau tidak).
- Berdasarkan tipe tiket yang dipilih, program menetapkan harga tiket yang sesuai (Rp50.000 untuk reguler dan Rp100.000 untuk VIP).
- Jika tipe tiket tidak valid, program mencetak pesan kesalahan dan menetapkan harga tiket menjadi 0.
- Jika pengguna memiliki kartu member dan harga tiket valid, program menghitung diskon 20% dari harga tiket.
- Total harga yang harus dibayar kemudian ditampilkan, dengan format dua angka desimal, jika harga tiket lebih dari 0.

## kode progam 
``` python
# Fungsi untuk menghitung total harga tiket
def hitung_harga_tiket():
    # Meminta input dari pengguna
    tipe_tiket = input("Masukkan tipe tiket (reguler/VIP): ").lower()
    status_member = input("Apakah Anda memiliki kartu member? (ya/tidak): ").lower()

    # Menentukan harga tiket berdasarkan tipe
    if tipe_tiket == "reguler":
        harga_tiket = 40000
    elif tipe_tiket == "vip":
        harga_tiket = 150000
    else:
        print("Tipe tiket tidak valid!")
        return  # Pastikan untuk mengembalikan dari fungsi jika tipe tidak valid
    
    # Menghitung diskon jika pengguna adalah member
    diskon = 0.2 if status_member == "ya" else 0
    total_harga = harga_tiket * (1 - diskon)

    # Menampilkan total harga
    print(f"Total harga yang harus dibayar: Rp{total_harga:.2f}")

# Memanggil fungsi
hitung_harga_tiket()
```
## output program 
``` python
Masukkan tipe tiket (reguler/VIP): VIP
Apakah Anda memiliki kartu member? (ya/tidak): ya
Total harga yang harus dibayar: Rp120000.00
PS C:\Users\NANDA>
```
## flowchart latihan 1



