# Minggu Pertama 

## Unix Command Line ( CLI ) 

> **Unix Command Line. Sebuah terminal atau shell atau juga program yang digunakan untuk menjalankan perintah atau command yang diinputkan oleh user sehingga sistem dapat menjalankan nya.** 

> **Shell. adalah program yang digunakan untuk berkomunikasi atau memerintah sistem**

Berikut ini Adalah Command dalam Gitbash : 

> - __ls__ Menampilkan daftar file dan folder
> - __ls -a__ Menampilkan Folder yang tersembunyi
> - __cd__ Perintah untuk berpindah folder 

        contoh : cd nama-folder atau cd "nama folder"

> - __cd..__ perintah untuk berpindah ke directory sebelumnya
> - __pwd__ perintah untuk menunjukan di directory mana kita berada 
> - __touch__ perintah untuk membuat suatu file

        contoh : touch readme.md

> - __Cp__ untuk mengcopy file

        contoh : Cp a.txt b.txt atau a.txt\nama_folder (untuk mengcopy ke folder yang lain nya)

> - __Cp -r__ mengcopy folder beserta isinya 

        contoh : Cp -r nama Folder

> - __mkdir__ perintah untuk membuat sebuah directory atau folder baru 
> - __rm -r__ perintah untuk menghapus sebuh directory atau folder
> - __rm__ perintah untuk menghapus sebuah file

## Git & GitHub Dasar

> **Git adalah Sebuah tools yang digunakan untuk melacak setiap perubahan file/folder pada suatu project.**

> **Github adalah sebuah perusahaan penyedia layanan hosting, manajemen project, dan sistem versioning code**

> ### Cara Konfigurasi Git 
    
       git  config --global user.name "Ricky jonathan"
       git- config --global user.email "Rickyjo@gmail.com"

> ### Mengecek konfigurasi berhasil atau tidak 
        git config --list
  
> ### Membuat Repository 
_Notes :_
buat didalam foler yang akan di push ke repo git
>   #### 1. Git Init
            
        git init     

>   #### 2. Git Status ( mengecek status git kita apakah ada perubahan atau tidak.  )

        git Status

>   #### 3. Git add .  ( untuk menambahkan semua file dalam folder  )

        git add . 

>   #### 4. Git commit ( menambahkan pesan atas perubahan yang terjadi dalam file atau folder )

        git commit -m "Commit Pertama"

>   #### 5. Git push -u origin master (untuk mengirimkan file dari komputer ke repo git)

        git push -u origin master


# HTML

- HTML adalah kerangka untuk membuat halaman web. 
    ibarat tubuh manusia HTML ini adalah tulang dalam tubuh kita yang menjadi kerangka bagaimana bentuk tubuh kita.

- Kerangka HTML 

        <html>
        <head>
        <title>
            Judul dari website
        </title>
        <body>
            isi dari website anda
        </body>
        </html>
- Tag Html
    
        1. <a>
        2. <p>
        3. <h1>,<h2>, - <h6>
        4. <title>
        5. <ul> & <ol>
        6. <img>
        7. <video>

- Attribute HTML
        
        1. id
        2. class
        3. Href
        4. src
        5. div


# CSS

> **Css dalah bahasa yang digunakan untuk mendesain, mempercantik, memberikan warna atau baju,memposisikan text terhadap halaman website.**

3 cara menggunakan CSS
-    Inline Styles => menyematkan code csspada elemen apapun di dalam body HTML dengan menggunakan atribut _style_.
    <P style="color: red">Masuk</button>
-    Internal Styles => CSS yang diletakkan pada bagian head suatu halaman HTML
    <head>
    <styles> isi dengan Content seperti padding,margin,bacground,color ataupun font</styles>
    </head>

-    Eksternal Styles => Membuat file tersendiri yang berekstensi dengan css. eksternal css dapat digunakan lebih dari 1 kali. Kemudian file tersebut di hubungkan ke dalam halaman HTML menggunakan tag _link_. 

            contoh Eksternal styles
            <link href="styles.css" type="text/css" rel="stylesheet"/>
            contoh Eksternal dari alamat website
            <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css"type="text/css" rel="stylesheet"/>

Cara Menggunakan CSS


1.   Background-Color
            
            body { 
                background-color: red;
            }
2.   font- size

            h1 {
                font- size : 6 px;
            }

3.   font-color
    
            p {
                color:red;
            }
4.   Nested Element

            .div{
                display: flex;
            }

## Algoritma & Pseudocode
> __Algoritma__ adalah deskripsi berupa step-step yang dibutuhkan untuk menyelesaikan suatu masalah. Kualitas dari Algoritma antara lain:
- Input dan output harus didefinisikan terlebih dahulu dengan tepat
- Setiap step harus benar-benar clear dan tidak ambigu
- Algoritma seharusnya tidak mengandung suatu code pada bahasa pemograman tertentu. Algoritma harus dibuat agar dapat digunakan dalam bahasa pemograman apapun.
### Contoh algoritma Sederhana
Kondisi Hujan
1. Apakah hujan?
2. Jika tidak hujan, kamu tidak perlu bawa payung
3. Jika hujan, segera cari payung
4. Ketika payung sudah ketemu, bawa payungnya
5. Jika payung tidak ketemu pastikan apakah masih hujan dan akan kembali berputar ke poin 2 dan 3 

# Java Script

## Apa itu JavaScript ?

>   **Javascript adalah bahasa pemograman yang sangat powerful yang digunakan untuk logic pada sebuah website dan juga bisa membuat website menjadi lebih interaktif**

## Syntax dan Statement JS
Syntax dapat dianalogikan layaknya kamus dan grammar pada bahasa pemrograman
> - __Alert()__
> - __prompt()__
> - __Confirm()__

# Console.log()
> **Console.log() adalah suatu method output yang mengirimkan pesan ke console web. sering digunakan dalam dalam pengerjaan project dan untuk error handling.** 

# Tipe Data Dalam JS
> - __Number__
> - __String__
> - __boolean__
> - __Null__
> - __Undefined__
> - __object__

# Variabel 
dapat diartikan Variabel ini ibarat sebuah Container yang menjadi wadah atau tempat menyimpan sebuah data atau nilai.

cara mendklarasikan Variabel di JS :
> - __Var__
> - __Let__
> - __const__

_NOTES_ : 
dikarenakan let mendukung kaidah global dan local variabel jadi dianjurkan untuk menggunakan let dibandingkan var untuk suatu variabel yang dapat dirubah


# operator 

- Assignment Operator (=) digunakan untuk menyimpan sebuah nilai pada variabel.

        let nama = "Ricky"

- Increment dan Decrement
Gunakan increment atau decrement untuk menambah atau mengurangi sebesar 1 nilai.

        let a = 10;
        a++; 
        console.log(a) // output 11

        let a = 10;
        a--; 
        console.log(a) // output 9

- Arithmetic Operator
adalah operator yang melibatkan operasi matematika.
    >   - Tambah (+)
    >   - Kurang (-)
    >   - Perkalian (*)
    >   - Pembagian (/)
    >   - Modulus (%) adalah sisa bagi 
            
## __Comparition Operator__ 
Operator yang membandingkan satu nilai dengan nilai lainnya dan Hasil operasi yang melibatkan comparison operator adalah antara true or false.
Simbol comparison operator
- Lebih kecil dari : <
- Lebih besar dari: >
- Lebih kecil atau sama dengan: <=
- Lebih besar atau sama dengan: >=
- Sama dengan: ===
- Tidak sama dengan: !==

## Logical Operator
>__Logical operator__ biasa digunakan untuk sebuah CONDITIONAL pada pemograman.Menghasilkan nilai BOOLEAN yaitu TRUE or FALSE
Simbol dari Logical Operator adalah sebagai berikut:
- AND operator : && => AND akan menghasilkan nilai true jika kedua atau semua premis bernilai TRUE. sebaliknya apabila ada false dan true akan menghasilkan false
- OR operator: || => OR akan menghasilkan nilai true jika salah satu premis mengandung nilai TRUE
- NOT operator: ! => NOT akan membalikkan sebuah nilai BOOLEAN. TRUE menjadi FALSE dan sebaliknya.



- ## JavaScript    Conditional 

    Merupakan Statement Percabangan yang menggambarkan suatu Kondisi Conditional statement akan mengecek kondisi spesifik dan menjalankan perintah berdasarkan kondisi tersebut dimana mereka mengecek apakah kondisi tersebut atau false. jika true maka code didalam akan dijalankan.

    Contoh Conditional 
    > - IF Statement
                
        let lapar = "iya";
        if (lapar == 'iya'){
	        console.log("makan")    
        }
        output : makan

    > - IF Else

        let lapar = "tidak";
        if (lapar == 'iya'){
	        console.log("makan")
         else {
                console.log("tidur")
        }
        output : tidur

    > - IF Else IF 
    > - Truthy And Falsy
    > - Switch Case 
    > - Ternary Operator

## JavaScript - LOOPING

> __Looping__ adalah statement yang mengulang sebuah instruksi hingga kondisi terpenuhi atau jika kondisi stop/berhenti tercapai.
- Manual Looping
-    __FOR LOOP__ => merupakan instruksi pengulangan yang dapat kita berikan pada program yang kita kembangkan.Gunakan FOR LOOP jika kita tahu seberapa banyak nilai pasti untuk pengulangannya

    Contoh :
    /* Perulangan */

    // For
    let n = 100
    for(let i=0 ; i < n+1; i++ ){
        console.log(i)
-    __WHILE LOOP__ akan menjalankan instruksi pengulangan kondisi bernilai TRUE.Gunakan WHILE LOOP jika kita tidak mengetahui jumlah pasti pengulangan.

    Contoh :
	    let angka = 1
	    while (angka <= 10){
		console.log(angka); 
        angka++;
	    }
-    __DO WHILE__ ingin menjalankan pengulangan 1 kali sebelum dilakukan pengecekan kondisi

    Contoh :
		m = 1
		do {
		   console.log("hello")
		   m++
		}while(m<=4)


