# Bab 8 — Manajemen Risiko

> Setup bagus tanpa risiko terukur = spekulasi.  
> GT membantu **di mana** invalidation; Bab ini mengatur **berapa** yang dipertaruhkan.

---

## 8.1 Definisi dasar

| Istilah | Arti praktis |
|---------|----------------|
| **Risiko (R)** | Jumlah uang (atau % akun) yang hilang jika SL terkena |
| **Invalidation** | Harga di mana ide setup batal (sering di luar R atau T relevan) |
| **Jarak SL** | `|harga entry − harga invalidation|` |
| **Reward** | Jarak ke TP1 (atau TP terencana) |
| **RR** | Reward ÷ Risiko (jarak) |

Ide GT: invalidation menempel pada **struktur TARI**, bukan angka bulat sembarangan.

---

## 8.2 Risiko per trade (aturan grup — default)

Usulkan default internal (boleh disesuaikan ketua grup):

| Jenis | % akun per trade (maks) |
|-------|-------------------------|
| Setup standar (ikut HTF) | **0.5% – 1%** |
| Counter-trend | **≤ 0.25% – 0.5%** |
| High conviction (jarang) | **≤ 1%** (bukan 2–5%) |

**Satu hari:** total risiko terbuka disarankan tidak melebihi **2–3%** akun.  
Setelah **3 loss beruntun**: stop trading hari itu (reset emosi).

---

## 8.3 Menghitung size posisi

```text
Risiko uang = % risiko × ekuitas
Size        = Risiko uang ÷ (jarak SL × nilai per pip/poin)
```

Contoh sederhana:

```text
Ekuitas     = 10_000
Risiko      = 1% → 100
Entry       = 101.50
SL          = 100.50  → jarak = 1.00
Nilai/poin  = 1 uang per 0.01 lot per 1.00 (contoh fiktif)

Size disesuaikan agar loss di SL ≈ 100, bukan “lot yang biasa dipakai”.
```

Yang penting: **size mengikuti jarak SL**, bukan sebaliknya.

---

## 8.4 Invalidation berbasis TARI

| Arah | Invalidation tipikal | Catatan |
|------|----------------------|--------|
| Long | Di bawah **R** candle trigger atau **R** zona | Buffer kecil boleh (spread/noise) |
| Short | Di atas **T** candle trigger atau **T** zona | Sama |
| Breakout long | Kembali di bawah level break (close) | Fake break |
| Breakout short | Kembali di atas level break (close) | Fake break |

Buffer: terlalu sempit → stop hunt; terlalu lebar → RR jelek & overrisk.  
Sesuaikan dengan **Julat** rata-rata TF trigger.

---

## 8.5 RR minimum

| Situasi | RR jarak (TP1 vs SL) |
|---------|---------------------|
| Default | ≥ **1 : 1.5** (lebih baik **1 : 2**) |
| Scalp LTF | Boleh 1 : 1 jika winrate & biaya (spread) sudah dihitung |
| Counter-trend | Target realistis; jangan memaksa 1 : 5 di zona padat |

Jika RR < ambang dan tidak bisa digeser entry/SL secara valid → **skip**.

---

## 8.6 Mengelola trade terbuka

| Tindakan | Kapan | Aturan |
|----------|--------|--------|
| **Hold** | Struktur masih valid | Biarkan rencana bekerja |
| **TP parsial** | Di TP1 / level struktur | Kunci sebagian; geser SL ke BE jika sesuai rencana |
| **Trail** | Swing baru terbentuk | SL mengikuti R (long) atau T (short) struktur baru |
| **Exit awal** | Ide batal sebelum SL | Close manual; catat alasan |
| **Dilarang** | “Tambah posisi karena floating loss” | Averaging loss tanpa rencana = diluar SOP |

---

## 8.7 Korelasi & overlapping

- Jangan buka 3 posisi yang hakikatnya **satu ide yang sama** (satu arah, satu level) seolah risiko terpisah.  
- Hitung sebagai **satu risiko agregat**.  
- Instrumen berkorelasi tinggi (mis. pasangan FX serupa) = risiko digabung.

---

## 8.8 Jurnal risiko (minimal)

Setiap trade catat:

1. % risiko & nominal  
2. Entry, SL, TP1 (harga)  
3. Jarak SL & RR rencana  
4. Hasil (R multiple: +1R, −1R, +0.5R, …)  
5. Apakah SL/TP dihormati? (ya/tidak + alasan)

Tanpa jurnal, Bab 7–8 hanya teori.

---

## 8.9 Checklist risiko pre-entry

- [ ] % risiko sesuai jenis setup  
- [ ] Jarak SL dari struktur TARI (bukan feeling)  
- [ ] Size dihitung dari risiko & jarak  
- [ ] RR ke TP1 ≥ ambang grup  
- [ ] Total risiko harian masih di bawah batas  
- [ ] Tidak ada overlapping ide yang sama  
- [ ] Siap loss penuh 1R tanpa mengubah SL impulsif

---

**Lanjut → [Bab 9 — Contoh Kasus](09-contoh-kasus.md)**  
**Kembali → [Bab 7 — Setup Entry & Exit](07-entry-exit.md)**
