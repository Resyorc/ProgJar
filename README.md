# Tugas ProgJar

## Deskripsi
Implementasi sederhana dari komunikasi jaringan menggunakan socket di Python. Dalam implementasi ini, terdapat dua skrip Python terpisah yang mewakili client dan server.

## Komponen Utama
- **Client**: Skrip ini bertanggung jawab untuk mengirimkan sebuah angka ke server melalui koneksi TCP. Angka ini dimasukkan oleh pengguna melalui input. Setelah mengirimkan angka, client menunggu respons dari server dan mencetaknya.

- **Server**: Skrip ini bertanggung jawab untuk menerima koneksi dari client, menerima angka yang dikirimkan oleh client, memeriksa apakah angka tersebut genap atau ganjil, dan mengirimkan respons kembali ke client berdasarkan hasil pemeriksaan.

## Implementasi
- **Client**: Menggunakan modul socket untuk membuat socket dan melakukan koneksi ke server. Pengguna diminta untuk memasukkan sebuah angka melalui input, yang kemudian dikirimkan ke server. Setelah menerima respons dari server, client mencetaknya dan menutup koneksi.

- **Server**: Juga menggunakan modul socket untuk membuat socket dan mendengarkan koneksi dari client. Ketika ada koneksi masuk, server menerima angka dari client, memeriksa apakah angka tersebut genap atau ganjil, dan mengirimkan respons yang sesuai kembali ke client. Setelah itu, server menutup koneksi.

## Penggunaan
1. Jalankan skrip server terlebih dahulu dengan menjalankan skrip `server.py`.
2. Kemudian jalankan skrip client dengan menjalankan skrip `client.py`.
3. Ketika client meminta, masukkan sebuah angka.
4. Server akan memberikan respons apakah angka tersebut genap atau ganjil.
5. Setelah mendapatkan respons, client akan menutup koneksi.

**Penting:** Pastikan host dan port yang digunakan oleh client dan server sesuai dan tidak bertentangan. Dalam implementasi ini, host dan port yang digunakan adalah `'localhost'` dan `12345`.
