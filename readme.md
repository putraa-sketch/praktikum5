# PRAKTIKUM 5

## Step 1 : Fungsi

![Screenshot 2024-11-22 161002](https://github.com/user-attachments/assets/901ebcbf-7a7e-4132-b5e1-81d0a824fef7)


Bagian pertama kode mendefinisikan sebuah fungsi bernama hitung_nilai_akhir. Fungsi ini memiliki tiga parameter: tugas, uts, dan uas, yang mewakili nilai tugas, nilai Ujian Tengah Semester (UTS), dan nilai Ujian Akhir Semester (UAS). Fungsi ini menggunakan rumus perhitungan nilai akhir: 
Nilai Akhir=(40%×Tugas)+(30%×UTS)+(30%×UAS)
Setelah nilai dihitung, fungsi menggunakan fungsi bawaan Python round untuk membulatkan hasilnya menjadi dua angka di belakang koma. Hasil akhir dikembalikan ke pemanggil fungsi.

## Step 2 : Variabel

![Screenshot 2024-11-22 161039](https://github.com/user-attachments/assets/f4c8cdaf-3401-4a7d-bc76-bd3d3c06ab69)


Variabel data_mahasiswa adalah sebuah list kosong yang digunakan untuk menyimpan data mahasiswa. Nantinya, setiap data mahasiswa akan ditambahkan ke dalam list ini dalam bentuk dictionary (kamus). Setiap dictionary berisi informasi lengkap tentang mahasiswa, termasuk NIM, nama, nilai tugas, UTS, UAS, dan nilai akhir.

## Step 3 : Menu Utama (Perulangan While)

![Screenshot 2024-11-22 161108](https://github.com/user-attachments/assets/37c7c210-8e82-44a4-9a5f-1b1b3ab154df)


Bagian ini adalah inti dari program, berupa perulangan while yang terus berjalan hingga pengguna memilih untuk keluar dari program. Pada setiap iterasi, program menampilkan menu pilihan utama berupa beberapa opsi: Lihat, Tambah, Ubah, Hapus, Cari, dan Keluar. Pilihan pengguna diambil menggunakan fungsi input dan diubah menjadi huruf kecil (lower()) agar program bisa menangani input tanpa mempermasalahkan huruf besar atau kecil.

## Step 4 : Menambah Data 

![Screenshot 2024-11-22 161159](https://github.com/user-attachments/assets/8dd0d18c-601f-4804-8809-a0b26904730d)


Ketika pengguna memilih opsi Tambah Data ('t'), program meminta input untuk setiap data mahasiswa: NIM, Nama, Nilai UTS, Nilai UAS, dan Nilai Tugas. Data ini diinput satu per satu melalui fungsi input, kemudian nilai-nilai numerik (UTS, UAS, Tugas) diubah menjadi tipe integer menggunakan int().

Setelah semua data diterima, nilai akhir mahasiswa dihitung dengan memanggil fungsi hitung_nilai_akhir. Selanjutnya, data mahasiswa disimpan dalam dictionary yang berisi semua informasi tadi:

![Screenshot 2024-11-22 161229](https://github.com/user-attachments/assets/4289b164-c702-41cb-8691-8cf506b5dfb2)


Dictionary ini kemudian ditambahkan ke list data_mahasiswa menggunakan fungsi append.

## Step 5 : Melihat Daftar Nilai

![Screenshot 2024-11-22 161435](https://github.com/user-attachments/assets/ba929cca-6fe1-4fde-9fe1-818cd2065a95)


Jika pengguna memilih untuk Melihat Daftar Nilai ('l'), program mencetak judul tabel dan kolom-kolom data, yaitu: NO, NIM, Nama, Tugas, UTS, UAS, dan Nilai Akhir. Batas tabel ditandai dengan garis =.

Untuk setiap mahasiswa yang tersimpan di list data_mahasiswa, program mencetak data dalam format tabel menggunakan perulangan for:

## Step 6 : Keluar dari Program

![Screenshot 2024-11-22 161510](https://github.com/user-attachments/assets/5f73dfce-34aa-4425-afc3-57bcae346f29)

Jika pengguna memilih Keluar ('k'), program mencetak pesan bahwa program telah selesai dan menggunakan perintah break untuk keluar dari perulangan while, sehingga program berhenti berjalan.

## Step 7 : Opsi Tidak Valid

![Screenshot 2024-11-22 161531](https://github.com/user-attachments/assets/226130c0-1fe3-4019-9e73-1848a01bd6a0)

Jika pengguna memasukkan pilihan yang tidak tersedia dalam menu (selain l, t, atau k), program akan memberikan pesan kesalahan sederhana dan kembali menampilkan menu.

## Step 8 : Run Program
Tahap akhir adalah uji coba code program yang sudah dibuat dengan mencoba berbagai kemungkinan yang ada.

### Case 1 : Menu Utama
Ketika program pertama kali dijalankan, akan muncul menu seperti ini:

![Screenshot 2024-11-22 161618](https://github.com/user-attachments/assets/86be36a2-0793-4e56-bea6-38d5a65f0917)


### Case 2 : Tambah Data (T)
Jika Anda memilih opsi T untuk menambahkan data, program akan meminta Anda untuk mengisi informasi berikut:

![WhatsApp Image 2024-11-22 at 16 06 41](https://github.com/user-attachments/assets/23f5463e-15e1-4b6b-952d-4bdafe09be63)

### Case 3 : Lihat Data (L)
Jika Anda memilih opsi L untuk melihat data yang telah dimasukkan, output yang ditampilkan akan berupa tabel seperti berikut:

![WhatsApp Image 2024-11-22 at 16 06 42 (1)](https://github.com/user-attachments/assets/7d316c99-30ad-4adb-9bc1-af8e540c335e)


### Case 4 : Keluar Program (K)

Jika Anda memilih opsi K, program akan berhenti tanpa pesan tambahan.

### Case 5 : Error Handling (Input Tidak Valid)
Jika Anda memasukkan pilihan menu yang tidak valid, program akan menampilkan pesan seperti berikut dan kembali ke menu utama:

![Screenshot 2024-11-22 162138](https://github.com/user-attachments/assets/b378ab5b-39a2-4300-bda1-71fb06b6ba70)

### Output :
Hasil dari output:

![WhatsApp Image 2024-11-22 at 16 06 42](https://github.com/user-attachments/assets/c05068f9-8478-425f-947b-474bcc66cc2a)

# FLOWCHART DAFTAR MULAI

![flowchartimage](https://github.com/user-attachments/assets/553a90b2-4f5e-4421-a599-4ab5353dc5e7)


## Step 1 :
Titik mulai sebuah program atau alur.

## Step 2 :
lalu lakukan inisialisasi dengan menampilkan menu yang tersedia

## Step 3 :
Inputkan code menu yang ingin dilakukan, setiap code berisi [L]ihat, [T]ambah, [U]bah, [H]apus, [C]ari, [K]eluar.

## Step 4 :
Dalam kasus ini semua kemgkinan dapat terjadi, kondisi yang diperlukan sesuai apa yang akan diinputkan user.
Jika [L]ihat, maka user akan di tampilkan sebuah tabel dari daftar nilai, namun jika tabel belum ada isi/kosong maka akan tampil tidak ada data, jika ada maka ditampilkan sebuah data nilai mahasiswa. Setelah tampilkan data maka akan kembali menuju inisialisasi menu.
Jika [T]ambah, user diminta memasukan sebuah data yang berupa :

*   NIM
*   Nama
*   Nilai Tugas
*   Nilai UTS
*   Nilai UAS

Lalu User akan diarahkan kembali ke inisialiasi menu.
Jika [U]bah, sama dengan [L]ihat jika tidak ada data nilai maka akan tampil tidak ada data nilai namun [U]bah kalau ada data nilai user diminta menginputkan Nomor urut yang akan diubah, setelah itu diminta untuk mengisi atau menginputkan data valid yang diubah. Setelah itu user kembali ke inisialisasi menu.

1. Jika [C]ari, user diminta memasukan nama yang dicari, setelah itu maka akan ditampilkan tabel daftar    nilai mahasiswa. Setelah itu kembali ke inisialisasi menu.

2. Jika [H]apus, user akan ditampilkan daftar nilai lalu diminta memasukan sebuah nomor yang ingin dihapus dari daftar. Setelah itu kembalu ke inisialisasi menu.

3. jika [K]eluar, User akan keluar program dan program akan berhenti.

# Kesimpulan :
Kesimpulan dari program ini adalah bahwa ia dirancang sebagai alat sederhana namun efektif untuk mengelola data mahasiswa. Program ini memungkinkan pengguna untuk menambahkan informasi mahasiswa, seperti NIM, nama, nilai tugas, UTS, dan UAS, sekaligus menghitung nilai akhir berdasarkan bobot yang telah ditentukan. Program memberikan kemudahan melalui menu berbasis teks, sehingga pengguna dapat memilih berbagai opsi dengan cepat, seperti menambah data, melihat daftar mahasiswa, atau keluar dari program.sg
