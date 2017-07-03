# Hatsukoi
Very nice fansub theme
=============================
Jika ada apa-apa contact [Orang Tampan](https://www.facebook.com/MuhammadFaisal21)

## Notes
- Usahakan memakai url untuk gambar, kecuali asset site itu sendiri karena github repo kecil mang
- Category itu case-sensitive jadi caps dalam satu huruf dan tidak memakai caps berpengaruh dalam link
- Jangan memakai space dalam category pakai "-" tanpa tanda kutip untuk memisahkan kata dalam category

## Pemakaian

#### Mengubah Logo dan Cover Utama

Di directory **_data/settings.yml** ubah value **logo** dan **cover**

#### Membuat Post

1. Buat file dalam  folder **_post** dengan format **YEAR-MONTH-DAY-title.html**
2. **Masukkan** kode di bawah ini dalam file postnya di paling atas, ubah sesuka hati kecilmu
```shell
---
title: Hunter x Hunter 160 Subtitle Indonesia (Judul)
category: Hunter-x-Hunter (Nama Anime) Jangan pake space, ganti dengan "-" tanpa tanda kutip
thumb: url-gambar.jpg (Thumbnail Post)
480p: (Bisa berapa aja)
  - link: www.google.com
    web: google
  - link: www.facebook.com
    web: facebook
  - link: www.google.com
    web: google
  - link: www.facebook.com
    web: facebook
720p: (Bisa berapa aja)
  - link: www.google.com
    web: google
  - link: www.facebook.com
    web: facebook
  - link: www.google.com
    web: google
  - link: www.facebook.com
    web: e
---
```

#### Menambahkan anime

1. Buat file dalam  folder **anime/** dengan format **Nama-Anime.html**, ingat **ubah space dengan '-' tanpa tanda kutip**
2. **Masukkan** kode di bawah ini dalam file postnya di paling atas, ubah sesuka hati kecilmu
```shell
---
thumb: url-gambar.jpg (Thumbnail Anime)
genre: Action (Genre)
status: Ongoing (Status)
sinopsis : asdasdasd (Sinopsis)
category: Hunter-x-Hunter (Nama Anime) Samakan degan category postnya
---
```

#### Menambah jumlah relawan dalam page about

Di directory **_data/relawan.yml** ubah value di bawah
```shell
- img: url-gambar.jpg (Gambar)
  color: (Background keterangan relawan (default putih))
  name: ARU (Nama)
  role: Web Designer (Role)
```

Semua ini berpacu pada aturan Jekyll pada [Jekyll Docs](http://jekyllrb.com/docs/)
