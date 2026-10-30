# EKSPLORA Mini Website — v6

Versi demo yang telah disesuaikan dengan alur EKSPLORA: hanya dua jenis akun (Siswa dan Operator Sekolah), pengelolaan ekstrakurikuler dinamis, pendaftaran dan verifikasi, badge keanggotaan, jadwal, pengumuman dengan sasaran pembaca, dan laporan. Nama sekolah tampil di halaman awal dan dapat diubah operator melalui Pengaturan Sistem.

## Isi paket
- `index.html` — halaman utama dan dialog login.
- `style.css` — desain responsif.
- `script.js` — alur demo dan penyimpanan data browser.
- `assets/eksplora-logo.png` — logo EKSPLORA.

## Akun demo

| Jenis akun | Username | Kata sandi |
|---|---|---|
| Siswa | `siswa01` | `EksploraS01!` |
| Siswa | `siswa02` | `EksploraS02!` |
| Siswa | `siswa03` | `EksploraS03!` |
| Siswa | `siswa04` | `EksploraS04!` |
| Siswa | `siswa05` | `EksploraS05!` |
| Operator Sekolah | `operator_sekolah` | `Operator01!` |

Di dialog login, tombol **Lihat daftar akun demo** dapat digunakan untuk mengisi kredensial demo.

## Pembaruan versi 6
- Menu Dokumentasi Kegiatan di akun Operator Sekolah dihapus.
- Nama sekolah ditampilkan di bagian awal website dan pada dialog masuk. Nama awal contoh: **SMAN 1 ATHERION**.
- Operator dapat mengubah nama sekolah melalui **Pengaturan Sistem**; perubahan langsung tampil pada halaman awal di browser yang sama.
- Tampilan dashboard diperbarui dengan navigasi dan kartu bergaya portal administrasi, sambil mempertahankan logo, warna biru, ilustrasi hero, dan identitas visual EKSPLORA.

## Fitur yang diterapkan

### Siswa
- Dashboard.
- Eksplorasi Ekstrakurikuler.
- Pendaftaran dan riwayat status: Menunggu Verifikasi, Sedang Diproses, Diterima, Ditolak, dan Dibatalkan.
- Pembatalan pengajuan sebelum keputusan penerimaan.
- Pencegahan pengajuan ganda selama pengajuan sebelumnya masih aktif.
- Ekstrakurikuler Saya dan badge keanggotaan berdasarkan penerimaan resmi.
- Kalender Kegiatan.
- Informasi dan Pengumuman: informasi umum dapat dilihat semua siswa; informasi khusus hanya terlihat anggota ekstrakurikuler terkait.
- Profil Saya.

### Operator Sekolah
- Dashboard statistik tanpa bagian Kegiatan Mendatang.
- Data Siswa bersifat baca-saja.
- Data Ekstrakurikuler: tambah, edit, buka/tutup pendaftaran, nonaktifkan, dan aktifkan kembali.
- Data Pendaftaran serta Verifikasi dan Penerimaan.
- Data Keanggotaan dan riwayat.
- Kalender Kegiatan.
- Informasi dan Pengumuman dengan pilihan sasaran pembaca.
- Rekapitulasi dan Laporan (CSV dan cetak/PDF).
- Pengaturan Sistem (termasuk nama sekolah yang tampil di halaman awal) dan Profil Akun.

Ekstrakurikuler baru langsung muncul pada daftar aktif siswa. Ekstrakurikuler yang dinonaktifkan tidak menerima pendaftar baru dan tidak tampil pada daftar eksplorasi aktif; riwayat pendaftaran dan keanggotaan tetap disimpan. Penonaktifan mengakhiri keanggotaan aktif yang terkait dan memindahkannya ke riwayat.

## Cara menjalankan
1. Ekstrak ZIP.
2. Buka `index.html` di browser untuk menjalankan demo lokal.
3. Untuk memperbarui GitHub Pages, unggah/replace `index.html`, `style.css`, `script.js`, dan folder `assets` ke root repository, lalu commit perubahan.

## Catatan penting
Ini masih prototype front-end. Data disimpan di `localStorage` browser, sehingga perubahan operator tidak tersinkron otomatis ke perangkat siswa lain. Akun demo dan kata sandi berada di JavaScript. Jangan gunakan untuk data pribadi atau kata sandi sungguhan. Penggunaan nyata memerlukan backend, database bersama, autentikasi aman, serta validasi hak akses di server.
