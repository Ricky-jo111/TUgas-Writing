# Minggu Ke 2

## JavaScript Scope 

> **Scope adalah konsep dalam flow data variabel. Terdapat dua jenis variabel scope yang ada di JavaScript yaitu Global Variable dan Local Variable.**

> **Local Scope adalah Variabel lokal hanya dapat diakses dari dalam fungsi tersebut.**

> **Global Scope Semua variabel yang dibuat di luar fungsi disebut variabel global JavaScript.**

## JavaScript Function

> **Sebuah Code Yang disatukan menjadi satu kelompok yang berfungsi untuk menyelesaikan suatu task**

deklarasi Function 

    function greeting(){
        console.log("hai Semua")
    }

Memanggil fungsi 

    greeting()
    Atau  
    console.log(greeting())

## Parameter dan Argumen

### Parameter Function

    Function Penambahan(a, b) {
        return a + b;
    }
### Argumen Function
    Function Penambahan(a, b) {
        return a + b;
    }
    console.log(Penambahan(5, 5)) // output 10 

Default Parameters
> __Default paramaters__ digunakan untuk memberikan nilai awal/default pada parameter function. Default parameters bisa digunakan jika kita ingin menjaga function agar tidak error saat dipanggil tanpa argumen

    Function biodata(name= 'stranger') {
        return 'Hello ' + name;
    }
    console.log(biodata('John')); //outputnya "Hello John" -->
    console.log(biodata()); //outputnya "Hello stranger"

# Data Type Built In prototype & Method

### **Tipe data dalam JavaScript**

#### Primitive

> - Numbers
> - String
> - Booleans
> - Undefined
> - Null

#### Non-Primitive 

> - Objects
> - Arrays
> - Functions

## HTML DOM 
Dom adalah suatu cara untuk memanipulasi element HTML 

Section Selecting elements

    getElementById() – select an element by id.

    getElementsByName() – select elements by name.

    getElementsByTagName()  – select elements by a tag name.

    getElementsByClassName() – select elements by one or more class names.

    querySelector()  – select elements by CSS selectors.

Manipulating elements HTML

Caranya
Mencari Element HTML
Mengubah Konten Element (Element.textContent dapat kita gunakan untuk
mengubah teks di dalam sebuah element
)
- Element.textContent
    
        .textContent = “<span>Teks Heading</span”

- Element.innerHTML

        .innerHTML = “<span>Teks Heading</span”


