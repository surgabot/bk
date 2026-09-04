# Bab 3 — Parameter TABRANIJ

> Definisi resmi kode, komponen, representasi matematis, dan keterangan.

---

## 3.1 Asal-usul nama TABRANIJ

**TABRANIJ** bukan singkatan acak. Huruf-hurufnya **disusun, ditimbang, dan ditata** agar:

1. **Kalimat** — urutan baca terasa alami (dari puncak ke dasar, dari open ke close)  
2. **Visual** — setiap kode bisa dikaitkan dengan posisi di candle  
3. **Bilingual** — istilah Indonesia + padanan matematis (puncak, kodomain, domain, range)  
4. **Hafalan** — asosiasi kuat: satu rangkaian huruf = satu sistem baca lengkap  

Urutan tetap: **T – A – B – R – A – N – I – J**

---

## 3.2 Tabel master (definisi resmi)

| No | Kode | Komponen | Representasi matematis | Keterangan |
|----|------|----------|------------------------|------------|
| 1 | **T** | Tinggi | Puncak Atas | Harga tertinggi pada suatu periode |
| 2 | **A** | Atas | Kodomain Atas | Sumbu atas (atasnya neto/body) |
| 3 | **B** | Bawah | Kodomain Bawah | Sumbu bawah (bawahnya neto/body) |
| 4 | **R** | Rendah | Dasar Bawah | Harga terendah pada suatu periode |
| 5 | **A** | Awal | Konstanta | Harga awal / pembukaan pada suatu periode |
| 6 | **N** | Neto | Domain | Harga antara awal dan inti (body) |
| 7 | **I** | Inti | Variabel Saat Ini | Harga sekarang / harga penutupan |
| 8 | **J** | Julat | Range | Jangkauan antara rendah dan tinggi |

### Catatan dua huruf **A**

Dalam TABRANIJ ada **dua peran “A”** yang berbeda konteks:

| Konteks | Makna |
|---------|--------|
| **A = Atas** | Kodomain atas body (sumbu atas neto) |
| **A = Awal** | Konstanta pembukaan periode |

Saat berbicara, sebut lengkap: **“Atas”** atau **“Awal”**, jangan hanya “A”, agar tidak ambigu.

---

## 3.3 Pemetaan visual di candle

```
        T  ← Tinggi (Puncak Atas)
        │
        │     wick atas
        │
    A ──┤  ← Atas (Kodomain Atas)  = max(Awal, Inti)
        │
        │     N = Neto (Domain / body)
        │
    B ──┤  ← Bawah (Kodomain Bawah) = min(Awal, Inti)
        │
        │     wick bawah
        │
        R  ← Rendah (Dasar Bawah)

    Awal (Konstanta) ── open
    Inti (Variabel)  ── close / harga saat ini
    Julat (Range)    ── T − R  (jangkauan penuh)
```

---

## 3.4 Hubungan matematis ringkas

| Relasi | Rumus / aturan |
|--------|----------------|
| Atas (kodomain) | `Atas = max(Awal, Inti)` |
| Bawah (kodomain) | `Bawah = min(Awal, Inti)` |
| Neto (domain) | Segmen harga **antara Awal dan Inti** (body) |
| Julat (range) | `J = Tinggi − Rendah` = `T − R` |
| Bias naik | Inti ≥ Awal (body menutup di atas atau sama dengan open) |
| Bias turun | Inti < Awal |

**Inti** = variabel saat ini (penutupan / harga sekarang).  
**Awal** = konstanta pembukaan periode yang sedang dibaca.

---

## 3.5 Asosiasi hafalan (bilingual)

| Kode | ID | EN / matematis | Gambar mental |
|------|----|----------------|---------------|
| T | Tinggi | Peak / High | Puncak gunung |
| A | Atas | Upper codomain | Atap body |
| B | Bawah | Lower codomain | Lantai body |
| R | Rendah | Floor / Low | Dasar lembah |
| A | Awal | Constant / Open | Titik mulai (tetap) |
| N | Neto | Domain / Body | Isi di antara open–close |
| I | Inti | Variable / Close | Titik “sekarang” |
| J | Julat | Range | Lebar seluruh candle |

Kalimat pengingat:

> **Tinggi–Atas–Bawah–Rendah** mengurung struktur; **Awal–Neto–Inti** mengisi body; **Julat** mengukur jarak Rendah ke Tinggi.

---

## 3.6 Checklist baca satu periode

- [ ] **T** — sudah identifikasi harga tertinggi periode  
- [ ] **R** — sudah identifikasi harga terendah periode  
- [ ] **Awal** — open / konstanta pembukaan  
- [ ] **Inti** — close / variabel saat ini  
- [ ] **Atas / Bawah** — kodomain body = max/min (Awal, Inti)  
- [ ] **Neto** — domain body terbaca (arah & ukuran)  
- [ ] **Julat** — `T − R`  
- [ ] Bias — Inti vs Awal (naik / turun)  

---

## 3.7 Preset di tool (latihan)

| Preset | Karakter dalam bahasa TABRANIJ |
|--------|--------------------------------|
| Bullish | Inti ≥ Awal → Neto mengarah naik |
| Bearish | Inti < Awal → Neto mengarah turun |
| Doji | Awal ≈ Inti → Neto hampir nol |
| Long Wick | Julat besar, wick panjang (T/R menjauh dari Atas–Bawah) |
| Hammer | Wick bawah dominan (R jauh di bawah Bawah) |
| Random | Latihan acak |

---

**Lanjut → Bab 4 (akan dilengkapi setelah fondasi ini dikunci)**  
**Kembali → [Bab 2 — Konsep GT](02-konsep-gt.md)**
