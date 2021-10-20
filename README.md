Templat LaTeX Tesis Informatika ITB
===================================
oleh: Petra Novandi <me@petrabarus.net>  
dimodifikasi: Faris Rizki Ekananda <work@farisekananda.dev>  
original repo: https://github.com/petrabarus/if-itb-latex/

Dokumen ini merupakan templat LaTeX yang ditujukan untuk laporan
tesis di program studi Teknik Informatika ITB. Templat ini penulis
gunakan dalam penulisan laporan tesis penulis dan dengan semangat
berbagi penulis memutuskan untuk mempublikasikan templat ini agar
dapat digunakan oleh banyak orang.

Silakan mengunduh, menggunakan, memodifikasi, dan menyebarkan
templat ini. :)

Contoh Hasil Build
---------
https://drive.google.com/file/d/1cRmhjs1gcVDRZ_SJGqA3ONM5jQIE6lx6/view

Kebutuhan
---------

Program telah diuji dalam sistem operasi Linux Ubuntu 20.04 dan Windows 10. Untuk melakukan instalasi
perangkat lunak yang dibutuhkan, eksekusi perintah berikut.

```
sudo apt-get -qq update && sudo apt-get install -y --no-install-recommends \
    texlive-fonts-recommended texlive-latex-extra texlive-fonts-extra \
    dvipng texlive-latex-recommended texlive-lang-other \
    texlive-bibtex-extra biber xzdec
```

Untuk Windows, Anda dapat melakukan instalasi TeXLive pada [link berikut](https://mirror.ctan.org/systems/texlive/tlnet/install-tl-windows.exe). Manual Instalasi dapat dilihat pada [link berikut](https://www.tug.org/texlive/windows.html). Jangan lupa cek environment variable Anda dan pastikan terdapat PATH menuju `<texlive_installation_directory>\2021\bin\win32`

Penggunaan
----------

Templat ini telah dilengkapi oleh skrip untuk melakukan kompilasi
Makefile. Untuk melakukan kompilasi cukup eksekusi perintah berikut

```bash
# untuk linux
make

# untuk windows
make.bat
```

Hasil kompilasi akan berada pada berkas `output/thesis.pdf`.

Integrasi VSCode LaTeX Workshop
----------

![Demo Gif](demo.gif)

Template ini telah diintegrasikan dengan VSCode extension LaTeX Workshop sehingga dapat melakukan build otomatis, memakai synctex, serta linter. Terdapat 2 file konfigurasi setelan vscode yang terdapat pada folder .vscode. Defaultnya adalah setelan Windows, namun Anda dapat menggantinya dengan setelan linux.

Shortcut Latex Workshop yang berguna
----------
`ctrl + alt + v` pada `*.tex` -> buka file `pdf` interaktif  
`ctrl + alt + j` pada `*.tex` -> pergi ke lokasi kursor pada `pdf` yang dibuka  
`ctrl + klik kanan` pada `*.pdf` -> pergi ke lokasi kursor pada file `.tex` yang sesuai  

Troubleshooting
----------
**Q: Bagaimana cara menghilangkan border merah pada hyperlink di pdf?**  
A: Pada file `config/if-itb-thesis.sty`, Ubah `\usepackage{hyperref}` menjadi `\usepackage[hidelinks]{hyperref}`.

Kontribusi
----------

Templat ini dapat digunakan secara gratis, akan tetapi penulis sangat
berharap adanya kritik serta saran dari pengguna untuk meningkatkan
kualitas hasil dan penggunaan templat ini.

Kritik dan saran tersebut dapat dikirim melalui URL
<https://github.com/darkGrimoire/ta1-latex-itb>.

Terima Kasih
-----------

* Steven Lolong atas pemberian templat LaTeX yang asli.
* Peb Ruswono Aryan atas bantuan pelengkapan struktur dokumen.
