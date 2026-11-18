# Teks deskripsi

Toko Y memiliki banyak tenaga penjualan (salesperson) untuk menjual beberapa komoditasnya di sekitar dunia. Kebijakan toko menyatakan bahwa setiap wilayah hanya memiliki satu tenaga penjualan yang menjual seluruh komoditas toko secara eksklusif. Seorang tenaga penjualan diizinkan untuk mendistribusikan di banyak wilayah. Harga setiap komoditas diatur berbeda untuk setiap wilayah.

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

[Frontiers in Education]([https://emisa-journal.org/emisa/article/view/318](https://www.frontiersin.org/journals/education/articles/10.3389/feduc.2025.1554089/full)) mengizinkan di bawah [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/)
