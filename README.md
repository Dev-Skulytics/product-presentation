# Skulytics Product Update — June 2026

Halaman product update statis (single-page HTML) untuk Skulytics.

## Struktur

```
index.html    → halaman utama (semua CSS/JS inline)
assets/       → gambar & logo
```

## Jalankan secara lokal

Cukup buka `index.html` di browser, atau jalankan server lokal:

```bash
python3 -m http.server 8000
# buka http://localhost:8000
```

## Deploy ke GitHub Pages

### 1. Buat repo di GitHub lalu push

```bash
git remote add origin https://github.com/USERNAME/SKulytics-Product-Update.git
git push -u origin main
```

(Ganti `USERNAME` dengan username/organisasi GitHub kamu.)

Atau kalau pakai [GitHub CLI](https://cli.github.com/), satu perintah saja:

```bash
gh repo create SKulytics-Product-Update --public --source=. --push
```

### 2. Aktifkan GitHub Pages

1. Buka repo di GitHub → **Settings** → **Pages**
2. Di bagian **Build and deployment**, pilih **Source: GitHub Actions**
3. Selesai — setiap push ke `main` akan otomatis ter-deploy lewat workflow di `.github/workflows/deploy.yml`

Situs akan tersedia di:

```
https://USERNAME.github.io/SKulytics-Product-Update/
```
