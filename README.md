# BK — Buku Pegangan Grup Investasi & Trading

**Metode GT (Grafik Tabranij)**

Repository private untuk buku pegangan internal grup investasi & trading.

## Mulai di sini

- **[Daftar Isi Buku](docs/00-daftar-isi.md)**
- **[Bab 1 — Pengenalan](docs/01-pengenalan.md)**
- **[Bab 2 — Konsep GT](docs/02-konsep-gt.md)**
- **[Bab 3 — Parameter TABRANIJ](docs/03-parameter-tabranij.md)**
- **Tool:** [Tabranij Pro v3](tools/tabranij-visualizer/)

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
| **N** | Neto | `\|I − Awal\|` | Lebar body |
| **J** | Julat | `T − R` | Jangkauan penuh periode |

**Identitas:** `Julat = Atas + Neto + Bawah`

**Bias:** naik jika `I ≥ Awal`, turun jika `I < Awal`.

---

## Struktur Repository

```
bk/
├── docs/
├── tools/tabranij-visualizer/
├── assets/
├── contoh/
└── referensi/
```

## Status

| Komponen | Status |
|----------|--------|
| Pengertian TABRANIJ | ✅ Final (TARI + rentang) |
| Tool Tabranij Pro v3 | ✅ Ada (akan diselaraskan rumus) |
| Bab 1–3 (Fondasi) | ✅ Diselaraskan |
| Bab 4–12 | ⏳ Menyusul |
