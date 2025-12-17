# ⏳ Master Cuti 

Halaman **Master Cuti** digunakan oleh Administrator atau HRD untuk mengelola jenis-cuti yang tersedia bagi karyawan, termasuk penetapan jatah hari yang diizinkan untuk setiap cuti. Data di halaman ini akan muncul sebagai opsi saat karyawan membuat [Pengajuan Cuti](../../../fitur-tambahan/users/pengajuan-cuti.md).

## 1. Cara Mengakses Halaman

1.  *Login* menggunakan akun **Administrator** atau **HRD**.
2.  Akses **Master Data**.
3.  Pilih opsi **"Master Cuti"**.

![master cuti](../../../assets/master-cuti.jpg)

## 2. Tabel Daftar Cuti

Tabel utama menampilkan daftar cuti yang telah terdaftar dalam sistem:

| Kolom | Keterangan Data |
| :--- | :--- |
| **No** | Nomor urut daftar. |
| **Cuti** | Nama cuti yang diakui (Contoh: **Cuti Tahunan**, **Cuti Menikah**). |
| **Jatah** | Jumlah kuota hari yang diberikan untuk cuti ini per periode (Contoh: **12** untuk Cuti Tahunan). |
| **Hari** | Kolom penanda durasi cuti (digunakan untuk menandakan cuti yang durasinya tetap, misalnya: Cuti Menikah 3 Hari). |
| **Aksi** | Tombol untuk mengelola data cuti. |

## 3. Menambahkan Cuti Baru

Untuk mendaftarkan cuti baru:

1.  Klik tombol **"+ Tambah Cuti"** (biru) di pojok kiri atas halaman.
    ![tambah cuti](../../../assets/tambah-cuti.jpg)
2.  Isi formulir yang muncul:
    * **Cuti:** Masukkan nama yang jelas.
    * **Jatah:** Masukkan jumlah hari kuota (Contoh: **3**). Jika tidak ada kuota (misalnya Cuti Menikah yang ditentukan per kejadian), masukkan **0**.
    * **Hari:** (Opsional) Tentukan durasi spesifik jika cuti tersebut memiliki durasi tetap, jika tidak masukkan **0**.
3.  Klik **"Submit"** untuk menambahkan cuti ke dalam sistem.

## 4. Mengelola Data Cuti (Aksi)

Kolom **Aksi** pada tabel memungkinkan Anda untuk memelihara data cuti:

| Tombol | Tindakan (Aksi) | Kegunaan |
| :---: | :--- | :--- |
| :material-pencil: | **Edit** (Kuning) | Mengubah **Cuti** atau **Jatah** hari. Setelah diedit, klik **"Submit"** untuk memperbarui. |
| :material-trash-can: | **Hapus** (Merah) | Menghapus cuti secara permanen dari sistem. |

!!! danger "Dampak Perubahan Jatah"
    Mengubah atau menghapus **Jatah Cuti Tahunan** dapat memengaruhi perhitungan sisa cuti yang telah digunakan oleh karyawan. Lakukan perubahan ini dengan koordinasi yang ketat dengan tim HRD.

---

### ❓ Keterkaitan Data

!!! note "Keterkaitan"
    * **Pengajuan Karyawan:** Nama-nama cuti yang terdaftar di sini adalah opsi yang dapat dipilih oleh karyawan saat mereka mengisi formulir [Pengajuan Cuti](../../users/pengajuan-cuti.md).
    * **Penghitungan Sisa Cuti:** Sistem menggunakan nilai **Jatah** yang Anda tentukan di sini sebagai batas atas kuota cuti tahunan karyawan.