Asumsikan definisi dari Entity-Relationship (ERD) sebagai berikut:
ERD dibuka dengan `@startchen` dan ditutup dengan `@endchen`. 
Untuk menyatakan entitas: `entity Bangunan {}`, `entity Orang {}`. 
Untuk menyatakan hubungan: `relationship dimiliki {}`. 
Untuk menyatakan atribut, tulis di dalam kurung elemen: `entity Bangunan { nama, lokasi }`, `entity Orang { nama { depan, belakang } }`. 
Untuk menghubungkan antarentitas, tuliskan dua pernyataan: `Bangunan -N- dimiliki` dan `dimiliki -1- Orang`
Untuk menentukan kardinalitas, terdapat 4 jenis: `-1-` berarti maksimal satu, minimal nol (0..1),  `-N-` berarti maksimal banyak, minimal nol (0..N), `=1=` berarti maksimal satu, minimal satu (1..1),  `=N=` berarti maksimal banyak, minimal satu (1..N).

Berikut adalah contoh ERD, yang menyatakan bahwa Orang memiliki nol
atau beberapa Mobil dan bahwa Mobil dapat diparkir di satu Garasi. Selain itu, dinyatakan bahwa
Mobil harus selalu dimiliki oleh setidaknya satu orang:

```uml
@startchen

entity Orang {
  Nama
}
entity Mobil {
  NomorPlat
}
entity Garasi {
  NomorGarasi
}

relationship memiliki {}
relationship diparkir_di {}

Orang -N- memiliki
memiliki =N= Mobil

Mobil -1- diparkir_di
diparkir_di -N- Garasi

@endchen
```

Buatkan ERD menggunakan sintaksis tersebut untuk skenario berikut dan jangan
menambahkan informasi apa pun yang tidak dideskripsikan di sini dan jangan menambahkan
penjelasan apa pun:

(Deskripsi tugas taruh di sini)
