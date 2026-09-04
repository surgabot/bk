# Bab 10 — Tool Visualizer Tabranij Pro

> Tool adalah **cermin** definisi Bab 3–6, bukan pengganti disiplin Bab 7–8.

---

## 10.1 Fungsi tool

| Fungsi | Manfaat untuk grup |
|--------|---------------------|
| Visual 3D / 2D candle | Melihat TARI dan rentang secara spasial |
| Slider T, Awal, R, Inti | Latihan “what if” tanpa platform trading |
| Hitung otomatis Atas, Neto, Bawah, Julat | Verifikasi identitas `J = A+N+B` |
| Bias | Konfirmasi I ≷ Awal |
| Multi-candle / TF / history | Latihan Bab 6 |

Tool **tidak** memberi sinyal beli/jual otomatis.

---

## 10.2 Lokasi di repository

```text
tools/tabranij-visualizer/
```

**Cara paling stabil (disarankan):**

1. Pakai **satu file HTML** lengkap (versi stabil TARI).  
2. Buka lewat browser (double-click atau `python3 -m http.server`).  
3. Hindari mengandalkan loader multi-part (`p0.js`…`p3.js`) jika sering error `atob` / `Failed to fetch`.

Loader multi-part hanya untuk eksperimen distribusi file besar di GitHub.

---

## 10.3 Peta kontrol → konsep GT

| Kontrol di tool | Konsep buku |
|-----------------|-------------|
| Slider / input **Tinggi (T)** | Titik TARI |
| **Awal** | Titik TARI (konstanta open) |
| **Rendah (R)** | Titik TARI |
| **Inti (I)** | Titik TARI (close / harga sekarang) |
| **Atas** | Rentang wick atas |
| **Neto** | Rentang body |
| **Bawah** | Rentang wick bawah |
| **Julat** | `T − R` |
| **Bias** | I vs Awal |
| Mode Single / Multi | Bab 4 vs Bab 6 |
| Timeframe | Label konteks, bukan feed live broker |
| History | Latihan rangkaian candle |

---

## 10.4 Latihan wajib dengan tool

### Latihan 1 — Identitas Julat

1. Set sembarang TARI valid (`T ≥ max(Awal,I)`, `R ≤ min(Awal,I)`).  
2. Baca Atas, Neto, Bawah, Julat.  
3. Pastikan `Atas + Neto + Bawah = Julat` (toleransi pembulatan).

### Latihan 2 — Doji

1. Set `I = Awal`.  
2. Neto harus ≈ 0.  
3. Atas + Bawah ≈ Julat.

### Latihan 3 — Wick dominan

1. Buat Bawah ≫ Neto (mirip hammer-like).  
2. Buat Atas ≫ Neto (mirip shooting-star-like).  
3. Latih satu kalimat bacaan **tanpa** langsung bilang entry.

### Latihan 4 — Multi-candle

1. Mode multi: susun 3–5 candle.  
2. Isi tabel Bias | Neto | Atas | Bawah (Bab 6).  
3. Tulis satu kalimat arah.

---

## 10.5 Batasan tool (penting)

| Bukan fungsi tool | Implikasi |
|-------------------|-----------|
| Data live broker | Angka latihan / manual |
| Order execution | Entry tetap di platform trading |
| Manajemen risiko otomatis | % risiko & size dihitung manual (Bab 8) |
| “Akurasi prediksi” | Tidak ada; hanya visualisasi struktur |

---

## 10.6 Troubleshooting singkat

| Gejala | Tindakan |
|--------|----------|
| `Failed to fetch` / `atob` | Pakai **HTML tunggal**, hard refresh, atau server lokal |
| Blank / Three.js tidak muncul | Perlu koneksi CDN; coba server lokal `http://localhost` |
| Angka aneh / identitas gagal | Cek urutan T ≥ … ≥ R; jangan I di luar [R, T] |
| Tampilan beda dengan buku | Pastikan rumus: Atas/Bawah memakai max/min(Awal,I) |

---

## 10.7 Checklist pemakaian tool di sesi grup

- [ ] Semua anggota paham TARI = titik, Atas/Neto/Bawah/Julat = rentang  
- [ ] Satu orang share screen tool atau chart live + bahasa GT  
- [ ] Latihan identitas Julat minimal 1×  
- [ ] Diskusi case tanpa memaksa “langsung entry”  
- [ ] Hasil case menarik disimpan ke `contoh/` (opsional)

---

**Lanjut → [Bab 11 — Checklist Harian Grup](11-checklist-harian.md)**  
**Kembali → [Bab 9 — Contoh Kasus](09-contoh-kasus.md)**
