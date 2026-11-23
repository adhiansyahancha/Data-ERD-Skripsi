# Teks deskripsi

Departemen Transportasi ingin menyimpan data pengemudi dan kendarannya. Departemen ini hanya berfokus pada pengemudi kendaraan saat ini dan juga hanya berfokus pada kendaraan yang sedang dioperasikan oleh pengemudi tersebut. Seorag pengemudi mengoperasikan paling banyak satu kendaraan dan satu kendaraan dioperasikan oleh paling banyak satu pengemudi. Pengemudi harus memiliki lisensi pengemudi, nama (yang terdiri dari nama pertama dan nama terakhir), sedangkan kendaraan harus memiliki nomor plat, VIN, tahun pembuatan, warna, pembuat, dan model. VIN adalah nomor identifikasi kendaraan dan bersifat unik untuk setiap kendaraan.

(Catatan: Ini merupakan modifikasi dari pertanyaan 8 yang menggunakan hubungan 1-1, pertanyaan aslinya sebenarnya merupakan modifikasi juga dari contoh pada subbab "One-to-One")

# ERD Acuan

```uml
@startchen

entity Pengemudi {
  Nama {
    Pertama
    Akhir
}
  SIM <<key>>
}

entity Kendaraan {
  VIN <<key>>
  NomorPlat <<key>>
  TahunPembuatan
  Pembuat
  Warna
  Model
}

relationship mengoperasikan {
}

Pengemudi =1- mengoperasikan
mengoperasikan -1- Kendaraan

@endchen
```

# Lisensi

[Ron McFadyen dari Applied Computer Science Department, University of Winnipeg](https://www.acs.uwinnipeg.ca/rmcfadyen/CreativeCommons/) mengizinkan di bawah [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/)
