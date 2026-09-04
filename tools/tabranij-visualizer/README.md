# Tabranij Pro v3.1 — TARI

Visualizer diselaraskan dengan definisi final TABRANIJ di buku pegangan.

## Model matematis

### Titik (TARI)
| Kode | Input tool | Arti |
|------|------------|------|
| **T** | Tinggi | High |
| **A** | Awal | Open (konstanta) |
| **R** | Rendah | Low |
| **I** | Inti | Close / harga saat ini |

### Rentang (otomatis)
| Kode | Rumus | Arti |
|------|--------|------|
| **Atas** | `T − max(Awal, I)` | Wick atas |
| **Bawah** | `min(Awal, I) − R` | Wick bawah |
| **Neto** | `|I − Awal|` | Lebar body |
| **Julat** | `T − R` | Range penuh |

**Identitas:** `Julat = Atas + Neto + Bawah` (dicek di UI dengan ✓)

**Bias:** Bullish jika `I ≥ Awal`, Bearish jika `I < Awal`

Body digambar dari **Awal → Inti**.

## Cara buka

```bash
cd tools/tabranij-visualizer
python3 -m http.server 8080
# buka http://localhost:8080
```

## File yang dibutuhkan

- `index.html` — loader
- `p0.js` … `p3.js` — payload aplikasi (gzip+base64)

> Download ZIP repo, extract, lalu jalankan local server di folder ini.
