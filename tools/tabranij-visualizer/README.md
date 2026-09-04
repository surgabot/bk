# Tabranij Pro v3.1 — TARI

## Status

Loader multi-file di repo sedang diperbaiki.

**Sementara:** pakai file tunggal `tabranij-pro-v31.html` yang dibagikan di chat Grok.

```bash
python3 -m http.server 8080
# buka http://localhost:8080/tabranij-pro-v31.html
```

## Model matematis

| Jenis | Kode | Rumus / arti |
|-------|------|----------------|
| Titik | **TARI** | Tinggi, Awal, Rendah, Inti |
| Rentang | Atas | `T − max(Awal, I)` |
| Rentang | Bawah | `min(Awal, I) − R` |
| Rentang | Neto | `|I − Awal|` |
| Rentang | Julat | `T − R` |

**Identitas:** `Julat = Atas + Neto + Bawah`  
**Bias:** naik jika `I ≥ Awal`
