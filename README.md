# Ujian SMK Mandiri (Exambro)

Aplikasi Android berbasis WebView dengan mode terkunci untuk ujian.

- Layar awal: **Siswa** dan **Admin / Guru**
- Admin: isi tautan ujian, lihat nilai, bagikan CSV, ganti PIN
- Siswa: isi nama, NIS, kelas, lalu ujian terbuka dalam mode terkunci
- Tanpa tautan, aplikasi memakai soal bawaan (ubah di `app/src/main/assets/index.html`, bagian `PENGATURAN GURU`)
- PIN awal admin: `123456` (segera ganti)
- Keluar dari ujian: tekan tombol Kembali, lalu masukkan PIN admin

## Cara membuat APK lewat GitHub
1. Buat repository baru di GitHub, unggah seluruh isi folder ini.
2. Buka tab **Actions**, jalankan **Build APK** (atau otomatis saat push).
3. Setelah selesai, unduh artifact `ujian-smk-mandiri-apk`, lalu pasang `app-debug.apk` di HP siswa.

## Catatan
- Mode kunci layar (screen pinning) meminta konfirmasi sistem satu kali di HP.
- Nilai tersimpan di perangkat tempat siswa mengerjakan.
- Untuk tautan eksternal, aplikasi hanya mencatat siapa yang memulai (nilai tampil “-”).
