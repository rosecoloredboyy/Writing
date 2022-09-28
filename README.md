# Week 1
Writing and Presentation week 1

## Unix Command Line

- ### CLI (Command Line Interface)
  <div align="justify">adalah antarmuka pengguna (UI) berbasis teks yang digunakan untuk menjalankan program, mengelola file komputer, dan berinteraksi dengan komputer.
- ### Shell
  <div align="justify">Agar bisa terhubung dengan komputer maka user akan memerlukan penerjemah. Shell adalah program yang menerima perintah, kemudian meneruskan perintah tersebut ke system untuk dieksekusi.
- ### Terminal
  <div align="justify">User dan komputer dihubungkan dengan namanya terminal, yaitu sebuah tempat/aplikasi dimana user dapat mengetikan atau memberikan suatu perintah. Disinilah tempat dimana shell akan berperan.

- ### Command

  - pwd (print working directory) adalah command untuk melihat current working directory
  - dir (directory) adalah command untuk melihat directory
  - cd (change directory) adalah command untuk pindah directory
  - ls (list) adalah command untuk melihat isi file di dalam directory
  - touch adalah command untuk membuat file directory
  - cp (copy) adalah comand untuk menyalin file directory
  - mv (move) adalah command untuk memindahkan file directory
  - rm (remove) adalah command untuk menghapus file directory

  &nbsp;

## Git & Github

- ### Apa itu Git & Github

  - Git
    <div align="justify">Merupakan aplikasi yang bertugas untuk mencatat perubahan seluruh file atau repository suatu project, yang biasanya digunakan oleh programmer sebagai tempat untuk menyimpan file programan mereka karena lebih efektif.

  - Github
    <div align="justify">Merupakan vendor penyedia layanan git yang dimiliki oleh microsoft atau secara definisi merupakan layanan hosting berbasis web sebagai repositori git.

  &nbsp;

  ### Mengapa wajib menggunakan Git & Github?

  <div align="justify">Alasan utamanya adalah biasanya programmer tidak akan bekerja sendiri selamanya. Maka dari itu dengan menggunakan Git & Github akan memudahkan programmer untuk bisa bekerja sama dalam sebuah tim. Tujuan besarnya adalah programmer bisa berkolaborasi dengan programmer lainnya dengan mengerjakan proyek yang sama tanpa harus repot copy paste folder aplikasi yang terupdate.

&nbsp;

- ### Command di dalam Git & Github

  - Konfigurasi git
    git config global user.name "alwan"
    git config global user.email alalpribadi@gmail.com
    Melihat hasil konfigurasi dengan git config --list Config list
  - Membuat Repository
    - git init digunakan untuk membuat repositori baru
    - git Status digunakan untuk melihat apakah terjadi perubahan atau tidak pada Git
    - git add untuk menambah file baru/file yang telah diubah pada Git
    - git remote menghubungkan remote repository dengan project local yang telah kita buat direktorinya
    - git commit -m "commit message" digunakan untuk menyimpan perubahan pada Git
    - git push -u origin master digunakan untuk mengirimkan/perubahan file ke remote repository
    - git branch -b [nama branch] digunakan untuk membuat branch baru
    - git checkout digunakan untuk berpindah branch
    - git merge digunakan untuk menggabungkan branch cabang ke branch master ( git merge origin/(nama branch))
    
## HTML

- Definisi HTML

  <div align="justify">Merupakan bahasa komputer yang digunakan untuk membuat kerangka atau struktur untuk Web pages (halaman website) di internet. Bagaimana peran HTML pada web development? Web browser seperti Chrome, Firefox, Edge, Safari, atau Opera akan membaca dokumen HTML. Dokumen HTML yang berisi tag-tag HTML akan memberitahu browser bagaimana cara menampilkan sebuah konten.

&nbsp;

- Kerangka HTML

  HTML memiliki sebuah kerangka seperti gambar dibawah ini

  ```html
  <html>
  <head>
  <title>
      Judul Website
    </title>
  <body>
      saya sedang belajar pemrograman HTML dasar.
    </body>
  </html>
  ```

    <div align="justify">Sintak diatas biasa disebut dengan kerangka bahasa pemrograman HTML. Didalam website selalu ada title untuk tiap-tiap web, untuk memasukkan title didalam web kamu harus mengetikkan diantara tag title (dapat diisikan dengan nama website kamu atau yang lainnya). Untuk memasukkan konten-konten, kamu dapat memasukkannya atau mengetikkannya didalam program tepat diantara tag body (Ganti titik-titik dengan konten).

  &nbsp;

- Tag HTML

  <div align="justify">Tag adalah sebuah penanda awalan dan akhiran dari sebuah elemen di HTML. Tag dibuat dengan kurung siku (<...>), lalu di dalamnya berisi nama tag dan kadang juga ditambahkan dengan atribut.

  &nbsp;

  <div align="justify">Tag selalu ditulis berpasangan. Ada tag pembuka dan ada tag penutupnya. Namun, ada juga beberapa tag yang tidak memiliki pasangan penutup. Tag penutup ditulis dengan menambahkan garis miring (/) di depan nama tag.

  &nbsp;

  Contoh tag HTML

  - Tag untuk membuat tulisan tebal dan miring

    ```html
    <b>Tebal</b> <i>Miring</i>
    ```

    Hasilnya di browser

    ![](gambar/tebal-miring.JPG)

  - Tag HTML Untuk Membuat tulisan dengan link

    ```html
    <a href="">Welcome To Mobile Lejenn</a>
    ```

    Hasilnya di web browser

    ![](gambar/link.jpg)

  - Tag HTML Untuk Menampilkan gambar

    ```html
    <img src="https://bit.ly/2FKluzq" alt="Si Kucing"></img>
    ```

    Hasilnya di web browser

    ![](gambar/gambar.jpg)

    &nbsp;

- Deploy HTML

  <div align="justify">Deploy adalah sebuah proses untuk menyebarkan aplikasi yang sudah kita kerjakan supaya bisa digunakan oleh orang-orang. Jika aplikasi kita HTML atau Web App kita perlu mendeploy ke server. Untuk melakukan hal tersebut kita bisa menggunakan layanan yang bernama Netlify

## CSS

- Definisi CSS

  <div align="justify">CSS adalah bahasa komputer yang digunakan untuk menambahkan design ke suatu halaman website di internet agar terlihat lebih cantik/menarik. CSS adalah singkatan dari Cascading Style Sheets. Kita ibaratkan HTML adalah kerangka yang memberi sturuktur pada website, maka CSS adalah baju yang memberi warna dan layout pada website.

&nbsp;

- Cara Menggunakan CSS
    
  1. Inline Styles

     Kita menambahkann CSS langsung pada atribut HTML

     ```html
     <p style="color:red">Tulisan ini berwarna merah</p>
     ```

     ![](gambar/inline.jpg)

  &nbsp;

  2. Internal CSS

     Kita menggunakan element/tag `<style>` untuk menyisipkan kode CSS. element/tag `<style>` diletakkan di dalam element `<head>`

     ```html
     <!DOCTYPE html>
     <html>
       <head>
         <title>Website Pertamaku</title>
         <style>
           body {
             background-color: yellow;
           }
           h1 {
             color: blue;
           }
           p {
             color: red;
           }
         </style>
       </head>
       <body>
         <h1>Website Pertamaku</h1>
         <p>Selamat Datang</p>
       </body>
     </html>
     ```

     Tampilan dari sintaks diatas adalah

     ![](gambar/internal-css.jpg)

     &nbsp;

  3. Eksternal CSS

     <div align="justify">Kita akan menyisipkan kode CSS dengan cara membuat file CSS terpisah, dan lalu menyambungkannya dengan file HTML dengan menggunakan element <link>. Element <link> tersebut diletakkan di dalam element <head>

     Contoh:

     <div align="justify">Kita memiliki dua file: index.html untuk file HTML-nya dan styles.css untuk file CSS-nya.

     ```html
     <!-- File index.html -->

     <!DOCTYPE html>
     <html>
       <head>
         <title>Website Pertamaku</title>
         <link rel="stylesheet" href="styles.css" />
       </head>
       <body>
         <h1>Website Pertamaku</h1>
         <p>Selamat Datang</p>
       </body>
     </html>
     ```

     ```css
     /* File styles.css */

     body {
       background-color: pink;
     }
     h1 {
       color: blue;
     }
     p {
       color: black;
     }
     ```

     Tampilan dari sintaks diatas adalah

     ![](gambar/ekstenal-css.jpg)

     &nbsp;

- CSS Syntax

  <div align="justify">CSS Syntax adalah syntax yang digunakan untuk menunjuk atau memilih HTML element mana yang ingin diberi style (dihias). CSS syntax terdiri dari selector, property, dan value.

  Syntaxnya seperti ini:

  ```css
  p {
    color: blue;
  }
  ```

  Penjelasan :

  - p

    Adalah sebuah selector berupa element HTML yang akan diubah

  - color

    <div align="justify">Adalah sebuah properti berupa bagian mana dari element HTML yang akan diubah. Contoh diatas kita akan mengubah warna dari teks yang ada di element p

  - blue

    Adalah value yaitu nilai/hiasan berupa warna biru

  &nbsp;

## Algoritma dan Struktur Data

- Algoritma

  - <div align="justify">Algoritma Adalah deskripsi berupa step-step yang dibutuhkan untuk menyelesaikan suatu masalah. Untuk menyelesaikan suatu masalah, tentunya kita harus mempunyai data struktur, nah data inilah yang akan kita gunakan untuk menyelesaikan suatu masalah dengan menggunakan algoritma.

  &nbsp;

  - Mengapa kita memerlukan algoritma?

    Manfaat algoritma antara lain:

    - <div align="justify">Membantu menyederhanakan suatu program yang rumit dan juga besar.
    - <div align="justify">Mempermudah pembuatan program yang dapat menyelesaikan masalah tertentu.
    - <div align="justify">Membantu menyelesaikan suatu masalah dengan logika dan juga sistematis.

  &nbsp;

  - Kualitas Algortima

    Kualitas wajib dari algoritma

    - <div align="justify">Input dan output harus didefinisikan terlebih dahulu dengan tepat
    - <div align="justify">Setiap step harus benar-benar clear dan tidak ambigu
    - <div align="justify">Algoritma seharusnya tidak mengandung suatu code pada bahasa pemograman tertentu.
    - <div align="justify">Algoritma harus dibuat agar dapat digunakan dalam bahasa pemograman apapun.
      
    &nbsp;

- Pseudocode

  - <div align="justify">Pseudocode adalah menuliskan algoritma sebelum kita implementasikan ke bahasa pemograman tertentu.

    &nbsp;

  - Pseudocode berdasarkan kondisi masalah

    - Procedural

      Procedural adalah cara berpikir secara runtun. Artinya serangkaian perintah yang berurutan.

      &nbsp;

    - Conditional

      Conditional digunakan saat dibutuhkan percabangan kasus. Komputer akan melakukan suatu tindakan jika suatu kondisi terpenuhi.

      Jika hari ini tidak hujan, maka Bob pergi ke pasar,

      jika tidak maka Bob dirumah aja.

    &nbsp;

    - Looping

      Komputer dapat melakukan sebuah proses yang sama berulang-ulang.

      Jika membutuhkan perulangan dalam kasus tertentu, kita bisa menggunakan Looping.

      &nbsp;

    - Recursive

      Recursive adalah pola pikir dalam algoritma yang memanggil method/function didalam sebuah function
