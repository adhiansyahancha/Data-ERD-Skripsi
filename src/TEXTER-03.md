# Teks deskripsi

Sebuah model kibor (papan ketik komputer) dideskripsikan dengan nama model, kode internal, dan tahun dirilis. Model-model kibor memiliki ukuran yang beragam yang mencerminkan tata letak (layout) dan tujuan penggunaannya yang berbeda-beda. Model kibor dilengkapi dengan satu jenis switch yang menentukan suara dan rasa mengetik. Sebuah switch dideskripsikan dengan nama, gaya aktuasi, dan rasa menekan. Ciri-ciri lain seperti bahan casing, tipe pemasangan, dan profil suara bisa dicatat untuk menggambarkan model kibor lebih lanjut.

(Catatan: Deksripsi ketiga tidak dimasukkan karena tidak diindasikan pada model referensinya. "mounting style" diterjemahkan jadi tipe pemasangan)

# ERD Acuan

```uml
@startchen

entity ModelKibor {
  Kode <<key>>
  Nama
  TahunPembuatan
  Bahan
  MountingStyle
  Suara
}

entity Ukuran {
  Nama <<key>>
  TataLetak
  TujuanPenggunaan
}

entity Switch {
  Nama <<key>>
  Aktuasi
  RasaTekanan
}

relationship memiliki_ukuran {
}

relationship pakai_switch {
}

ModelKibor =N= memiliki_ukuran
memiliki_ukuran -1- Ukuran

ModelKibor =N= pakai_switch
pakai_switch -1- Switch

@endchen
```

# Lisensi

[Tatjana Stojanović, Kristina Jovanović, Sasa Lazarevic](https://doi.org/10.5281/zenodo.20497271) mengizinkan di bawah [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/)
