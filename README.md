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
