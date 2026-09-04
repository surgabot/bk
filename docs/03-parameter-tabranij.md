# Bab 3 — Parameter TABRANIJ

> Daftar lengkap parameter + cara mengisinya di tool dan di analisa manual.

## 3.1 Tabel master

| Kode | Nama | Warna di tool | Sifat | Rumus / sumber |
|------|------|---------------|--------|----------------|
| **T** | Tinggi | Biru | Input | High / titik tertinggi setup |
| **A** | Awal | Putih | Input | Open / acuan awal |
| **R** | Rendah | Merah | Input | Low / titik terendah |
| **I** | Inti | Hijau | Input | Titik poros (core) |
| **N** | Neto | Primer (cyan) | Turunan | `2 × I − A` |
| **J** | Julat | — | Turunan | `max(T,A,N,R) − min(T,A,N,R)` |
| **Atas** | Atas body | — | Turunan | `max(A, N)` |
| **Bawah** | Bawah body | — | Turunan | `min(A, N)` |

---

## 3.2 Cara menentukan Inti (I)

Inti adalah parameter paling “subjektif” di awal latihan. Beberapa pendekatan yang dipakai grup:

1. **Midpoint body klasik** — titik tengah antara open dan close candle referensi  
2. **Level struktur** — harga yang sering dihormati (VWAP sesi, midpoint range, dll.) sesuai kesepakatan grup  
3. **Inti dari setup** — level yang sudah disepakati di plan sebelum entry  

Yang penting: **sekali Inti ditetapkan untuk setup itu, jangan digeser seenaknya** hanya karena harga bergerak.

---

## 3.3 Preset di tool (untuk latihan)

| Preset | Karakter |
|--------|----------|
| Bullish | Body hijau, N di atas A |
| Bearish | Body merah, N di bawah A |
| Doji | A ≈ N (body sangat kecil) |
| Long Wick | Julat besar, wick panjang |
| Hammer | Wick bawah dominan |
| Random | Latihan cepat, acak |

Gunakan preset untuk melatih mata, lalu input angka real dari chart.

---

## 3.4 Checklist isi parameter

Sebelum menyimpulkan bias:

- [ ] T ≥ semua titik relevan (atau sadar jika N menembus T)  
- [ ] R ≤ semua titik relevan (atau sadar jika N menembus R)  
- [ ] I berada di zona yang disepakati setup  
- [ ] A sesuai open / acuan yang dipakai grup  
- [ ] N dihitung ulang: `2I − A`  
- [ ] Bias dicek: N ≥ A atau tidak  

---

**Lanjut → Bab 4 (akan dilengkapi)**  
**Kembali → [Bab 2 — Konsep GT](02-konsep-gt.md)**
