# Tabranij Pro v3.0

Visualizer 3D metode **GT (Grafik Tabranij)** dengan fitur lanjutan.

## Fitur Baru

| Fitur | Keterangan |
|-------|------------|
| **Multi-Candle** | Tampilkan 2–12 candle berdampingan di scene 3D |
| **Timeframe** | M1 · M5 · M15 · H1 · H4 · D1 (slider range menyesuaikan) |
| **History** | Simpan/muat state (localStorage, max 30 entry) |
| Mode Single/Multi | Toggle cepat |
| Generate Series | Buat series acak dengan drift harga |
| Navigasi Candle | Tombol ‹ › untuk pilih candle aktif |
| + Candle | Tambah candle manual ke series |
| Export PNG · Copy · Direction flip | Tetap tersedia |

## Cara Membuka

1. Download folder `tools/tabranij-visualizer/` (index.html + d0.js + d1.js)
2. Buka `index.html` di browser **via local server**:

```bash
cd tools/tabranij-visualizer
python3 -m http.server 8080
# lalu buka http://localhost:8080
```

> Karena app di-load via script + gzip decompress, buka lewat `file://` langsung mungkin gagal (CORS). Gunakan local server seperti di atas.

## File

- `index.html` — loader
- `d0.js` / `d1.js` — payload aplikasi (gzip+base64)

## Status

✅ v3.0 siap dipakai
