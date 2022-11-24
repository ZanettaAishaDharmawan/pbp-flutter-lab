# Tugas 7 
## Jelaskan apa yang dimaksud dengan stateless widget dan stateful widget dan jelaskan perbedaan dari keduanya.
Stateless widget merupakan sebuah widget yang bersifat statis dan tidak dapat diubah. Sedangkan, stateful widget merupakan widget yang dinamis dan dapat diubah.
- Stateless widget terupdate saat terinisialisasi, tidak memiliki setState(), widget bersifat static, dan tidak dapat terupdate saat sedang berjaln kecuali terdapat peristiwa external.
- Stateful widget terupdate secara dinamis, memiliki internal setState(), widget bersifat dinamis, dan dapat diupdate ketika sedang dijalankan.

## Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.
- ```Scaffold```: Mengimplementasikan struktur  dasar tata letak visual desain
- ```Appbar```: Untuk membuat bar yang ada pada atas layar
- ```Text```: Untuk menulis teks di layar
- ```Padding```: Menambahkan jarak pada suatu elemen 
- ```Row```: Mengatur tata letak widget secara horizontal
- ```Column```: Mengatur tata letak widget secara vertikal
- ```Expanded```: Memperluas child dari Row
- ```FloatingActionButton```: Menampilkan button
- ```Icon```: Menampilkan ikon

## Apa fungsi dari setState()? Jelaskan variabel apa saja yang dapat terdampak dengan fungsi tersebut.
Fungsi setState() bertugas untuk memberitahu widget bahwa ada object yang berubah pada state sehingga akan melakukan build ulang pada Widget tersebut. Variabel yang terdampak pada fungsi tersebut adalah variabel yang sifanya mutable dan terdeklarasi secara global di sebuah class. 

## Jelaskan perbedaan antara const dengan final.
Const dan final merupakan keyword yang digunakan untuk membuat variabel yang bersifat immutable. Const digunakan untuk mengassign suatu value dari variabel sebelum runtime. Sedangkan, final digunakan untuk mengassign value dari variabel setelah runtime.

## Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.
- Membuat sebuah direktori baru untuk membuat applikasi flutter
- Membuat aplikasi flutter dengan mengetik ```flutter create counter_7``` di cmd
- Mengedit di main.dart
- Menambahkan boolean ```isVisible``` dengan nilai true
- Menambahkan fungsi ```_decrementConter()``` untuk mengurangi counter
- Menambahkan fungsi ```_showButton()``` untuk mengeset nilai dari boolean
- Mengedit teks akan muncul tulisan 'GENAP' jika variable _counter % 2 == 0, jika tidak akan muncul tulisan 'GANJIL'
- Menambahkan widget FloatingActionButton untuk menampilkan button
- Program telah selesai dibuat dapat dijalankan melalui cmd dengan perintah flutter run


# Tugas 8

## Jelaskan perbedaan Navigator.push dan Navigator.pushReplacement.
Navigator push dan navigator push replacement berfungsi untuk ke halaman lainnya. Perbedaannya adalah jika menggunakan navigator push, route screen yang lama tidak dihapus sehinggga bisa kembali ke route tersebut. Jika navigator push replacement route screen yang lama dihapus dan tidak dapat kembali ke route yang lama.

## Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.
- ```Row```: Mengatur tata letak widget secara horizontal
- ```Column```: Mengatur tata letak widget secara vertikal
- ```Text```: Untuk menulis teks di layar
- ```Padding```: Menambahkan jarak pada suatu elemen 
- ```Row```: Mengatur tata letak widget secara horizontal
- ```Column```: Mengatur tata letak widget secara vertikal
- ```Form```: Berupa container untuk menampung form field widget
- ```TextFormField```: Menerima input dari user

## Sebutkan jenis-jenis event yang ada pada Flutter (contoh: onPressed).
- ```OnPressed```
- ```OnSaved```
- ```OnChanged```

## Jelaskan bagaimana cara kerja Navigator dalam "mengganti" halaman dari aplikasi Flutter.
Ketika kita menjalankan navigator push, screen baru akan ditambahkan ke stack sehingga screen sebelumnya tertimpa dengan screen yang baru. Screen yang di push akan berada di paling atas stack, sehingga screen seolah olah berganti dan dapat dilihat oleh user.

## Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.
1. Menambahkan DrawerApp() pada main dan implementasinya di drawer.dart
2. Pada drawer.dart menambahkan beberapa routing ke halaman counter_7, form, dan data_budget
3. Membuah halaman form untuk menerima input data Judul, Nominal, dan datetime
4. Menyimpan input ke dalam card dan tersimpan dalam list
5. Menampilkan card ke halaman data_budget
