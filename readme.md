# Apa itu fastfetch?

Singkatnya, Fastfetch adalah cli untuk menampilkan spek dan informasi sistem device di terminal. Untuk lebih detailnya dan konfigurasi2nya bisa dilihat di repo officialnya fastfetch - [GitHub/fastfetch](https://github.com/fastfetch-cli/fastfetch)

## 💻 Instalasi

## Requirements

- Terminal Windows (powershell) buat jalanin cmd dan fastfetch (download di [sini](https://apps.microsoft.com/detail/9n0dx20hk701?hl=en-US&gl=ID))
  > Terminal OS lain macem MacOS dan Linux mungkin juga bisa cuma ini aku buatnya di Windows😅
  > mungkin perlu di modif sedikit buat OS lain
- Scoop package manager (download di [sini](https://scoop.sh/))
- Chafa (instruksi di [sini](#-install-chafa))
- Nerd Font buat tampilin icon2 (download di [sini](https://www.nerdfonts.com/font-downloads))

## Stepnya

Install dulu fastfetch pake scoop:

```powershell
scoop install fastfetch

```

trus generate dulu config.jsonc pake cmd ini:

```powershell
fastfetch --gen-config-full

```

Trus download atau copy isi file raw [config.jsonc](https://github.com/Scintilla7/fastfetch-config/blob/main/config.jsonc) trus paste ke config.jsonc yang sudah di generate tadi

> bisa aktifin module2 di bagian Connection di config.jsonc biar bisa tampilin adapter network beserta status koneksi, public ip, local ip sama dns. Tinggal di uncomment aja pake `ctrl + /`

udah tinggal jalanin cmd fastfetch di terminal:

```powershell
fastfetch

```

## 🖼️ Screenshot Terminal

Tampilan fastfetch di terminal Windows:

![Terminal](https://github.com/Scintilla7/fastfetch-config/blob/main/screenshot/fastfetch.jpg)

Dengan mengaktifkan modul connection di config.jsonc:

![Terminal_Connection](https://github.com/Scintilla7/fastfetch-config/blob/main/screenshot/fastfetch_connection.jpg)

Src gambar logo di [credits](#credits)

## 📦 Install Chafa

Command buat install chafa pake scoop:

```powershell
scoop install chafa

```

Cek Chafa di web officialnya - [Chafa](https://hpjansson.org/chafa/)

---

## 🖼️ Konversi Gambar ke Format Sixel pake Chafa

Pake command ini buat convert gambar ke format sixel biar bisa ditampilin di terminal Windows:

```powershell
chafa -f sixel -s WxH "path/gambar/ori" > "path/jadi/gambar_sixel.sixel"

```

Ubah `WxH` dengan ukuran resolusi yang diinginkan (misalnya `40x40`).

Sesuaiin `"path/gambar/ori"` dengan path gambar asal dan `"path/jadi/gambar_sixel.sixel"` dengan path untuk output gambar sixel.

---

## 🖼️ Cara Mengubah Logo

Edit baris ini di config.jsonc:

```json
{
  "logo": {
    "source": "~/.config/fastfetch/logos/bina_sticker_1.sixel", // edit path gambar sixel disini
    "type": "raw",
    "height": 20,
    "width": 40,
    "padding": {
      "top": 7,
      "left": 2,
    },
  },
}
```

---

## ⚙️ Cek Detail Modul Fastfetch

Cmd buat tampilin modul2 fastfetch:

```powershell
fastfetch --list-modules

```

Cmd buat tampilin detail format modul2 fastfetch:

```powershell
fastfetch -h [module]-format

```

(Ganti `[module]` dengan nama modul di --list-modules, contoh: `fastfetch -h cpu-format`)

---

### Credits

Didasarkan pada desain fastfetch user **SoupCat-Py** (cek di [sini](https://github.com/SoupCat-Py/fastfetch-configs))  
Src gambar logo ss 1: [HoYoLab](https://www.hoyolab.com/article/43382173) - ganti ke bahasa Jepang  
Src gambar logo ss 2: [Facebook](https://web.facebook.com/reel/1493260242352600) - sticker ada di komentar
