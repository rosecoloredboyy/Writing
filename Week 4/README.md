# Writing
### **Asycnhronous**
Kode yang dituliskan secara asynchronous akan dieksekusi di belakang thread utama atau biasa disebut main thread. Hal tersebut tidak akan membloking proses runtime atau menunggu hingga proses selesai dilakukan. Sembari menunggu proses tersebut selesai, compiler akan mengeksekusi perintah kode selanjutnya.
- Promise 
  Secara sederhana Promise merupakan sebuah janji. Logika cara kerja Promise sama seperti selayaknya kamu membuat janji dengan seseorang. Contohnya kamu membuat janji   dengan temanmu untuk belajar bersama. Terdapat beberapa kemungkinan yang terjadi kepada janji yang kamu buat dengan temanmu tadi yaitu kamu belum memenuhi janjimu,     kamu sudah memenuhi janjimu, atau kamu tidak memenuhi janji bekerja kelompokmu.

  Layaknya kamu membuat janji, terdapat tiga kemungkinan state yang dapat terjadi di dalam Promise, antara lain:
  - Pending : Dalam keadaan awal, tidak terpenuhi atau tidak ditolak
  - Fulfilled : Artinya terpenuhi atau sukses
  - Rejected : Artinya tidak terpenuhi atau gagal
 
- Fetch
  Fetch API pada javascript adalah kegiatan untuk meminta/request layanan ke endpoint/letak url yang akan menerima request pada website secara local maupun public,       untuk mengambil response resource / sumber daya berupa data berformat json atau text yang biasa dilakukan programmer untuk membangun website yang membutuhkan data     dari website lain ataupun website yang membutuhkan konsep microservice didalamnya.
- HTTP Request yaitu berfungsi sebagai alat komunikasi frontend dengan backend
- HTTP Request Method
  - GET untuk mengambil data 
  - HEAD untuk mengambil informasi tentang URL dari Web Server
  - POST untuk mengirimkan data
  - PUT untuk mengirimkan atau memperbaharui data
  - DELETE untuk menghapus data
 
 ### **Responsive Web Design**

- **Responsive Web Desin** yaitu suatu tampilan website yang dapat menyesuikan dengan perangkat yang digunakan
- Chrome Dev Tools merupakan tools pada google chrome yang digunakan sebagai tools Responsive Web Design
- Untuk mengakses Chrome Dev Tools yaitu 
  > ctrl + shift + j
  > ctrl + shift + m digunakan untuk melihat toggle bar 
- Dalam menggunakan Responsive Web Design pada bagian HTML perlu ditambahkan **viewport** pada bagian head agar tampilan website dapat menyesuaikan dengan berbagai device
- **Media Query** salah satu cara untuk mengatur suatu website agar bisa terdiri dari beberapa jenis 
- Penggunaan media query yang umum digunakan adalah min-width dan max-width
- Contoh penerapan media query 
  `` @media screen and (max-width: 767px)``
- Cara mengkondisikan Media Query ada 2 cara yaitu:
  - Memisahkan beberapa file css sesuai dengan tampilan device yang ingin dibuat 
  - Menggabungkan semua styling css device menjadi 1 
- Breakpoint yaitu istilah saat terjadi perubahan ukuran pada suatu website ketika berganti device
- Terdapat 3 jenis breakpoint yaitu desktop, tablet, dan mobile phone
- Contoh breakpoint dapat ditulis seperti ini
  ```
  @media screen and (min-width: 300px) and (max-width: 767px) {
  body {
    background-color: white 
    }
   }
  ```
- Flexbox bertujuan untuk membuat website yang lebih efisien dalam mengatur, menata dan item pada dalam sebuah wadah bahkan ketika ukurannya tidak diketahui dan/atau dinamis (dengan menggunakan kata "flex").
- Flexbox properties :
  - Flex direction : menetapkan sumbu utama item, sehingga menentukan arah item fleksibel ditempatkan di wadah fleksibel. 
  - Flex Wrap : Secara default, semua item pada flexbox akan mencoba berada dalam satu baris. Maka dengan flex wrap kita dapat mengubah hal tersebut.
  - Flex flow : cara singkat untuk properti flex-direction dan flex-wrap, yang bersama-sama menentukan sumbu utama dan sumbu silang container flex. Nilai default adalah baris nowrap.
  - Align items : membantu mendistribusikan item-item yg ada di dalam container
- Grid merupakan sistem tata letak berbasis dua dimensi.
- Pada Grid ada 2 jenis yaitu grid container dan grid item.


### **Bootstrap**
- Bootstrap adalah salah satu framework opensource yang berfungsi membuat suatu responsive website
- Komponen utama bootstrap :
  - bootstrap.css
  - bootstrap.js
- Cara konfigurasi bootstrap :
  - Membuat tag boostrap di HEAD. Cara memanggil css bootstrap dengan menggunakan href lalu mengganti link href css lokal dengan link boostrap online.
- Penggunaan theme color pada boostrap dapat menggunakan keyword berikut :
  ```
  $theme-colors: (
  "primary":    $primary,
  "secondary":  $secondary,
  "success":    $success,
  "info":       $info,
  "warning":    $warning,
  "danger":     $danger,
  "light":      $light,
  "dark":       $dark
  );
  ```
 ![warna-bootstrap-4](https://user-images.githubusercontent.com/114548824/196225817-815bb6e4-8d52-403a-af1e-eb629e178cca.png)


- Layout pada boostrap :
  - Breakpoints merupakan suatu cara yang dilakukan untuk membuat desain responsif dengan mengontrol kapan tata letak yang disesuaikan dengan ukuran perangkat
    tertentu.
    - Breakpoints pada bootstrap ada 5 yaitu sm, md, lg, xl dan xxl.
 - Container adalah blok dasar atau pembungkus boostrap yang terdiri dari contain, pad dan align  yang menyelaraskan konten website dalam perangkat atau area      
   pandang tertentu.
   - Terdapat 3 container pada boostrap yaitu :
   - .container, yang menerapkan lebar maksimum pada setiap breakpoint responsif
   - .container-{breakpoint}, menerapkan lebar 100% sampai dengan breakpoint yang ditentukan.
   - .container-fluid, menerapkan 100% ukurannya dari breakpoints
 - Grid System pada bootstrap yang terdiri dari 12 kolom default.
 - Grid system pada bootstrap menggunakan container,baris dan kolom untuk menata dan menyelaraskan konten,yang dibangun menggunakan flexbox dan itu sudah responsive.
 - Grid system bootstrap :
   - .col-lg digunakan untuk mengatur grid pada ukuran monitor yang besar
   - .col-md digunakan pada monitor komputer berukuran sedang
   - .col-sm digunakan untuk mengatur monitor pada tablet
   - .col-xs digunakan untuk mengatur monitor pada handphone 
