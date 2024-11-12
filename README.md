# Transjakarta-Analysis

Hello! Pada kesempatan kali ini, saya akan mencoba untuk menganalisis data penumpang Transjakarta yang naik pada 1 - 30 April 2023, dimana proyek ini adalah salah satu bagian dari pembelajaran di Purwadhika tentang Data Analisis.
Hasil analisis ini saya tujukan untuk pihak marketing dari PT. Transjakarta.

**Latar Belakang**

Banyaknya kendaraan yang ada di jalan raya menimbulkan kemacetan, sehingga menimbulkan kemacetan. Salah satu solusi yang dapat digunakan adalah dengan menggunakan transportasi umum. Diharapkan dengan banyaknya masyarakat yang menggunakan transportasi umum, maka kendaraan yang ada di jalan raya juga dapat berkurang dan kemacetan akan ikut berkurang.

**Tujuan**

Tujuan dari analisis ini adalah untuk meningkatkan minat masyarakat untuk naik transjakarta dengan melihat dari karakteristik penumpang transjakarta yang dianalisis.

**Rumusan Masalah**
1. Berdasarkan gender, mana yang lebih banyak naik transjakarta?
2. Berdasarkan kategori usia, mana yang lebih banyak naik transjakarta?
3. Apakah ada hubungan antara variabel usia dengan variabel harga transjakarta?
4. Apakah ada hubungan antara variabel usia dengan variabel jam tap in?
5. Paycard Bank apa yang paling banyak digunakan?
6. Kapan terjadi lonjakan jumlah penumpang?
7. Siapa yang paling sering naik transjakarta?

**Hasil Analisis**

Untuk menganalisis data, saya menggunakan pandas, seaborn, dan matplotlib.pyplot.
Untuk membuat dashboard, saya menggunakan tableau yang bisa diakses di [sini](https://public.tableau.com/views/TransjakartaDashboard_17313362769770/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link).

Berdasarkan **gender**, diperoleh piechart berikut.

![image](https://github.com/user-attachments/assets/af2b3b69-43f2-43c8-ba80-9597a3b3f707)

Insight yang kita peroleh adalah penumpang perempuan lebih banyak daripada penumpang laki-laki.

Berdasarkan **kategori usia**, diperoleh barchart berikut.

![image](https://github.com/user-attachments/assets/99a46746-f74d-4658-8c6e-e684a6e5112f)

Dari chart tersebut, kita peroleh bahwa dari kategori 11-20 tahun sampai dengan kategori 31-40 tahun, jumlah penumpang terus bertambah. Setelah kategori 40 tahun, jumlah penumpang semakin menurun. Penumpang terbanyak adalah penumpang di kategori usia 31-40 tahun.

Hubungan variabel usia dengan harga transjakarta dapat dilihat dari scatterplot berikut.

![image](https://github.com/user-attachments/assets/070c513c-5085-4607-935a-7afde8a60cce)

Hubungan variabel usia dengan waktu tap in dapat dilihat dari scatterplot berikut.

![image](https://github.com/user-attachments/assets/1646c957-d808-4960-a9a3-650e15209cd5)

Dari kedua scatterplot tersebut, dapat kita lihat bahwa variabel usia tidak memiliki hubungan dengan harga transjakarta maupun dengan waktu tap in.

Berdasarkan **paycard bank** yang digunakan penumpang, diperoleh barchart berikut.

![image](https://github.com/user-attachments/assets/2fa9b2ad-d60b-41f8-8789-bb079010a96a)

Dari chart tersebut, kita peroleh paycard yang paling banyak digunakan oleh para penumpang adalah paycard dari Bank DKI.

Berdasarkan **waktu tap in**, diperoleh waktu lonjakan jumlah penumpang.
1. Berdasarkan **jam tap in**, diperoleh line chart berikut.

![image](https://github.com/user-attachments/assets/425d2340-5f9e-44b7-a18e-68e45a487907)

Kita peroleh waktu terjadi lonjakan jumlah penumpang adalah pada jam 6 pagi dan jam 5 sore, dimana jam 6 pagi ini adalah waktu berangkat kerja atau berangkat sekolah dan jam 5 sore ini adalah waktu pulang bekerja atau pulang sekolah.

2. Berdasarkan **hari tap in**, diperoleh bar chart berikut.

![image](https://github.com/user-attachments/assets/7b7fd7fe-94cc-47a7-9c1c-45f222aa35b2)

Kita peroleh bahwa penumpang lebih banyak menggunakan transjakarta pada waktu weekdays (Senin-Jumat).

Berdasarkan **frekuensi naik transjakarta**, kita peroleh distribusi frekuensinya sebagai berikut.

![image](https://github.com/user-attachments/assets/0422cf10-65c5-4c99-94aa-1311d3e91b25)

Dari boxplot tersebut, kita peroleh frekuensi terkecilnya adalah 1 kali, sedangkan frekuensi terbanyaknya adalah 40 kali. Median dari data frekuensi tersebut adalah 9 kali.

Kita juga bisa melihat persebarannya menggunakan histogram sebagai berikut.

![image](https://github.com/user-attachments/assets/88cb20cb-4c5b-47c8-856a-48b7d517c00a)

Bisa dilihat bahwa lebih banyak penumpang yang naik transjakarta hanya 1-5 kali saja dalam satu bulan.

Selanjutnya, kita tarik data 10 penumpang **tersering** menggunakan transjakarta. Diperoleh data berikut.

![image](https://github.com/user-attachments/assets/72ecc792-8bfd-434f-b345-7180ab8aa809)

**Kesimpulan**

Dari analisis tersebut, kita peroleh:
1. Proporsi penumpang perempuan lebih besar daripada proporsi penumpang laki-laki.
2. Kategori usia yang paling banyak naik transjakarta adalah kategori 31-40 tahun, dimana kategori ini adalah kategori usia produktif. Semakin tua usianya, maka jumlah penumpang transjakarta semakin sedikit.
3. Tidak ada hubungan antara variabel usia dengan harga transjakarta dan dengan waktu tap in.
4. Paycard yang sering digunakan adalah paycard Bank DKI.
5. Lonjakan jumlah penumpang terjadi di jam 6 pagi dan jam 5 sore. Berdasarkan harinya, penumpang transjakarta lebih banyak pada weekdays daripada saat weekends.
6. Diperoleh 10 penumpang tersering menggunakan transjakarta dan dari persebaran data frekuensinya, kita peroleh lebih banyak penumpang yang naik transjakarta hanya 1-5 kali saja dalam sebulan.

**Rekomendasi**

1. Membuat program loyalitas dengan harapan dapat mempertahankan penumpang yang memang sudah sering menggunakan transjakarta dan menarik minat masyarakat lainnya untuk menggunakan transjakarta. Program loyalitas ini bisa dengan mendapatkan poin jika mereka naik transjakarta. Poin ini nantinya bisa ditukar atau diredeem, bisa dengan kesempatan naik transjakarta secara gratis ataupun bisa bekerjasama dengan merchant-merchant lain agar poin ini dapat ditukar saat membeli barang di merchant tersebut.
2. Membuat program khusus pelajar, dengan memberikan harga khusus pelajar/mahasiswa.

Rekomendasi lainnya, tentu tentang kenyamanan penumpang. Dengan dijaganya kebersihan dan ketertiban di dalam transjakarta, juga haltenya, tentunya penumpang akan semakin senang menggunakan transjakarta. Pembangunan sarana dan prasarana di halte juga dapat menarik minat calon penumpang, seperti adanya AC, toilet, tempat isi saldo kartu, dan mesin untuk membeli minuman, wifi, bisa membuat calon penumpang lebih nyaman ketika menunggu bus di halte.

Sekian hasil analisis saya tentang karakteristik penumpang transjakarta untuk meningkatkan jumlah penumpang. Tentunya ini masih sangat banyak kekurangannya dan saya sangat berharap feedback dari teman-teman untuk menjadi pelajaran bagi saya ke depannya.

Sampai jumpa di lain kesempatan! See ya!







