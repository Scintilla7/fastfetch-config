# 💻 Instalasi

Generate dulu config.json pake cmd ini:

```powershell
fastfetch --gen-config-full

```

Trus download atau copy isi file raw [config.json](https://github.com/Scintilla7/fastfetch-config/blob/main/config.jsonc) trus paste ke config.json yang sudah di generate tadi

> bisa aktifin module connection di config.json biar bisa tampilin public ip, local ip sama dns
> tinggal di uncomment aja

## 🖼️ Screenshot Terminal

Tampilan fastfetch di terminal Windows:
![Terminal](https://github.com/Scintilla7/fastfetch-config/blob/main/screenshot/fastfetch.jpg)

## 🔗 Repo Fastfetch

[GitHub - fastfetch-cli/fastfetch](https://github.com/fastfetch-cli/fastfetch)

---

## 📦 Install Chafa

Command buat install chafa pake scoop (install dulu scoop di [sini](https://scoop.sh/)):

```powershell
scoop install chafa

```

---

## 🖼️ Konversi Gambar ke Format Sixel

Pake command ini buat convert gambar ke format sixel biar bisa ditampilin di terminal Windows:

```powershell
chafa -f sixel -s WxH "path/gambar/ori" > "path/jadi/gambar_sixel.sixel"

```

Ubah `WxH` dengan ukuran resolusi yang diinginkan (misalnya `40x40`).

Sesuaiin `"path/gambar/ori"` dengan path gambar asal dan `"path/jadi/gambar_sixel.sixel"` dengan path untuk output gambar sixel.

---

## ⚙️ Cek Detail Modul Fastfetch

Cmd buat tampilin modul2 fastfetch:

```powershell
fastfetch --list-modules

```

Cmd buat tampilin detail format modul2 fastfetch:

```powershell
fastfetch -h <module>-format

```

(Ganti `<module>` dengan nama modul di --list-modules, contoh: `fastfetch -h cpu-format`)

---
