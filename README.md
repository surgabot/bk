# BK — Buku Pegangan Grup Investasi & Trading

**Metode GT (Grafik Tabranij)**

Repository private untuk buku pegangan internal grup investasi & trading.

## Mulai di sini

- **[Daftar Isi Buku](docs/00-daftar-isi.md)**
- **[Bab 1 — Pengenalan](docs/01-pengenalan.md)**
- **[Bab 2 — Konsep GT](docs/02-konsep-gt.md)**
- **[Bab 3 — Parameter TABRANIJ](docs/03-parameter-tabranij.md)**
- **[Bab 4 — Membaca Candle dengan GT](docs/04-membaca-candle.md)**
- **[Bab 5 — Bias, Arah, dan Struktur](docs/05-bias-arah-struktur.md)**
- **[Bab 6 — Multi-Candle & Timeframe](docs/06-multi-candle-timeframe.md)**
- **Tool:** [Tabranij Pro](tools/tabranij-visualizer/) · file stabil: unduh HTML tunggal dari rilis / artifacts

---

## Apa itu TABRANIJ?

**TABRANIJ** adalah susunan huruf dan kode yang ditata agar kalimat, visual, dan bilingual-nya berkesan — memudahkan cara membaca grafik sambil mengasosiasikan agar mudah dihafal.

Urutan huruf: **T · A · B · R · A · N · I · J**

### Dua jenis komponen

**Titik (posisi harga) — akronim TARI**

| Kode | Komponen | Keterangan |
|------|----------|------------|
| **T** | Tinggi | Harga tertinggi periode (puncak) |
| **A** | Awal | Harga pembukaan (konstanta) |
| **R** | Rendah | Harga terendah periode (dasar) |
| **I** | Inti | Harga saat ini / penutupan (variabel) |

> Hafalkan: **TARI** = **T**inggi · **A**wal · **R**endah · **I**nti

**Rentang (ukuran ruang)**

| Kode | Komponen | Rumus | Keterangan |
|------|----------|--------|------------|
| **A** | Atas | `T − max(Awal, I)` | Panjang wick atas |
| **B** | Bawah | `min(Awal, I) − R` | Panjang wick bawah |
| **N** | Neto | `|I − Awal|` | Lebar body |
| **J** | Julat | `T − R` | Jangkauan penuh periode |

**Identitas:** `Julat = Atas + Neto + Bawah`

**Bias:** naik jika `I ≥ Awal`, turun jika `I < Awal`.

---

## Struktur Repository

```
bk/
├── docs/          # Bab 1–12
├── tools/         # Tabranij visualizer
├── assets/
├── contoh/
└── referensi/
```

## Status

| Komponen | Status |
|----------|--------|
| Pengertian TABRANIJ | ✅ Final (TARI + rentang) |
| Bab 1–3 (Fondasi) | ✅ |
| Bab 4–6 (Membaca Grafik) | ✅ |
| Bab 7–9 (Eksekusi) | ⏳ Menyusul |
| Bab 10–12 (Alat & Disiplin) | ⏳ Menyusul |
| Tool visualizer | ✅ File HTML stabil (loader multi-part opsional) |
