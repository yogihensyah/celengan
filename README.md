# Celengan 🐷

Aplikasi pencatatan keuangan pribadi: catat uang masuk dan keluar, kategorikan, lihat laporan bulanan.
Satu file (`index.html`), tanpa server dan tanpa build. Data tersimpan di browser (localStorage).

## Deploy ke GitHub Pages

1. Buat repository baru di GitHub, misalnya `celengan` (boleh Public atau Private jika akun mendukung Pages privat).
2. Upload `index.html` dan `README.md` ke branch `main` (tombol **Add file → Upload files**).
3. Buka **Settings → Pages**.
4. Di **Build and deployment**, pilih **Source: Deploy from a branch**, branch **main**, folder **/ (root)**, lalu **Save**.
5. Tunggu 1–2 menit. Alamatnya: `https://<username>.github.io/celengan/`

Lewat terminal:

```bash
git init
git add index.html README.md
git commit -m "Celengan"
git branch -M main
git remote add origin https://github.com/<username>/celengan.git
git push -u origin main
```

Lalu aktifkan Pages seperti langkah 3–4.

## Pasang seperti aplikasi di HP

- **Android (Chrome)**: menu ⋮ → *Add to Home screen*.
- **iPhone (Safari)**: tombol Share → *Add to Home Screen*.

## Soal data (penting)

- Data disimpan **per browser dan per alamat situs**. Membuka di HP dan laptop berarti catatannya terpisah.
- Menghapus data situs atau riwayat browser akan **menghapus catatan**.
- Gunakan tombol **💾 Cadangkan** di bagian bawah halaman untuk mengunduh file `.json`, dan **📂 Pulihkan** untuk memasukkannya kembali. Ini juga cara memindahkan data antar perangkat.
- **📄 Ekspor CSV** menghasilkan file untuk Excel atau Google Sheets (pemisah titik koma).
- Mode private/incognito biasanya tidak menyimpan data setelah tab ditutup.

## Catatan

- Font dimuat dari Google Fonts. Jika offline, aplikasi memakai font bawaan perangkat.
- Mengganti isi `index.html` di repo tidak menghapus data pengguna, karena data ada di browser.
