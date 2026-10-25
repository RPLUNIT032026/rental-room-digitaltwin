# User Story - Rental Room Digital Twin

## Daftar Aktor

| Aktor | Deskripsi |
|-------|-----------|
| Penyewa | Pengguna yang menyewa kamar |
| Pemilik/Admin | Pengelola properti dan sistem |
| Sistem | Sistem digital twin yang memantau kondisi kamar |

---

## Daftar User Story

### US-01: Melihat Daftar Kamar
**Sebagai** penyewa,
**saya ingin** melihat daftar kamar beserta status ketersediaannya,
**agar** saya dapat memilih kamar yang sesuai kebutuhan.

**Kriteria Penerimaan:**
- Daftar kamar menampilkan nama, harga, fasilitas, dan status (tersedia/terisi).
- Penyewa dapat memfilter kamar berdasarkan harga dan fasilitas.

**Prioritas:** Tinggi | **Story Point:** 3

---

### US-02: Melihat Kondisi Kamar secara Digital Twin
**Sebagai** penyewa,
**saya ingin** melihat representasi digital (digital twin) dari kamar,
**agar** saya dapat mengetahui kondisi dan tata letak kamar tanpa datang langsung.

**Kriteria Penerimaan:**
- Visualisasi kamar tampil dengan data terbaru.
- Data kondisi (suhu, kelembapan, status listrik) ditampilkan secara real-time.

**Prioritas:** Tinggi | **Story Point:** 8

---

### US-03: Memesan Kamar
**Sebagai** penyewa,
**saya ingin** memesan kamar secara online,
**agar** proses penyewaan lebih cepat dan mudah.

**Kriteria Penerimaan:**
- Penyewa dapat memilih tanggal mulai dan durasi sewa.
- Sistem menampilkan total biaya sebelum konfirmasi.
- Status kamar berubah menjadi "dipesan" setelah pemesanan berhasil.

**Prioritas:** Tinggi | **Story Point:** 5

---

### US-04: Registrasi dan Login
**Sebagai** pengguna,
**saya ingin** mendaftar dan masuk ke akun saya,
**agar** data dan transaksi saya aman.

**Kriteria Penerimaan:**
- Pengguna dapat mendaftar dengan email dan kata sandi.
- Pengguna dapat login dan logout.
- Hak akses dibedakan antara penyewa dan admin.

**Prioritas:** Tinggi | **Story Point:** 3

---

### US-05: Melakukan Pembayaran
**Sebagai** penyewa,
**saya ingin** membayar sewa secara online,
**agar** saya tidak perlu membayar secara tunai.

**Kriteria Penerimaan:**
- Tersedia minimal satu metode pembayaran.
- Bukti pembayaran dapat dilihat dan diunduh.
- Status pembayaran diperbarui otomatis.

**Prioritas:** Sedang | **Story Point:** 5

---

### US-06: Mengelola Data Kamar
**Sebagai** pemilik/admin,
**saya ingin** menambah, mengubah, dan menghapus data kamar,
**agar** informasi kamar selalu akurat.

**Kriteria Penerimaan:**
- Admin dapat melakukan operasi CRUD data kamar.
- Perubahan langsung tampil di halaman penyewa.

**Prioritas:** Tinggi | **Story Point:** 5

---

### US-07: Memantau Seluruh Kamar
**Sebagai** pemilik/admin,
**saya ingin** memantau kondisi semua kamar dalam satu dashboard,
**agar** saya dapat mengambil tindakan cepat jika ada masalah.

**Kriteria Penerimaan:**
- Dashboard menampilkan status semua kamar.
- Kamar bermasalah ditandai dengan indikator khusus.

**Prioritas:** Sedang | **Story Point:** 8

---

### US-08: Menerima Notifikasi
**Sebagai** pemilik/admin,
**saya ingin** menerima notifikasi saat terjadi anomali (misalnya suhu tidak normal atau listrik padam),
**agar** masalah dapat segera ditangani.

**Kriteria Penerimaan:**
- Notifikasi terkirim saat nilai sensor melewati ambang batas.
- Riwayat notifikasi dapat dilihat.

**Prioritas:** Sedang | **Story Point:** 5

---

### US-09: Mengajukan Laporan Kerusakan
**Sebagai** penyewa,
**saya ingin** melaporkan kerusakan fasilitas kamar,
**agar** masalah segera diperbaiki.

**Kriteria Penerimaan:**
- Penyewa dapat mengirim laporan dengan deskripsi dan foto.
- Penyewa dapat melihat status penanganan laporan.

**Prioritas:** Rendah | **Story Point:** 3

---

### US-10: Melihat Laporan dan Riwayat Transaksi
**Sebagai** pemilik/admin,
**saya ingin** melihat laporan pemesanan dan pembayaran,
**agar** saya dapat mengevaluasi pendapatan dan okupansi.

**Kriteria Penerimaan:**
- Laporan dapat difilter berdasarkan periode.
- Laporan dapat diekspor (PDF/Excel).

**Prioritas:** Rendah | **Story Point:** 5

---

## Ringkasan Prioritas

| ID | User Story | Aktor | Prioritas | SP |
|----|-----------|-------|-----------|----|
| US-01 | Melihat daftar kamar | Penyewa | Tinggi | 3 |
| US-02 | Melihat digital twin kamar | Penyewa | Tinggi | 8 |
| US-03 | Memesan kamar | Penyewa | Tinggi | 5 |
| US-04 | Registrasi dan login | Semua | Tinggi | 3 |
| US-05 | Pembayaran online | Penyewa | Sedang | 5 |
| US-06 | Mengelola data kamar | Admin | Tinggi | 5 |
| US-07 | Memantau seluruh kamar | Admin | Sedang | 8 |
| US-08 | Notifikasi anomali | Admin | Sedang | 5 |
| US-09 | Laporan kerusakan | Penyewa | Rendah | 3 |
| US-10 | Laporan dan riwayat transaksi | Admin | Rendah | 5 |
