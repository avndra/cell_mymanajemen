# Sparepart Plan Buat Manajemen

## Tujuan

Mencatat sparepart yang sering dibutuhkan agar modal tidak terjebak di stok yang jarang laku.

---

# Kategori Prioritas

## Prioritas A (Wajib Stok)

Sparepart yang sering dicari pelanggan.

### LCD

- Redmi Note Series
- Redmi 9A
- Redmi 9C
- Redmi 10
- Redmi 12
- Redmi 13C

### Baterai

- Redmi Note Series
- Oppo A Series
- Vivo Y Series

### Charger

- Type-C
- Micro USB
- Lightning

### Flexible

- Charger Port
- Power Button
- Volume Button

---

## Prioritas B (Stok Terbatas)

### Kamera

- Kamera depan
- Kamera belakang

### Speaker

- Speaker atas
- Speaker bawah

### Earpiece

---

## Prioritas C (Pesan Jika Ada Order)

### Mainboard

### IC Power

### IC Charging

### Face ID Module

### Komponen iPhone tertentu

---

# Vendor / Supplier

| Supplier | Produk | Kontak | Catatan |
|-----------|----------|----------|----------|
| Supplier A | LCD | - | Harga stabil |
| Supplier B | Baterai | - | Pengiriman cepat |

---

# Target Stok Minimum

| Barang | Minimal |
|----------|----------|
| LCD Redmi 9A | 2 |
| LCD Redmi 9C | 2 |
| LCD Redmi 12 | 2 |
| Charger Type-C | 10 |
| Charger Micro USB | 10 |

---

# Sistem Restock

## Restock Otomatis

Jika stok <= minimum:

Status:

```text
RESTOCK REQUIRED
```

Contoh:

```text
LCD Redmi 9A
Stok : 1
Minimum : 2

RESTOCK REQUIRED
```

---

# Barang Fast Moving

Daftar barang yang paling cepat terjual.

| Barang | Bulan Ini |
|----------|----------|
| LCD Redmi 9A | 8 |
| Charger Type-C | 20 |
| Baterai Oppo A16 | 5 |

---

# Barang Slow Moving

Daftar barang yang jarang keluar.

| Barang | Bulan Ini |
|----------|----------|
| Kamera Redmi Note 8 | 0 |
| IC Power Samsung A20 | 0 |

Evaluasi setiap 3 bulan.

---

# Catatan Kerugian

Catat:

- Barang rusak
- Barang hilang
- Salah beli
- Garansi supplier

Contoh:

2026-07-12
LCD Redmi 9C retak saat pemasangan.
Kerugian: Rp 85.000

---

# Target Jangka Panjang

- [ ] Sistem inventori berbasis React dengan Python
- [ ] Barcode sparepart
- [ ] Dashboard stok
- [ ] Multi cabang
- [ ] Laporan otomatis bulanan
