# Tutorial menjalankan DiKantin di VS Code

## 1. Siapkan folder proyek

1. Unduh dan ekstrak `DiKantin-Mobile-VSCode.zip` ke folder yang mudah ditemukan.
2. Buka **Visual Studio Code**.
3. Pilih **File → Open Folder...**.
4. Pilih folder hasil ekstrak yang berisi `index.html`, `style.css`, dan `app.js`.
5. Jika VS Code menanyakan apakah kamu percaya pada folder tersebut, pilih **Trust** untuk folder proyek yang baru diekstrak.

## 2. Jalankan halaman web

Cara termudah adalah memakai ekstensi Live Server:

1. Klik ikon **Extensions** di sisi kiri VS Code.
2. Cari **Live Server** dan pasang ekstensi tersebut.
3. Buka file `index.html` dari Explorer di sisi kiri.
4. Klik **Go Live** di pojok kanan bawah. Browser akan membuka prototipe.
5. Setelah mengubah file, simpan dengan `Ctrl+S`. Live Server akan memuat ulang halaman.

Alternatifnya, buka `index.html` langsung di browser. Live Server lebih nyaman saat mengedit karena perubahan akan dimuat ulang otomatis.

## 3. Tampilkan seperti layar ponsel

Di Chrome atau Edge:

1. Buka halaman dari Live Server.
2. Tekan `F12` untuk membuka Developer Tools.
3. Tekan `Ctrl+Shift+M` untuk menyalakan **Device Toolbar**.
4. Pilih perangkat ponsel dari menu perangkat, atau gunakan mode **Responsive**.
5. Untuk ukuran umum, atur lebar ke `390` dan tinggi ke `844`.
6. Muat ulang halaman bila tampilan belum menyesuaikan.

Pada layar komputer, konten tetap dibatasi selebar ponsel dan berada di tengah. Tidak ada tata letak desktop terpisah.

## 4. Coba alur pemesanan

1. Dari layar masuk, tekan **Lanjut jelajah sebagai tamu**.
2. Pilih **Makan di tempat**.
3. Pilih salah satu kantin, lalu tekan **Simulasikan QR terdeteksi**. Nomor meja bisa diubah sebelum menekan tombol itu.
4. Konfirmasi meja dan pilih tenant.
5. Tambah atau kurangi makanan di halaman menu.
6. Buka keranjang, cek voucher dan total pembayaran.
7. Tekan **Bayar sekarang**, lalu **Simulasikan pembayaran berhasil**.
8. Di halaman pelacakan, tekan **Tandai pesanan selesai** untuk membuka layar ulasan.

## 5. Ubah isi dan tampilan

- Ubah teks, daftar kantin, tenant, dan menu di `app.js`.
- Ubah warna utama di variabel `:root` pada bagian atas `style.css`.
- Ganti gambar dengan file baru di folder `assets/`, lalu sesuaikan alamat file pada `app.js`.
- `index.html` adalah titik awal yang menghubungkan stylesheet dan JavaScript.

## Catatan

Ini prototipe front-end. Login, scan QR, kode QRIS, pembayaran, status pesanan, poin, dan ulasan tidak terhubung ke layanan nyata. Kode QR pada layar pembayaran adalah pola visual demo dan tidak dapat dipindai.
