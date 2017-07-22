# Hatsukoi Fansubs
Jika ada apa-apa atau ada yang kurang, [contact me](https://www.facebook.com/MuhammadFaisal21)

## Notes
- Usahakan memakai url external untuk gambar, kecuali asset site itu sendiri karena github repo kecil mang
- Category itu **case-sensitive** jadi caps dalam satu huruf dan tidak memakai caps berpengaruh dalam link
- **Jangan memakai space** dalam category pakai "-" tanpa tanda kutip untuk memisahkan kata dalam category

## Ukuran Assets
- logo: max-width 200px, height bebas
- cover utama/banner: width 100%, height 220px
- thumbnail anime: max-width 225px, max-height 318px
- thumbnail post: width 70%, height 226px

## Pemakaian

### Mengubah Logo dan Cover Utama

Di directory **_data/settings.yml** ubah value **logo** dan **cover**

### Membuat Post

1. Buat file dalam  folder **_post** dengan format **YEAR-MONTH-DAY-title.html**
2. **Masukkan** kode di bawah ini dalam file postnya di paling atas, ubah sesuka hati kecilmu
```shell
---
title: Hunter x Hunter 160 Subtitle Indonesia (Judul)
category: Hunter-x-Hunter (Nama Anime) Jangan pake space, ganti dengan "-" tanpa tanda kutip
thumb: url-gambar.jpg (Thumbnail Post)
date: 2017-07-03 19:45:01 +07:00 (Waktu Post) dengan format YYYY-MM-DD HH:MM:SS +/-TTTT
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

### Menambahkan anime

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

### Menambah jumlah relawan dalam page about

Di directory **_data/relawan.yml** ubah value di bawah
```shell
- img: url-gambar.jpg (Gambar)
  color: (Background keterangan relawan (default putih))
  name: ARU (Nama)
  role: Web Designer (Role)
```

### Menambah page

1. Di directory **pages/** buat file dengan format **judul-page.html**
2. **Tambahkan** kode di bawah ini di paling atas filenya
```shell
---
title: About (Judul Page)
permalink: about.html (Nama File Pagenya) Judul page bisa berbeda ini nya
---
```

### Menambah Navigation untuk Page

1. Masuk ke **_includes/header.html**
2. Tambah kode ini ke dalam file **di bawah tag a terakhir**
```shell
<a class="page-link {% if page.url == '/faq.html' %}current{% endif %}" target="_top" href="{{ site.url }}/faq">FAQ</a>
```
- ubah **/faq.html** dengan **directory pagenya** jika page memiliki front matter **permalink** ubah seperti contoh di atas, **tidak perlu direktori lengkapnya**, jika tidak ada **permalink** ubah seperti **/pages/faq.html**
- ubah **{{ site.url }}/faq** dengan **{{ site.url }}/nama-page** jika ada **permalink** front matternya, jika tidak ada pakai direktori pagenya seperti **{{ site.url }}/pages/faq**

Semua ini berpacu pada aturan Jekyll pada [Jekyll Docs](http://jekyllrb.com/docs/)
