---
layout: post
title: "Javascript dan Config YML"
---
### Javascript dan Config YML

### Javascript
JavaScript adalah bahasa pemrograman yang digunakan untuk membuat situs web interaktif. Dalam proyek Jekyll, Anda dapat menambahkan file JavaScript ke dalam folder `assets/js` dan menghubungkannya ke halaman HTML Anda.
- Buat folder `assets/js` di dalam direktori proyek Jekyll Anda.
- Buat file JavaScript baru di dalam folder tersebut, misalnya `scripts.js`, dan isi dengan kode berikut:
```javascript
function myFunction() {
    alert("maila cewe paling cakep sedunia");
  }
```

### Config YML
Config YML adalah file konfigurasi yang digunakan oleh Jekyll untuk mengatur berbagai aspek dari situs web. File ini biasanya terletak di root direktori proyek Jekyll dan memiliki nama `_config.yml`. Di dalamnya, Anda dapat menentukan berbagai pengaturan seperti nama situs, deskripsi, URL, dan lainnya.
- Isi file `_config.yml` dengan kode berikut:
{% raw %}
```yaml
url: 'https://mailaazizaa.github.io/'
plugins:
  - jekyll-feed
  - jekyll-sitemap
  - jekyll-seo-tag
```