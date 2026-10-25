## PERHITUNGAN KONDISI KAMAR
### Digital Twin Kamar Kos
| Parameter | Nilai | Satuan | Perhitungan | Hasil |
|---|---:|---|---|---|
| Suhu Ruangan | 28 | °C | 20 - 30 °C | Normal |
| Kelembapan Ruangan | 65 | % | 40 - 70 % | Normal |
| Status Lampu | AKTIF | - | AKTIF = Menyala | Menyala |
### Keterangan
| Parameter | Kondisi |
|---|---|
| Suhu < 20 °C | Dingin |
| Suhu 20 - 30 °C | Normal |
| Suhu > 30 °C | Panas |
| Kelembapan < 40 % | Kering |
| Kelembapan 40 - 70 % | Normal |
| Kelembapan > 70 % | Lembap |
| Lampu AKTIF | Menyala |
| Lampu OFF | Mati |
### Kesimpulan
Berdasarkan data yang diperoleh:
- Suhu ruangan **28 °C** → **Normal**
- Kelembapan ruangan **65 %** → **Normal**
- Status lampu **AKTIF** → **Menyala**
**Kondisi kamar: NORMAL**

**Hasil: Function Point ≈ 118,8 FP** (UFP 111 × VAF 1,07)

**1. Unadjusted Function Point (bobot IFPUG)**

| Komponen | Fungsi | Bobot | Subtotal |
|---|---|---|---|
| ILF (data internal) | Penyewa (rendah), Kamar (rendah), Kontrak (sedang), Pembayaran (sedang), Data Sensor (sedang) | 7+7+10+10+10 | 44 |
| EIF (data eksternal) | Gateway Pembayaran (rendah) | 5 | 5 |
| EI (input) | Registrasi penyewa (sedang), Kelola data kamar (rendah), Buat kontrak (sedang), Catat pembayaran (sedang), Terima data sensor (sedang), Kontrol kunci pintu (rendah) | 4+3+4+4+4+3 | 22 |
| EO (output) | Laporan hunian (sedang), Laporan pembayaran (sedang), Laporan konsumsi listrik (tinggi), Notifikasi anomali (sedang), Tagihan sewa (rendah) | 5+5+7+5+4 | 26 |
| EQ (query) | Status kamar real-time (sedang), Riwayat pembayaran (rendah), Data penyewa (rendah), Riwayat sensor (sedang) | 4+3+3+4 | 14 |
| **UFP** | | | **111** |

**2. Value Adjustment Factor (14 karakteristik, skala 0–5)**

Komunikasi data 5, Pengolahan terdistribusi 3, Performa 4, Konfigurasi padat 2, Laju transaksi 3, Entri data online 4, Efisiensi pengguna 4, Update online 3, Pemrosesan kompleks 3, Reusabilitas 2, Kemudahan instalasi 2, Kemudahan operasional 3, Banyak lokasi 1, Kemudahan perubahan 3.

- Total Degree of Influence (TDI) = 42
- VAF = 0,65 + (0,01 × 42) = **1,07**

**3. Function Point**

FP = UFP × VAF = 111 × 1,07 = **118,77 ≈ 118,8 FP**

Kalau produktivitas tim diasumsikan 10 jam/FP, estimasi usahanya sekitar 1.188 jam kerja.

Fungsi, tingkat kompleksitas, dan skor di atas adalah asumsi saya berdasarkan diagram yang sudah kita buat. Sesuaikan dengan fitur Sprint 2 kalau ada yang berbeda. Mau saya buatkan versi Excel dengan rumus otomatis supaya mudah diubah?
