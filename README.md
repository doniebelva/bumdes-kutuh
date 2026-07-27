# Laporan Studi Lapangan: BUMDes Manik Sedana Desa Kutuh

Laporan Studi Lapangan Kinerja Organisasi, Pelatihan Kepemimpinan Administrator (PKA) Angkatan XVIII Tahun Anggaran 2026, Kelompok II. Lokus: BUMDes Manik Sedana, Desa Kutuh, Kecamatan Kuta Selatan, Kabupaten Badung, Bali. Kunjungan 27 Juli 2026.

## Isi folder

```
index.html                          halaman laporan (satu halaman, tanpa dependensi eksternal)
assets/                             foto tetap yang dipakai hero dan profil lokus
dokumentasi/daftar-foto.json        daftar foto dokumentasi kunjungan
dokumentasi/CARA-MENAMBAH-FOTO.md   panduan menambah foto bagi anggota kelompok
```

Halaman tidak memuat font, skrip, atau gambar dari server luar, sehingga dapat dibuka langsung dari berkas lokal maupun dari hosting statis mana pun.

## Menambah foto dokumentasi

Seksi Dokumentasi Kunjungan membaca `dokumentasi/daftar-foto.json` secara otomatis. Anggota kelompok cukup mengunggah foto ke folder `dokumentasi/` lalu menambahkan datanya pada berkas JSON tersebut, tanpa perlu menyentuh `index.html`. Langkah rincinya ada pada [dokumentasi/CARA-MENAMBAH-FOTO.md](dokumentasi/CARA-MENAMBAH-FOTO.md).

Agar anggota dapat mengunggah sendiri lewat peramban, tambahkan mereka sebagai collaborator melalui menu Settings, Collaborators pada repositori ini.

## Cara publikasi di GitHub Pages

1. Buat repositori baru di GitHub, misalnya `laporan-studi-lapangan-kutuh`, dengan visibilitas publik.
2. Unggah seluruh isi folder ini, yaitu `index.html`, folder `assets`, dan `README.md`, ke akar repositori. Bisa lewat tombol **Add file, Upload files** pada halaman repositori, atau melalui perintah git berikut.

```bash
git init
git add .
git commit -m "Laporan studi lapangan BUMDes Manik Sedana Desa Kutuh"
git branch -M main
git remote add origin https://github.com/NAMA-AKUN/laporan-studi-lapangan-kutuh.git
git push -u origin main
```

3. Buka menu **Settings**, pilih **Pages**, lalu pada bagian *Build and deployment* tetapkan Source ke **Deploy from a branch**, Branch ke **main**, dan folder ke **/ (root)**. Simpan.
4. Tunggu sekitar satu sampai dua menit. Alamat laporan akan tersedia di `https://NAMA-AKUN.github.io/laporan-studi-lapangan-kutuh/`.

## Sumber data

Data profil dan keuangan bersumber dari situs resmi Desa Kutuh (kutuh-badung.desa.id, data Siskeudes APBDesa 2026), Peraturan Desa Kutuh Nomor 12 Tahun 2021 tentang Pendirian BUMDes Manik Sedana, serta publikasi ilmiah yang tercantum pada bagian Referensi di dalam halaman.

## Lisensi foto

Seluruh foto berasal dari Wikimedia Commons dengan lisensi Creative Commons Attribution-ShareAlike, karya Riska Diamitri, Jenhan Putra, Alharomain354, dan Chaecilly. Atribusi tercantum pada tiap gambar di dalam halaman.
