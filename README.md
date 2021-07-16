# PLC Traffic Light System
Pada projek ini digunakan disain sederhana dimana terdapat tiga tiang lampu lalu lintas di masing-masing simpang, hal ini dapat dilihat pada gambar 3.1 yang terdapat dibawah ini.

![Gambar 3.1 Sketsa Awal Desain Projek Lampu Lalu Lintas 3 Simpang](/images/logo.png)
 

Pada gambar 3.1 terlihat setiap persimpangan memiliki dua kotak lampu dimana salah satunya adalah lampu untuk pejalan kaki sedangkan satunya adalah lampu lalu lintas. Agar pengkabelan lebih efisien dan ringkas PLC diletakkan seperti pada gambar 3.1, sehingga dapat mengurangi penggunaan kabel yang terlalu Panjang dari PLC ke Lampu.
Untuk Pengaturan waktu hidupnya lampu sepenuhnya menggunakan timer build-in pada PLC sehingga sistem menjadi sensorless atau tanpa sensor. Lama waktu hidupnya lampu berturut turut yaitu merah 60 detik, hijau 20 detik, dan kuning 10 detik. Waktu yang digunakan dalam penyetelan lampu merah, kuning dan hijau adalah untuk keperluan simulasi sehingga dapat diubah sesuai dengan kondisi lapangan jika dibutuhkan.  


3.2 Material dan Komponen I/O
Material yang digunakan untuk Projek ini berupa PLC OMRON CJ1M, yang mana merupakan PLC yang memiliki 30 Port I/O dengan tegangan 24 VDC. Agar lebih jelas dapat dilihat pada Gambar 3.2
 
Gambar 3.2 PLC OMRON CJ1M 

Komponen – Komponen I/O yang digunakan untuk merealisasikan projek ini dapat dilihat pada table-tabel dibawah ini.
Tabel 3.1 Input Pada Sistem Lampu Lalu Lintas 3 Simpang
No	Peralatan Input	Terminal Input pada PLC
1	Push Button Start NO (Hijau)	0.00
2	Push Button Stop NC (Merah)	0.01
Tabel 3.2 Output Pada Sistem Lampu Lalu Lintas 3 Simpang
No	Peralatan Output	Terminal Output pada PLC
1	Lampu LED Hijau Simpang 1 (24 VDC)	1.00
2	Lampu LED Kuning Simpang 1 (24 VDC)	1.01
3	Lampu LED Merah Simpang 1 (24 VDC)	1.02
4	Lampu LED Pejalan Kaki Merah Simpang 1 (24 VDC)	1.03
5	Lampu LED Pejalan Kaki Hijau Simpang 1 (24 VDC)	1.04
6	Lampu LED Hijau Simpang 2 (24 VDC)	1.05
7	Lampu LED Kuning Simpang 2 (24 VDC)	1.06
8	Lampu LED Merah Simpang 2 (24 VDC)	1.07
9	Lampu LED Pejalan Kaki Merah Simpang 2 (24 VDC)	1.08
10	Lampu LED Pejalan Kaki Hijau Simpang 2 (24 VDC)	1.09
11	Lampu LED Hijau Simpang 3 (24 VDC)	1.10
12	Lampu LED Kuning Simpang 3 (24 VDC)	1.11
13	Lampu LED Merah Simpang 3 (24 VDC)	1.12
14	Lampu LED Pejalan Kaki Merah Simpang 3 (24 VDC)	1.13
15	Lampu LED Pejalan Kaki Hijau Simpang 3 (24 VDC)	1.14

Keterangan :
Lampu untuk projek ini diseragamkan menggunakan LED agar lebih terang dan hemat energi, serta digunkan LED dengan tegangan 24 VDC agar tidak membuang banyak pengeluaran pada relay dan power supply ataupun Konverter AC/DC.  

3.3 Sketsa Pengkabelan Peralatan I/O
Pada Sketsa Pengkabelan Peralatan I/O digunakan aplikasi ProfiCAD. Untuk hasil dari penggambaran sketsa pengkabelan dengan aplikasi tersebut dapat dilihat pada gambar 3.2

 
Gambar 3.3 Sketsa Pengkabelan Pada PLC OMRON CJ1M

Pada PLC CJ1M digunakan pengkabelan Input bertipe sourcing sedangkan output bertipe sinking, hal ini dilakukan agar tercapai pengkabelan yang efektif dan efisien. 
