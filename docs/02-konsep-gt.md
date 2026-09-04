# Bab 2 — Konsep Metode GT

## 2.1 Ide dasar: poros Inti

Di metode GT, **Inti (I)** adalah pusat.

Dari Inti, kita “memantulkan” Awal untuk mendapat Neto:

```
Neto (N) = 2 × Inti (I) − Awal (A)
```

Artinya:

- Jika A di **bawah** I, maka N akan di **atas** I (jarak sama).  
- Jika A di **atas** I, maka N akan di **bawah** I.  

Ini yang membuat body candle GT punya logika **simetri terhadap Inti**.

---

## 2.2 Empat titik input vs titik turunan

**Input (bisa diubah di tool):**

- Tinggi (T)  
- Awal (A)  
- Rendah (R)  
- Inti (I)  

**Turunan (otomatis):**

- Neto (N) = `2I − A`  
- Atas body = `max(A, N)`  
- Bawah body = `min(A, N)`  
- Julat (J) = rentang visual tertinggi − terendah dari {T, A, N, R}  

Di visualizer, T ditandai **biru**, R **oranye/merah**, I **putih/inti**, body hijau (bull) atau merah (bear).

---

## 2.3 Bias: Bullish vs Bearish

Aturan sederhana:

| Kondisi | Bias |
|---------|------|
| `N ≥ A` | **Bullish** (body hijau) |
| `N < A` | **Bearish** (body merah) |

Karena `N = 2I − A`:

- Bullish berarti Inti “mendorong” ke arah yang membuat Neto di atas atau sama dengan Awal.  
- Bearish sebaliknya.  

**Flip arah** di tool (tombol Naik/Turun) memantulkan A terhadap I, sehingga bias bisa dibalik untuk simulasi skenario lawan.

---

## 2.4 Julat (J) — ukuran “ruang” candle

Julat mengukur seberapa lebar struktur candle dalam kerangka GT:

```
J = max(T, A, N, R) − min(T, A, N, R)
```

Kegunaan praktis:

- Julat besar → volatilitas / rentang besar → stop dan target perlu disesuaikan  
- Julat kecil → candle “sempit” (mirip doji dalam bahasa klasik)  

Julat **bukan** selalu sama dengan `T − R` klasik, karena N bisa lebih ekstrem dari T atau R.

---

## 2.5 Hubungan dengan candle klasik (OHLC)

Pemetaan kasar (bukan 1:1 mutlak):

| GT | OHLC klasik (kira-kira) |
|----|-------------------------|
| T | High |
| R | Low |
| A | Open (atau acuan awal setup) |
| N | Close “efektif” dalam logika GT |
| I | Titik tengah logis / core (bukan selalu midpoint body) |

GT **tidak mengganti** OHLC. GT memberi **lapisan baca** di atas struktur harga: di mana poros Inti, ke mana Neto, dan bagaimana bias terbentuk.

---

## 2.6 Satu candle vs multi-candle

- **Single:** fokus paham T, A, R, I, N, J pada satu batang.  
- **Multi:** rangkaian candle — bias bisa berganti, struktur naik/turun terbaca dari urutan body dan wick.  

Timeframe (M1 … D1) mengubah “skala” volatilitas di tool (range slider), agar latihan mendekati karakter TF yang dipakai grup.

---

## 2.7 Ringkasan konsep

1. Inti = poros.  
2. Neto = pantulan Awal terhadap Inti.  
3. Bias = perbandingan N vs A.  
4. Julat = lebar struktur GT.  
5. Tool visualizer dipakai untuk melatih mata, bukan untuk “prediksi ajaib”.  

---

**Lanjut → [Bab 3 — Parameter TABRANIJ](03-parameter-tabranij.md)** (akan dilengkapi)

**Kembali → [Bab 1 — Pengenalan](01-pengenalan.md)**
