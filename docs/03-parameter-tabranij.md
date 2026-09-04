# Bab 3 — Parameter TABRANIJ

> Definisi final: titik **TARI** dan empat **rentang**.

---

## 3.1 Asal-usul nama

**TABRANIJ** disusun agar mudah dihafal (kalimat, visual, bilingual).  
Empat **titik** di dalamnya diikat lagi sebagai akronim **TARI**:

```
TARI = Tinggi · Awal · Rendah · Inti
```

---

## 3.2 Tabel master final

### A. Titik (posisi harga) — TARI

| Urutan TARI | Kode | Komponen | Representasi | Keterangan |
|-------------|------|----------|--------------|------------|
| 1 | **T** | Tinggi | Puncak Atas | Harga tertinggi periode |
| 2 | **A** | Awal | Konstanta | Harga pembukaan periode |
| 3 | **R** | Rendah | Dasar Bawah | Harga terendah periode |
| 4 | **I** | Inti | Variabel Saat Ini | Harga sekarang / penutupan |

### B. Rentang (ukuran ruang)

| Kode | Komponen | Representasi | Rumus | Keterangan |
|------|----------|--------------|--------|------------|
| **A** | Atas | Kodomain / wick atas | `T − max(Awal, I)` | Panjang wick atas |
| **B** | Bawah | Kodomain / wick bawah | `min(Awal, I) − R` | Panjang wick bawah |
| **N** | Neto | Domain body | `\|I − Awal\|` | Lebar body |
| **J** | Julat | Range | `T − R` | Jangkauan penuh |

**Identitas:**

```
Julat = Atas + Neto + Bawah
```

---

## 3.3 Dua huruf “A”

| Sebutan | Jenis | Makna |
|---------|--------|--------|
| **Awal** | Titik (anggota TARI) | Open / konstanta |
| **Atas** | Rentang | Wick atas |

Selalu sebut **“Awal”** atau **“Atas”**, jangan hanya “A”.

---

## 3.4 Urutan kerja praktis

1. Catat **TARI**: T, Awal, R, Inti  
2. Hitung rentang:  
   - `Atas = T − max(Awal, I)`  
   - `Bawah = min(Awal, I) − R`  
   - `Neto = |I − Awal|`  
   - `Julat = T − R`  
3. Verifikasi: `Atas + Neto + Bawah ≟ Julat`  
4. Bias: `I ≥ Awal` → naik; `I < Awal` → turun  

---

## 3.5 Asosiasi hafalan

| Kelompok | Isi | Gambar mental |
|----------|-----|----------------|
| **TARI** | Tinggi, Awal, Rendah, Inti | Empat “pasak” harga |
| Rentang luar | Atas, Bawah | Wick atas & bawah |
| Rentang isi | Neto | Ketebalan body |
| Rentang total | Julat | Seluruh tinggi candle |

Kalimat pengingat:

> Isi **TARI** dulu; lalu ukur **Atas–Neto–Bawah**; jumlahnya wajib sama dengan **Julat**.

---

## 3.6 Checklist satu periode

**Titik (TARI)**  
- [ ] Tinggi (T)  
- [ ] Awal  
- [ ] Rendah (R)  
- [ ] Inti (I)  

**Rentang**  
- [ ] Atas = `T − max(Awal, I)`  
- [ ] Bawah = `min(Awal, I) − R`  
- [ ] Neto = `|I − Awal|`  
- [ ] Julat = `T − R`  
- [ ] `Atas + Neto + Bawah = Julat`  

**Bias**  
- [ ] Inti vs Awal → naik / turun  

---

## 3.7 Preset tool (latihan)

| Preset | Baca TABRANIJ |
|--------|----------------|
| Bullish | I ≥ Awal; Neto = lebar body naik |
| Bearish | I < Awal; Neto = lebar body turun |
| Doji | Neto ≈ 0 (Awal ≈ Inti) |
| Long Wick | Atas dan/atau Bawah besar relatif Neto |
| Hammer | Bawah dominan (wick bawah panjang) |
| Random | Latihan acak |

---

**Lanjut → Bab 4 (siap dilanjutkan)**  
**Kembali → [Bab 2 — Konsep GT](02-konsep-gt.md)**
