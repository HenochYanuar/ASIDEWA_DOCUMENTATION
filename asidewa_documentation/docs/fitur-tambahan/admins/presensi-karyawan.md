# 📈 Laporan Presensi Karyawan per Divisi

Fitur ini memungkinkan Administrator/HRD melihat riwayat absensi terperinci untuk seluruh karyawan, difilter berdasarkan divisi dan periode waktu (bulan/tahun).

## 1. Langkah 1: Memilih Divisi


Halaman awal menampilkan opsi untuk memilih Divisi mana yang laporannya ingin Anda tinjau.

1.  Akses **Menu Administrator**.
2.  Pilih opsi **"Data Presensi"**.
3.  Anda akan melihat tombol-tombol yang mewakili setiap divisi perusahaan .
4.  Klik pada tombol **Divisi** yang laporannya ingin Anda akses.

![pilih divisi](../../assets/data-presensi-divisi.jpg)

## 2. Langkah 2: Memfilter Periode Waktu

Setelah memilih divisi (misalnya, **Absen Divisi IT dan SIMRS**), Anda akan melihat tampilan yang memungkinkan Anda memfilter data berdasarkan Bulan dan Tahun:

1.  Gunakan *dropdown* **Bulan** dan **Tahun** untuk memilih periode yang ingin Anda tinjau.
2.  Klik tombol **"Filter"** untuk memuat data absensi.
3.  Secara *default*, sistem akan menampilkan data 6 bulan terakhir untuk masing-masing divisi.

![daftar presensi](../../assets/daftar-presensi.jpg)

## 3. Langkah 3: Membaca Tabel Presensi Detail

Tabel ini memberikan data kehadiran *real-time* dan status validasi absensi:

| Kolom | Keterangan Data |
| :--- | :--- |
| **NIK & Nama** | Identitas karyawan yang tercatat presensinya. |
| **Shift** | Jenis *shift* yang seharusnya dikerjakan karyawan pada tanggal tersebut (Contoh: **Siang** atau **Pagi**). |
| **Tanggal Masuk** | Tanggal dan jam absensi masuk yang tercatat. |
| **Status Masuk** | Status validasi absensi masuk (Contoh: **Cuti**, **Tepat Waktu**, **Terlambat**). |
| **Tanggal Keluar** | Tanggal dan jam absensi pulang yang tercatat. |
| **Status Keluar** | Status validasi absensi pulang (Contoh: **Tepat Waktu**, **Pulang Cepat**). |
| **Keterangan** | Detail status keterlambatan (Contoh: **Terlambat**, **Tidak Terlambat**). |
| **Total Durasi** | Total waktu kerja yang dihitung pada hari tersebut. |

### Contoh Status Khusus:

* **Status Cuti/Libur:** Jika status tercatat **Cuti** atau **Libur**, kolom **Jam Masuk** dan **Jam Pulang** akan tercatat **00:00:00** dan **Total Durasi** akan menjadi **0 menit**.
* **Pulang Cepat:** Karyawan tercatat melakukan absensi pulang sebelum durasi *shift* yang ditentukan selesai.

## 4. Export Data (Cetak Total)

Anda dapat mengekspor data laporan presensi ini untuk keperluan administrasi dan penggajian:

1.  Klik tombol **"Cetak"** (merah) yang berada di sudut kanan atas tabel.
2.  Sistem akan memproses dan mengunduh data laporan sesuai dengan filter bulan dan tahun yang sedang aktif.

---

### ❓ Manajemen Data

!!! note "Perhatian"
    * **Bagaimana cara memperbaiki data absensi yang salah?**
        * Jika ada data yang salah (misalnya, tercatat **Pulang Cepat** padahal karyawan kerja penuh), Anda dapat menghubungi **Administrator (IT)**, meskipun kasus ini akan jarang terjadi kecuali terdapat *human error*.

➡️ Lanjutkan ke panduan Admin berikutnya: [Daftar Karyawan](../admins/persetujuan-cuti.md)