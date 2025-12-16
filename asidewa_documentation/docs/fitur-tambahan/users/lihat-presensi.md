# 📊 Riwayat Absensi Bulanan

Fitur ini memungkinkan Anda untuk meninjau secara rinci seluruh catatan kehadiran Anda selama periode satu bulan penuh. Halaman ini sangat berguna untuk memverifikasi absensi Anda, memastikan tidak ada data yang terlewat, dan melihat status cuti atau izin.

## 1. Cara Mengakses Halaman

1.  Buka aplikasi **ASI DEWA**.
2.  Setelah *login*, navigasikan ke **Menu Utama** (tombol garis tiga di bagian kiri atas layar).
3.  Pilih opsi **"Riwayat Presensi"**.
4.  Secara *default*, halaman akan menampilkan riwayat untuk bulan saat ini.

## 2. Membaca Tabel Riwayat Absensi

Tabel riwayat ini menampilkan data kehadiran Anda berdasarkan tanggal, dimulai dari tanggal terbaru.

> ![history absence](../../assets/riwayat-absensi.jpg)

Tabel terdiri dari kolom-kolom berikut:

| Nama Kolom | Keterangan |
| :--- | :--- |
| **Tanggal** | Tanggal spesifik terjadinya absensi atau status non-kerja. |
| **Hari** | Nama hari dalam seminggu. |
| **Jam Masuk** | Waktu yang tercatat saat Anda menekan tombol Absen Masuk. |
| **Status Masuk** | Menunjukkan hasil verifikasi absensi masuk Anda. |
| **Jam Pulang** | Waktu yang tercatat saat Anda menekan tombol Absen Pulang. |
| **Status Pulang** | Menunjukkan hasil verifikasi absensi pulang Anda. |

---

## 3. Penjelasan Status Absensi

Kolom **Status Masuk** dan **Status Pulang** memberikan informasi cepat tentang jenis kehadiran atau ketidakhadiran Anda pada hari tersebut:

| Status | Makna | Tindakan Lanjut |
| :--- | :--- | :--- |
| **Tepat Waktu** | Absensi berhasil dilakukan, sesuai dengan jam *shift* dan dalam batas toleransi lokasi yang ditentukan. | Data kehadiran valid. |
| **Terlambat** | Absensi Masuk dilakukan melewati batas waktu toleransi yang ditetapkan perusahaan. | Dapat memerlukan pengajuan Koreksi Absensi jika ada alasan mendesak. |
| **Pulang Cepat** | Absensi Pulang dilakukan lebih awal dari jadwal yang ditetapkan pada *shift* Anda pada hari tersebut. | Dapat memerlukan pengajuan Koreksi Absensi jika ada alasan mendesak. |
| **Cuti** | Hari tersebut adalah Hari Cuti yang telah diajukan dan disetujui. Jam Masuk dan Pulang akan tercatat **00:00**. | Data kehadiran valid sebagai Cuti. |
| **Libur** | Hari tersebut adalah Hari Libur yang telah diatur oleh penanggung jawab divisi Anda. Jam Masuk dan Pulang akan tercatat **00:00** | Data kehadiran valid sebagai Libur. |

<!-- ## 4. Cara Melihat Bulan Lain

Untuk melihat riwayat absensi bulan sebelumnya:

1.  Cari *dropdown* menu atau tombol navigasi bulan (biasanya berada di bagian atas tabel, bertuliskan **"Bulan Desember 2025"**).
2.  Pilih bulan yang Anda inginkan (misalnya, **"November 2025"**).
3.  Tabel akan otomatis memuat dan menampilkan riwayat absensi untuk bulan yang dipilih. -->

---

### ❓ Data Tidak Akurat

!!! danger "Tindakan Cepat"
    Jika Anda menemukan ketidaksesuaian data (misalnya Anda sudah absen tetapi tercatat **"Tidak Hadir"**), silakan hubungi Penanggung Jawab Divisi Anda, untuk melakukan konfirmasi kepada **HRD** dan **administrator** (IT)

➡️ Lanjutkan ke panduan: [Pengajuan Cuti](../users/pengajuan-cuti.md)