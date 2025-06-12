---
layout: post
title: "Membuat Web dengan Jekyll Serve"
---
### Membuat Web dengan Jekyll Serve

Untuk membuat personal web dengan Jekyll dan publish di GitHub Page ikuti langkah-langkah berikut ini:
1. Buat akun di GitHub dengan username sesuai nama masing-masing.
2. Buat repository baru dengan nama username dan github.io contoh: \
jika username nya adalah `mailaazizaa`\
maka nama repository buat seperti ini `mailaazizaa.github.io`
3. Clone repository tersebut ke lokal
```bash
git@github.com:mailaazizaa/mailaazizaa.github.io.git
```
4. Masuk ke dalam folder repository tersebut kemudian install Jekyll dengan perintah berikut melaui terminal
```bash
gem install jekyll bundler
```
5. Jalankan perintah bundle init untuk inisialisasi folder terebut sebagai proyek
  jekyll seperti perintah berikut ini. Hasil dari perintah tersebut adalah file baru
  dengan nama Gemfile.
```bash
bundle init
```

6. Edit file `Gemfile` dan tambahkan kode berikut pada baris paling bawah
```bash
gem "jekyll"
```

7. Buat file baru dengan nama index.html, kemudian isi dengan struktur dasar HTML
8. Jalankan jekyll build untuk build web yang telah dibuat sehingga menhasilkan
  directory _site.
```bash
jekyll build
```
9.Kemudian jalankan perintah jekyll serve untuk menjalankan web yang telah
  dibuat di web browser dengan alamat http://localhost:4000 atau 127.0.0.1:4000
```bash
jekyll serve
```

10. Jika web telah berhasil dibuka, edit file Gemfile.lock dengan menambahkan
  platform linux pada bagian platform seperti pada gambar berikut.
```bash
PLATFORMS
  x86_64-linux
```

11. Untuk push repositori ke GitHub ketik perintah-perintah berikut
```bash
git add .
git commit -m "isi pesan commit"
git push
```

---

## Membuat List Teman
- Ubah file `index.html` yang telah dibuat sebelumnya menjadi:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1>Nama: Maila Aziza</h1>
    <p>Deskripsi Diri: Saya merupakan mahasiswa semester 2 prodi Teknik Informatika di Politeknik Negeri Lhokseumawe.</p>
       <h2>Berikut list Teman-teman saya di kelas:</h2>
       <ul>
        <li><a href="https://mailaazizaa.github.io/" target="_blank">Maila Aziza</a></li>
       </ul> 
</body>
</html>
```

- Untuk membuat list teman, buat file baru dengan nama `friends.md`, kemudian isi dengan kode berikut:

```markdown
---
layout: default
title: Friends
---
# Friends page

Berikut teman-teman saya di kelas:
- [Maila Aziza](https://mailaazizaa.github.io/)
- ...
```