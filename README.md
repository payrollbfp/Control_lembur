# Portal Rekap Lembur — GitHub Pages + Supabase

Belum dideploy. Paket ini siap dipasang setelah Supabase dan repository GitHub dibuat.

## Supabase
1. Buat project Supabase baru.
2. Buka SQL Editor, tempel seluruh isi `supabase.sql`, lalu Run. Jika percobaan sebelumnya gagal pada fungsi `crypt`, jalankan ulang seluruh SQL versi terbaru dari baris pertama.
3. Buka Project Settings > API dan salin Project URL serta anon/public key.
4. Tempel keduanya ke `config.js`. Jangan gunakan service_role key.

## GitHub Pages
1. Upload semua file dalam folder ini ke repository GitHub.
2. Settings > Pages > Deploy from a branch > `main` dan `/root`.
3. Buka URL GitHub Pages yang diberikan.

## Verifikasi duplikat
Sistem memeriksa kombinasi Periode + Nopeg + Nama sebelum penyimpanan. Jika sudah ada, popup menampilkan uploader dan tanggal upload sebelumnya. Tombol Batal mempertahankan data lama; Ganti Data Lama menghapus data lama dan menyimpan data baru.

## Penguncian
Tanggal 1–20: upload dan hapus dapat dilakukan PIC. Mulai tanggal 21: perubahan memerlukan PIN Payroll `654321`. Tombol Kosongkan Database selalu memerlukan PIN dan hanya digunakan setelah report berhasil di-download.
