# Ex-withdraw — simulasi edukasi

Semua saldo adalah kredit virtual lokal. Tidak ada pembayaran, transfer, atau penarikan uang nyata. Tidak ada backend atau database eksternal.

## Jalankan
1. Pasang Node.js 20 atau 22.
2. `npm install`
3. `npm run dev`
4. Buka alamat lokal yang dicetak Vite.

## Build / Vercel
`npm run build` menghasilkan `dist/`. Di Vercel pilih framework Vite, build command `npm run build`, output directory `dist`. `vercel.json` mengarahkan semua rute SPA ke `index.html`.

Admin demo terbuka tanpa autentikasi dan hanya mengubah localStorage browser. **ADMIN LOKAL — TIDAK AMAN UNTUK PRODUKSI**. Jangan masukkan data sensitif.