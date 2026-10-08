# ProktorBrowser untuk Linux (.deb)

Paket Debian untuk ProktorBrowser (Pusmenjar, Kemendikbudristek) yang dapat dipasang di Linux Mint, Ubuntu, Debian, dan turunannya. Aplikasi berjalan langsung di Linux tanpa Wine atau mesin virtual.

## Unduh

Ambil file `.deb` terbaru di halaman [Releases](../../releases).

Versi saat ini: **22.7.31** (`proktorbrowser_22.7.31_amd64.deb`, arsitektur amd64)

## Instalasi

### Lewat GUI

1. Buka folder Downloads.
2. Klik dua kali file `.deb`, atau klik kanan lalu pilih **Buka dengan Pemasang Paket** (GDebi).
3. Klik **Pasang Paket**.
4. Masukkan password akun Linux Anda, lalu tunggu sampai selesai.

### Lewat terminal

```bash
cd ~/Downloads
sudo dpkg -i proktorbrowser_22.7.31_amd64.deb
sudo apt-get install -f
```

Perintah kedua memasang dependensi yang belum ada.

## Menjalankan

Cari **ProktorBrowser** di menu aplikasi, atau jalankan dari terminal:

```bash
proktorbrowser
```

Setelah terbuka, status OS, CPU, RAM, dan koneksi internet akan dicek otomatis. Jika semuanya tercentang hijau, klik **RUN** untuk masuk ke halaman login CBT Proktor.

## Tips

### Keluar dari layar penuh

Aplikasi berjalan dalam mode kiosk. Untuk keluar, tekan `Alt + F4` atau pindah jendela dengan `Alt + Tab`.

### Tombol Sign-In tidak bisa diklik

- Periksa kembali ID Proktor dan password.
- Setelah mengisi ID Proktor, tekan `Tab` atau klik di luar kolom.
- Lihat tulisan **Tenant** di atas tombol. Sign-In hanya aktif jika server Pusmendik menemukan jadwal ujian aktif untuk ID Proktor tersebut.

## Menghapus

```bash
sudo apt remove --purge proktorbrowser
```

## Disclaimer

Repositori ini hanya membantu proktor dan teknisi sekolah yang memakai Linux untuk menjalankan asesmen. Tidak ada perubahan pada logika keamanan, backend, enkripsi, maupun server resmi Kemendikbudristek.
