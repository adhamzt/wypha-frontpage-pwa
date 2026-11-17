# WYPHA Frontpage & Storefront Studio PWA (V1.0 Pioneer Edition)

Repositori siap pakai untuk men-deploy **Halaman Muka & Studio Katalog `#koleksi` WYPHA PrintLab** sebagai Progressive Web App (PWA) di **Cloudflare Pages melalui GitHub**, sekaligus mendukung penyematan (*embed*) penuh di **Google Sites**.

## Struktur File
- `index.html` — Engine Studio + Halaman Muka Interaktif (3D Hologram Keychain Customizer, Katalog `#koleksi`, Sandbox Demo 45 Edu-Game +5/-5 Koin & Brankas Bintang, Kalkulator Hemat, dan Cek Kuota 18 Tahun Warga Lokal).
- `manifest.json` — Konfigurasi instalasi PWA Android/iOS/Desktop.
- `sw.js` — Service Worker untuk dukungan Offline-First & caching instan.
- `icon-192.svg` & `icon-512.svg` — Ikon vektor aplikasi PWA.
- `_headers` — Konfigurasi header Cloudflare Pages (mengizinkan embed `<iframe>` di dalam Google Sites tanpa terblokir `X-Frame-Options`).

## Cara Deploy ke Cloudflare Pages via GitHub
1. Buat repository baru di GitHub (misalnya `wypha-frontpage-pwa`) lalu unggah seluruh file di dalam folder ini ke root repository.
2. Masuk ke **Cloudflare Dashboard** ➔ **Workers & Pages** ➔ **Create application** ➔ **Pages** ➔ **Connect to Git**.
3. Pilih repository `wypha-frontpage-pwa`.
4. Pada bagian **Build settings**:
   - **Framework preset**: `None`
   - **Build command**: *(kosongkan)*
   - **Build output directory**: `/`
5. Klik **Save and Deploy**. Dalam 30 detik, situs PWA Anda aktif dan otomatis terupdate setiap kali Anda melakukan perubahan di GitHub!
