# Aplikasi Denah + RAB MCK 3x4 Meter

Aplikasi web untuk menampilkan denah visual, tampak bangunan, tampak atap, dan Rencana Anggaran Biaya (RAB) MCK sederhana ukuran 3 m x 4 m.

## Layout

- Ukuran total: 3 m x 4 m = 12 m²
- WC tertutup: 1 m x 1,5 m
- Bak mandi: 2 m x 2 m
- Teras: 3 m x 2 m
- Teras sudah termasuk di dalam ukuran total 3 m x 4 m
- Atap: atap miring satu arah dengan rangka baja ringan dan penutup spandek/polycarbonate

## Fitur

- Denah visual 2D sesuai layout MCK
- Tampak depan, belakang, kiri, kanan
- Tampak atap sesuai hitungan item pekerjaan atap pada RAB
- Satu halaman langsung scroll, tanpa pindah tab
- Detail spesifikasi bangunan
- RAB lengkap per kelompok pekerjaan
- Total biaya otomatis
- Status batas anggaran maksimal Rp42.000.000
- Download PDF detail bangunan (termasuk denah, tampak, dan atap)
- Download PDF RAB
- Responsive untuk desktop dan mobile
- Build single-file menggunakan Vite

## Catatan Estimasi Harga

Harga pada aplikasi adalah estimasi rata-rata untuk wilayah Madura/Sumenep dan dapat berubah sesuai lokasi, akses material, kualitas bahan, toko bangunan, serta ongkos tukang. Sebelum pembangunan, angka RAB sebaiknya dicek ulang di lokasi.

## Install

```bash
npm ci
```

atau:

```bash
npm install
```

## Run Lokal

```bash
npm run dev
```

## Build

```bash
npm run build
```

Hasil build akan muncul di folder:

```txt
dist/
```

Karena memakai `vite-plugin-singlefile`, hasil deploy utama biasanya cukup berupa satu file:

```txt
dist/index.html
```

## Deploy ke GitHub Pages

Cara paling simpel:

1. Jalankan `npm run build`.
2. Upload isi folder `dist` ke repository GitHub Pages.
3. Pastikan file utama bernama `index.html`.
4. Aktifkan GitHub Pages dari branch/folder deploy yang kamu pakai.

Jika upload source project ke GitHub, jangan upload `node_modules`.
