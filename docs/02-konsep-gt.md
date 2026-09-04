# Bab 2 — Konsep Metode GT

## 2.1 GT, TABRANIJ, dan TARI

**GT** = **Grafik Tabranij**.

Sistem baca mengikuti kode **TABRANIJ**, dengan empat **titik** yang dihafal sebagai **TARI**:

```
T A B R A N I J
│   │ │ │ │ │ └─ Julat   (rentang penuh)
│   │ │ │ │ └─── Inti    (titik · variabel)     ─┐
│   │ │ │ └───── Neto    (rentang body)           │ TARI
│   │ │ └─────── Awal    (titik · konstanta)    ─┤ (titik:
│   │ └───────── Rendah  (titik)                 ─┤  T, Awal,
│   └─────────── Bawah   (rentang wick bawah)     │  R, Inti)
└─────────────── Tinggi  (titik)                 ─┘
                 Atas    (rentang wick atas)  ← huruf A kedua dalam TABRANIJ
```

Catatan: dalam urutan huruf TABRANIJ, **A** muncul dua kali — **Atas** (rentang) dan **Awal** (titik). Saat bicara, sebut lengkap agar tidak ambigu.

---

## 2.2 Titik dulu, baru rentang

Alur baca yang disarankan:

1. Isi **TARI** — Tinggi, Awal, Rendah, Inti  
2. Hitung **rentang**:  
   - Atas = `T − max(Awal, I)`  
   - Bawah = `min(Awal, I) − R`  
   - Neto = `|I − Awal|`  
   - Julat = `T − R`  
3. Cek identitas: `Atas + Neto + Bawah = Julat`  
4. Tentukan bias dari Inti vs Awal  

---

## 2.3 Visual satu periode

```
T ───────────────  Tinggi (titik)
    ║ Atas         rentang wick atas
────╫────────────  max(Awal, I)
    ║ Neto         rentang body
────╫────────────  min(Awal, I)
    ║ Bawah        rentang wick bawah
R ───────────────  Rendah (titik)

Awal · Inti = dua ujung body (titik)
Julat       = T − R = Atas + Neto + Bawah
```

---

## 2.4 Definisi matematis final

### Titik — TARI

| Kode | Komponen | Representasi | Keterangan |
|------|----------|--------------|------------|
| **T** | Tinggi | Puncak | Harga tertinggi periode |
| **A** | Awal | Konstanta | Harga pembukaan |
| **R** | Rendah | Dasar | Harga terendah periode |
| **I** | Inti | Variabel saat ini | Harga sekarang / penutupan |

### Rentang

| Kode | Komponen | Rumus | Keterangan |
|------|----------|--------|------------|
| **A** | Atas | `T − max(Awal, I)` | Wick atas |
| **B** | Bawah | `min(Awal, I) − R` | Wick bawah |
| **N** | Neto | `\|I − Awal\|` | Lebar body |
| **J** | Julat | `T − R` | Range penuh |

---

## 2.5 Bias

| Kondisi | Bias |
|---------|------|
| `I ≥ Awal` | Naik / Bullish |
| `I < Awal` | Turun / Bearish |

Body mengarah dari **Awal → Inti**. Neto hanya mengukur **besar** body, bukan arah.

---

## 2.6 Ringkasan konsep

1. **TARI** = empat titik wajib.  
2. **Atas, Bawah, Neto, Julat** = empat rentang.  
3. `Julat = Atas + Neto + Bawah`.  
4. Bias dari perbandingan Inti vs Awal.  
5. Tool dan bab berikutnya mengikuti definisi ini.  

---

**Lanjut → [Bab 3 — Parameter TABRANIJ](03-parameter-tabranij.md)**  
**Kembali → [Bab 1 — Pengenalan](01-pengenalan.md)**
