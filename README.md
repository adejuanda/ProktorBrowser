```markdown
# ProktorBrowser for Linux Mint & Ubuntu (.deb)

Porting native aplikasi resmi ProktorBrowser (Pusmenjar / Kemendikbudristek) untuk sistem operasi Linux (Linux Mint, Ubuntu, Debian, dan turunannya).

Berjalan 100% native tanpa Wine, tanpa VirtualBox, ringan, hemat RAM, dan sudah dilengkapi icon resmi di Menu Aplikasi.

---

## 1. Unduh Aplikasi

Unduh file instalasi paket Debian (.deb) versi terbaru di menu [Releases](../../releases):

👉 [Download proktorbrowser_22.7.31_amd64.deb](../../releases)

---

## 2. Cara Instalasi

Pilih salah satu cara di bawah ini:

### Opsi A: Lewat Klik Mouse / GUI (Paling Mudah)
1. Buka folder Downloads tempat file .deb tadi diunduh.
2. Klik dua kali pada file `proktorbrowser_22.7.31_amd64.deb` (atau klik kanan > pilih Buka dengan Pemasang Paket / GDebi).
3. Klik tombol Pasang Paket (Install Package).
4. Masukkan password Linux Anda, lalu tunggu beberapa detik hingga instalasi selesai.

---

### Opsi B: Lewat Terminal
Buka terminal (Ctrl + Alt + T), lalu jalankan:

```bash
cd ~/Downloads
sudo dpkg -i proktorbrowser_22.7.31_amd64.deb
sudo apt-get install -f
```

---

## 3. Cara Menjalankan

- Buka Menu Aplikasi (Start Menu) di Linux Mint / Ubuntu Anda.
- Cari: ProktorBrowser (sudah dilengkapi logo resmi).
- Atau jalankan langsung dari terminal:
  ```bash
  proktorbrowser
  ```

Setelah aplikasi terbuka, seluruh status hardware (OS, CPU, RAM) dan Internet Connection akan tercentang hijau otomatis. Klik tombol RUN untuk masuk ke halaman login CBT Proktor.

---

## 4. Tips Penggunaan Penting

1. Cara Keluar dari Layar Penuh (Kiosk Mode):
   Karena aplikasi berjalan dalam mode ujian layar penuh terkunci (kiosk), gunakan kombinasi tombol keyboard:
   `Alt + F4 atau Alt + Tab`

2. Tombol Sign-In Tidak Bisa Diklik / Terkunci:
   - Pastikan ID Proktor dan Password diketik dengan benar.
   - Setelah mengetik ID Proktor, klik di luar kolom atau tekan tombol Tab.
   - Perhatikan tulisan "Tenant : ..." di atas tombol. Tombol Sign-In hanya akan aktif jika server Pusmendik mendeteksi jadwal ujian aktif untuk ID Proktor tersebut.

---

## 5. Cara Menghapus (Uninstall)

Jika kegiatan asesmen/ujian telah selesai dan Anda ingin mencopot aplikasi:

```bash
sudo apt remove --purge proktorbrowser
```

---

## 6. Disclaimer
Repositori ini ditujukan semata-mata untuk mempermudah proktor dan teknisi sekolah pengguna sistem operasi Linux dalam menjalankan tugas asesmen pendidikan tanpa mengubah logika keamanan, backend, enkripsi, maupun server resmi Kemendikbudristek.
```
