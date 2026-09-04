# BK — Buku Pegangan Grup Investasi & Trading

**Metode GT (Grafik Tabranij)**

Repository private untuk buku pegangan internal grup investasi & trading.

## Mulai di sini

- **[Daftar Isi Buku](docs/00-daftar-isi.md)**
- **[Bab 1 — Pengenalan](docs/01-pengenalan.md)**
- **[Bab 2 — Konsep GT](docs/02-konsep-gt.md)**
- **[Bab 3 — Parameter TABRANIJ](docs/03-parameter-tabranij.md)**
- **Tool:** [Tabranij Pro v3](tools/tabranij-visualizer/)

## Struktur Repository

```
bk/
├── docs/                      # Isi buku pegangan
│   ├── 00-daftar-isi.md
│   ├── 01-pengenalan.md
│   ├── 02-konsep-gt.md
│   ├── 03-parameter-tabranij.md
│   └── … (bab selanjutnya)
├── tools/tabranij-visualizer/ # Tool 3D interaktif
├── assets/                    # Gambar & diagram
├── contoh/                    # Contoh kasus
└── referensi/
```

## Parameter GT (ringkas)

| Kode | Nama | Keterangan |
|------|------|------------|
| **T** | Tinggi | High / titik tertinggi |
| **A** | Awal | Open / acuan awal |
| **R** | Rendah | Low / titik terendah |
| **I** | Inti | Poros (core) |
| **N** | Neto | `2 × I − A` |
| **J** | Julat | Rentang struktur GT |

Bias: **Bullish** jika `N ≥ A`, **Bearish** jika `N < A`.

## Status

| Komponen | Status |
|----------|--------|
| Tool Tabranij Pro v3 | ✅ Multi-candle, TF, History |
| Bab 1–3 (Fondasi) | ✅ Terisi |
| Bab 4–12 | ⏳ Menyusul |
