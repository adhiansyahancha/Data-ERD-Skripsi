# Teks deskripsi

Toko Y memiliki banyak tenaga penjualan (salesperson) yang bertugas menjual berbagai komoditasnya di berbagai wilayah di dunia. Kebijakan toko menetapkan bahwa setiap wilayah hanya dilayani oleh satu tenaga penjualan, yang bertugas menjual seluruh komoditas toko secara eksklusif di wilayah tersebut. Seorang tenaga penjualan diperbolehkan mendistribusikan komoditas di banyak wilayah. Harga setiap komoditas ditetapkan secara berbeda di setiap wilayah.

# ERD Acuan

```uml
@startchen

entity Komoditas {
Nomor
Nama
}

entity Salesperson {
Nomor
Nama
}

entity Wilayah {
Nomor
Nama
}

relationship jual {
}

relationship Komwil {
Harga
}

Salesperson -1- jual
jual -N- Wilayah

Komoditas -N- Komwil 
Komwil -N- Wilayah

@endchen
```

# Lisensi

[Frontiers in Education](https://www.frontiersin.org/journals/education/articles/10.3389/feduc.2025.1554089/full) mengizinkan di bawah [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/)
