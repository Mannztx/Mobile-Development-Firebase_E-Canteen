# INTEGRASI CLOUD FIRESTORE (E-Canteen Poliwangi)

### Disusun Oleh:
Nama: Firman Ardiansyah
NIM: 362458302101
Prodi: TRPL
Kelas: 2D

## TUGAS PRAKTIKUM
### TUGAS WAJIB
1. Jalankan aplikasi dan buktikan bahwa data yang tampil sesuai dengan yang ada di Firebase Console.
- [](images/menus-page.png)
Dari gambar tersebut terbukti bahwa data yang tampil pada aplikasi sesuai dengan data yang ada di Firestore Database (Firebase Console).
2. Lakukan pemesanan, dan tunjukkan kepada Dosen/Asisten bahwa data pesanan masuk ke koleksi orders di Console.
- [](images/pesan.png)
- [](images/pesanan-berhasil.png)
- [](images/bukti-pesanan.png)
Dari beberapa gambar tersebut terbukti bahwa aplikasi dapat melakukan pemesanan dan data pemesanan itu masuk ke koleksi orders di Firestore Database Firebase Console, yang mana data orders tersebut berisi informasi seperti customer_name (nama pemesan), menu_item (menu yang dipesan), price (harga), status (menunggu), dan timestamp (waktu pemesanan).
### TANTANGAN (Point Plus)
1. Tambahkan field category (misal: ’Makanan’, ’Minuman’) pada data di Firebase.
2. Di aplikasi, tambahkan 2 tombol (”Makanan” dan ”Minuman”).
3. Gunakan .where(’category’, isEqualTo: ...) pada query StreamBuilder untuk memfilter list sesuai tombol yang ditekan.
### CATATAN
Jika terdapat kendala atau error seperti data tidak muncul di aplikasi, permission denied, cocoaPods not installed (MacOS), maka periksa penulisan nama koleksi (menus/menu) atau nama field (name/nama) karena firestore bersifat sensitif (jika data tidak muncul di aplikasi), jalankan "sudo gem install cocoapods" kemudian masuk ke folder ios/ dan jalankan "pod install" (jika error: cocoaPods not installed), buka tab rules di firestore ubah menjadi allow read write if true (jika error: permission denied).
