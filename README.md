# WPA Connect Bandung Kulon — MVP

## Jalankan lokal
1. Install Node.js LTS: https://nodejs.org
2. Ekstrak ZIP dan buka folder di VS Code.
3. Terminal: `npm install`
4. Terminal: `npm run dev`
5. Buka alamat localhost yang muncul di terminal.

## Deploy ke Vercel
1. Upload project ke repository GitHub.
2. Di https://vercel.com/new, import repository tersebut.
3. Framework preset: Vite; Build command `npm run build`; Output directory `dist`.
4. Klik Deploy.

## Batasan keamanan
Data kegiatan disimpan di localStorage browser ini, belum tersinkron antar pengguna. Role switcher hanya simulasi tampilan, bukan login/otorisasi. Data awal adalah sintetis. Jangan memasukkan identitas, status HIV, informasi kesehatan, nomor telepon pribadi, atau data pribadi ODHIV. Sebelum operasional bersama, tambahkan backend/database, autentikasi, akses berbasis peran di server, audit log, backup, dan peninjauan keamanan.
