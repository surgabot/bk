# Bab 12 — Glosarium

> Istilah resmi grup.  
> Jika ragu, kembali ke Bab 3 (parameter) dan Bab 4–6 (cara baca).

---

## 12.1 Inti metode

| Istilah | Arti |
|---------|------|
| **GT** | Grafik Tabranij — metode baca grafik grup ini |
| **TABRANIJ** | Susunan kode huruf: T·A·B·R·A·N·I·J (titik + rentang) |
| **TARI** | Empat **titik** harga: **T**inggi · **A**wal · **R**endah · **I**nti |

---

## 12.2 Titik (TARI)

| Kode | Nama | Arti |
|------|------|------|
| **T** | Tinggi | Harga tertinggi periode (high) |
| **Awal** | Awal | Harga pembukaan periode (open); konstanta |
| **R** | Rendah | Harga terendah periode (low) |
| **I** | Inti | Harga penutupan atau harga saat ini (close / live) |

> Jangan menyingkat Awal hanya “A” tanpa konteks — bentrok dengan **Atas**.

---

## 12.3 Rentang

| Kode | Nama | Rumus | Arti |
|------|------|--------|------|
| **Atas** | Atas | `T − max(Awal, I)` | Panjang wick atas |
| **Bawah** | Bawah | `min(Awal, I) − R` | Panjang wick bawah |
| **Neto** | Neto | `|I − Awal|` | Lebar body |
| **Julat** | Julat | `T − R` | Jangkauan penuh periode |

**Identitas:** `Julat = Atas + Neto + Bawah`

---

## 12.4 Bias & arah

| Istilah | Arti |
|---------|------|
| **Bias naik** | `I > Awal` (atau `≥` sesuai kesepakatan grup) |
| **Bias turun** | `I < Awal` |
| **Netral / doji** | `I ≈ Awal` → Neto ≈ 0 |
| **Arah** | Kecenderungan dari **rangkaian** bias (bukan satu candle) |
| **Counter-trend** | Trade melawan arah HTF (size lebih kecil) |

---

## 12.5 Struktur & eksekusi

| Istilah | Arti |
|---------|------|
| **Swing high** | Area **T** menonjol lalu harga ditolak |
| **Swing low** | Area **R** menonjol lalu harga ditolak |
| **Zona** | Area support/resistance / pullback tempat ide dibangun |
| **Trigger** | Perilaku candle yang mengizinkan entry |
| **Invalidation** | Harga di mana ide batal (sering di luar T atau R relevan) |
| **Break & hold** | Tembus level + Awal/close bertahan di sisi break |
| **Fake break** | Tembus sebentar lalu kembali ke dalam range |
| **HTF / MTF / LTF** | Timeframe tinggi / menengah / rendah |

---

## 12.6 Risiko

| Istilah | Arti |
|---------|------|
| **R (unit risiko)** | 1× kerugian jika SL terkena sesuai rencana |
| **RR** | Reward : Risk (jarak TP vs jarak SL) |
| **Size** | Besaran posisi; dihitung dari % risiko dan jarak SL |
| **Trail** | Menggeser SL mengikuti struktur baru yang menguntungkan |
| **BE (break-even)** | SL dipindah ke area entry (atau sedikit profit) |

---

## 12.7 Tool & proses

| Istilah | Arti |
|---------|------|
| **Tabranij Pro** | Tool visualizer di `tools/tabranij-visualizer/` |
| **HTML tunggal** | File visualizer lengkap tanpa loader `p0–p3` (paling stabil) |
| **Jurnal** | Catatan trade: TARI, rencana, hasil R, pelajaran |
| **Skip** | Keputusan sadar untuk tidak entry |

---

## 12.8 OHLC ↔ GT (cepat)

| OHLC | GT |
|------|-----|
| Open | Awal |
| High | T |
| Low | R |
| Close | I (jika candle selesai) |

---

## 12.9 Kalimat baku grup (contoh)

- “TARI dulu, baru rentang.”  
- “Julat wajib = Atas + Neto + Bawah.”  
- “Bias dari I vs Awal; arah dari rangkaian.”  
- “Entry tanpa invalidation = tidak valid.”  
- “Skip itu keputusan, bukan ketinggalan.”

---

## 12.10 Indeks bab

| Topik | Bab |
|-------|-----|
| Pengenalan | 1 |
| Konsep GT | 2 |
| Parameter TABRANIJ | 3 |
| Baca satu candle | 4 |
| Bias, arah, struktur | 5 |
| Multi-candle & TF | 6 |
| Entry & exit | 7 |
| Risiko | 8 |
| Contoh kasus | 9 |
| Tool | 10 |
| Checklist harian | 11 |
| Glosarium | 12 |

---

**Selesai — Buku Pegangan GT (Bab 1–12).**  
**Daftar isi → [00-daftar-isi.md](00-daftar-isi.md)**  
**Kembali → [Bab 11 — Checklist Harian](11-checklist-harian.md)**
