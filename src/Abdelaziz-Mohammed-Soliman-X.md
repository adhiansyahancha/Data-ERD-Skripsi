# Teks deskripsi

Toko X memiliki banyak tenaga penjualan (salesperson) untuk menjual beberapa komoditasnya di sekitar dunia. Kebijakan toko menyatakan bahwa setiap tenaga penjualan diizinkan untuk menjual komoditas toko di setiap wilayah. Lebih lanjut lagi, beberapa tenaga penjualan diizinkan untuk menjual komoditas di wilayah yang sama. Dalam kasus ini, setiap tenaga penjualan dapat mematok harga yang berbeda untk setiap jenis komoditas.

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

relationship KomSales {
}

relationship Komwil {
Harga
}

relationship SalesWil {
}

Salesperson -N- SalesWil
SalesWil -M- Wilayah

Komoditas -N- Komwil 
Komwil -M- Wilayah

Komoditas -N- KomSales
KomSales -M- Salesperson

@endchen
```

# Lisensi

[Frontiers in Education]([https://emisa-journal.org/emisa/article/view/318](https://www.frontiersin.org/journals/education/articles/10.3389/feduc.2025.1554089/full)) mengizinkan di bawah [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/)
