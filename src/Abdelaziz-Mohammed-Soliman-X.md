# Teks deskripsi

Toko X memiliki banyak tenaga penjualan (salesperson) yang bertugas menjual berbagai komoditasnya di berbagai wilayah di dunia. Kebijakan toko menetapkan bahwa setiap tenaga penjualan diperbolehkan menjual komoditas toko di setiap wilayah. Selain itu, beberapa tenaga penjualan diperbolehkan menjual komoditas yang sama di wilayah yang sama. Dalam kasus ini, setiap tenaga penjualan dapat menetapkan harga yang berbeda untuk setiap jenis komoditas.

# ERD Acuan

```uml
@startchen

entity Komoditas {
ID
Nama
}

entity Salesperson {
ID
Nama
}

entity Wilayah {
ID
Nama
}

relationship jual {
Harga
}

jual -N- Komoditas
jual -N- Salesperson
jual -N- Wilayah

@endchen
```

# Lisensi

[Frontiers in Education](https://www.frontiersin.org/journals/education/articles/10.3389/feduc.2025.1554089/full) mengizinkan di bawah [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/)
