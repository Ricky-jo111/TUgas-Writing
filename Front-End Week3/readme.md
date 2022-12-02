# Week 3

## React Context 

>Context menyediakan cara untuk oper data melalui diagram komponen tanpa harus oper props secara manual di setiap tingkat.

>Dalam aplikasi React yang khusus, data dioper dari atas ke bawah (parent ke child) melalui props, tetapi ini bisa menjadi rumit untuk tipe props tertentu (mis. preferensi locale, tema UI) yang dibutuhkan oleh banyak komponen di dalam sebuah aplikasi. Context menyediakan cara untuk berbagi nilai seperti ini di antara komponen tanpa harus oper prop secara explisit melalui setiap tingkatan diagram.


## React testing 

> Proses memverifikasi bahwa test assertions kita benar dan bahwa mereka tetap benar sepanjang masa aplikasi. Test assertion ini adalah ekspresi boolean yang mengembalikan nilai true kecuali ada bug di kode Anda.

### Unit Testing
> Pengujian unit adalah suatu proses menguji setiap bagian kode untuk memverifikasi bahwa mereka berfungsi secara independen seperti yang diharapkan. Karena arsitektur komponen React, tes unit adalah fit alami. Mereka juga lebih cepat karena Anda tidak harus bergantung pada browser.

### Pengujian Fungsional
> Tes fungsional yang digunakan untuk menguji perilaku bagian dari aplikasi Tes fungsional biasanya ditulis dari perspektif pengguna. Suatu fungsi biasanya tidak terbatas pada komponen tunggal. Ini bisa menjadi bentuk penuh atau seluruh halaman.

### Pengujian Integrasi
> Pengujian integrasi adalah strategi pengujian di mana semua komponen individu diuji sebagai kelompok. Pengujian terintegrasi mencoba untuk mereplikasi pengalaman pengguna dengan menjalankan tes pada browser yang sebenarnya. Ini jauh lebih lambat daripada pengujian fungsional dan tes unit karena setiap rangkaian pengujian dijalankan pada browser langsung.