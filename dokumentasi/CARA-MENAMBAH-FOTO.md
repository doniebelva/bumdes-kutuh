# Cara menambah foto dokumentasi

Galeri pada seksi **Dokumentasi Kunjungan** membaca berkas `daftar-foto.json` di folder ini. Menambah foto cukup dua langkah dan tidak perlu mengubah `index.html`.

## Langkah 1: unggah berkas foto

Taruh berkas foto di folder `dokumentasi/` ini. Ketentuan yang disarankan:

- Format `.jpg`, ukuran lebar maksimal sekitar 1600 piksel, besar berkas di bawah 500 KB agar halaman tetap ringan.
- Nama berkas memakai huruf kecil, tanpa spasi, diawali nomor urut. Contoh: `01-paparan-perbekel.jpg`, `02-office-tour-bumdes.jpg`.
- Hindari tanda baca dan huruf beraksen pada nama berkas.

## Langkah 2: daftarkan datanya

Buka `daftar-foto.json`, lalu tambahkan satu objek untuk setiap foto. Berkas ini berisi satu larik, dan setiap objek dipisahkan koma. Contoh isi lengkap:

```json
[
  {
    "berkas": "01-paparan-perbekel.jpg",
    "judul": "Paparan Perbekel Desa Kutuh",
    "keterangan": "Pemaparan strategi pengembangan BUMDes Manik Sedana kepada peserta PKA Angkatan XVIII.",
    "waktu": "27 Juli 2026, 09.30 WITA",
    "lokasi": "Grha Sabha, Kantor Perbekel Kutuh",
    "oleh": "Tulus Suparto"
  },
  {
    "berkas": "02-office-tour-bumdes.jpg",
    "judul": "Office tour kantor BUMDes",
    "keterangan": "Peninjauan ruang kerja dan unit layanan BUMDes Manik Sedana.",
    "waktu": "27 Juli 2026, 11.00 WITA",
    "lokasi": "Kantor BUMDes Manik Sedana",
    "oleh": "Ranu Fatah Wijoyo"
  }
]
```

Kolom `berkas` wajib diisi dan harus sama persis dengan nama berkas foto, termasuk huruf besar kecilnya. Kolom `judul`, `keterangan`, `waktu`, `lokasi`, dan `oleh` bersifat opsional, namun sangat dianjurkan karena justru data inilah yang membedakan dokumentasi laporan dari sekadar kumpulan foto.

Perhatikan dua kesalahan yang paling sering terjadi: koma tertinggal setelah objek terakhir, dan tanda kutip yang memakai kutip miring hasil salin tempel dari Word. Keduanya membuat berkas gagal dibaca dan galeri tidak muncul.

## Menyimpan perubahan

Bagi anggota yang sudah ditambahkan sebagai collaborator, seluruh proses ini bisa dilakukan langsung dari peramban pada halaman repositori GitHub, lewat tombol **Add file, Upload files** untuk foto dan tombol pensil untuk menyunting `daftar-foto.json`. Situs akan memperbarui diri sekitar satu menit setelah perubahan tersimpan.

## Catatan etika dokumentasi

Sesuai Panduan Wawancara Studi Lapangan, pastikan izin dokumentasi sudah diperoleh dari narasumber sebelum foto dipublikasikan. Hindari menampilkan dokumen internal, data pribadi, atau papan informasi yang memuat angka yang belum boleh dibuka ke publik, mengingat repositori ini bersifat publik.
