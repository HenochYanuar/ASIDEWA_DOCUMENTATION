# 🌐 Dokumentasi API (Endpoint) ASI DEWA

Dokumen ini mencantumkan semua *endpoint* yang tersedia dalam sistem, diklasifikasikan berdasarkan fungsionalitas pengguna (*users*) dan administrasi (*admins*).

## 1. ⚙️ Endpoint Administrasi (CMS)

Semua *endpoint* Administrasi diawali dengan URL dasar: `http://[BASE_URL]/admins/`.

### A. Akses Dasar dan Laporan Absensi

| URL Path | Nama Fungsi | Deskripsi |
| :--- | :--- | :--- |
| **`/admins/login/`** | `login` | Halaman *Login* untuk Administrator/HRD. |
| **`/admins/logout/`** | `logout` | Logout dari sesi Administrator. |
| **`/admins/dashboard/`** | `dashboard` | Halaman utama/Ringkasan data untuk Administrator. |
| **`/admins/absen/`** | `index_absen` | Halaman utama untuk melihat data presensi (memilih divisi). |
| **`/admins/absen/<str:divisi_id>`** | `absen` | Menampilkan laporan absensi karyawan berdasarkan ID Divisi yang dipilih. |
| **`/admins/err403/`** | `err403` | Halaman *Error* 403 (Forbidden/Tidak memiliki akses). |
| **`/admins/err404/`** | `err404` | Halaman *Error* 404 (Not Found). |

### B. Master Data

| URL Path | Nama Fungsi | Deskripsi |
| :--- | :--- | :--- |
| **`/admins/divisi/`** | `divisi_master` | Halaman utama Master Data Divisi. |
| **`/admins/divisi/add/`** | `addDivisi` | Menambah data Divisi baru. |
| **`/admins/divisi/edit/<str:id>`** | `editDivisi` | Mengubah data Divisi berdasarkan ID. |
| **`/admins/divisi/delete/<str:id>`** | `deleteDivisi` | Menghapus data Divisi berdasarkan ID. |
| **`/admins/jadwal/`** | `jadwal_master` | Halaman utama Master Data Jadwal (*Shift*). |
| **`/admins/jadwal/add/`** | `addJadwal` | Menambah data Jadwal (*Shift*) baru. |
| **`/admins/jadwal/edit/<str:id>`** | `editJadwal` | Mengubah data Jadwal berdasarkan ID. |
| **`/admins/jadwal/delete/<str:id>`** | `deleteJadwal` | Menghapus data Jadwal berdasarkan ID. |
| **`/admins/cuti/`** | `cuti_master` | Halaman utama Master Data Jenis Cuti dan Jatah. |
| **`/admins/cuti/add/`** | `addCuti` | Menambah jenis Cuti baru. |
| **`/admins/cuti/edit/<str:id>`** | `editCuti` | Mengubah data jenis Cuti berdasarkan ID. |
| **`/admins/cuti/delete/<str:id>`** | `deleteCuti` | Menghapus data jenis Cuti berdasarkan ID. |

### C. Manajemen Karyawan

| URL Path | Nama Fungsi | Deskripsi |
| :--- | :--- | :--- |
| **`/admins/addUser/`** | `addUser` | Endpoint untuk menambah pengguna (karyawan) baru secara cepat. |
| **`/admins/karyawan/`** | `karyawan` | Halaman daftar seluruh Karyawan (Admin). |
| **`/admins/karyawan/<str:nik>`** | `detail_karyawan` | Melihat detail profil dan data karyawan tertentu berdasarkan NIK. |
| **`/admins/karyawan/edit/<str:nik>`** | `editKaryawan` | Mengubah data Karyawan berdasarkan NIK. |
| **`/admins/karyawan/delete/<str:nik>`** | `deleteKaryawan` | Menghapus data Karyawan berdasarkan NIK. |

### D. Mapping Jadwal dan Persetujuan Cuti

| URL Path | Nama Fungsi | Deskripsi |
| :--- | :--- | :--- |
| **`/admins/mapping_jadwal/`** | `mapping_jadwal` | Halaman utama untuk *mapping* jadwal per divisi. |
| **`/admins/mapping_jadwal/add/`** | `buat_jadwal` | Endpoint untuk membuat jadwal *mapping* baru (misalnya, untuk bulan baru). |
| **`/admins/mapping_jadwal/save/`** | `save_jadwal` | Endpoint untuk menyimpan jadwal *mapping* yang baru dibuat. |
| **`/admins/mapping_jadwal/edit/<str:divisi_id>/<int:tahun>/<str:bulan>`** | `edit_jadwal` | Mengubah *mapping* jadwal untuk Divisi, Tahun, dan Bulan tertentu. |
| **`/admins/mapping_jadwal/update/`** | `update_jadwal` | Endpoint untuk memperbarui dan menyimpan jadwal *mapping* yang telah diedit. |
| **`/admins/persetujuan_cuti/`** | `persetujuan_cuti` | Halaman daftar antrian pengajuan cuti yang perlu di-*approve* atau di-*reject*. |
| **`/admins/persetujuan_cuti/<int:id>`** | `detail_pengajuan` | Melihat detail pengajuan cuti tertentu berdasarkan ID. |

---

## 2. 👤 Endpoint Pengguna (User)

Semua *endpoint* Pengguna (Karyawan) diawali dengan URL dasar: `http://[BASE_URL]/users/`.

### A. Absensi dan Data Pribadi

| URL Path | Nama Fungsi | Deskripsi |
| :--- | :--- | :--- |
| **`/users/absensi/`** | `absence` | Endpoint utama untuk melakukan Absen Masuk atau Absen Pulang. |
| **`/users/jadwal/`** | `jadwal` | Melihat jadwal *shift* karyawan yang sedang *login* untuk satu periode. |
| **`/users/presensi/`** | `presensi` | Melihat riwayat absensi bulanan karyawan yang sedang *login*. |
| **`/users/profil/<str:nik>`** | `profile` | Melihat atau mengakses halaman profil karyawan berdasarkan NIK. |

### B. Pengajuan Cuti Karyawan

| URL Path | Nama Fungsi | Deskripsi |
| :--- | :--- | :--- |
| **`/users/pengajuan_cuti/`** | `pengajuan_cuti` | Halaman untuk membuat dan melihat daftar pengajuan cuti pribadi. |
| **`/users/pengajuan_cuti/edit/<int:id>`** | `edit_pengajuan_cuti` | Mengubah detail pengajuan cuti yang telah dibuat (berdasarkan ID). |
| **`/users/pengajuan_cuti/delete/<int:id>`** | `delete_pengajuan_cuti` | Menghapus/membatalkan pengajuan cuti yang masih *pending* (berdasarkan ID). |