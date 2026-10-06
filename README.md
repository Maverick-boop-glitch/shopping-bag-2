# Landing Page Tas Belanja Lipat - Made by Kain

Landing page statis (HTML + CSS + JS, tanpa build) untuk iklan Google Ads.
Harga Rp30.000/pcs, semua tombol menuju WhatsApp +62 813-1129-3656.

## Isi folder

```
index.html                     halaman utama
assets/tas-belanja-lipat.jpg   foto produk
assets/logo-made-by-kain.png   logo
assets/favicon.png             ikon tab browser
_headers                       aturan cache Cloudflare Pages
robots.txt
```

## Deploy: GitHub + Cloudflare Pages

1. Buat repository baru di GitHub (misalnya `tas-belanja-lipat`), lalu upload semua isi folder ini
   (Add file > Upload files, seret semua file dan folder `assets`, lalu Commit).
2. Masuk ke Cloudflare Dashboard > Workers & Pages > Create > Pages > Connect to Git.
3. Pilih repository tadi, lalu isi pengaturan build:
   - Framework preset: **None**
   - Build command: **(kosongkan)**
   - Build output directory: **/**
4. Klik Save and Deploy. Situs akan aktif di `https://<nama-proyek>.pages.dev`.
5. (Opsional) Custom domain: di proyek Pages > Custom domains > Set up a custom domain.

Setiap kali ada perubahan yang di-commit ke GitHub, Cloudflare akan deploy ulang otomatis.

## Sebelum iklan tayang

- **Ukuran dan bahan:** cari teks `GANTI` di `index.html`, isi ukuran (cm) dan jenis kain.
- **Google tag:** cari `GOOGLE ADS: tempel kode Google tag` di `index.html`, tempel kode gtag.js dari akun Google Ads di baris itu.
- **Konversi klik WhatsApp:** cari `AW-XXXXXXXXX/XXXXXXXX` dan ganti dengan ID/label konversi dari Google Ads
  (Tujuan > Konversi > Buat tindakan konversi > Situs web).
- **Foto:** foto mockup memuat logo merek lain. Untuk menghindari penolakan iklan, ganti
  `assets/tas-belanja-lipat.jpg` dengan foto asli produk (nama file tetap sama).
- **Pesan WhatsApp otomatis:** ubah variabel `msg` di bagian `<script>` paling bawah `index.html`.
