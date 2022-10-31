# Minggu Ke 3 

## JavaScript Array
> Array merupakan struktur data yang digunakan untuk menyimpan sekumpulan data dalam satu tempat.

Cara Mendeklarasi Array : 

    let array = [
        "jeruk", 
        "semangka", 
        "pepaya",
        "rambutan"
    ]
> **cara menambah data di belakang**

    arrBuah.push("duku")

> **cara menambah data di depan**

    arrBuah.unshift("anggur")

> **cara menghapus data terakhir duku dan anggur**
    
    arrBuah.pop()

> **cara menghapus data pertama jeruk,semangka,pepaya dan rambutan**
    
    arrBuah.shift()

> cara menghapus, menyisipkan dan mengganti data 
    
    arrBuah.splice(2, 1) //menghapus data
    arrBuah.splice(2, 0, "buah naga") //menyisipkan data
    arrBuah.splice(2, 1, "buah naga") // mengganti data

## Looping array

> ### For Loop

    for(let i = arrBuah.length[-1] ; i > 0; i--){
        console.log(arBuah[i])
    }
> ### For of
    
    for(let buah of arrBuah){
        console.log(buah)
    }

> ### ForEach

    arrBuah.forEach((item) => {
        console.log(item)
    })

> ## map

    arrBuah.map((item, index) => {
        console.log(item)
    })
_notes_ : ForEach tidak mereturn nilai untuk map Dia mereturn Nilai


## Object

> **Sebuah tipe data pada variable yang menyimpan properti dan fungsi**

### Membuat objek 

    let ayam = {
        sayap : 2,
        kaki  : 2
        }
    }

### Cara mengakses object 

> 1. Dot notation

    console.log(ayam.sayap);
     
> 2. Bracket

    console.log(ayam["kaki"])

> 3. memamggil nama object dengan variabel

    let properti = "kaki";
    console.log(siswa[properti])

### Menambahkan Properti baru Ke dalam Objek

Menggunakan Dot Notation

    ayam.bulu = "hitam"

Menggunakan bracket 

    ayam["bulu"] = "hitam"

### Mengganti nilai dari properti 

Menggunakan Dot Notation

    ayam.sayap = 50

Menggunakan Bracket

    ayam["sayap"] = 50

### Mendelete sebuah properti 

    delete ayam.bulu

### Objek Method 

    let mobil = {
      Maju : function(){
        return "jalan"
      },
      stop : function(){
        return "berhenti"
      }
    }

## Built In Method

#### Contoh objek 
    
    let siswa = {
        nama : "dila",
        umur : 17,
        hobi : "membaca",
    };
    
#### method 

    console.log(object.keys(siswa)) // merubah object menjadi array diambil dari key properti. 

    console.log(object.values(siswa)) // merubah object menjadi array diambil dari value properti. 

## Nested Object 

keadaan dimana suatu object menyimpan object lain didalamnya

    let buku = {
        judul   : "tips masak-masakan Bali",
        tahun   : 2022,
        penulis : {
            penulis1 : {
                nama : "Bu made",
                umur : 35,
                kota : "bali"
            }
            penulis2 : {
                nama : "Wayan Ketot"
                umur : 40,
                kota : "bali"
            }

        }
    }

## Loop Object


### melooping semua properti di dalam sebuah object

    
    // For IN 

        for (x in siswa){
            console.log(x)
        }

untuk nested Object

        let buku = {
                judul   : "tips masak-masakan Bali",
                tahun   : 2022,
                penulis : {
                    penulis1 : {
                        nama : "Bu made",
                        umur : 35,
                        kota : "bali"
                    },
                    penulis2 : {
                        nama : "Wayan Ketot",
                        umur : 40,
                        kota : "bali"
                    }
                }
            }
        for (x in buku.penulis){
                console.log(buku.penulis[x])
            }
    

## Array Of Object

metode untuk menyimpan banyak tipe data dalam satu variable

    let users = [
        {
            nama   : "dila",
            alamat : "bandung",
            umur   : 17
        },
        {
            nama   : "audzan",
            alamat : "jakarta",
            umur   : 18
        },
        {
            nama   : "dolton",
            alamat : "bandung",
            umur   : 17
        },
    ];

    // Looping pada Array Of object

    let data = users.map((el) => {
        console.log(el.nama);
    })

    // Menambah properti baru 
    
        users[0].status = "aktif"

    atau jika ingin semua index ditambahkan properti yang baru

        let data = users.map((el) => {
            el.status = "aktif"
                return el
        })

## Recursive 

> Recursive adalah function yang memanggil dirinya sendiri sampai kondisi tertentu. Recursive kebanyakan digunakan untuk case matematika, fisika, kimia, dan yang berhubungan dengan calculation.

Ciri dari rekursif:

- Fungsi rekursif selalu memiliki kondisi yang menyatakan kapan fungsi tersebut berhenti. Kondisi ini harus dapat dibuktikan akan tercapai, karena jika tidak tercapai maka kita tidak dapat membuktikan bahwa fungsi akan berhenti, yang berarti algoritma kita tidak benar.
- Fungsi rekursif selalu memanggil dirinya sendiri sambil mengurangi atau memecahkan data masukan setiap panggilannya. karena tujuan utama dari rekursif ialah memecahkan masalah dengan mengurangi masalah tersebut menjadi masalah-masalah kecil.


    Sintaks untuk fungsi rekursif adalah:

    function recurse() {
        // function code
        recurse();
        // function code
    }
 

## Asynchronous 
 
 Synchronous adalah teknik pengerjaannya dilakukan secara rutut atau step bay step. sedangkan Asynchronous adalah teknil mengerjakannya secara pararel yaitu mengerjakan kegiatan 1 dan yang lain berbarengan dengan tujuan yang sama. 

### Asynchronous - Promise
    // 1 Promise Chains

    const returnsAPromise = function (string) {
    return new Promise((resolve, reject) => {
        if (typeof string === "string") {
        resolve(`${string} is a resolved promise now`);
        } else {
        reject("Not a string!");
        }
    });
    };

    returnsAPromise("1").then((item) => {
    console.log(item);
    });

### Asynchronous - Async Await

    // 2 Async/Await

    // Synchronous

    const sayHello = (num, word) => {
    console.log(`Customer no.${num} says ${word}`);
    };

    sayHello(1, "Hi");
    sayHello(2, "Hello");

    // Async/Await
    const sayAsyncHello = async (num, word) => {
    await setTimeout(() => {
        console.log(`Customer no.${num} says ${word}`);
    }, 2000);
    };

    sayAsyncHello(3, "Yo");
    sayHello(4, "Yep");
    sayHello(5, "Never better");

## Web Storage 
Memahami localStorage vs sessionStorage
> __localStorage dan sessionStorage__ hampir identik dan memiliki API yang sama. Perbedaannya adalah bahwa dengan __sessionStorage__, data hanya bertahan sampai jendela atau tab ditutup. sedangkan __localStorage__, data dipertahankan hingga pengguna secara manual menghapus cache browser atau hingga aplikasi web Anda menghapus data. 

Jenis Web Storage
- Localstorage, session, IndexDB, Cookies, Trust Token, Web SQL
- Umumnya diguanakan FE : Local, Session, IndexDB
- Yang perlu di komunikasikan oleh BE : Cookies