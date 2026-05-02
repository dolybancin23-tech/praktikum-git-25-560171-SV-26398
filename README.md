# Tugas Praktikum Git & GitHub - Reservasi Klinik Gigi

Repository ini berisi kode sumber untuk bagian "reservasi website Klinik". Proyek ini dikerjakn untuk memenuhi dokumentasi dan simulasi alur kerja Git dan GitHub.

## Identitas Mahasiswa
- **Nama:** Doly Immanuel
- **NIM:** 25/560171/SV/26398
- **Program Studi:** Teknologi Rekayasa Perangkat Lunak (TRPL)
- **Instansi:** Universitas Gadjah Mada

---

## Alur Kerja Praktikum


1. **Inisialisasi & Version Control Dasar (Tugas 1)**
   - Menginisialisasi repository secara lokal menggunakan `git clone`.
   - Membangun struktur HTML dasar dan *styling* CSS secara bertahap.
   - Mencatat setiap perubahan menggunakan 5 riwayat *commit* berstandar *Conventional Commits* (seperti `feat:`, `style:`, `chore:`).
   - Mengimplementasikan file `.gitignore` untuk mencegah file *log* sementara (`error.log`) terunggah ke server.

2. **Branching & Pull Request (Tugas 2)**
   - Menerapkan konsep isolasi fitur dengan membuat percabangan (*branching*) terpisah untuk pengembangan: `feature/navbar`, `feature/footer`, dan `hotfix/typo`.
   - Menggabungkan kode ke *branch* utama (`main`) menggunakan metode *Pull Request* (PR) di GitHub dengan strategi *Squash and merge* dan *Merge commit*.
   - Mengamankan *branch* utama dengan mengaktifkan **Branch Protection Rule** (*Require a pull request before merging*).

3. **Resolusi Konflik & Interactive Rebase (Tugas 3)**
   - **Simulasi Konflik:** Membuat dua *branch* eksperimen (`experiment/bg-green` dan `experiment/bg-blue`) yang mengubah baris kode CSS yang sama. Resolusi konflik diselesaikan secara manual saat proses *merge* di GitHub.
   - **Interactive Rebase:** Menggunakan perintah `git rebase -i HEAD~3` pada *branch* `feature/rebase-test` untuk merapikan riwayat dengan melebur (*squash*) 3 *commit* sementara menjadi 1 *commit* yang bersih.

4. **Kolaborasi & Manajemen Proyek (Tugas 4)**
   - Mendokumentasikan rencana pengembangan melalui pembuatan 3 tiket di tab **Issues** GitHub.
   - Menambahkan rekan pengembang (`dinarnoe`) ke dalam proyek sebagai **Collaborator**.
   - Melakukan perilisan versi perdana aplikasi menggunakan fitur **Releases & Tags** dengan versi `v1.0.0`.
   - Menyusun dokumentasi komprehensif pada file `README.md`.

---

## 📸 Bukti Pengerjaan Praktikum

### 1. Bukti Riwayat Commit & Branching (Tugas 1 & 3)
> **Catatan:** Gambar di bawah ini adalah tangkapan layar dari hasil perintah `git log --oneline --graph --all` yang menunjukkan riwayat 5 commit awal, pembuatan branch fitur, serta riwayat *merge* dan *rebase*.

*(TEMPAT GAMBAR 1)*

### 2. Bukti Branch Protection Rule (Tugas 2)
> **Catatan:** Gambar di bawah ini membuktikan bahwa branch `main` telah dilindungi dengan aturan *Require a pull request before merging*, sehingga tidak bisa di-push secara langsung tanpa proses *review*.

*(TEMPAT GAMBAR 2)*

---

## 📝 Dokumentasi Perintah Git yang Digunakan

Berikut adalah daftar perintah Git yang telah dipraktikkan secara langsung dari terminal selama pengerjaan proyek ini:

| Perintah Git | Deskripsi / Fungsi dalam Praktikum |
| :--- | :--- |
| `git clone [url]` | Mengunduh (*clone*) repository dari GitHub ke penyimpanan lokal. |
| `git add [file]` | Menambahkan file yang diubah ke dalam *staging area* untuk persiapan commit. |
| `git commit -m "pesan"` | Menyimpan perubahan ke dalam riwayat lokal Git dengan pesan berstandar. |
| `git push origin [branch]`| Mengunggah commit yang sudah dibuat di *local storage* menuju server GitHub. |
| `git pull origin main` | Menarik pembaruan (*update*) terakhir dari branch main di GitHub. |
| `git checkout -b [nama]` | Membuat cabang (*branch*) baru dan langsung berpindah ke cabang tersebut. |
| `git checkout [nama]` | Berpindah dari satu *branch* ke *branch* lainnya. |
| `git merge` | Menggabungkan *branch* untuk mendemonstrasikan proses resolusi konflik. |
| `git rebase -i HEAD~3` | Memanipulasi riwayat commit secara interaktif (fitur *Squash*). |

---
*Dokumentasi ini dibuat untuk memenuhi penugasan praktikum.*