# Minggu Ke 4

## Asynchronous Wait & Fetch

> terdapat 3 fitur yang selalu dipakai ketika menggunakan JavaScript. kita perlu menjalankan eksekusi kode secara “asinkronus” ke dalam “event loop” dari proses utama JavaScript itu sendiri yaitu :

Mendeklarasi Promise

    Function GetUser(id) {
    return new Promise ((resolve, reject) => {
        if (id !== "" && id !== underfined) {
            resolve (id) ;
        } else {
            reject ("ID Harus Di Isi");
        }
    });
}

Penggunaan nya 

    GetUser ()
    .then ((response) => {
        console.log(response);
    })
    .catch ((error) =>{
        console.log(error);
    });

    
## Fetch Data

> Fetch Data merupakan fungsi atau alat kominikasi HTTP yang bertujuan untuk mengembalikan dan mengirim data pada suatu server.       

        fetch("https://api.themoviedb.org/3/discover/movie?api_key=6585f85a6001577a80630a9fc6d49114")
        .then(result => result.json()
        ).then(data => {
            showMovies(data.results);
        })

## **Git dan Github Lanjutan**

- Dengan menggunakan github kita dapat bekerja secara berkolaborasi, biasanya dalam pembuatan sebuah website yang melibatkan beberapa orang per-orang akan mengerjakan satu fitur dengan branch masing-masing yang nantinya akan di combine di main branch

- Github sendiri dapat memudahkan kita dalam berkolaborasi dengan memantau semua perubahan yang ada

- Di Github dapat menggunakan akun github organisasi, agar dapat bekerja berkolaborasi

- Repository nantinya dapat dibuat beberapa cabang (branch) untuk memisahkan satu pekerjaan dan pekerjaan lainnya

- Biasanya dalam berkolaborasi akan ada branch utama ( Main Branch ), digunakan hanya untuk perubahan yang telah fixed ( tahap production, sudah di publish )

- Lalu dibuat branch ke 2 (secondary branch ) yaitu branch development, dari branch dev nanti akan bercabang ke branch sesuai dengan pekerjaan masing2 jadi tiap individu memiliki branch masing2. Digunakan untuk menampung branch2 yang ada

- Pull Request, digunakan untuk menggabung branch individu ke branch dev

- Merge, dimana permintaan pull request sudah disetujui oleh team leader ( Menggabungkan )

- Setiap Push perubahan pastikan untuk selalu pull request ke branch diatasnya agar perubahan masuk ke branch development.

- Conflict, terjadi karena adanya 2 orang yang memanipulasi branch yang sama

- Cara menangani conflict bisa dengan merge terlebih dahulu perubahan terbaru, lalu memilih perubahan yang diinginkan.

## Responsive Web Desain

> Responsive Web Design (RWD) ini bertujuan untuk membuat desain websitekita dapat diakses dalam device apapun. Device yang umumnya digunakan adalah lapto/pc, smartphone, dan tablet.
### Tambahkan tampilan di HTML. Pada html terdapat meta viewport yang diperlukan pada responsive seluler

    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>

    </body>
    </html>

### Media Query

> Jenis Media Query untuk responsive web design umumnya hanya menggunakan 2 jenis media query yaitu **main-width** dan **mas-width**.
    Contoh:

    @media screnn and (min-width: your pixel){

    }
    @media screnn and (max-width: your pixel){

    }

> media query digunakan untuk membuat beberapa styles tergantung pada jenis device. terdapat 2 cara dalam menggunakan media query

## Boostrep 5

> Bootstrap adalah framework HTML, CSS, dan JavaScript yang berfungsi untuk mendesain website responsive dengan cepat dan mudah.

> Kemudahan yang ditawarkan oleh Bootstrap adalah Anda tak perlu coding komponen website dari nol. Framework ini tersusun dari kumpulan file CSS dan JavaScript berbentuk class yang tinggal pakai.

> Class yang disediakan Bootstrap juga cukup lengkap. Mulai dari class untuk layout halaman, class menu navigasi, class animasi, dan masih banyak lainnya.