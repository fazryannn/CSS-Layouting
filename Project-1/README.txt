FAZ-GARAGE - Website Artikel Sederhana
Latihan CSS Layouting (Project-1)
Rabu 14 Okt 2026

Update Rabu 21 Okt 2026
Menambah: sidebar tentang penulis

Update Selasa 10 Nov 2026
Menambah: navbar fixed dengan kolom pencarian, logo GitHub, tampilan responsif smartphone

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
    img/github.png      logo GitHub

Bagian Halaman
1. Navbar     menempel di atas layar (fixed), berisi kolom pencarian
2. Logo       logo GitHub di pojok kanan atas, menuju profil GitHub
3. Header     nama website dan menu navigasi
4. Hero       foto sampul
5. Konten     dua kolom
               - Artikel (kiri): judul, penulis, tanggal, tiga sub judul, penutup
               - Sidebar (kanan): foto dan deskripsi singkat penulis
6. Footer     hak cipta

Materi CSS yang Dipraktikkan
1. Box model: margin auto, padding, border
2. Dimensi: max-width 960px agar halaman menyusut di layar kecil
3. Box sizing: border-box
4. Display: inline-block untuk menu horizontal
5. CSS reset ringan pada ul dan li, margin 0 pada body
6. Background: background-image, background-size cover, background-position,
   background-color sebagai cadangan jika gambar gagal dimuat
7. Pseudo class: a:hover pada menu dan tombol
8. Tipografi: font-family, font-size 1.0625rem (17px), line-height 1.7
9. Warna: pola background, kartu putih, aksen oranye
10. Float: artikel float left, sidebar float right, foto penulis float left
    agar teks mengalir di sebelahnya, kolom pencarian float right
11. Clearfix: .clearfix::after (content, display block, clear both) pada
    pembungkus dua kolom agar tingginya mengikuti kolom dan footer tetap di bawah
12. Pseudo element: ::after
13. Position: fixed (navbar), absolute (logo GitHub), relative (container)
14. Z-index: navbar di atas semuanya, logo di atas header dan hero
15. Overflow: hidden pada container agar logo tidak membuat halaman bisa digeser
16. Media query: max-width 768px untuk tampilan smartphone

Lebar Kolom
Artikel 62.5% (600px dari 960px) + sidebar 31.25% (300px dari 960px) = 93.75%.
Sisa 6.25% (60px di layar lebar) menjadi jarak di antara kedua kolom.
Memakai persen supaya kolom ikut menyusut saat layar mengecil.

Tampilan Responsif (layar 768px ke bawah)
1. Artikel dan sidebar tersusun ke bawah (float dimatikan, lebar 100%)
2. Hero dipendekkan menjadi 200px dan diposisikan di tengah
3. Logo GitHub dikecilkan menjadi 90px
4. Kolom pencarian dipersempit menjadi 150px
5. Teks sidebar dibesarkan menjadi 14px

Palet Warna
Latar halaman    #f4f5f7 (cadangan) dan pola background.png
Kartu artikel    #ffffff
Teks             #111827
Aksen / link     #c2410c
Garis hero       #e5e7eb
Navbar           salmon
Tombol Cari      #1f2937
Footer           #1f2937

Cara Menjalankan
Buka file index.html di browser. Pastikan folder img berisi
hero1.jpg, background.png, argii.jpg, dan github.png, dan berada di folder
yang sama dengan index.html.
Untuk menguji tampilan smartphone: tekan F12 di Chrome, lalu klik ikon
Toggle device toolbar (Ctrl+Shift+M).

Catatan
Parent yang semua isinya di-float akan menciut jadi tinggi nol.
Perbaiki dengan clearfix pada parent-nya, bukan dengan margin besar.

Pada box-sizing border-box, padding ikut mengurangi lebar elemen.
Foto sidebar diberi jarak dengan margin-right (bukan padding-right)
agar tidak gepeng, dan object-fit: cover agar foto terpotong rapi.

Elemen fixed tidak memakan ruang, jadi body diberi padding-top setinggi navbar (40px)
agar bagian atas halaman tidak tertutup.

Kolom pencarian baru tampilan saja, fungsi pencariannya belum dibuat.

Download gambar bebas pakai
https://unsplash.com/

Download pattern / pola untuk background halaman
http://subtlepatterns.com/

Penulis: Argi Fazryana