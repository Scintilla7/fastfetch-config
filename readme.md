# 🔗 Repo Fastfetch

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
