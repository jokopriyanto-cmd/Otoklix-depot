# Otoklix Depot (PWA)

Aplikasi Otoklix Depot (Isi Form, Check-in, WO, Inventaris, Dashboard, Investigasi) yang tampilannya
dihosting di GitHub Pages dan datanya tetap di Google Apps Script + Google Sheet.

- `index.html` : seluruh tampilan aplikasi. Memanggil Apps Script lewat POST ke `API_URL` (lihat bagian `<head>`).
- `sw.js`, `manifest.webmanifest`, `icons/` : agar bisa dipasang di HP/laptop.
- Backend: `Code.gs` di Apps Script Depot (fungsi `doPost` dengan daftar putih `WA_API_FN`).

Kalau link /exec Apps Script berganti, ubah `API_URL` di `index.html`.
Setiap mengubah `index.html`, naikkan `VER`/nama cache di `sw.js` supaya HP memuat versi baru.
