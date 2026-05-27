# Catat Anggaran (PWA)

Aplikasi pencatatan anggaran berbasis Progressive Web App (PWA). Aplikasi ini dirancang minimalis dan berjalan sepenuhnya secara luring (offline) menggunakan teknologi IndexedDB melalui antarmuka web.

## Fitur Tersedia
- **Dark/Light Mode:** Responsif menyesuaikan pengaturan sistem atau dapat diatur manual.
- **Multi Wallet:** Pengaturan dan pemisahan saldo untuk berbagai dompet/akun.
- **Target Tabungan:** Pemantauan persentase pencapaian target menabung.
- **Backup & Restore Data:** Data aman, simpan dalam bentuk format JSON ke lokal komputer/HP.
- **AI Analisis Pengeluaran:** Ringkasan logis dan generatif berdasarkan data log pengeluaran bulanan.
- **Pengingat Tagihan:** Daftar tagihan/kewajiban bayar mendatang (UI disiapkan untuk *extend* ke depan).
- **Chart Dashboard:** Visualisasi chart donat.
- **Pencarian & Riwayat:** Log transaksi riwayat detail disertai filter pencarian.
- **Penyimpanan Lokal:** 100% Client-side storage menggunakan IndexedDB (Dexie.js).
- **Kustomisasi Label:** Menambah atau menghapus kategori untuk Pemasukan dan Pengeluaran.

## Cara Pemasangan & Menjalankan (Development)
Karena ini merupakan Progressive Web App dan menggunakan fitur Service Worker, aplikasi **harus** dijalankan di atas protokol HTTP/HTTPS (tidak bisa sekadar klik ganda file HTML di direktori *file://*).

1. Letakkan ke-tiga file (`index.html`, `manifest.json`, `sw.js`) di dalam satu folder (misal: `anggaran-app`).
2. Jalankan lokal server di direktori tersebut.
   - Menggunakan Python: `python -m http.server 8000`
   - Menggunakan Node/NPX: `npx serve .` atau `npx http-server`
3. Buka browser dan arahkan ke `http://localhost:8000`.
4. Untuk menginstal aplikasi di Desktop/Mobile, tekan logo "Install App" pada kolom URL browser Anda (Chrome/Edge/Safari).
