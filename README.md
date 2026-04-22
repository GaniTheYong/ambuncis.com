# Rambuncis Static Site

Migrasi statis dari `rambuncis.com` WordPress ke situs multi-page yang siap di-host di GitHub Pages atau static hosting lain.

## Struktur

- `index.html`: halaman utama
- `kitchenset-lemari/`, `kaca-toko/`, `plafon/`, `pintu/`, `jendela/`, `sliding-doors/`, `project-lainnya/`: halaman produk dan galeri
- `project-kami/`: redirect ke `project-lainnya/`
- `assets/styles.css`: stylesheet global
- `assets/site.js`: interaksi ringan untuk menu mobile
- `assets/images/`: aset gambar lokal hasil migrasi
- `CNAME`: custom domain `rambuncis.com`

## Publish ke GitHub Pages

1. Push isi repo ke branch `main`.
2. Di GitHub, buka `Settings > Pages`.
3. Pada `Build and deployment`, pilih `Deploy from a branch`.
4. Pilih branch `main` dan folder `/ (root)`.
5. Pastikan DNS domain `rambuncis.com` diarahkan ke GitHub Pages.

## Catatan

- File `.nojekyll` disertakan supaya GitHub Pages tidak menganggap struktur folder ini sebagai proyek Jekyll.
- Semua gambar utama sudah dipindahkan ke repo agar situs tidak bergantung lagi ke server WordPress lama.
