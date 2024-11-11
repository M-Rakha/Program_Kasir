# Program Kasir

Program kasir ini dibuat untuk memudahkan proses transaksi penjualan, dengan fitur-fitur seperti menambah barang ke keranjang, menampilkan daftar barang, menghitung total harga, dan mencetak struk belanja.

## Struktur Data

Program ini menggunakan tiga kelas utama untuk mengorganisir data :

## Kelas Barang
Kelas Barang digunakan untuk menyimpan informasi setiap barang yang dijual.

```python
class Barang:
    def __init__(self, kode, nama, harga):
        self.kode = kode    # String - kode unik barang
        self.nama = nama    # String - nama barang
        self.harga = harga  # Integer - harga barang
```

### Penjelasan :
- kode: Menyimpan kode unik untuk setiap barang, yang dapat digunakan untuk mengidentifikasi dan mencari barang.
- nama: Menyimpan nama barang.
- harga: Menyimpan harga jual barang.


