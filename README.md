# Pusat Pelaporan Isu TLX Training Gate

## Isu yang Dapat Dilaporkan

Anda dapat melaporkan isu pada TLX Training Gate ketika Anda merasa:

1. Terdapat kesalahan/ambiguitas pada deskripsi soal
2. Time limit atau memory limit yang diberikan grader terlalu ketat atau kurang adil untuk bahasa tertentu
3. Kasus uji pada grader kurang variatif
4. Ada soal yang mendasar dan seharusnya ditambahkan sebagai soal latihan
5. Solusi Anda sudah benar, tetapi grader menganggapnya salah

## Tata Cara Melaporkan

1. Pastikan isu Anda memang perlu untuk dilaporkan. Lihat bagian [Sering Ditanyakan](#sering-ditanyakan) sebagai panduan.

2. Periksa apakah isu yang mirip sudah pernah dilaporkan di [daftar isu](https://github.com/ia-toki/Training-TLX/issues?utf8=%E2%9C%93&q=is%3Aissue).

   * Bila sudah ada, artinya isu Anda sedang/sudah diselidiki dan diselesaikan. Isu Anda tidak perlu dilaporkan lagi.
   * Bila belum ada, tambahkan isu di [sini](https://github.com/ia-toki/Training-TLX/issues)

3. Tuliskan judul yang deskriptif, misalnya:

   * Kesalahan kasus uji soal "barisan hewan ternak"
   * Time limit terlalu ketat untuk soal "pesta bebek"
   * Soal "Tantangan Dengklek" ambigu

4. Isikan deskripsi isu Anda dengan singkat, jelas, dan padat. Cantumkan link/alamat halaman website untuk memudahkan pemeriksaan isu, seperti link menuju soal, submission (terutama untuk laporan "solusi saya sudah benar tetapi wrong answer"), dan sebagainya.

## Sering Ditanyakan

### Solusi saya sudah benar, mengapa masih wrong answer?

#### Pastikan Anda mencetak baris baru pada akhir keluaran.

Benar:
```
halo<baris baru>
dunia<baris baru>
```
Salah:
```
halo<baris baru>
dunia
```
#### Pastikan tidak ada kelebihan spasi atau baris baru di akhir keluaran Anda.
Benar:
```
halo<baris baru>
dunia<baris baru>
```
Salah:
```
halo<baris baru>
dunia<baris baru>
<baris baru>
```
Salah:
```
halo <baris baru>
dunia <baris baru>
```

#### Pastikan solusi Anda mampu menangani berbagai kasus

Grader memiliki banyak kasus uji untuk memastikan program Anda menghasilkan solusi yang benar pada semua jenis kasus. Benar untuk beberapa kasus uji contoh belum tentu benar untuk seluruh kasus uji.

Bila Anda kesulitan dalam mendapatkan kasus uji yang menyebabkan solusi Anda salah, bertanyalah pada forum atau grup Olimpiade Informatika Indonesia.

#### Pastikan penggunaan tipe data Anda tepat.

Perhatikan apakah tipe data Anda dapat menyimpan bilangan sebesar yang dibutuhkan. Sebagai catatan, berikut rentang tipe data variabel yang umum digunakan:

Jenis | Nama (Pascal) | Name (C++) | Rentang
------|---------------|------------|--------
integer 16 bit | integer | short | -32768 .. 32767
integer 32 bit | longint | int | -2147483648 .. 2147483647 
integer 64 bit | int64 | long long | -9223372036854775808 .. 9223372036854775807

### Solusi saya sudah benar, mengapa masih runtime error?

Periksalah apakah solusi Anda mengalami division by zero, mengakses elemen array di luar batas, menggunakan terlalu banyak memori.

### Apakah grader sedang down?

Anda tidak perlu melaporkan isu semacam ini di sini. Cukup laporkan di grup Olimpiade Informatika Indonesia.
