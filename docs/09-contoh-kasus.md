# Bab 9 — Contoh Kasus

> Kasus di bawah **ilustratif** (angka dibulatkan).  
> Fokus pada alur berpikir GT, bukan “sinyal copy-paste”.

---

## 9.1 Cara membaca setiap kasus

Setiap kasus mengikuti template yang sama:

1. Konteks multi-TF  
2. TARI / rentang di TF trigger  
3. Rencana entry–SL–TP  
4. Risiko  
5. Hasil & pelajaran

---

## 9.2 Kasus A — Continuation long (sukses)

### Konteks

- **H4:** bias naik beruntun; harga di atas support `R ≈ 1.0800`  
- **H1:** pullback 4 candle bias turun; Neto mengecil  
- **M15:** basing di zona 1.0810–1.0820

### Candle trigger (M15)

```text
T = 1.0824
Awal = 1.0812
R = 1.0808
I = 1.0822

Atas  = 1.0824 − 1.0822 = 0.0002
Bawah = 1.0812 − 1.0808 = 0.0004
Neto  = 0.0010
Julat = 0.0016
Bias  = naik
```

### Rencana

| Item | Nilai |
|------|--------|
| Entry | Break `T = 1.0824` |
| SL | `1.0806` (di bawah R trigger & buffer) |
| TP1 | `1.0860` (menuju swing H1) |
| Jarak SL | 18 poin |
| Jarak TP1 | 36 poin |
| RR | 1 : 2 |
| Risiko | 0.75% akun |

### Hasil

Harga break T, hold Awal candle berikutnya di atas level, mencapai TP1.  
**+2R**.

### Pelajaran

- Pullback dengan Neto mengecil = bahan continuation, bukan panik sell  
- Invalidation menempel R struktur, bukan angka “dibulatkan jauh”

---

## 9.3 Kasus B — Fake break short (loss terkontrol)

### Konteks

- **H1:** range; resistance `T ≈ 150.00` sudah 2× ditolak (Atas besar)  
- Trader melihat close singkat di atas 150.00 dan entry short “rejection”

### Candle yang memicu (salah baca)

```text
T = 150.40
Awal = 149.90
R = 149.70
I = 150.20

Bias naik, Neto = 0.30, Atas = 0.20
```

Trader short di 150.10 karena “sudah jauh di atas level”, SL di 150.45.

### Yang terjadi

Candle berikutnya Awal di atas 150.00, bias naik lanjut → SL terkena.  
**−1R**.

### Pelajaran

- Close di atas level + Awal hold = **break**, bukan otomatis reversal  
- Rejection yang valid: I kembali *ke dalam* range + konfirmasi bias lawan  
- Loss 1R dengan SL tertulis = hasil yang bisa diterima; yang salah adalah bacaan break vs reject

---

## 9.4 Kasus C — Reversal di support (mixed)

### Konteks

- **H4:** turun; mendekati support lama `R ≈ 0.9900`  
- **H1:** Julat membesar; Bawah besar di 0.9902 (penolakan)

### Trigger H1

```text
T = 0.9940
Awal = 0.9910
R = 0.9900
I = 0.9935

Atas = 0.0005 · Bawah = 0.0010 · Neto = 0.0025 · Bias naik
```

### Rencana

| Item | Nilai |
|------|--------|
| Entry | Close H1 / agresif di atas Awal 0.9910 |
| SL | 0.9895 |
| TP1 | 0.9960 |
| RR | ≈ 1 : 1.7 |
| Risiko | 0.5% (counter ke arah H4 sebelumnya) |

### Hasil

TP1 tercapai sebagian (+1R), sisa ditrail lalu exit di 0.9948 saat H4 masih belum clear break struktur bear.  
Total ≈ **+1.3R**.

### Pelajaran

- Counter-trend: size lebih kecil (Bab 8)  
- Ambil parsial di level masuk akal; jangan memaksa “full TP” melawan HTF yang belum berbalik

---

## 9.5 Kasus D — Skip (tidak entry)

### Situasi

- LTF M5 bias naik kuat, Neto besar  
- **H1/H4** bias turun, harga di bawah resistance yang baru saja ditolak

### Keputusan

**Tidak entry long.**  
Alasan: trigger LTF melawan HTF tanpa setup counter tertulis & tanpa RR nyaman ke resistance.

### Pelajaran

- “Candle bagus” di LTF ≠ wajib trade  
- Skip adalah keputusan profesional, bukan ketinggalan

---

## 9.6 Template jurnal kasus (salin)

```text
Tanggal / instrumen / TF konteks / TF trigger:
Konteks 1 kalimat:
TARI trigger: T= … Awal= … R= … I= …
Atas= … Neto= … Bawah= … Julat= … Bias=
Entry / SL / TP1:
Risiko % / RR rencana:
Hasil (R):
Apa yang benar:
Apa yang salah / perbaikan:
```

Simpan contoh nyata grup di folder `contoh/` agar Bab 9 terus hidup.

---

## 9.7 Ringkasan Bagian III

| Bab | Inti |
|-----|------|
| 7 | Entry hanya dengan konteks + zona + trigger; exit = SL/TP/struktur |
| 8 | % risiko, size dari jarak SL, RR, disiplin harian |
| 9 | Latihan bacaan: sukses, loss terkontrol, mixed, skip |

---

**Bagian III selesai.**  
**Lanjut → [Bab 10 — Tool Visualizer Tabranij Pro](10-tool-visualizer.md)**  
**Kembali → [Bab 8 — Manajemen Risiko](08-manajemen-risiko.md)**  
**Daftar isi → [00-daftar-isi.md](00-daftar-isi.md)**
