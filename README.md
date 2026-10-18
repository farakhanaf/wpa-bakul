# WPA Connect Bandung Kulon — v0.2

Aplikasi React + Vite untuk portal informasi publik dan pratinjau ruang kerja internal WPA Bandung Kulon.

## Yang tersedia
- Halaman awal publik sebagai halaman default (tidak langsung masuk dashboard).
- Pusat edukasi dengan pencarian dan ringkasan topik.
- Direktori layanan contoh yang ditandai perlu verifikasi.
- Agenda/kampanye contoh yang tidak mengklaim sebagai jadwal resmi.
- Pusat bantuan dengan peringatan tentang situasi darurat dan privasi.
- Portal internal demo dengan pratinjau peran CO, Kader WPA, dan Pimpinan wilayah.
- Form laporan kegiatan demo dan daftar 18 indikator sebagai struktur awal.
- Responsif untuk desktop dan ponsel.

## Menjalankan secara lokal
1. Install Node.js versi LTS.
2. Ekstrak ZIP ini, lalu buka folder proyek di VS Code.
3. Buka terminal di folder yang berisi `package.json`.
4. Jalankan `npm install`.
5. Jalankan `npm run dev` dan buka alamat yang ditampilkan.
6. Sebelum deploy, jalankan `npm run build`.

## Deploy ke Vercel
- Upload/push folder proyek ke repository GitHub baru atau repository yang sesuai.
- Import repository tersebut di Vercel.
- Framework preset: Vite; Build command: `npm run build`; Output directory: `dist`.
- `vercel.json` sudah menyertakan rewrite untuk SPA.

## Batasan penting — baca sebelum digunakan
- Login di portal internal hanyalah pratinjau UI. Tidak ada autentikasi atau otorisasi nyata.
- Data laporan demo disimpan di `localStorage` browser dan tidak tersinkronisasi antarperangkat.
- Jangan memasukkan nama, status HIV, informasi medis, kontak privat, atau identitas ODHIV ke aplikasi ini.
- Konten edukasi adalah materi awal dan perlu ditinjau KPA/petugas kesehatan sebelum dipublikasikan sebagai informasi resmi.
- Direktori layanan dan agenda belum diverifikasi lengkap; jangan mengarang atau memublikasikan alamat, nomor telepon, jam, atau jadwal tanpa konfirmasi.
- Fitur rujukan/evakuasi ODHIV belum dibuat. Fitur tersebut memerlukan SOP, persetujuan, petugas berwenang, jalur eskalasi, serta keamanan backend sebelum dipertimbangkan.

## Struktur utama
- `src/App.jsx`: halaman, navigasi, state, data contoh, dan perilaku UI.
- `src/styles.css`: seluruh gaya visual dan responsivitas.
- `src/main.jsx`: titik masuk React.
- `index.html`: metadata browser.
