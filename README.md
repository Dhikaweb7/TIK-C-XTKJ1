# TIK-C-XTKJ1
Materi bahasa pemograman C

# Pengenalan bahasa C
  <a href="https://id.m.wikipedia.org/wiki/C_(bahasa_pemrograman)">Bahasa pemograman C</a>
  ### Alat yang diperlukan
  
  - <a href="https://id.m.wikipedia.org/wiki/Penyunting_teks">Text Editor / IDE</a>
  - <a href="https://id.m.wikipedia.org/wiki/Kompilator">Kompiler</a>

  #### Rekomendasi 
   
   untuk Laptop
   
   - <a href="https://www.bloodshed.net/">DEV C++</a>
       
  karena lengkap dengan kompiler bahasa C dan C++ tanpa harus mendownload secara manual
  
  untuk android dapat menggunakan aplikasi yang tersedia di playstore dengan kata kunci pencarian ``C++``
# Membuat Program Pertama bahasa C
  fungsi komentar adalah membantu kalian memahami kode program
  komentar satu / lebih dapat ditulis dengan ``/*`` dan diakhiri dengan ``*/``
  komentar satu baris dapat diketik dengan ``//``
  ```c
   /* Program pertamaku: */
   /* Mencetak "Halo Dunia!" */
   
   #include <stdio.h>
     int main(){  // Fungsi utama program
        printf("Halo Dunia!\n"); // cetak Halo Dunia! ke layar
       return 0; // program berjalan dengan benar
      }
   ```
   # Komponen dalam bahasa C


   - Kata kunci

   - identifer

   - variabel

   - tipe data

   - konstanta

   # Kata kunci (Keyword)


 Merupakan kata yang memiliki makna khusus yang tidak dapat diubah dan digunakan sebagai identifier.
 terdapat 32 kata kunci standar pada bahasa C, yaitu :
  
   
 - auto
 - double
- int
- struct
- break
- else
- long
- switch
- case
- enum
- register
- typedef
- char
- extern
- return
- union
- continue
- for
- signed
- void
- do
- if
- static
- while
- default
- goto
- sizeof
- volatile
- const
- float
- short
- usigned


# Identifier

adalah nama unik yang dapat kalian ingat yang kalian berikan kepada variabel atau fungsi.
Identifier terdiri atas serangkaian karakter dengan aturan berikut :

- Tidak boleh sama dengan Keyword dalam bahasa C.
- Disusun dari kombinasi huruf (besar dan kecil), angka dan underscore ``_`` .
- Bersifat Case-sensitive, atau sensitif terhadap huruf besar dan kecil contohnya , Aku dan aku adalah dua identifier yang berbeda.

# Tipe Data

Komputer dapat mengelolah data yang beragam ,baik angka maupun karakter disimpan oleh komputer dalam bentuk biner
program perlu mengetahui bagaimana bilangan biner itu dibaca sehingga terbuatlah tipe data, 
yang memiliki nama tipe, jenis data, dan rentang yang berbeda. 
pada bahasa C terdapat beberapa tipe data :


| Nama Tipe | Jenis Data | Ukuran Memori | Rentang |
|---        |---         |---            |---      |
| int       | Bilangan bulat | 4 byte   | -2.1x10 pangkat 9 |
| short    | Bilangan bulat | 2 byte | -32768 hingga 32767 |
| long | Bilangan bulat | 8 byte | -9.2x10 pangkat 8 |
| float | Bilangan rill | 4 byte | 1.2x10 pangkat 38 hingga 3.4x10 pangkat 38 |
| double | Bilangan rill | 8 byte | 2.3x10 pangkat 308 hingga 1.7x10 pangkat 308 |
| char | Karakter | 1 byte | -127 hingga 128

Perhatikan bahwa rentang yang diberikan memungkinkan 
nilai negatif hingga positif, atau disebut tipe data ``signed``.
Apabila kalian menambahkan kata kunci ``unsigned`` di depan tipe data, tipe data tersebut hanya menampung
bilangan positif dengan rentang dari 0 hingga 2 ( jumlah bit ) - 1

> GUNAKAN TIPE DATA SESUAI KEBUTUHAN KALIAN
sebagai contoh saat mengolah data usia manusia dalam satuan tahun,
kalian cukup menggunakan tipe data short yang memerlukan memori lebih kecil.
agar program yang kalian buat lebih efisien memori
