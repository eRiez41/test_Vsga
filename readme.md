Pemesanan Taxi Online


Ini adalah sebuah program untuk melakukan pemesanan taksi online. Aplikasi ini pakai bahasa PHP dan HTML untuk tampilan antarmukanya.
Sistem ini memungkinkan pengguna untuk melakukan pemesanan taksi dengan memberikan nama, nomor telepon, jenis mobil yang dipilih, dan jarak yang akan ditempuh. Sistem kemudian menghitung total biaya berdasarkan jarak yang ditempuh dan menampilkan detail pemesanan beserta biayanya.

Referensi : Bootstrap, Open Ai Chatgpt

Instruksi :

Variabel $mobil adalah sebuah array yang berisi jenis-jenis mobil yang tersedia untuk pemesanan.

Array $mobil diurutkan secara ascending menggunakan fungsi sort().

Sistem menggunakan Bootstrap CSS, dan berkas CSS terhubung di bagian head HTML.

Sistem menampilkan logo layanan taksi online.

Fungsi hitung_sewa() menghitung biaya berdasarkan jarak yang ditempuh dan biaya sewa per kilometer. Fungsi ini mengalikan jarak ($jarak) dengan biaya sewa ($biaya_sewa) dan mengembalikan biaya yang dihitung.

Sistem menghasilkan menu dropdown untuk memilih jenis mobil berdasarkan data dalam array $mobil menggunakan perulangan.

Ketika tombol "Pesan" diklik, sistem melakukan langkah-langkah berikut:

Mengambil data input pengguna dari formulir.
Memeriksa jarak yang ditempuh ($jarak_tempuh) untuk menentukan biaya menggunakan pernyataan percabangan if-else.
Memanggil fungsi hitung_sewa() untuk menghitung biaya berdasarkan jarak dan biaya sewa.
Menyimpan detail pemesanan dalam file JSON (data.json) dengan mengonversi array PHP menjadi format JSON menggunakan json_encode().
Mengambil detail pemesanan yang tersimpan dari file JSON dan mengonversinya kembali menjadi array PHP menggunakan json_decode().
Perhitungan biaya didasarkan pada jarak yang ditempuh. Jika jarak kurang dari atau sama dengan 10 kilometer, biaya diatur menjadi 1000 Rupiah Indonesia (IDR). Jika jarak lebih dari 10 kilometer, biaya dihitung dengan menambahkan 1000 IDR dan mengalikan selisih antara jarak dan 10 kilometer dengan 5000 IDR.

Biaya yang dihitung disimpan dalam variabel $tagihan dengan memanggil fungsi hitung_sewa() dengan parameter jarak dan biaya sewa.

Detail pemesanan, termasuk nama pelanggan, nomor telepon, jenis mobil, jarak yang ditempuh, dan total biaya, ditampilkan pada halaman web.

Penggunaan
Klon repositori atau unduh berkas ke mesin lokal Anda.

Pastikan Anda memiliki lingkungan pengembangan PHP yang sudah diatur (misalnya, XAMPP, WAMP, atau MAMP).

Letakkan berkas-berkas tersebut di direktori server web yang sesuai (misalnya, htdocs untuk XAMPP).

Mulai server web dan akses berkas PHP melalui browser web.

Isi detail yang diperlukan dalam formulir, seperti nama, nomor telepon, jenis mobil, dan jarak yang akan ditempuh.

Klik tombol "Pesan" untuk melihat detail pemesanan dan total biayanya.

Detail pemesanan, termasuk nama pelanggan, nomor telepon, jenis mobil, jarak yang ditempuh, dan total biaya, akan ditampilkan pada halaman web dibawah form.