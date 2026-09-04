# Bab 4 — Membaca Candle dengan GT

> Satu candle = satu “kalimat” TABRANIJ.  
> Baca **titik** dulu (TARI), lalu ukur **rentang**, baru simpulkan bias.

---

## 4.1 Urutan baca yang disarankan

Jangan langsung menebak “bullish/bearish” dari warna saja. Ikuti urutan:

```
1. TARI   →  Tinggi · Awal · Rendah · Inti
2. Rentang →  Atas · Neto · Bawah · Julat
3. Cek     →  Atas + Neto + Bawah ≟ Julat
4. Bias    →  Inti ≷ Awal
5. Bentuk  →  proporsi wick vs body
```

Kalimat pengingat:

> **Pasak dulu, ukur ruang, cek jumlah, baru arah.**

---

## 4.2 Memetakan OHLC ke TARI

| OHLC klasik | Kode GT | Nama |
|-------------|---------|------|
| High | **T** | Tinggi |
| Open | **Awal** | Awal |
| Low | **R** | Rendah |
| Close (atau harga sekarang) | **I** | Inti |

**Catatan penting**

- **Inti** = harga penutupan **jika** candle sudah selesai;  
  atau **harga saat ini** jika candle masih berjalan.
- **Awal** tetap (konstanta) sepanjang periode yang sama.
- Warna candle **bukan** definisi utama; definisi utama adalah **I vs Awal**.

---

## 4.3 Menghitung rentang (satu langkah)

Setelah empat titik diketahui:

```text
Atas  = T − max(Awal, I)     → wick atas
Bawah = min(Awal, I) − R     → wick bawah
Neto  = |I − Awal|           → lebar body
Julat = T − R                → tinggi total
```

**Identitas wajib:**

```text
Julat = Atas + Neto + Bawah
```

Jika tidak cocok (selisih > toleransi pembulatan), cek ulang titik TARI — ada yang salah catat.

---

## 4.4 Membaca proporsi

Proporsi memberi “karakter” candle, bukan sinyal masuk otomatis.

| Pola proporsi | Ciri rentang | Bacaan ringkas |
|---------------|--------------|----------------|
| **Body dominan** | Neto besar vs Atas & Bawah | Keputusan harga kuat ke arah bias |
| **Doji** | Neto ≈ 0 (Awal ≈ Inti) | Keseimbangan / keraguan |
| **Wick atas panjang** | Atas besar | Penolakan di zona tinggi |
| **Wick bawah panjang** | Bawah besar | Penolakan di zona rendah |
| **Hammer-like** | Bawah ≫ Atas, Neto sedang | Tekanan beli dari bawah (konteks penting) |
| **Shooting-star-like** | Atas ≫ Bawah, Neto sedang | Tekanan jual dari atas (konteks penting) |
| **Marubozu-like** | Atas ≈ 0 dan Bawah ≈ 0 | Body hampir penuh Julat |

> Nama pola klasik boleh dipakai sebagai **bahasa sekunder**.  
> Bahasa primer grup: **TARI + Atas/Neto/Bawah/Julat**.

---

## 4.5 Contoh numerik

### Contoh A — bias naik, body sedang

```text
T = 105
Awal = 100
R = 98
I = 103
```

Hitung:

```text
Atas  = 105 − max(100, 103) = 105 − 103 = 2
Bawah = min(100, 103) − 98  = 100 − 98  = 2
Neto  = |103 − 100| = 3
Julat = 105 − 98 = 7
Cek   : 2 + 3 + 2 = 7 ✓
Bias  : I > Awal → naik
```

Bacaan: naik dengan wick seimbang; body 3 dari 7.

### Contoh B — doji di tengah range

```text
T = 110
Awal = 105
R = 100
I = 105
```

```text
Atas  = 110 − 105 = 5
Bawah = 105 − 100 = 5
Neto  = 0
Julat = 10
Cek   : 5 + 0 + 5 = 10 ✓
Bias  : I = Awal → netral (doji)
```

Bacaan: tidak ada body; pasar menguji atas dan bawah setara.

### Contoh C — wick bawah dominan

```text
T = 102
Awal = 101
R = 90
I = 100
```

```text
Atas  = 102 − max(101, 100) = 102 − 101 = 1
Bawah = min(101, 100) − 90  = 100 − 90  = 10
Neto  = |100 − 101| = 1
Julat = 102 − 90 = 12
Cek   : 1 + 1 + 10 = 12 ✓
Bias  : I < Awal → turun (lemah)
```

Bacaan: body kecil, wick bawah panjang — tekanan jual sempat dalam, lalu tertarik naik kembali mendekati Awal. **Jangan langsung “beli” hanya karena wick panjang**; tunggu Bab 5 (struktur) dan Bab 7 (entry).

---

## 4.6 Checklist baca satu candle

**Titik**
- [ ] T tercatat  
- [ ] Awal tercatat  
- [ ] R tercatat  
- [ ] I tercatat (close atau live)

**Rentang**
- [ ] Atas dihitung  
- [ ] Bawah dihitung  
- [ ] Neto dihitung  
- [ ] Julat dihitung  
- [ ] Identitas Atas + Neto + Bawah = Julat

**Simpulan singkat**
- [ ] Bias: naik / turun / netral  
- [ ] Proporsi: body / wick atas / wick bawah  
- [ ] Satu kalimat bacaan (tanpa paksa entry)

---

## 4.7 Kesalahan umum

| Kesalahan | Akibat | Perbaikan |
|-----------|--------|-----------|
| Hanya lihat warna | Salah baca saat candle live | Pakai I vs Awal |
| Lupa max/min di rumus Atas/Bawah | Identitas Julat gagal | Selalu `max(Awal,I)` dan `min(Awal,I)` |
| Menyamakan “A” untuk Awal dan Atas | Bingung di diskusi grup | Sebut **Awal** atau **Atas** |
| Langsung entry dari satu candle | Overtrade | Satu candle = informasi, bukan setup lengkap |
| Mengabaikan Julat | Tidak tahu “ukuran” gerakan | Selalu catat Julat |

---

## 4.8 Latihan singkat

Hitung TARI + rentang + bias untuk data berikut (jawaban di akhir bab):

1. `T=50, Awal=45, R=40, I=48`  
2. `T=50, Awal=48, R=40, I=42`  
3. `T=50, Awal=45, R=40, I=45`  

---

## 4.9 Jawaban latihan

1. Atas=2, Bawah=5, Neto=3, Julat=10 → naik  
2. Atas=2, Bawah=2, Neto=6, Julat=10 → turun  
3. Atas=5, Bawah=5, Neto=0, Julat=10 → netral (doji)  

---

**Lanjut → [Bab 5 — Bias, Arah, dan Struktur](05-bias-arah-struktur.md)**  
**Kembali → [Bab 3 — Parameter TABRANIJ](03-parameter-tabranij.md)**
