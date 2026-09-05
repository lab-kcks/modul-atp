## Daftar Isi

- [Persiapan Environment](#persiapan-environment)
  - [Instalasi MinGW](#instalasi-mingw)
  - [Setting PATH Environment Variable](#setting-path-environment-variable)
  - [Instalasi Microsoft Visual Studio Code](#instalasi-microsoft-visual-studio-code)

# Persiapan Environment

Sebelum memulai praktikum, pastikan kalian sudah menyiapkan environment untuk pemrograman bahasa C. Berikut adalah beberapa hal yang perlu diperhatikan:

- Instalasi compiler C (contoh: MinGW untuk Windows)
- Pengaturan PATH environment variable agar compiler dapat diakses dari command line
- Instalasi text editor atau IDE (rekomendasi: Microsoft Visual Studio Code)

Modul ini akan membahas langkah-langkah untuk menyiapkan environment tersebut agar kalian dapat mulai menulis dan menjalankan program C dengan lancar.

## Instalasi MinGW

Buka browser, kemudian buka website [MSYS2](https://www.msys2.org/).

![](assets/20260905_104542_image.png)

Kemudian download untuk **x86_64** pada *link* yang ada pada halaman website.

![](assets/20260905_104628_image.png)

Jika sudah terunduh, buka file **.exe** nya, kemudian lakukan instalasi seperti biasa. Cukup klik **Next** hingga akhir untuk memulai instalasi, dan tunggu hingga selesai.

![](assets/20260905_104752_image.png)

Jika sudah selesai, centang **Run MSYS2 now** dan klik **Finish**.

![](assets/20260905_105138_image.png)

Sebuah jendela **Terminal** akan muncul.

![](assets/20260905_105213_image.png)

Di situ, masukkan perintah seperti ini (cukup *copy-paste*) saja, lalu Enter:

```bash
pacman -S --needed base-devel mingw-w64-ucrt-x86_64-toolchain
```

![](assets/20260905_105427_image.png)

Langsung klik Enter saja, kemudian masukkan **Y**, lalu Enter lagi.

![](assets/20260905_105513_image.png)

Tunggu hingga selesai. Jika sudah, kalian bisa cek apakah berhasil terinstall apa belum, dengan mengetikkan:

```bash
gcc --version
```

![](assets/20260905_113119_image.png)

Jika sudah seperti di atas, maka MinGW dan compiler berhasil terinstall.

## Setting PATH Environment Variable

Buka Start -> cari "environment variable".

![](assets/20260905_140002_image.png)

Kemudian, klik **Environment Variables**.

![](assets/20260905_140048_image.png)

Akan muncul tampilan seperti ini. Klik dua kali pada **Path** yang berada di **System variables**.

![](assets/20260905_140138_image.png)

![](assets/20260905_140157_image.png)

Klik **New**, dan masukkan path berikut pada kolom baru:

```bash
C:\msys64\ucrt64\bin
```

![](assets/20260905_140346_image.png)

Klik OK hingga semua jendela tertutup.

Sekarang compiler sudah bisa diakses oleh Windows. Untuk mengujinya bisa melalui Windows Powershell.

![](assets/20260905_140538_image.png)

Kemudian ketik:

```bash
gcc --version
```

![](assets/20260905_140610_image.png)

## Instalasi Microsoft Visual Studio Code

[WIP]
