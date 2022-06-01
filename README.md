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
- Menerima input jumlah minterm/maxterm dan indeks minterm/maxterm
- Menampilkan output hasil minimisasi dalam bentuk SoP (*Sum of Product*) dan dalam bentuk PoS (*Product of Sum*) dengan parameter `A`, `B`, dan seterusnya

### Fitur
- Minimisasi logika dengan ukuran **1 - 8 bit**
- Tidak menerima input *don't care* dan dianggap tidak ada *don't care*
- Ukuran bit hanya bisa diganti di bagian *header file*

### Fitur yang Ingin Diimplementasikan
- [ ] Menerima input *Don't care*

### Dokumentasi
Contoh penggunaan program:

Misalkan ingin dicari 

![alt text](https://github.com/DentAlpha/Minimisasi-Quine-McCluskey/blob/main/Dokumentasi/Minterm.png?raw=true)

Maka input yang diberikan ke program adalah

![alt text](https://github.com/DentAlpha/Minimisasi-Quine-McCluskey/blob/main/Dokumentasi/input.png?raw=true)

Proses yang dijalankan oleh program akan ditampilkan sebagai berikut

![alt text](https://github.com/DentAlpha/Minimisasi-Quine-McCluskey/blob/main/Dokumentasi/proses.png?raw=true)

Diperoleh output sebagai berikut

![alt text](https://github.com/DentAlpha/Minimisasi-Quine-McCluskey/blob/main/Dokumentasi/output.png?raw=true)

Hasil yang diberikan oleh program sesuai dengan kalkulator minimisasi logik pada internet

![alt text](https://github.com/DentAlpha/Minimisasi-Quine-McCluskey/blob/main/Dokumentasi/solusi.png?raw=true)

## Program : `quinecluskey_bitsSizeInput.c`

### Spesifikasi Program
- Menerima input ukuran bit, jumlah minterm/maxterm, dan indeks minterm/maxterm
- Menampilkan output hasil minimisasi dalam bentuk SoP dan dalam bentuk PoS dengan parameter `A`, `B`, dan seterusnya

### Fitur
- Minimisasi logika dengan ukuran **1 - 26** bit dengan jumlah minterm/maxterm maksimal 518008 buah (secara teoritis;tidak diuji)
- Tidak menerima input *don't care* dan dianggap tidak ada *don't care*

### Fitur yang Ingin Diimplementasikan
- [ ] Menerima input *Don't care*
- [ ] Mengganti penggunaan *array* dengan alokasi memori agar minimisasi untuk jumlah minterm yang besar dapat dilakukan

## Referensi
-	Brown S. D. dan Vranesic Z. G, Fundamentals of digital logic with VHDL design, 2000.
