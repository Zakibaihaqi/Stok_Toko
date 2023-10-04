https://mystoktoko.adaptable.app/main/


1)Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step 

   *Membuat sebuah proyek Django baru
	-membuat direktori utama bernama web_stok_toko
	-buka command prompt, alihkan ke direktori tersebut
	-lakukan konfigurasi git pada direktori utama
	-konfigurasikan juga nama pengguna dan surel yang dimiliki
	-buat virtual environment dan aktifkan virtual environment
	-membuat file requirements.txt di dalam direktori web_stok_toko
	-pasang dependencies yang telah dimasukkan ke requirements.txt
	-buat proyek Django bernama stok_toko
	-melakukan runserver untuk test
	-buat file baru bernama .gitignore di dalam direktori web_stok_toko
   *membuat aplikasi dengan nama main pada proyek tersebut
	-aktifkan virtual environment pada direktori utama
	-jalankan perintah untuk membuat aplikasi baru bernama main
   *melakukan routing pada proyek agar dapat menjalankan aplikasi main
	-buka berkas settings.py yang ada di dalam direktori proyek
	-cari INSTALLED_APPS
	-masukkan 'main' ke dalam INSTALLED_APPS agar aplikasi main dapat berjalan
   *Membuat model pada aplikasi main dengan nama item 
	-buka berkas models.py yang ada di direktori aplikasi main
	-buat kelas bernama item dan sertakan atribut wajib yang dibutuhkan kedalamnya
   *Membuat sebuah fungsi pada views.py untuk dikembalikan ke dalam sebuah template yang menampilkan nama aplikasi 
	-buat direktori baru bernama templates di dalam direktori aplikasi main
	-di dalam direktori templates buat file baru bernama main.html
	-isi file main.html dengan nama dan kelas
	-buka berkas views.py yang ada di dalam direktori aplikasi main
	-integrasikan dengan file main.html
   *Membuat sebuah routing pada urls.py aplikasi main untuk memetakan fungsi yang telah dibuat pada views.py
	-buat file urls.py di dalam direktori aplikasi main
	-isi nama aplikasi dan urlpatterns
	-buka urls.py di direktori proyek
	-masukkan path aplikasi main pada urlpatterns
   *Melakukan deployment ke Adaptable terhadap aplikasi yang sudah dibuat 
	-buat repositori baru pada akun github
	-buat branch utama baru
	-hubungkan repositori lokal dengan repositori github
	-lakukan git add untuk semua file yang akan di push ke github
	-lakukan commit
	-lakukan push pada brach yang telah dibuat
	-buatlah aplikasi baru pada Adaptable dan hubungkan dengan repositori github yang baru saja dibuat
	-sesuaikan pengaturan aplikasi
	-lakukan deploy app jika seluruh pengaturan sudah sesuai
   *Membuat sebuah README.md yang berisi tautan menuju aplikasi Adaptable yang sudah di deploy
	-buat file README.md di dalam direktori utama pada repositori lokal
	-jawab pertanyaan dan kerjakan soal
	-lakukan add, commit, dan push ke repositori github


2)![bagan (1)_page-0001](https://github.com/Zakibaihaqi/Stok_Toko/assets/112550171/221d42cc-1e73-4eb5-ba00-c9cc02ed5b54)



3)Jelaskan mengapa kita menggunakan virtual environment? Apakah kita tetap dapat membuat aplikasi web berbasis Django tanpa menggunakan virtual environment?

-Kita menggunakan virtual environment dengan tujuan untuk membuat lingkungan kerja python yang terisolasi.Setiap proyek berbeda terkadang membutuhkan versi program yang berbeda pula. Oleh karena itu, kita perlu menggunakan virtual environment. Dengan begitu tidak ada saling ganggu antar proyek yang sedang didevelop dan untuk mencegah proyek yang sedang dikerjakan mengalami crash.

-Kita tetap dapat membuat aplikasi web tanpa virtual environment. akan tetapi aplikasi web yang dibuat akan menjadi sangat terbatas.


4)MVC (Model-View-Controller):

Model: Ini adalah bagian yang menangani data dan berpikir tentang apa yang seharusnya terjadi di belakang layar. Misalnya, ketika Anda membuat aplikasi untuk mengelola daftar kontak, Model akan menangani data kontak itu sendiri.
View: Bagian ini berfokus pada tampilan yang dilihat oleh pengguna. Ketika Anda melihat daftar kontak Anda di aplikasi, Anda sedang melihat bagian View.
Controller: Ini adalah orang tengah. Ketika Anda menambahkan kontak baru atau mengedit yang sudah ada, Controller akan menghubungkan View dengan Model. Ini seperti "mengatur" interaksi antara tampilan dan data.


MVT (Model-View-Template):

Model: Seperti yang disebutkan sebelumnya, ini adalah tempat data dikelola.
View: Ini mirip dengan bagian View dalam MVC. Ini menangani tampilan, seperti cara data ditampilkan kepada pengguna.
Template: Bagian unik di Django. Ini adalah bagian yang membantu View untuk menampilkan data dengan cara yang benar. Template memungkinkan Anda untuk membuat tampilan HTML dengan mudah tanpa perlu menulis kode HTML panjang.


MVVM (Model-View-ViewModel):

Model: Tetap merupakan bagian yang menangani data.
View: Ini adalah apa yang Anda lihat ketika menggunakan aplikasi. Tampilan diatur dengan baik di sini.
ViewModel: Ini adalah bagian yang membantu menghubungkan Model dan View. Ini memproses data dari Model agar dapat ditampilkan dengan baik di View. Misalnya, jika Anda membuat aplikasi untuk menampilkan cuaca, ViewModel akan mengambil data cuaca dan menampilkannya di tampilan dengan cara yang mudah dimengerti.


Di Django, kita akan menggunakan MVT. Django adalah kerangka kerja yang menyederhanakan proses pengembangan web dengan cara yang terstruktur. Itu membuatnya lebih mudah bagi Anda untuk mengatur bagian Model (data), View (tampilan), dan Template (tampilan HTML) dalam proyek web kita.
<<<<<<< HEAD



TUGAS 3

1)Apa perbedaan antara form POST dan form GET dalam django?
POST
  -Nilai variabel tidak ditampilkan di URL
  -Lebih aman
  -Tidak dibatasi panjang string
  -Biasanya untuk input data melalui form
  -Digunakan untuk mengirim data-data penting seperti password

GET
  -Nilai variabel ditampilkan di URL sehingga user dapat dengan mudah memasukkan nilai variabel baru
  -Kurang aman
  -Dibatasi panjang string sampai 2047 karakter
  -Biasanya untuk input data melalui link
  -Digunakan untuk mengirim data-data tidak penting

2)Apa perbedaan utama antara XML, JSON, dan HTML dalam konteks pengiriman data?

--HTML adalah blok utama untuk pengembangan web dan biasanya digunakan untuk menentukan struktur page
--XML adalah bahasa markup dan menggunakan struktur tag untuk mewakili item data
--JSON adalah pasangan yang berisi key-value untuk membuat struktur seperti map yang didasarkan pada javascript


3)Mengapa JSON sering digunakan dalam pertukaran data antara aplikasi web modern?

JSON sering digunakan dalam pertukaran data antara aplikasi web modern karena memiliki sintaks yang sederhana dan mudah dipahami, format data yang ringan, JSON juga mendukung berbagai tipe data dasar, mendukung nesting, terintegrasi dengan JavaScript, dan masih banyak lagi.

4)

   *Membuat input form untuk menambahkan objek model pada app sebelumnya
	-merubah path 'main/' menjadi ''
	-membuat kerangka views dan hubungkan dengan views pada main
	-buat file baru dengan untuk forms dan buat kelas ProductForm
	-import kelas ProductForm pada views
	-buat fungsi baru untuk membuat item baru berdasarkan request.POST
	-masukkan item pada fungsi show_main pada views
	-pada main views import create_product dan tambahkan pula path
	-buat file baru dengan nama create_product.html di templates
   *Tambahkan 5 fungsi views untuk melihat objek yang sudah ditambahkan dalam format HTML,XML,JSON,XML by ID, dan JSON by ID
	-import HttpResponse dari django.http dan serializers dari django.core pada views di direktori main
	-buat fungsi show_xml
	-masukkan data setelah itu return
	-buat fungsi yang kurang lebih sama untuk json
	-buat fungsi show_xml_by_id dan tambahkan parameter untuk id
	-buat fungsi yang sama untuk show_json_by_id
   *Membuat routing URL untuk masing-masing views yang telah ditambahkan pada poin 2
	-buka urls yang ada di folder main import fungsi show_xml, show_json, show_xml_by_id, show_json_by_id yang telah dibuat
	-tambahkan path url ke dalam urlpatterns untuk setiap fungsi


![Screenshot (11)](https://github.com/Zakibaihaqi/Stok_Toko/assets/112550171/8f661ccc-9fab-49db-83f0-ec3f5e11f056)
![Screenshot (16)](https://github.com/Zakibaihaqi/Stok_Toko/assets/112550171/23cba88c-145d-47f5-8a37-a4b8ee849ffb)
![Screenshot (17)](https://github.com/Zakibaihaqi/Stok_Toko/assets/112550171/4dd7b813-abc3-405d-9bba-557aa0057543)
![Screenshot (15)](https://github.com/Zakibaihaqi/Stok_Toko/assets/112550171/a51f3749-689a-452c-bba6-ac66922e879d)
![Screenshot (14)](https://github.com/Zakibaihaqi/Stok_Toko/assets/112550171/a8a67348-a7ca-4ad6-9fb3-60dcbb46f8c3)






Tugas 4

1)Apa itu Django UserCreationForm, dan jelaskan apa kelebihan dan kekurangannya?

-UserCreationForm adalah salah satu komponen dalam django yang digunakan untuk membuat formulir pendaftaran pengguna. Form ini digunakan untuk mengumpulkan informasi pengguna seperti username dan password 
-Kelebihan yang dimiliki UserCreationForm diantara lain, terdapat validasis untuk memastikan informasi yang dimasukkan pengguna sesuai dengan ketentuan minimal seperti kata sandi yang cukup kuat, dan form otentifikasi yang sudah terintegrasi dengan django.
-kekurangan yang dimiliki UserCreationForm diantara lain, UserCreationForm tidak dapat menjamin keamanan, tampilan UserCreationForm memiliki tampilan baku yang perlu disesuaikan dengan desain dan tampilan aplikasi.

2)Apa perbedaan antara autentikasi dan otorisasi dalam konteks Django, dan mengapa keduanya penting?
-Autentikasi merupakan proses verifikasi identitas pengguna. Autentikasi dilakukan dengan menggunakan sistem otentikasi bawaan yang mencakup pengguna(user) dan sesi(session).
-Otorisasi merupakan proses mengendalikan apa yang dapat diakses oleh pengguna yang terautentikasi. Otorisasi dapat mengatur hak akses dan izin pengguna terhadap sumber daya atau tindakan dalam aplikasi.
-Autentikasi penting untuk memastikan bahwa setiap pengguna yang masuk merupakan pengguna yang sah dan otorisasi penting untuk memastikan pengguna yang sudah diautentikasi memiliki akses yang dibatasi.

3)Apa itu cookies dalam konteks aplikasi web, dan bagaimana Django menggunakan cookies untuk mengelola data sesi pengguna?
-Cookies adalah data yang disimpan pada sisi klien(pengguna) dan digunakan oleh server web untuk mengidentifikasi dan melacak informasi tertentu terkait sesi atau pengguna pada aplikasi web
-berikut cara django menggunakan cookies
   *memulai sesi pengguna
	ketika pengguna mengakses situs web django, server akan membuat sesi pengguna yang unik. Sesi pengguna ini digunakan untuk menyimpan data sesi
   *menyimpan data dalam cookie
	Django akan menyimpan data sesi pengguna dalam cookie dengan cara yang aman
   *mengambil data sesuai keperluan
	ketika pengguna membuat permintaan ke server, Django akan mengambil data sesi yang sesuai dari cookie dan membuatnya tersedia untuk pengolahan dalam kode aplikasi
   *menyimpan perubahan ke cookie
	Jika data sesi pengguna berubah selama sesi, Django akan mengganti cookie sesi dengan yang baru, jika diperlukan, untuk mencerminkan perubahan tersebut.
   *mengakhiri sesi pengguna
	Saat sesi pengguna berakhir, cookie sesi akan dihapus atau diabaikan, dan data sesi tidak lagi tersedia.

4)Apakah pengguna cookies aman secara default dalam pengembangan web, atau apakah ada risiko potensial yang harus diwaspadai?
terdapat beberapa hal yang harus diwaspadai:
   -Penyalahgunaan cookies
	cookies dapat digunakan untuk berbagai kemungkinan, seperti untuk menampilkan yang sesuai dengan preferensi pengguna dengan tujuan pengguna mengklik iklan
   -Pencurian cookies
	penyerang yang berhasil mencuri cookies pengguna dapat melakukan aksi atas nama pengguna yang sah

5)Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step
*Mengimplementasikan fungsi registrasi, login, dan logout untuk memungkinkan pengguna mengakses aplikasi dengan lancar
   -import redirect, UserCreationForm, messages pada views di dalam direktori main
   -buat fungsi untuk registrasi
   -buat template registrasi pada direktori main/template
   -tambahkan fungsi dan path register pada urls
   -import authenticate dan login di views pada direktori main
   -buat fungsi login
   -buat template login pada direktori main/template
   -tambahkan fungsi dan path login pada urls
   -import logout pada views
   -buat fungsi logout
   -tambahkan button logout pada template main
   -tambahkan fungsi dan path logout pada urls
   -import login_required pada views
   -tambahkan @login_required

*Membuat dua akun pengguna dengan masing-masing tiga dummy data menggunakan model yang telah dibuat pada aplikasi sebelumnya untuk setiap akun di lokal
   -buka cmd
   -arahkan pada direktori project dan nyalakan environment
   -jalankan program dengan python manage.py runserver
   -lakukan registrasi untuk dua akun
   -tambahkan pada setiap akun masing-masing tiga data

*Menghubungkan model item dengan user
   -import User pada models di dalam direktori main
   -tambahkan user = models.ForeignKey pada fungsi item
   -tambahkan item.user pada fungsi create_item di dalam views
   -filter item pada show_main
   -lakukan migrasi model

*Menampilkan detail informasi pengguna yang sedang logged in seperti username dan menerapkan cookies seperti last login pada halaman utama aplikasi
   -import datetime pada views 
   -tambahkan response.set_cookie pada fungsi login_user 
   -tambahkan last_login pada fungsi show_main
   -tambahkan response.delete_cookie('last_login;) pada fungsi logout
   -tambahkan last login pada template main



Tugas 5

1)Jelaskan manfaat setiap element selector dan kapan waktu yang tepat untuk menggunakannya
*Container
   -container merupakan kelas yang digunakan untuk membuat wadah utama dalam desain responsif. Biasa digunakan saat ingin mengatur konten utama di tengah halaman dan mengendalikan lebar content
*container-fluid
   -merupakan kelas yang digunakan untuk membuat wadah utama cocok untuk desain web full-width. Biasa digunakan saat ingin konten ingin mengisi seluruh lebar layar
*row
   -merupakan kelas yang digunakan untuk membuat baris di dalam wadah. Digunakan ketika ingin mengelompokkan elemen ke dalam baris
*col
   -merupakan kelas yang digunakan untuk membuat kolom dalam baris. Digunakan ketika ingin mengatur tata letak kolom
*btn
   -merupakan kelas yang digunakan untuk membuat tombol. Biasa digunakan untuk membuat tombol yang responsif dan konsisten dengan desain
*navbar
   -merupakan kelas yang digunakan untuk membuat menu navigasi. Biasa digunakan saat ingin menambahkan menu navigasi ke situs web
*form-control
   -merupakan kelas yang digunakan untuk mengubah elemen input seperti teks. Biasa digunakan saat ingin merancang formulir input yang seragam dan mudah diidentifikasi

2)jelaskan HTML5 Tag yang kamu ketahui
-<header> digunakan untuk mendefinisikan bagian atas dari sebuah dokumen HTML
-<nav> digunakan untuk mengelompokkan elemen untuk navigasi
-<video> digunakan untuk menyisipkan video di page web
-<audio> digunakan untuk menyisipkan audio di page web
-<footer> digunkan untuk mendefinisikan bagian bawah dari sebuah dokumen atau elemen tertentu

3)jelaskan perbedaan margin dan padding 
*Margin
   -margin mengatur ruang di luar elemen
   -margin tidak mempengaruhi tampilan atau tata letak elemen
   -margin elemen dapat mempengaruhi elemen-elemen lain disekitar dengan cara mengatur jarak
   -margin digunakan untuk mengendalikan jarak antara elemen-elemen di luar elemen tersebut

*Padding
   -padding mengatur ruang di dalam elemen
   -padding mempengaruhi tampilan elemen itu sendiri
   -padding tidak mempengaruhi elemen-elemen di luar elemen itu sendiri
   -padding digunakan untuk mengendalikan ruang di dalam elemen

4)Jelaskan perbedaan antara framework CSS tailwind dan bootstrap. Kapan sebaiknya menggunakan Bootstrap daripada Tailwind, dan sebaliknya?
-Bootstrap memiliki komponen siap pakai, gaya desain yang konsisten, kustomisasi, dan dokumentasi yang kuat
-Tailwind memiliki Utility-First Approach, ringan, kustomisasi total, dan dokumentasi yang baik
-Bootstrap lebih cocok digunakan ketika ingin meluncurkan situs dengan cepat dan tidak ingin menghabiskan banyak waktu untuk desain kustom, sementara tailwind lebih cocok digunakan ketika ingin memiliki kontrol lebih besar pada desain dan tidak ingin dibatasi oleh gaya default framework

5)
*Kustomisasi halaman login, register, dan tambah inventori semenarik mungkin
   -tambahkan Bootstrap CSS dan juga JS
   -tambahkan navbar pada base.html dan sesuai navbar sesui keinginan
   -kustomisasi halaman login,register sesuai keinginan
   -kustomisasi inventori sesuai keinginan

*kustomisasi halaman daftar inventori menjadi lebih berwarna maupun menggunakan approach lain seperti menggunakan card
   -tambahkan div class container mt-5 untuk membuat tulisan pada lebih ke tengah
   -berikan row dan colom pada Name dan Class
   -Tambahkan border pada table
   -berikan warna pada button dan text