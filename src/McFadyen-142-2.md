# Teks deskripsi

Sebuah perusahaan memberikan nomor pegawai kepada setiap karyawannya dan setiap pegawai memiliki nomor identitas yang diberikan oleh pemerintah. Untuk setiap pegawai, perusahaan mencatat nama depan, nama belakang, dan tanggal lahirnya.

# ERD Acuan

```uml
@startchen

entity Pegawai {
  NamaDepan
  NamaBelakang
  TanggalLahir
  NomorPegawai <<key>>
  IDPemerintah <<key>>
}

@endchen
```

# Lisensi

[Ron McFadyen dari Applied Computer Science Department, University of Winnipeg](https://www.acs.uwinnipeg.ca/rmcfadyen/CreativeCommons/) mengizinkan di bawah [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/)
