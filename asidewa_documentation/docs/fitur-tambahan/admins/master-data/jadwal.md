# ⏰ Master Jadwal

Halaman **Master Jadwal** digunakan oleh Administrator untuk mendefinisikan dan mengelola semua kode *shift* (jadwal kerja) dan status non-kerja (Cuti, Libur) yang berlaku di perusahaan, beserta jam masuk dan jam keluar yang spesifik.

## 1. Cara Mengakses Halaman

1.  *Login* menggunakan akun **Administrator**.
2.  Akses **Master Data**.
3.  Pilih opsi **"Master Jadwal"**.

![master jadwal](../../../assets/mapping-jadwal.jpg)

## 2. Tabel Daftar Jadwal

Tabel utama menampilkan daftar seluruh *shift* dan status non-kerja yang terdaftar:

| Kolom | Keterangan Data |
| :--- | :--- |
| **No** | Nomor urut daftar. |
| **ID Jadwal** | Kode unik untuk jadwal (*shift*), digunakan dalam [Mapping Jadwal Karyawan](../../divisions/mapping-jadwal.md) (Contoh: **M001**, **P001**, **S001**). |
| **Nama Jadwal** | Nama deskriptif untuk *shift* atau status (Contoh: **Malam**, **Pagi**, **Siang**). |
| **Jam Masuk** | Waktu mulai kerja yang ditetapkan (Contoh: **07:30:00** untuk Pagi). |
| **Jam Keluar** | Waktu selesai kerja yang ditetapkan (Contoh: **14:30:00** untuk Pagi). |
| **Aksi** | Tombol untuk mengelola data jadwal. |

### Contoh Kode Non-Kerja:
* **CUTI:** Jam Masuk **00:00:00** dan Jam Keluar **00:00:00**.
* **LIBUR:** Jam Masuk **00:00:00** dan Jam Keluar **00:00:00**.

## 3. Menambahkan Jadwal Baru

Untuk mendaftarkan *shift* atau kode non-kerja baru:

1.  Klik tombol **"+ Tambah Jadwal"** (biru) di pojok kiri atas halaman.
    ![tambah-jadwal](../../../assets/tambah-jadwal.jpg)
2.  Isi formulir yang muncul:
    * **ID Jadwal:** Masukkan kode unik (Contoh: **SPL** untuk *Split Shift*).
    * **Nama Jadwal:** Masukkan nama deskriptif (Contoh: **Split Shift**).
    * **Jam Masuk:** Tentukan waktu mulai *shift* (Contoh: **09:00:00**).
    * **Jam Keluar:** Tentukan waktu selesai *shift* (Contoh: **18:00:00**).
3.  Klik **"Submit"** untuk menambahkan jadwal ke dalam sistem.

## 4. Mengelola Data Jadwal (Aksi)

Kolom **Aksi** pada tabel memungkinkan Anda untuk memelihara data jadwal:

| Tombol | Tindakan (Aksi) | Kegunaan |
| :---: | :--- | :--- |
| :material-pencil: | **Edit** (Kuning) | Mengubah **Nama Jadwal**, **Jam Masuk**, atau **Jam Keluar**. Setelah diedit, klik **"Submit"** untuk memperbarui. |
| :material-trash-can: | **Hapus** (Merah) | Menghapus data jadwal secara permanen dari sistem. |

!!! danger "Dampak Perubahan"
    Perubahan atau penghapusan jadwal (terutama Jam Masuk/Keluar) akan **mempengaruhi perhitungan status absensi karyawan** di masa depan dan dapat mengganggu data *mapping* jadwal yang sudah ada. Lakukan perubahan dengan hati-hati.

---

### ❓ Keterkaitan Data

* **Mapping Jadwal:** Kode **ID Jadwal** yang Anda definisikan di sini adalah yang digunakan oleh Penanggung Jawab Divisi saat [Mapping Jadwal Karyawan](../../divisions/mapping-jadwal.md).
* **Perhitungan Absensi:** Jam Masuk dan Jam Keluar yang ditetapkan di sini menjadi patokan sistem untuk menentukan status absensi karyawan, seperti **Tepat Waktu** atau **Terlambat**.

➡️ Lanjutkan ke panduan Admin berikutnya: [Master Jenis Cuti](../master-data/cuti.md)