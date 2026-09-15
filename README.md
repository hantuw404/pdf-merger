# PDF Merger — Pas Foto / Dokumen

Gabung foto/scan dokumen jadi satu PDF langsung di browser. Urutan tetap: KTP, Paspor, Pas Foto, KK, Akta, lalu halaman teks Email & WhatsApp.

## Fitur
- **100% offline** — satu file HTML, semua library (pdf-lib + OpenCV.js) sudah tergabung, tanpa server
- **Efek scan (OpenCV)** — luruskan dokumen yang miring (perspective warp), auto white-balance, perbaikan kontras
- **Preview** hasil PDF di panel samping sebelum download
- **Drag & drop** atau klik untuk unggah gambar (jpg/png/webp)
- Nama di isi → output otomatis `NAMA.pdf`

## Cara pakai
1. Buka `index.html` di browser (Chrome/Edge/Firefox)
2. Isi nama pemilik dokumen
3. Tarik/klik gambar ke slot 1–5
4. Centang **Efek scan** kalau foto mentah/miring
5. Isi Email Aktif & WhatsApp Aktif
6. Klik **Buat PDF & Preview** → cek hasil → **Download**

## Urutan halaman PDF
1. KTP
2. Paspor (halaman biodata)
3. Pas Foto 4 × 6 (tanpa efek scan)
4. Kartu Keluarga
5. Akta Kelahiran
6. Email
7. WhatsApp

> File tidak pernah dikirim ke mana pun — semua proses berjalan di browser lokal.

## Teknis
- [pdf-lib](https://pdf-lib.js.org) untuk generate PDF
- [OpenCV.js](https://docs.opencv.org) untuk deteksi dokumen & perspective correction
- Tanpa build step, tanpa dependency install