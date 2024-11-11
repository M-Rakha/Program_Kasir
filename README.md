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

### Implementasi:

- Saat membuat program kasir, kita perlu membuat objek Barang untuk setiap jenis barang yang dijual, dengan menyediakan kode, nama, dan harga.
- Objek Barang ini akan digunakan di seluruh program, terutama saat menambahkan barang ke keranjang dan menampilkan daftar barang.

## Kelas ItemKeranjang

Kelas ItemKeranjang digunakan untuk menyimpan detail setiap item dalam keranjang belanja.

```python
class ItemKeranjang:
    def __init__(self, barang, jumlah):
        self.barang = barang      # Objek Barang
        self.jumlah = jumlah      # Integer - jumlah barang
        self.subtotal = barang.harga * jumlah  # Integer - total harga
```

### Penjelasan:

- barang: Menyimpan objek Barang yang terkait dengan item ini.
- jumlah: Menyimpan jumlah barang yang dibeli.
- subtotal: Menghitung dan menyimpan total harga untuk item ini.

### Implementasi:

- Saat menambahkan barang ke keranjang, kita akan membuat objek ItemKeranjang yang menghubungkan objek Barang dengan jumlah yang dibeli.
- Objek ItemKeranjang ini akan digunakan untuk menampilkan daftar barang dalam keranjang dan menghitung total harga belanja.

## Kelas Keranjang

Kelas Keranjang digunakan untuk menyimpan daftar barang yang dibeli oleh pelanggan.

```python
class Keranjang:
    def __init__(self):
        self.items = []  # List - menyimpan item belanjaan
```

### Penjelasan:

- items: Menyimpan daftar objek ItemKeranjang yang merepresentasikan barang-barang yang ada dalam keranjang.

### Implementasi:

- Saat pelanggan menambahkan barang ke keranjang, kita akan membuat objek ItemKeranjang dan menambahkannya ke dalam daftar items di objek Keranjang.
- Objek Keranjang akan digunakan untuk menampilkan daftar barang, menghitung total harga, dan mencetak struk belanja.


