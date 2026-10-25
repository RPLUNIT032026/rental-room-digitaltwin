# Project Initiation Document
## Digital Twin Kamar Kos (rental-room-digitaltwin)

- Tim: [Hajid,Bagus,Rafly]
- Tanggal Inisiasi: 7 September 2026
- Versi: 1.0

## 1. Latar Belakang
Pengelolaan kamar kos masih manual: data penyewa, kontrak, dan pembayaran dicatat di buku atau pesan singkat, sementara kondisi kamar (suhu, listrik, pintu) tidak terpantau. Digital twin membuat replika digital tiap kamar yang tersinkron dengan sensor IoT secara real-time, sehingga hunian, kontrak, dan pembayaran bisa dikelola dari satu sistem.

## 2. Tujuan
1. Memantau kondisi kamar secara real-time (suhu, daya listrik, status pintu).
2. Mendigitalkan data penyewa, kamar, kontrak, dan pembayaran.
3. Menyediakan laporan hunian, pembayaran, dan konsumsi listrik untuk pemilik kos.
4. Memberi penyewa akses ke status kamar, tagihan, dan kontrol pintu.

## 3. Ruang Lingkup
Dalam lingkup:
- Manajemen penyewa, kamar, kontrak, pembayaran
- Digital twin dengan sinkronisasi data sensor
- Sensor suhu, listrik, dan pintu
- Dashboard pemilik kos dan aplikasi penyewa
- Notifikasi anomali dan tagihan
- Integrasi layanan pembayaran

Di luar lingkup:
- Pengadaan sensor secara massal
- Integrasi platform pemesanan pihak ketiga
- Sistem akuntansi dan pajak lengkap

## 4. Deliverable
- Dokumen perancangan (use case, activity, class, object, context, deployment)
- Aplikasi web pemilik kos
- Aplikasi penyewa
- Modul digital twin
- Basis data
- Dokumen pengujian

## 5. Pemangku Kepentingan
- Pemilik Kos: sponsor dan pengguna utama
- Penyewa: pengguna
- Tim Pengembang: pelaksana
- Dosen/Pembimbing: peninjau
- Layanan Pembayaran: pihak eksternal

## 6. Estimasi
Ukuran sistem 118,8 FP (UFP 111 x VAF 1,07). Dengan produktivitas 10 jam/FP, usaha sekitar 1.188 jam kerja.

## 7. Milestone
- Sprint 1: Inisiasi dan analisis kebutuhan
- Sprint 2: Perancangan sistem (UML, DFD, FP)
- Sprint 3: Implementasi inti (basis data, penyewa, kamar)
- Sprint 4: Integrasi sensor dan digital twin
- Sprint 5: Pengujian dan perbaikan


## 8. Risiko dan Mitigasi
- Sensor tidak tersedia atau tidak stabil: gunakan simulator data sensor
- Koneksi internet tidak stabil: buffering dan sinkronisasi ulang
- Kebutuhan berubah: tinjau backlog tiap sprint
- Waktu dan tim terbatas: prioritaskan fitur inti
- Keamanan data dan kontrol pintu: autentikasi, otorisasi per peran, enkripsi

## 9. Kriteria Keberhasilan
- Data sensor tampil di dashboard dengan jeda beberapa detik
- Semua fungsi inti lolos pengujian
- Pemilik kos dapat melihat laporan hunian, pembayaran, dan listrik
- Penyewa dapat melihat status kamar, tagihan, dan mengontrol pintu

## 10. Persetujuan
| Nama | Peran | Tanda Tangan | Tanggal |
|---|---|---|---|
| [isi nama] | Project Manager | | |
| [isi nama] | Pemilik Kos | | |
| [isi nama] | Dosen/Pembimbing | | |
