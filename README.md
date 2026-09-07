# TABRANIJ — Buku Pegangan Metode GT

**Grafik Tabranij** · Buku pegangan grup investasi & trading  
Bab 1–15 · Metode membaca lilin harga dengan sistem TABRANIJ

**T**inggi · **A**tas · **B**awah · **R**endah · **A**wal · **N**eto · **I**nti · **J**ulat

---

## Apa itu TABRANIJ?

TABRANIJ adalah sistem kode visual untuk membaca anatomi satu lilin harga secara cepat, konsisten, dan bilingual.

| Huruf | Nama | Arti |
|-------|------|------|
| **T** | Tinggi | Harga tertinggi periode |
| **A** | Atas | `max(Awal, Inti)` — tepi atas tubuh |
| **B** | Bawah | `min(Awal, Inti)` — tepi bawah tubuh |
| **R** | Rendah | Harga terendah periode |
| **A** | Awal | Harga pembuka |
| **N** | Neto | `|Inti − Awal|` — tubuh kristal |
| **I** | Inti | Harga kini / penutupan |
| **J** | Julat | `Tinggi − Rendah` — seluruh tinggi |

**Identitas inti:**  
`Julat = Atas + Neto + Bawah`  
**Bias arah:** `Inti ≷ Awal`

---

## Daftar Isi

### Bagian I — Fondasi
1. [Pengenalan](docs/01-pengenalan.md)  
2. [Konsep Metode GT](docs/02-konsep-gt.md)  
3. [Parameter TABRANIJ](docs/03-parameter-tabranij.md)

### Bagian II — Membaca Grafik
4. [Membaca Candle dengan GT](docs/04-membaca-candle.md)  
5. [Bias, Arah, dan Struktur](docs/05-bias-arah-struktur.md)  
6. [Multi-Candle & Timeframe](docs/06-multi-candle-timeframe.md)

### Bagian III — Eksekusi
7. [Setup Entry & Exit](docs/07-entry-exit.md)  
8. [Manajemen Risiko](docs/08-manajemen-risiko.md)  
9. [Contoh Kasus](docs/09-contoh-kasus.md)

### Bagian IV — Alat & Disiplin
10. [Tool Visualizer Tabranij Pro](docs/10-tool-visualizer.md)  
11. [Checklist Harian Grup](docs/11-checklist-harian.md)  
12. [Glosarium](docs/12-glosarium.md)

### Bagian V — Finansial & Kebiasaan
13. [Nasihat Investasi](docs/13-nasihat-investasi.md)  
14. [Jurnal Trading](docs/14-jurnal-trading.md)  
15. [Mengelola Keuntungan dengan Bijak](docs/15-mengelola-keuntungan.md)

---

## Tool

**[Tabranij Pro Visualizer](tools/tabranij-visualizer/)**  
File HTML tunggal yang stabil. Buka langsung di browser.

Lab 3D terkait: [surgabot.github.io/tabranij](https://surgabot.github.io/tabranij/)

---

## Status

| Komponen | Status |
|----------|--------|
| Definisi TABRANIJ | ✅ |
| Bab 1–12 (inti metode GT) | ✅ |
| Bab 13–15 (investasi, jurnal, profit) | ✅ |
| Tool visualizer HTML | ✅ |

---

## Repo terkait

- [surgabot/tabranij](https://github.com/surgabot/tabranij) — Lab kristal 3D anatomi lilin harga
- [surgabot/grafiktabranij](https://github.com/surgabot/grafiktabranij) — Indikator MQL5 + token

---

*Surga Bot · Metode GT · TABRANIJ*
