# Writing Week 3
## **JavaScript Intermediate**
### **Array**
- **Array** merupakan pengorganisasian data dan tempat penyimpanan data 
- Array adalah tipe data list order yang dapat menyimpan tipe data apapun dialamnya seperti string, number, boolean dan lainnya
- contoh Array 
``` 
    Let randomData = ['ini string', 20, true];
    console.log(randomData);
```
- Membuat Array : Array didefinisikan dengan square brackets []
- Mengakses Array : Array pada javascript dihitung mulai dari index ke- 0 
- Const in Array
  - Apabila menggunakan let, array dapat diubah dengan nilai yang baru
  - Const tidak dapat melakukan update data. Namun dapat melakukan update konten nilai di dalam array
  - Tidak dapat mengubah array dengan array baru jika menggunakan const
 - contoh penggunaan const 
 ``` 
    const orang = ['rehan', 'rizky', 'jamal'];
    orang[2] = ['saipul'];

    console.log(orang)// output : ['rehan','rizky','saipul']
```
- **Array Properti**. Array memiliki 5 properti yang sering digunakan yaitu :
  - constructor
  - length
  - index 
  - input
  - prototype
- .length yaitu mengembalikan nilai dari jumlah panjang data suatu array
    ``` 
    let orang = ['rehan', 'rizky', 'jamal'];
    console.log(orang.length) // output 3
    ```
- **Array Method**  atau biasa disebut dengan built in methods 

### **Multidimensional Array**
   > Multidimensional array bisa dianalogikan sebagai array of array
- Multidimensional array sama seperti matriks yaitu memiliki 2 dimensi (x,y)

### **JavaScript Object**
- Object adalah benda mati maupun benda hidup adalah object.
Pada programming object adalah sebuah tipe data pada variabel yg menyimpan properti dan fungsi (method)
- Properti adalah data lengkap dari sebuah object
- Method adalah action dari sebuah object. 
- Saat pemanggilan properti object dapat menggunakan bracket notation
- Update object 
  - Object dapat mengupdate value dari key yang sudah tersedia
  - Object dapat menambah key dan value baru
 
- Method : jika value yang dimasukkan pada properti berupa function 
- console adalah global javascript object dan log adalah properti yang berupa function dari object console
- Nested Object
- Pass by reference : mengubah data pada object melalui function dan memasukkan object sebagai parameter function
- Looping pada object
- Array of object

### **JavaScript Recursive**
- Recursive adalah fungsi yang memanggil dirinya sendiri sampai suatu kondisi tertentu terpenuhi
- A new paradigm :
  - Procedural
  - Conditional
  - Looping
  - Modular (function)
  - Recursive
- Ciri dari recursive:
  - Fungsi recursive memiliki kondisi yang menyatakan kapan fungsi tersebut berhenti. 
  - fungsi recursive selalu memaanggil dirinya sendiri sambil mengurangi atau memecahkan data masukan setiap panggilannya.
  
### **JavaScript REGEX**
- **Regex** adalah susunan karakter/karakter spesial yang menggambarkan pattern/pola untuk pencarian text pada sebuah string atau document
   > REGEX = Text Matching
- Contoh penggunaan Regex :
  - Validasi input dari sebuah form
  - Mencari keyword tertentu pada email atau halaman web
  - Mencari IP adress dalam kisaran tertentu
- Membuat Pola Regex
  - Literals adalah konsep regex adalah konsep yang paling sederhana yaitu dengan membuat regex sesuai dengan text yang ingin dicari
- Built in Method Regex
  - test() yaitu built in method untuk regex yang mengembalikan nilai Boolean untuk kecocokan sebuah nilai yang dicari
    ``` 
    let regex1 = new RegExp('Cat');
    console.log(regex1.test('Cat'))// true
    ```
  - Karakter Set digunakan untuk mencari minimal 1 karakter yang sesuai. Karakter set menggunakan bracket square []
    ``` 
    let regex1 = new RegExp('[a-z]');
    console.log(regex1.test('abc'))// true
     ```
  - match() yaitu method yang mengembalikan nilai array dari karakter yang match
   - Flags pada javascript :
     - i : untuk menghandle case-sensitive. Tidak mempermasalhkan besar kecilnya karakter
     - g : untuk mencari kedalam seluruh string yang ingin dicari. Jika tidak menggunakan flags g maka sistem akan mengembalikan nilai array pertama yang ditemukan tanpa melanjutkan pencarian
- Karakter Set Short Syntax  
  - \d : seluruh number/digit character
  - \w : alphanumeric character
  - \s : whitespace character (space,tab,newline)
  - Negasi dari set short syntax yaitu menggunakan tanda ^
  - Quantifiers berfungsi untuk membuat format regex menjadi lebih rapi. 
  - Quantifiers ditandai dengan format {} 
  contoh saat mencari roa{3}r maka akan match dengan string 'roaaar'
  - Quantifiers besifat greedy akan mengambil nilai yang paling besar atau maksimal
  contoh saat mencari roa{3,5}r maka akan match dengan 'roaaar' dan 'roaaaaar' maka yang akan didapatkan adalah yang 'roaaaaar'
  - Anchor yaitu digunakan jika ingin mencari karakter yang sama persis. 
  - Anchor diawali dengan ^ dan diakhiri dengan $
  - Alternation yaitu digunakan untuk mencari karakter yang sama persis dengan lebih dari 1 kalimat
  - Alternation ditandai dengan format (|)
    ``` 
    let search = /^Belajar Tailwind CSSs$ |^ Tailwind CSS$/
    console.log(search.test{'Tailwind CSS'}); output : true
    ```

### **JavaScript OOP**
- **OOP** atau Object Oriented Programming adalah suatu paradigma dalam pemrograman 
- 4 Pilar dalam OOP :
  - Encapsulation adalah cara untuk membatasi akses langsung ke properti atau method dari sebuah objek
  - Inheritance adalah sebuah proses dimana sebuah kelas mewariskan properti dan method ke kelas lain atau childnya
  - Polymorpishm adalah kemampuan dari suatu objek untuk memiliki banyak bentuk
  - Abstraction adalah teknik untuk menyembunyikan detail tertentu dari sebuah object atau method dan hanya menampilkan fitur penting dari objek tersebut

### **JavaScript Modules**
- Modules memungkinkan untuk memecah kode menjadi file terpisah sehingga mempermudah untuk maintain code
- JavaScript Module bergantung pada pernyataan impor dan ekspor

### **WEB STORAGE**
- Web Storage adalah wadah untuk sebuah data yang digunakan untuk penyimpanan data yang terikat di browsernya
- Jenis Web Storage yang umum digunakan yaitu :
  - Local Storage
  - Session storage
  - IndexDB
  - Cookies
- Cara menyimpan data pada local storage 
    ```
        let token = "ini tolong simpan" //key
        localStorage.setItem("token", token);
    ```
- Cara mengambil token
    ```
        localstorage.getItem("token", token);
        console.log(localStorage.getItem('token");
    ```
- Cara menghapus data 
    ```
        localStorage.removeItem("token")
    ```
### **Asynchronous**
- Asynchronous sebuah teknik yang menyelesaikan fungsi secara paralel
- Penggunaan asynchronous dapat dilakukan jika kita ingin mengambil data dari database
- Mengapa perlu menggunakan asynchronous? Asynchronous dibutuhkan ketika ada proses yangg membutuhkan waktu lama. Jadi kita bisa mengerjakan proses yg lain secara paralel.
- Callbacks adalah suatu function namun cara pengeksekusiannya yang berbeda yaitu hanya mengeksekusi pada point tertentu.

- **Asynchronous - Promise** merupakan suatu object dan digunakan hanya untuk satu event dengan menyimpan hasil dari sebuah operasi asynchronous baik itu hasil yang diinginkan (resolved value) atau alasan kenapa operasi itu gagal (failure reason)
 
- **Asynchronous - Async-Await** merupakan fitur yang hadir sejak ES2017 bekerja dengan cara menunda eksekusi hingga proses asynchronous selesai
- **Asynchronous - Fetch** merupakan cara baru dalam melakukan network request yang memanfaatkan sebuah Promise dalam penggunaanya. Karen Fetch mengembalikan sebuah Promise maka respon handling yang digunakan adalah **then** jika promise mengembalikan resolve dan **catch** jika promise mengembalikan nilai reject.

    

