# JGTC REBORN — Paket Lanjutan Tahap 5

Paket ini melanjutkan source code Tahap 4 dan menambahkan penjualan rute serta pembaruan versi rute. Struktur website, katalog `addons`, Firebase Authentication, pembayaran manual, Cloud Functions, Storage, dan alur riwayat pembelian dipertahankan.

## Fitur Tahap 5
- Penjualan pilihan update / perpanjang rute berdasarkan kepemilikan rute.
- Harga dan versi update ditetapkan admin utama.
- Keranjang dan checkout mendukung produk biasa dan update rute dalam satu pesanan.
- Validasi server terhadap harga, status aktif, kepemilikan rute, dan versi prasyarat.
- Persetujuan pembayaran menaikkan versi ownership dan menambahkan riwayat update.
- Download update menggunakan alur akses Tahap 4 setelah pembayaran lunas.

## File penting
- `index.html`, `styles.css`, `script.js`: antarmuka website lama + menu update rute.
- `firebase-bridge.js`: callable baru untuk membaca dan mengelola pilihan update.
- `functions/index.js`: validasi update, pembuatan order, approval ownership, dan download.
- `firestore.rules`, `storage.rules`: aturan akses Firebase.
- `TAHAP-5-PETUNJUK-DEPLOY.md`: panduan deployment, migrasi, dan pengujian.

## Mulai
Ikuti `TAHAP-5-PETUNJUK-DEPLOY.md`. Gunakan project ID Firebase yang sama dengan website aktif. Jangan mengganti UID admin utama atau menghapus koleksi lama.
