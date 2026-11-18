# Teks deskripsi

Seorang pegawai mengawasi pegawai lain.

(Catatan: Pengarang asli menerangkan bahwa "hubungan di sini adalah satu-ke-banyak: seorang pegawai bisa mengawasi banyak pegawai, dan seorang pegawai bisa diawasi oleh paling banyka satu pegawai lain.")

# ERD Acuan

```uml
@startchen

entity Pegawai {
}

relationship mengawasi {
}

Pegawai -1- mengawasi
mengawasi -N- Pegawai

@endchen
```

# Lisensi

[Ron McFadyen dari ACS Department, University of Winnipeg]([https://emisa-journal.org/emisa/article/view/318](https://www.frontiersin.org/journals/education/articles/10.3389/feduc.2025.1554089/full)) mengizinkan di bawah [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/)
