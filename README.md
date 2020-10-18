# Jarkom_Modul1_Lapres_C13

###LAPRES PRATIKUM MODUL 1 JARKOM

#####KELOMPOK C13 : 
######1) Rida Adila  05111840000002
######2) Bayu Surya B 051111840000114
*********

##### A) DISPLAY FILTER
####
1. Sebutkan webserver yang digunakan pada "testing.mekanis.me"!
####
######JAWAB :
Syntaxnya adalah :

![1 1](https://user-images.githubusercontent.com/71973415/96349155-eb805000-10d7-11eb-9d70-93cea4cd991c.png)
######
######

Hasilnya :

![1 2](https://user-images.githubusercontent.com/71973415/96349157-ecb17d00-10d7-11eb-80fb-b274654e3a01.png)
Sehingga web servernya ialah : nginx/1.14.0 (Ubuntu)
##
2. Simpan gambar "Tim_Kunjungan_Kerja_BAKN_DPR_RI_ke_Sukabumi141436.jpg"!
####
######JAWAB :
Klik menu file - export objects - http pada wireshark . Lalu ketikkan nama file yang akan mau di export. 

![2 1](https://user-images.githubusercontent.com/71973415/96349263-aad50680-10d8-11eb-9a23-cfd5ab99fb2b.png)

Lalu simpan file tersebut, sehingga hasil fotonya akan tampak sebagai berikut :

![2 2](https://user-images.githubusercontent.com/71973415/96349267-ac063380-10d8-11eb-949f-7d27233b40ee.jpg)
##
3. Cari username dan password ketika login di "ppid.dpr.go.id"!
####
######JAWAB :
Syntax nya adalah sebagai berikut :

![3 1](https://user-images.githubusercontent.com/71973415/96349359-57af8380-10d9-11eb-8162-71a4e418163b.png)

Kemudian, dari hasil paket yang muncul, pilih pada paket yang mengandung kata login

![3 2](https://user-images.githubusercontent.com/71973415/96349361-58481a00-10d9-11eb-906a-b433ba701f6b.png)

Setelah itu klik kana pada paket tsb, lalu pilih follow-tcp stream, sehingga akan muncul informasi mengenai paket tsb.

![3 3](https://user-images.githubusercontent.com/71973415/96349363-58e0b080-10d9-11eb-9f31-c54e2d5eb27e.png)

Didapatkan usernamnya adalaha 10pemuda, dan passwordnya adalah guncangdunia
##
4. Temukan paket dari web-web yang menggunakan basic authentication method!
####
######JAWAB :
Syntaxnya adalah sebagai berikut :

![4 1](https://user-images.githubusercontent.com/71973415/96349461-123f8600-10da-11eb-95f6-63ac94227236.png)

Hasil paket-paketnya adalah :

![4 2](https://user-images.githubusercontent.com/71973415/96349463-1370b300-10da-11eb-8e77-be669de4e276.png)
##
5. Ikuti perintah di aku.pengen.pw! Username dan password bisa didapatkan dari file .pcapng!
####
######JAWAB :
Syntaxnya adalah :

![5 1](https://user-images.githubusercontent.com/71973415/96349512-706c6900-10da-11eb-8806-9b45f8835b7e.png)

Lalu, pada paket yang terfilter klik kanan-follow-tcp stream untuk melihat informasinya. Sehingga didapatkan authorization nya, yakni basic dengan username dan password masih dalam bentuk base64

![5 5](https://user-images.githubusercontent.com/71973415/96349554-9f82da80-10da-11eb-85ae-21bc9b90e5f9.png)

Lalu kode basic tersebut kita decode kan pada website browser decode base64 :

![5 2](https://user-images.githubusercontent.com/71973415/96349517-719d9600-10da-11eb-85ef-e360a9df3139.png)


Sehingga didaptkan username dan passwordnya. Lalu kita buka website aku.pengen.pw dan masukkan username serta password yang telah didapat :

![5 3](https://user-images.githubusercontent.com/71973415/96349519-72362c80-10da-11eb-8271-652b06d216b4.png)

Sehingga akan muncul pertanyaan yang harus dijawab :

![5 4](https://user-images.githubusercontent.com/71973415/96349520-72362c80-10da-11eb-9fb9-e7a371bc29e3.png)
##
6. Seseorang menyimpan file zip melalui FTP dengan nama "Answer.zip". Simpan dan Buka file "Open This.pdf" di Answer.zip. Untuk mendapatkan password zipnya, temukan dalam file zipkey.txt (passwordnya adalah isi dari file txt tersebut).
####
######JAWAB :
Untuk syntax filter dan hasil paketnya adalah :

![6 1](https://user-images.githubusercontent.com/71973415/96356979-c7486180-111f-11eb-9a2c-74c4f4f72323.png)


Lalu dipilih pada paket yang mengandung tulisan "Answer.zip". Pada paket tsb di klik kanan-follow-tcp stream , lalu simpan file zip tsb.

![6 2](https://user-images.githubusercontent.com/71973415/96356980-c9122500-111f-11eb-9140-51dd1088bbf8.png)

Lalu cari lagi paket yang mengandung "zipkey.txt" untuk mendapatkan passwordnya :

![6 3](https://user-images.githubusercontent.com/71973415/96356981-c9aabb80-111f-11eb-8486-ce3d0632c882.png)

![6 4](https://user-images.githubusercontent.com/71973415/96356983-cca5ac00-111f-11eb-8096-3e02539fc8e7.png)

Lalu password tsb digunakan untuk membuka file "Open this.pdf" pada file "Answer.zip" , dan hasilnya akan nampak spt berikut ini setelah dimasukkan passnya :

![6 5](https://user-images.githubusercontent.com/71973415/96356984-cdd6d900-111f-11eb-9039-f24ad39158a9.png)
##
7. Ada 500 file zip yang disimpan ke FTP Server dengan nama 1.zip, 2.zip, ..., 500.zip. Salah satunya berisi pdf yang berisi puisi. Simpan dan Buka file pdf tersebut.
Your Super Mega Ultra Rare Hint = nama pdf-nya "Yes.pdf"
####
######JAWAB :
Untuk syntax filternya adalah sebagai berikut :

![7 1](https://user-images.githubusercontent.com/71973415/96357148-142d3780-1122-11eb-801c-5c4033a13e72.png)

Lalu pada hasil paket yang mengandung info terdapat "Yes.pdf" , klik kanan- follow - tcp stream :

![7 2](https://user-images.githubusercontent.com/71973415/96357149-14c5ce00-1122-11eb-8706-a94c9ba21831.png)

Setelah itu simpan filenya, dan akan nampak hasilnya seperti ini :

![7 3](https://user-images.githubusercontent.com/71973415/96357150-17c0be80-1122-11eb-91bb-5b6d54f7aff8.jpg)
##
8. Cari objek apa saja yang didownload (RETR) dari koneksi FTP dengan Microsoft FTP Service!
####
######JAWAB :
Pertama dicari dulu ftp dengan "microsoft" :

![8 1](https://user-images.githubusercontent.com/71973415/96357196-e4326400-1122-11eb-95b6-e2cf9ac428bd.png)

Lalu untuk mencari objek apa saja yg di download dari koneksi ftp, bisa dicari lagi dengan :

![8 2](https://user-images.githubusercontent.com/71973415/96357197-e5639100-1122-11eb-86eb-51fce4569265.png)


Setelah itu, hasil nya akan  muncul seperti ini :

![8 3](https://user-images.githubusercontent.com/71973415/96357198-e5fc2780-1122-11eb-96c2-c252cb3878f0.png)
##
9. Cari username dan password ketika login FTP pada localhost!
####
######JAWAB :
Syntax untuk mendapatkan pass pada localhost :

![9 1](https://user-images.githubusercontent.com/71973415/96357376-47bd9100-1125-11eb-884b-de5b0b48ea8d.png)

Ditemukan hasil passnya adalah dhana123
##
10. Cari file .pdf di wireshark lalu download dan buka file tersebut!
clue: "25 50 44 46" 
####
######JAWAB :
Mencari file pdf di wireshark, syntaxnya adalah :

![10 1](https://user-images.githubusercontent.com/71973415/96357436-ff52a300-1125-11eb-9fae-1b2caa73fa75.png)

Lalu, hasil paket yang terfilter akan nampak seperti di bawah ini. kemudia pilih pada salah satu paket dimana bagian info nya mengandung file .pdf :

![10 2](https://user-images.githubusercontent.com/71973415/96357437-ffeb3980-1125-11eb-85d9-ccac77c533f8.png)

Kemudian pada paket yg dipilih tsb klik kanan - follow - tcp stream , sehingga akan nampak informasinya seperti ini :

![10 3](https://user-images.githubusercontent.com/71973415/96357438-011c6680-1126-11eb-8b31-ec17d6c827df.png)


Lalu simpan filenya, untuk show and save data as nya diubah dulu menjadi "Raw". Dan kemudian isi pdf nya akan nampak seperti berikut :

![10 5](https://user-images.githubusercontent.com/71973415/96357441-04afed80-1126-11eb-9b6b-34af912e4f74.png)


*******
##### B) CAPTURE FILTER
####
11. Filter sehingga wireshark hanya mengambil paket yang mengandung port 21!
####
######JAWAB :
Syntax filternya adalah : port 21

![11 1](https://user-images.githubusercontent.com/71973415/96357503-134ad480-1127-11eb-8e59-416cc2921c85.jpg)
##
12. Filter sehingga wireshark hanya mengambil paket yang berasal dari port 80!
####
######JAWAB :
Syntax filternya adalah : src port 80

![12 1](https://user-images.githubusercontent.com/71973415/96357604-4a6db580-1128-11eb-8266-50f6eb5c2366.jpg)
##
13. Filter sehingga wireshark hanya menampilkan paket yang menuju port 443!
####
######JAWAB :
Syntax filternya :  dst port 443

![13 1](https://user-images.githubusercontent.com/71973415/96357612-7db04480-1128-11eb-864d-be6b6d0544bd.jpg)
##
14. Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!
####
######JAWAB :
Syntax filter : host *ip sendiri

![14 1](https://user-images.githubusercontent.com/71973415/96357688-4c844400-1129-11eb-833b-eed485fdc122.png)

![14 2](https://user-images.githubusercontent.com/71973415/96357689-4db57100-1129-11eb-9896-2c4c7d67d04a.png)
##
15. Filter sehingga wireshark hanya mengambil paket yang tujuannya ke monta.if.its.ac.id!
####
######JAWAB :

Syntax filter : dst *ip monta

![15 1](https://user-images.githubusercontent.com/71973415/96358177-696f4600-112e-11eb-85f4-90c840088283.png)
