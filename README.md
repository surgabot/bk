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

| Kode | Komponen | Representasi matematis | Keterangan |
|------|----------|------------------------|------------|
| **T** | Tinggi | Puncak Atas | Harga tertinggi pada suatu periode |
| **A** | Atas | Kodomain Atas | Sumbu atas (atasnya neto/body) |
| **B** | Bawah | Kodomain Bawah | Sumbu bawah (bawahnya neto/body) |
| **R** | Rendah | Dasar Bawah | Harga terendah pada suatu periode |
| **A** | Awal | Konstanta | Harga awal / pembukaan pada suatu periode |
| **N** | Neto | Domain | Harga antara awal dan inti (body) |
| **I** | Inti | Variabel Saat Ini | Harga sekarang / harga penutupan |
| **J** | Julat | Range | Jangkauan antara rendah dan tinggi |

### Cara menghafal (asosiasi)

```
T  Tinggi     → puncak
A  Atas       → sumbu atas body
B  Bawah      → sumbu bawah body
R  Rendah     → dasar
A  Awal       → konstanta (open)
N  Neto       → domain body
I  Inti       → variabel saat ini (close)
J  Julat      → range T−R
```

Baca dari luar ke dalam: **Tinggi–Rendah** membungkus **Atas–Bawah** body, yang terbentuk dari **Awal–Inti** (Neto), dengan **Julat** sebagai ukuran jangkauan.

---

## Struktur Repository

```
bk/
├── docs/                      # Isi buku pegangan
├── tools/tabranij-visualizer/ # Tool 3D interaktif
├── assets/
├── contoh/
└── referensi/
```

## Status

| Komponen | Status |
|----------|--------|
| Pengertian TABRANIJ | ✅ Resmi (tabel di atas) |
| Tool Tabranij Pro v3 | ✅ Multi-candle, TF, History |
| Bab 1–3 (Fondasi) | ✅ Diselaraskan |
| Bab 4–12 | ⏳ Menyusul |
