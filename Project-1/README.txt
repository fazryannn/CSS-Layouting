FAZ-GARAGE - Website Artikel Sederhana
Latihan CSS Layouting (Project-1)
Rabu 14 Okt 2026
Update Rabu 21 Okt 2026: menambah sidebar tentang penulis

Deskripsi
Website satu halaman berisi artikel "Perawatan Rutin Motor Agar Tetap Awet"
dengan sidebar tentang penulis di sebelah kanan.
Dibuat untuk mempraktikkan materi CSS layouting yang sudah dipelajari.

Struktur Folder
Project-1
    index.html          halaman artikel
    style.css           seluruh pengaturan tampilan
    README.txt          penjelasan project
    img/hero1.jpg       foto sampul
    img/background.png  pola background halaman
    img/argii.jpg       foto penulis di sidebar

Bagian Halaman
1. Header     nama website dan menu navigasi
2. Hero       foto sampul
3. Konten     dua kolom
               - Artikel (kiri): judul, penulis, tanggal, tiga sub judul, penutup
               - Sidebar (kanan): foto dan deskripsi singkat penulis
4. Footer     hak cipta

Materi CSS yang Dipraktikkan
1. Box model: margin auto, padding, border
2. Dimensi: max-width 960px agar halaman menyusut di layar kecil
3. Box sizing: border-box
4. Display: inline-block untuk menu horizontal
5. CSS reset ringan pada ul dan li
6. Background: background-image, background-size cover, background-position,
   background-color sebagai cadangan jika gambar gagal dimuat
7. Pseudo class: a:hover pada menu
8. Tipografi: font-family, font-size 1.0625rem (17px), line-height 1.7
9. Warna: pola background, kartu putih, aksen oranye
10. Float: artikel float left (600px), sidebar float right (300px),
    foto penulis float left agar teks mengalir di sebelahnya
11. Clearfix: .clearfix::after (content, display block, clear both) pada
    pembungkus dua kolom agar tingginya mengikuti kolom dan footer tetap di bawah
12. Pseudo element: ::after

Lebar Kolom
Artikel 600px + sidebar 300px = 900px dari container 960px.
Sisa 60px menjadi jarak di antara kedua kolom.

Palet Warna
Latar halaman    #f4f5f7 (cadangan) dan pola background.png
Kartu artikel    #ffffff
Teks             #111827
Aksen / link     #c2410c
Garis hero       #e5e7eb
Footer           #1f2937

Cara Menjalankan
Buka file index.html di browser. Pastikan folder img berisi
hero1.jpg, background.png, dan argii.jpg, dan berada di folder
yang sama dengan index.html.

Catatan
Parent yang semua isinya di-float akan menciut jadi tinggi nol.
Perbaiki dengan clearfix pada parent-nya, bukan dengan margin besar.

Pada box-sizing border-box, padding ikut mengurangi lebar elemen.
Foto sidebar diberi jarak dengan margin-right (bukan padding-right)
agar tidak gepeng, dan object-fit: cover agar foto terpotong rapi.

Download gambar bebas pakai
https://unsplash.com/

Download pattern / pola untuk background halaman
http://subtlepatterns.com/

Penulis: Argi Fazryana