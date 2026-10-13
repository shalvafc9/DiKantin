# DiKantin — web mobile

Prototipe web pemesanan makanan kantin kampus dengan tampilan khusus ponsel. Alur dan warna mengikuti referensi Figma: latar krem pucat, oranye hangat, hijau tua, dan teks cokelat gelap.

## Cara menjalankan di VS Code

1. Ekstrak folder proyek jika dibuka dari file ZIP.
2. Buka VS Code, pilih **File → Open Folder...**, lalu pilih folder `DiKantin-Mobile`.
3. Pada panel Extensions, cari dan pasang **Live Server**.
4. Buka `index.html`, lalu klik **Go Live** di pojok kanan bawah VS Code. Halaman akan terbuka di browser.
5. Untuk melihat ukuran ponsel di Chrome atau Edge, tekan `F12`, lalu `Ctrl+Shift+M`. Pilih ukuran ponsel atau masukkan lebar sekitar `390 px`.

Tidak perlu `npm install` atau server backend. Proyek ini dibuat dari HTML, CSS, dan JavaScript biasa.

## Alur prototipe

1. Masuk dengan NIM atau pilih **Lanjut jelajah sebagai tamu**.
2. Pilih **Makan di tempat** atau **Ambil sendiri**.
3. Cari dan pilih kantin.
4. Simulasikan scan QR, lalu konfirmasi nomor meja.
5. Pilih tenant dan tambahkan menu ke keranjang.
6. Ubah jumlah menu, catatan tenant, atau voucher di checkout.
7. Lanjutkan ke halaman QRIS demo.
8. Pilih **Simulasikan pembayaran berhasil**.
9. Lihat status pesanan, tandai selesai, lalu isi ulasan.

Navigasi bawah juga dapat dipakai untuk berpindah ke Beranda, Kantin, Scan meja, Pesanan, dan Profil.

## Struktur file

- `index.html` — elemen halaman dan pemanggil file CSS/JavaScript.
- `style.css` — warna, komponen, tata letak, dan aturan tampilan ponsel.
- `app.js` — data contoh, render layar, dan interaksi prototipe.
- `assets/` — gambar makanan dan suasana kantin yang dipakai di halaman.

Foto `es-teh-kampul.png` dan `tahu-krispi.png` dibuat khusus untuk melengkapi kartu menu yang belum memiliki foto di referensi.

## Mengubah warna

Di bagian `:root` pada `style.css`, sesuaikan variabel berikut:

```css
--paper: #fbf8ff;
--ink-soft: #584237;
--orange: #ea580c;
--green: #006c49;
```

## Batasan demo

Scan QR, login, pembayaran QRIS, status pesanan, poin, dan ulasan hanya simulasi sisi browser. Kode QR di halaman pembayaran tidak dapat dipindai dan tidak melakukan transaksi. Agar menjadi aplikasi produksi, bagian tersebut perlu dihubungkan ke kamera, server, akun kampus, dan penyedia pembayaran.
