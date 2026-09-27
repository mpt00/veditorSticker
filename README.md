# VEDITOR Sticker Catalog

Katalog sticker untuk aplikasi VEDITOR (repo aplikasi: `mpt00/veditor`).
Aplikasi mengambil `catalog.json` dari repo ini; **menambah sticker tidak perlu mengubah kode aplikasi.**

## Cara menambah sticker

1. Unggah berkas PNG/WebP **transparan** ke folder `stickers/` (maksimal 3 MB per berkas).
2. Tambahkan satu entri pada `catalog.json`:

```json
{ "id": "nama_unik", "name": "Nama di aplikasi", "category": "Kategori",
  "png": "https://raw.githubusercontent.com/mpt00/veditorSticker/main/stickers/nama_unik.png",
  "thumb": "https://raw.githubusercontent.com/mpt00/veditorSticker/main/stickers/nama_unik_thumb.png",
  "keywords": "kata, kunci", "durationMs": 3000 }
```

3. Naikkan angka `version` supaya perubahan mudah dilacak.
4. Di VEDITOR: `TOOLS > Sticker > SEGARKAN` (katalog disegarkan paling cepat sekali sehari).

## Aturan berkas

- Wajib PNG/WebP dengan latar transparan. Latar putih akan menutupi gambar di bawahnya.
- Tautan wajib `https://`.
- Ukuran 1000x1000 px sudah cukup; aplikasi menyesuaikan sendiri ke ukuran kanvas.
- Thumbnail 320x320 px mempercepat tampilan galeri (opsional; bila kosong, PNG utama dipakai).

## Mengganti alamat katalog di aplikasi

`TOOLS > Sticker > SUMBER URL` — tempel alamat `catalog.json` lain (mis. katalog pribadi),
atau tekan `Bawaan` untuk kembali ke katalog resmi ini.
