# BK — Buku Pegangan Grup Investasi & Trading

**Metode GT (Grafik Tabranij)** · Bab 1–12 lengkap

Repository private untuk buku pegangan internal grup investasi & trading.

## Mulai di sini

**[Daftar Isi](docs/00-daftar-isi.md)**

| Bagian | Bab |
|--------|-----|
| **I · Fondasi** | [1](docs/01-pengenalan.md) · [2](docs/02-konsep-gt.md) · [3](docs/03-parameter-tabranij.md) |
| **II · Membaca Grafik** | [4](docs/04-membaca-candle.md) · [5](docs/05-bias-arah-struktur.md) · [6](docs/06-multi-candle-timeframe.md) |
| **III · Eksekusi** | [7](docs/07-entry-exit.md) · [8](docs/08-manajemen-risiko.md) · [9](docs/09-contoh-kasus.md) |
| **IV · Alat & Disiplin** | [10](docs/10-tool-visualizer.md) · [11](docs/11-checklist-harian.md) · [12](docs/12-glosarium.md) |

**Tool:** [Tabranij Pro](tools/tabranij-visualizer/) — utamakan file HTML tunggal yang stabil.

---

## Apa itu TABRANIJ?

**TABRANIJ** adalah susunan huruf dan kode yang ditata agar kalimat, visual, dan bilingual-nya berkesan — memudahkan cara membaca grafik sambil mengasosiasikan agar mudah dihafal.

Urutan huruf: **T · A · B · R · A · N · I · J**

### Titik (TARI)

| Kode | Komponen | Keterangan |
|------|----------|------------|
| **T** | Tinggi | Harga tertinggi periode |
| **A** | Awal | Harga pembukaan (konstanta) |
| **R** | Rendah | Harga terendah periode |
| **I** | Inti | Harga saat ini / penutupan |

### Rentang

| Kode | Rumus | Keterangan |
|------|--------|------------|
| **Atas** | `T − max(Awal, I)` | Wick atas |
| **Bawah** | `min(Awal, I) − R` | Wick bawah |
| **Neto** | `|I − Awal|` | Body |
| **Julat** | `T − R` | Range penuh |

**Identitas:** `Julat = Atas + Neto + Bawah` · **Bias:** `I ≷ Awal`

---

## Status

| Komponen | Status |
|----------|--------|
| Pengertian TABRANIJ | ✅ Final |
| Bab 1–12 | ✅ Lengkap |
| Tool visualizer | ✅ HTML stabil |
