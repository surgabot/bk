# Bab 2 — Konsep Metode GT

## 2.1 GT dan TABRANIJ

**GT** = **Grafik Tabranij**.

Cara baca grafik dalam metode ini mengikuti sistem kode **TABRANIJ**: susunan huruf yang sudah ditimbang agar mudah diingat, dibaca secara visual, dan punya padanan matematis yang jelas.

```
T A B R A N I J
│ │ │ │ │ │ │ └─ Julat (Range)
│ │ │ │ │ │ └─── Inti (Variabel saat ini / close)
│ │ │ │ │ └───── Neto (Domain / body)
│ │ │ │ └─────── Awal (Konstanta / open)
│ │ │ └───────── Rendah (Dasar bawah)
│ │ └─────────── Bawah (Kodomain bawah body)
│ └───────────── Atas (Kodomain atas body)
└─────────────── Tinggi (Puncak atas)
```

---

## 2.2 Lapisan baca: luar → dalam

1. **Kerangka luar — T dan R**  
   Tinggi dan Rendah menetapkan **puncak** dan **dasar** periode.  
   Julat (J) = jarak keduanya.

2. **Kerangka body — Atas dan Bawah**  
   Kodomain atas/bawah body: sumbu atas dan bawah **Neto**.  
   `Atas = max(Awal, Inti)` · `Bawah = min(Awal, Inti)`.

3. **Isi body — Awal, Neto, Inti**  
   - **Awal** = konstanta (pembukaan)  
   - **Inti** = variabel saat ini (penutupan / harga sekarang)  
   - **Neto** = domain di antara keduanya (body)

Urutan hafalan mengikuti huruf TABRANIJ, sementara urutan **analisa** sering dari luar (T–R) ke dalam (Awal–Inti).

---

## 2.3 Definisi matematis tiap komponen

| Kode | Komponen | Representasi | Keterangan |
|------|----------|--------------|------------|
| **T** | Tinggi | Puncak Atas | Harga tertinggi periode |
| **A** | Atas | Kodomain Atas | Sumbu atas neto/body |
| **B** | Bawah | Kodomain Bawah | Sumbu bawah neto/body |
| **R** | Rendah | Dasar Bawah | Harga terendah periode |
| **A** | Awal | Konstanta | Harga pembukaan periode |
| **N** | Neto | Domain | Harga antara awal dan inti (body) |
| **I** | Inti | Variabel Saat Ini | Harga sekarang / penutupan |
| **J** | Julat | Range | Jangkauan rendah ke tinggi (`T − R`) |

---

## 2.4 Bias dari Awal dan Inti

| Kondisi | Bias |
|---------|------|
| Inti ≥ Awal | **Naik / Bullish** — variabel menutup di atas (atau sama) konstanta |
| Inti < Awal | **Turun / Bearish** — variabel menutup di bawah konstanta |

Neto (domain body) mengikuti arah itu: dari Awal menuju Inti.

---

## 2.5 Julat sebagai ukuran ruang

```
J = T − R
```

- Julat besar → periode volatil; wick dan body perlu dibaca hati-hati  
- Julat kecil → rentang sempit (sering mirip doji jika Neto juga kecil)  

Julat mengukur **jangkauan penuh** periode, bukan hanya tinggi body.

---

## 2.6 Satu periode vs banyak periode

- **Single:** kuasai T, A (Atas), B, R, A (Awal), N, I, J pada satu batang.  
- **Multi:** urutan Inti vs Awal antar candle membentuk struktur naik/turun.  
- **Timeframe:** mengubah skala periode (M1 … D1); kode TABRANIJ tetap sama.

---

## 2.7 Ringkasan konsep

1. TABRANIJ = sistem kode + hafalan + visual.  
2. T–R = kerangka luar; Atas–Bawah = kodomain body; Awal–Neto–Inti = isi body.  
3. Inti = variabel (close); Awal = konstanta (open).  
4. Julat = `T − R`.  
5. Tool visualizer melatih asosiasi huruf ↔ posisi di grafik.  

---

**Lanjut → [Bab 3 — Parameter TABRANIJ](03-parameter-tabranij.md)**  
**Kembali → [Bab 1 — Pengenalan](01-pengenalan.md)**
