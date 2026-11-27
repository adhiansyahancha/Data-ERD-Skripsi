# Teks deskripsi

Hotels have at least one or several rooms and each room is in turn part of exactly one hotel. Each room has a room number. Guests may stay in a hotel and book one or several rooms. A room may in turn be booked by none or more guests.

# ERD Acuan

```uml
@startchen

entity Hotel {
}
entity Room {
  RoomNumber
}
entity Guest {
}

relationship has {
}
relationship books {
}

Hotel =N= has
has =1= Room

Guest -N- books
books -N- Room

@endchen
```

# Lisensi

[EMISAJ - International Journal of Conceptual Modeling](https://emisa-journal.org/emisa/article/view/318) mengizinkan di bawah [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/ )
