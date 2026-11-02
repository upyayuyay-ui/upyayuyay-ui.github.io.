# CampusLife 6.0 — aplikasi siap dipasang

## Isi paket
- `index.html` — aplikasi CampusLife
- `manifest.json` — identitas dan konfigurasi instalasi
- `sw.js` — cache aplikasi agar halaman utama dapat dibuka offline setelah kunjungan pertama
- `icons/` — ikon aplikasi

## Cara memasang di Android
1. Unggah seluruh isi folder ini ke hosting yang mendukung **HTTPS** (misalnya GitHub Pages atau hosting web Anda).
2. Buka alamat `https://.../index.html` melalui Chrome Android.
3. Tunggu halaman selesai dimuat, lalu pilih **Install app / Tambahkan ke layar utama** dari menu Chrome.
4. Jalankan CampusLife dari ikon yang muncul.

## Cara memasang di komputer
1. Buka alamat HTTPS aplikasi melalui Chrome atau Edge.
2. Klik ikon **Install** di bilah alamat, atau pilih menu browser → **Install CampusLife**.

## Catatan penting
- PWA tidak dapat dipasang dengan benar langsung dari file HTML yang dibuka lewat `file://`. Aplikasi harus disajikan melalui HTTPS atau `localhost`.
- Data profil, jadwal, tugas, dan nilai disimpan di penyimpanan lokal browser/perangkat. Data tidak otomatis tersinkron antarperangkat. Jangan hapus data situs/browser jika ingin mempertahankannya.
- Aplikasi inti dapat dibuka offline setelah pertama kali dimuat dan tersimpan di cache. Beberapa aset eksternal (font, ikon Font Awesome, dan suara alarm) mungkin memerlukan internet.
- Pengingat yang memakai JavaScript berjalan saat aplikasi terbuka. Browser/OS dapat menangguhkan aplikasi di latar belakang, sehingga alarm tidak dijamin berbunyi ketika aplikasi ditutup.
- Paket ini adalah **PWA yang dapat di-install**, bukan APK Android native.
