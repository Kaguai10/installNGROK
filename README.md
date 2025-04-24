<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?size=30&color=00FF00&center=true&vCenter=true&width=600&lines=Panduan+Instalasi+Ngrok">
</div>

Ngrok adalah alat yang membuat terowongan aman ke localhost Anda, memungkinkan Anda mengekspos server lokal ke internet. Panduan ini menjelaskan cara menginstal Ngrok di Windows, Linux, dan macOS.

## Prasyarat

Sebelum memulai, pastikan Anda memiliki:
- Koneksi internet
- Terminal / command prompt dengan akses administrator atau root

## Langkah Instalasi

### 1. **Windows**

#### Menggunakan installer:
1. Unduh versi terbaru Ngrok untuk Windows dari [Halaman Unduhan Ngrok](https://ngrok.com/download).
2. Ekstrak file zip yang telah diunduh.
3. Tempatkan file `ngrok.exe` ke folder pilihan Anda (misalnya, `C:\ngrok`).
4. Tambahkan folder yang berisi `ngrok.exe` ke variabel lingkungan PATH sistem:
    - Klik kanan pada "This PC" lalu pilih "Properties".
    - Klik "Advanced system settings", lalu klik "Environment Variables".
    - Di bawah "System variables", cari "Path" lalu klik "Edit".
    - Tambahkan path lengkap ke folder `ngrok.exe`, misalnya `C:\ngrok\`.
5. Buka command prompt baru dan ketik `ngrok version` untuk memastikan instalasi berhasil.

#### Menggunakan Command Prompt:
1. Setelah mengunduh dan mengekstrak Ngrok, Anda juga bisa menjalankannya langsung:

```sh
cd C:\ngrok
ngrok version
```

### 2. **Linux**

#### Menggunakan terminal:
1. Unduh versi terbaru Ngrok untuk Linux dari [Halaman Unduhan Ngrok](https://ngrok.com/download).
2. Ekstrak file yang diunduh:

```bash
tar -zxvf ngrok-stable-linux-amd64.tar.gz
```

3. Pindahkan file `ngrok` ke direktori PATH sistem Anda agar bisa diakses dengan mudah:

```bash
sudo mv ngrok /usr/local/bin
```

4. Periksa versi untuk memastikan instalasi:

```bash
ngrok version
```

### 3. **macOS**

#### Menggunakan Homebrew (Disarankan):
1. Jika Homebrew belum terinstal, jalankan:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2. Instal Ngrok dengan Homebrew:

```bash
brew install ngrok
```

3. Periksa versi Ngrok:

```bash
ngrok version
```

#### Instalasi Manual:
1. Unduh versi terbaru Ngrok untuk macOS dari [Halaman Unduhan Ngrok](https://ngrok.com/download).
2. Ekstrak file:

```bash
tar -zxvf ngrok-stable-darwin-amd64.tar.gz
```

3. Pindahkan file `ngrok` ke PATH:

```bash
sudo mv ngrok /usr/local/bin
```

4. Cek versi:

```bash
ngrok version
```

## Penggunaan

Setelah terinstal, Anda bisa mulai menggunakan Ngrok untuk mengekspos layanan lokal:

```bash
ngrok http <nomor_port>
```

Contoh, jika server lokal Anda berjalan di port 8080:

```bash
ngrok http 8080
```

Ngrok akan memberikan URL publik yang meneruskan trafik ke server lokal Anda.

## Pemecahan Masalah

- Jika Ngrok tidak dikenali sebagai perintah, pastikan direktori tempat file `ngrok` berada sudah ditambahkan ke PATH.
- Jika terjadi masalah koneksi, periksa koneksi internet dan pengaturan firewall Anda.

Untuk informasi lebih lanjut, kunjungi [Dokumentasi Ngrok](https://ngrok.com/docs).
