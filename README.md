# Tugas Besar EL2008 Pemecahan Masalah dengan C: Minimisasi dengan Metode Quine-McCluskey

Anggota Kelompok:
- Adro Anra Purnama / 13220005
- Surya Dharma / 13220027
- Fariz Iftikhar Falakh / 13220029
- Senggani Fatah Sedayu / 13220035

## Metode Tabular
Metode Tabular atau dikenal juga sebagai Metode Quine-McCluskey adalah sebuah metode minimisasi persamaan boolean.
Metode ini melakukan minimisasi dengan mencari *essential implicant* dari *minterm* yang ingin disederhanakan. 

## Program : `quinecluskey.c`

### Spesifikasi Program
- Menerima input jumlah minterm dan indeks minterm (terdapat tambahan input ukuran bit untuk `quinecluskey_bitsSizeInput.c`)
- Menampilkan output hasil minimisasi dalam bentuk biner dan dalam bentuk parameter input (`a`, `b`, dan seterusnya)

### Fitur
- Minimisasi logika dengan ukuran 1 - 8 bit (1 - 26 bit untuk `quinecluskey_bitsSizeInput.c`)
- Tidak menerima input *don't care* dan dianggap tidak ada *don't care*
- Ukuran bit hanya bisa diganti di bagian *header file*

### Fitur yang Ingin Diimplementasikan
- [ ] Menerima input *Don't care*
- [ ] Validasi jumlah bit untuk `quinecluskey.c`
- [ ] Menerima input maxterm (*Product of Sum*)

### Dokumentasi
![alt text](https://github.com/DentAlpha/Minimisasi-Quine-McCluskey/blob/main/Dokumentasi/Test1.png?raw=true)

## Referensi
-	Brown S. D. dan Vranesic Z. G, Fundamentals of digital logic with VHDL design, 2000.
