# Week 2 FE

### PropTypes 

> PropTypes merupakan sebuah library untuk mengatur/meminimalisir data yang diterima ke suatu komponen dan memastikan type data yang masuk pada suatu komponen. Jika tidak sesuai, maka akan muncul pesan error. PropTypes merupakan library untuk menvalidasi props. Ini sangat membantu dalam meminimalkan bugs saat mengembangkan App besar. Jika props tidak benar type nya maka akan muncul warning.
	
	
### Router 

 > Routing adalah proses di mana pengguna diarahkan ke halaman yang berbeda berdasarkan tindakan atau permintaan mereka. Router ReactJS terutama digunakan untuk mengembangkan Aplikasi Web Halaman Tunggal. 
 
 > React Router digunakan untuk menentukan beberapa rute dalam aplikasi. React Router adalah sistem perpustakaan standar yang dibangun di atas React dan digunakan untuk membuat perutean di aplikasi React menggunakan Paket React Router.  
 
 > Tanpa React Router, tidak mungkin menampilkan banyak tampilan di aplikasi React. Sebagian besar situs media sosial seperti Facebook, Instagram menggunakan React Router untuk menampilkan banyak tampilan.

 Untuk menambahkan React Router ke proyek yang sudah ada, hal pertama yang harus Anda lakukan adalah menginstal dependensi yang diperlukan dengan alat pilihan antara lain: 
 NPM : 
 
    $ npm install react-router-dom@6

### State Management (REDUX)
 > Redux adalah state container untuk aplikasi JavaScript. Mengatur hubungan antara state dengan component pada React dapat dilakukan dengan hanya menggunakan state dan props. > 
 
 > Tetapi pada aplikasi yang memilliki banyak sekali component mengelola state bisa menjadi sedikit rumit. Semua modifikasi state juga dilakukan melalui Redux, store pada Redux menjadi satu-satunya tempat untuk mengelola state(single source of truth).
 >Aplikasi menjadi lebih konsisten dan mudah untuk ditest.ada beberapa konsep penting yang harus ada di dalam redux

 1. Reducers 
    
    > menentukan bagaimana status aplikasi berubah sebagai respons terhadap tindakan yang dikirim ke store.

 2. Action 

    > Action sendiri merupakan objek JavaScript biasa dan harus memiliki tipe properti (property type) untuk menunjukan jenis action yang akan dilakukan. Selain itu, Action harus memiliki muatan yang berisi informasi yang harus dikerjakan oleh action tersebut. Action pun dibuat melakui Action Creator

 3. Store
    
    > Store berfungsi untuk menyimpan status aplikasi. Sangat disarankan untuk hanya menyimpan satu store di aplikasi Redux apa pun. Anda dapat mengakses status yang disimpan, mengupdate status, dan mendaftarkan atau membatalkan pendaftaran listener melalui metode helper.