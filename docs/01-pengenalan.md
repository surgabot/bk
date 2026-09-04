# Bab 1 — Pengenalan

## 1.1 Untuk siapa buku ini

Buku pegangan ini dibuat khusus untuk **anggota grup investasi & trading** yang memakai metode **GT (Grafik Tabranij)**.

Tujuannya sederhana:

- Menyamakan bahasa dan cara baca grafik di dalam grup  
- Memberi kerangka kerja yang konsisten (parameter, bias, entry/exit)  
- Mengurangi keputusan impulsif dengan aturan yang jelas  

Bukan buku “jadi kaya cepat”. Ini buku **cara kerja**.

---

## 1.2 Apa itu Metode GT

**GT** = **Grafik Tabranij**.

Metode ini memandang satu candle (atau rangkaian candle) lewat parameter tetap:

| Kode | Nama | Arti singkat |
|------|------|----------------|
| **T** | Tinggi | Titik tertinggi (high) |
| **A** | Awal | Harga awal / open (atau titik acuan awal) |
| **R** | Rendah | Titik terendah (low) |
| **I** | Inti | Titik inti / core — pusat logika GT |
| **N** | Neto | Nilai turunan: `N = 2 × I − A` |
| **J** | Julat | Rentang: `J = max(T,A,N,R) − min(T,A,N,R)` |

Dari parameter ini muncul:

- **Atas** body = `max(A, N)`  
- **Bawah** body = `min(A, N)`  
- **Bias** = Bullish jika `N ≥ A`, Bearish jika `N < A`

Intinya: **Inti (I)** menjadi poros. Awal (A) dan Neto (N) saling “mirror” terhadap Inti.

---

## 1.3 Kenapa perlu kerangka yang sama

Tanpa kerangka:

- Satu anggota bilang “bullish”, yang lain bilang “masih ragu”  
- Entry beda-beda, risiko tidak terukur  
- Sulit review trade secara objektif  

Dengan GT:

- Semua memakai parameter yang sama  
- Bias bisa dicek ulang di tool visualizer  
- Diskusi grup jadi lebih cepat dan tepat  

---

## 1.4 Cara memakai buku ini

1. **Baca Bagian I** sampai paham parameter (Bab 1–3).  
2. **Latihan di tool** Tabranij Pro (folder `tools/tabranij-visualizer`).  
3. **Lanjut Bagian II** untuk cara baca struktur multi-candle.  
4. **Bagian III** dipakai saat eksekusi nyata (entry, exit, risiko).  
5. **Checklist** (Bab 11) dipakai setiap sesi trading.  

---

## 1.5 Batasan

- Metode ini **alat bantu**, bukan jaminan profit.  
- Market bisa invalidasi setup kapan saja.  
- Disiplin risiko lebih penting daripada “menebak arah”.  

---

**Lanjut → [Bab 2 — Konsep Metode GT](02-konsep-gt.md)**
