## JOBSHEET 7

## PERULANGAN 1

### Tujuan

Mahasiswa mampu menyelesaikan permasalahan/studi kasus menggunakan sintaks perulangan 1 dan mengimplemantasikannya dalam bahasa pemrogaman java.

### Alat dan Bahan
+ PC/laptop
+ Browser(chrome, firefox, safari)
+ Koneksi internet

### Praktikum

#### Percobaan 1 : Penggunaan for, while dan do-while

#### Waktu percobaan : 40 menit

1. Perhatikan flowchart perulangan for dibawah ini!

    <p align="left">
    <img width="197" height="259" src="images/flowchartFaktorial.png">
    </p>
    

> Flowchart diatas digunakan untuk menghitung nilai faktorial, selanjutnya kita akan membuat programnya berdasarkan
> flowchart di atas!

2. Tambahkan library Scanner, deklarasi Scanner, dan buat variabel angka untuk menampung data yang diinput melalui keyboard




```Java
// Ketik kode program di bawah sini
import java.util.Scanner;
int angka, faktorial = 1;

Scanner s = new Scanner(System.in);

System.out.print("Input angka: ");
angka = s.nextInt();
for(int i = 1; i<= angka; i++){
    faktorial = faktorial * i;
    System.out.printf("i = %d hasilnya adalah %d\n",i,faktorial);
}
System.out.println("Hasilnya adalah "+faktorial);
```

    Input angka: 7
    i = 1 hasilnya adalah 1
    i = 2 hasilnya adalah 2
    i = 3 hasilnya adalah 6
    i = 4 hasilnya adalah 24
    i = 5 hasilnya adalah 120
    i = 6 hasilnya adalah 720
    i = 7 hasilnya adalah 5040
    Hasilnya adalah 5040


3. Buatlah deklarasi dan inisialisasi variabel faktorial sesuai dengan flowchart diatas


```Java
// Ketik kode program di bawah sini
int angka, faktorial = 1;
System.out.print("Input angka: ");
angka = s.nextInt();
for(int i = 1; i <= angka; i++){
    faktorial = faktorial * i;
    System.out.printf("i = %d hasilnya adalah %d\n",i,faktorial);
}
System.out.println("Hasilnya adalah "+faktorial);
```

    Input angka: 7
    i = 1 hasilnya adalah 1
    i = 2 hasilnya adalah 2
    i = 3 hasilnya adalah 6
    i = 4 hasilnya adalah 24
    i = 5 hasilnya adalah 120
    i = 6 hasilnya adalah 720
    i = 7 hasilnya adalah 5040
    Hasilnya adalah 5040


4. Tambahkan struktur perulangan untuk menghitung hasil faktorial sebuah nilai yang diinputkan menggunakan for
    
    <p align="left">
    <img width="696" height="124" src="images/for.jpg" align="left">
    </p>


```Java
// Ketik kode program di atas di bawah sini
int angka, faktorial = 1;
System.out.println("====PROGRAM MENGHITUNG NILAI FAKTORIAL DENGAN FOR====");
System.out.print("Masukkan Bilangan : ");
angka = s.nextInt();
for(int i=1; i<=angka; i++)
    faktorial*=i;
System.out.print("Nilai faktorial bilangan tersebut adalah : "+ faktorial)
```

    ====PROGRAM MENGHITUNG NILAI FAKTORIAL DENGAN FOR====
    Masukkan Bilangan : 7
    Nilai faktorial bilangan tersebut adalah : 5040

5. Ubah nilai variabel faktorial seperti semula. Kemudian gunakan struktur perulangan while untuk menghitung hasil faktorial sebuah nilai yang diinputkan
    
    <p align="left">
    <img width="696" height="124" src="images/while.jpg" align="left">
    </p>


```Java
// Ketik kode program di atas di bawah sini
int angka, faktorial = 1;
faktorial=1;
System.out.println("====PROGRAM MENGHITUNG NILAI FAKTORIAL DENGAN WHILE====");
System.out.print("Masukkan Bilangan : ");
angka= s.nextInt();
int i=1;
while(i<=angka){
    faktorial*=i;
    i++;
}
System.out.print("Nilai faktorial bilangan tersebut adalah : "+ faktorial);
```

    ====PROGRAM MENGHITUNG NILAI FAKTORIAL DENGAN WHILE====
    Masukkan Bilangan : 7
    Nilai faktorial bilangan tersebut adalah : 5040

6. Kembalikan lagi nilai variabel faktorial seperti semula. Gunakan struktur perulangan do-while untuk menghitung hasil faktorial sebuah nilai yang diinputkan
    
    <p align="left">
    <img width="696" height="124" src="images/dowhile.jpg" align="left">
    </p>


```Java
// Ketik kode program di atas di bawah sini
faktorial=1;
System.out.println("=====PROGRAM MENGHITUNG NILAI FAKTORIAL DENGAN DO-WHILE=====");
System.out.print("Masukkan Bilangan : ");
angka= s.nextInt();
int i=1;
do{
    faktorial*=i;
    i++;
}
while(i<=angka);
System.out.print("Nilai faktorial bilangan tersebut adalah : "+ faktorial);
```

    =====PROGRAM MENGHITUNG NILAI FAKTORIAL DENGAN DO-WHILE=====
    Masukkan Bilangan : 7
    Nilai faktorial bilangan tersebut adalah : 5040

##### Pertanyaan
1. Pada program diatas, apakah kegunaan baris berikut?
<p align="left">
    <img src="images/hitungFaktorial.jpg" align="left">
    </p>

// Ketik jawaban disini
untuk mendeklarasikan operasi pada faktorial

2. Modifikasi program diatas dibagian struktur pemilihannya sehingga hasilnya menjadi seperti di bawah ini:
<p align="left">
    <img src="images/modifP1.jpg" align="left">
    </p>


```Java
// Ketik kode program di atas di bawah sini
faktorial=1;
System.out.println("=====PROGRAM MENGHIUNG NILAI FAKTORIAL");
System.out.print("Masukkan Bilangan : ");
angka = s.nextInt();

System.out.print(angka + "Faktorial = ");
for(int i=1; i<=angka; i++){
    faktorial*=i;
    System.out.printf(i + "x");
}
System.out.printf(" = "+faktorial);
```

    =====PROGRAM MENGHIUNG NILAI FAKTORIAL
    Masukkan Bilangan : 7
    7Faktorial = 1x2x3x4x5x6x7x = 5040




    java.io.PrintStream@601dd608



#### Percobaan 2 : Keluar dari perulangan menggunakan break

#### Waktu percobaan : 40 menit

1. Buatlah perulangan dengan menggunakan for yang memanfaatkan keyword break
<p align="left">
    <img width="696" height="124" src="images/for2.jpg" align="left">
    </p>


```Java
// Ketik kode program di atas di bawah sini
Scanner input=new Scanner(System.in);
int angka,total;
System.out.println("===PROGRAM FOR LOOP DENGAN BREAK===");
for(total=0;true;){
    System.out.print("Masukkan Bilangan : ");
    angka=input.nextInt();
    total+=angka;
    if(total>50) break;
}
System.out.println("Jumlah angka-angka yang telah dimasukkan : "+total);

```

    ===PROGRAM FOR LOOP DENGAN BREAK===
    Masukkan Bilangan : 35
    Masukkan Bilangan : 60
    Jumlah angka-angka yang telah dimasukkan : 95


2. Buat perulangan yang sama dengan struktur perulangan while
<p align="left">
    <img width="696" height="124" src="images/while2.jpg" align="left">
    </p>


```Java
// Ketik kode program di atas di bawah sini
int angka,total;
System.out.println("===PROGRAM WHILE LOOP DENGAN BREAK===");
total=0;
while(true){
    System.out.print("Masukkan Bilangan : ");
    angka=input.nextInt();
    total+=angka;
    if(total>50) break;
}
System.out.println("Jumlah angka-angka yang telah dimasukkan : "+total);
```

    ===PROGRAM WHILE LOOP DENGAN BREAK===
    Masukkan Bilangan : 40
    Masukkan Bilangan : 88
    Jumlah angka-angka yang telah dimasukkan : 128


3. Tuliskan perulangan diatas dalam struktur do-while
    <p align="left">
    <img width="696" height="124" src="images/dowhile2.jpg" align="left">
    </p>


```Java
// Ketik kode program di atas di bawah sini
int angka,total;
System.out.println("===PROGRAM DO-WHILE LOOP DENGAN BREAK===");
total=0;
do
{
    System.out.print("Masukkan Bilangan : ");
    angka=input.nextInt();
    total+=angka;
    if(total>50) break;
}
while(true);
System.out.println("Jumlah angka-angka yang telah dimasukkan : "+total);
```

    ===PROGRAM DO-WHILE LOOP DENGAN BREAK===
    Masukkan Bilangan : 45
    Masukkan Bilangan : 90
    Jumlah angka-angka yang telah dimasukkan : 135


##### Pertanyaan
1. Jelaskan fungsi kode program yang telah dibuat pada percobaan diatas!

// Ketik jawaban disini
menjumlahkan angka yang akan berhenti jika hasil lebih dari 50. Sedangkan percobaan 3 menjumlahkan angka yang kurang dari 50 dan menghitung rata-ratanya.

2. Jelaskan fungsi kode berikut!
    <p align="left">
    <img src="images/forPertanyaan2.jpg" align="left">
    </p>


// Ketik jawaban disini
jika angka yang dimasukkan lebih dari 50 maka akan langsung dilanjutkan ke perintah berikutnya tanpa dilakukan perhitungan.

#### Percobaan 3 : Keluar dari step perulangan menggunakan continue

#### Waktu percobaan : 40 menit

1. Buat program looping menggunakan struktur perulangan for seperti di bawah ini: 
<p align="left">
    <img src="images/forContinue.jpg" align="left">
    </p>



```Java
// Ketik kode program di atas di bawah sini
Scanner input=new Scanner(System.in);
int angka, total, count;
double avg;
count=0;
System.out.println("===PROGRAM FOR LOOOP DENGAN CONTINUE===");
for(int i=0;i<5;i++){
    System.out.print("Masukkan Bilangan : ");
    angka=input.nextInt();
    if(angka>=50) continue;
    total+=angka;
    count++;
}
System.out.println("Jumlah angka-angka yang kurang dari 59: "+total);
avg=(double)total/count;
System.out.println("Rata-rata angka yang kurang dari 50: "+avg);
```

    ===PROGRAM FOR LOOOP DENGAN CONTINUE===
    Masukkan Bilangan : 34
    Masukkan Bilangan : 27
    Masukkan Bilangan : 33
    Masukkan Bilangan : 48
    Masukkan Bilangan : 30
    Jumlah angka-angka yang kurang dari 59: 172
    Rata-rata angka yang kurang dari 50: 34.4



```Java
5. Jalankan program. Amati apa yang terjadi!
```

##### Pertanyaan
1. Jelaskan Perbedaan dari percobaan 2 dan percobaan 3

// Ketik jawaban disini
Scanner s=new Scanner(System.in); digunakan untuk mendeklarasikan Scanner, int angka, total; digunakan untuk mendeklarasikan variabel yang dibutuhkan, for(total = 0; true;) digunakan untuk mendeklarasikan exp1 dan exp2, angka = s.nextInt(); digunakan untuk memasukkan angka dari keyboard, total+=angka; digunakan untuk operasi perhitungan total, if(total>50) break; digunakan jika nilai total sudah lebih dari 50 maka proses selesai.

2. Jelaskan apa fungsi perintah kode program dibawah ini?
<p align="left">
    <img width="352" height="79" src="images/continuePertanyaan.jpg" align="left">
    </p>

// Ketik jawaban disini
Fungsi kode program diatas adalah untuk mendeklarasikan ekspresi 1 dan 2 dalam break.

### Tugas

#### Waktu pengerjaan Tugas: 140 menit

1. Buatlah program yang meminta masukan user sebuah bilangan bulat N (N > 0). Program kemudian menampilkan penjumlahan N bilangan genap positif pertama (bilangan genap ≥ 0).
Contoh: 
    •	Jika user memasukkan N = 10, program akan menghitung banyaknya jumlah bilangan positive di dalam range bilangan 1-10   kemudian menampilkan penjumlahan bilangan positive bilangan bilangan diantara 1-10 yaitu : 
        0 + 2 + 4 + 6 + 10 = 30. 
        Setelah itu program akan menampilkan rata-rata dari bilangan positive yang telah dijumlahkan tadi.
    •	Contoh output program dan flowchart
<br/><img width="303" height="529" src="images/hasilTugasFc.jpg" align="left"><br/>
  

<br/><img width="303" height="529" src="images/fcTugasJS7.png" align="left">



```Java
// Ketik kode program disini
int bil, jmlBilGenap, totalGenap = 1;
double avg;

System.out.print("Masukkan angka: ");
bil = s.nextInt();
jmlBilGenap = bil / 2;

System.out.printf("Banyaknya bilangan genap dari 1 sampai %d adalah %d\n",bil,jmlBilGenap);
System.out.print("Angka genap dalam range tersebut adalah");
for(int i=1;i<=bil;i++)
{
    if(i%2!=0)continue;
    System.out.printf(", %d",i);
    totalGenap += i;
}
avg = (double)(totalGenap-1) / jmlBilGenap;
System.out.printf("\nHasil penjumlahan bilangan genap dari 1 sampai %d adalah %d",bil,totalGenap-1);
System.out.printf("\nRata-rata bilangan genap dari 1 sampai %d adalah %.1f",bil,avg);
```

    Masukkan angka: 14
    Banyaknya bilangan genap dari 1 sampai 14 adalah 7
    Angka genap dalam range tersebut adalah, 2, 4, 6, 8, 10, 12, 14
    Hasil penjumlahan bilangan genap dari 1 sampai 14 adalah 56
    Rata-rata bilangan genap dari 1 sampai 14 adalah 8.0




    java.io.PrintStream@601dd608



2. Buatlah program untuk menampilkan angka 1 hingga angka masukan pengguna secara berurutan dan melompati angka kelipatan 5. Seperti tampilan di bawah ini
<p align="left">
<img width="184" height="328" src="images/tugas1.jpg" align="left">
</p>


```Java
// Ketik kode program disini
import java.util.Scanner;
Scanner s=new Scanner(System.in);
int x, i;
System.out.print("Masukkan Bilangan : ");
    i = s.nextInt();

for(x=1; x<=i; x++) {
if (x%5==0) continue;
System.out.println(x);
}
```

    Masukkan Bilangan : 19
    1
    2
    3
    4
    6
    7
    8
    9
    11
    12
    13
    14
    16
    17
    18
    19


3. Buatlah sebuah program yang menampilkan deret bilangan fibonacci sebagai berikut. Dimana bilangan yang terletak di sebelah kanan adalah hasil penjumlahan dari 2 bilangan sebelumnya
 <p align="left">
    <img width="451" height="226" src="images/fibo.png" align="left">
    </p>



```Java
// Ketik kode program disini
import java.util.Scanner;
        int limit, past, current, fibonacci;
        Scanner input = new Scanner(System.in);
        System.out.print("Masukan banyak bilangan yang mau ditampilkan: ");
        limit = input.nextInt();
        past = 0;
        current = 1;
        fibonacci = 1;
        for (int i =1; i <= limit; i++){
            fibonacci = past + current;
            System.out.printf("sumof: %d + %d = %d\n",past,current,fibonacci);
            past = current;
            current = fibonacci;
        }
```

    Masukan banyak bilangan yang mau ditampilkan: 10
    sumof: 0 + 1 = 1
    sumof: 1 + 1 = 2
    sumof: 1 + 2 = 3
    sumof: 2 + 3 = 5
    sumof: 3 + 5 = 8
    sumof: 5 + 8 = 13
    sumof: 8 + 13 = 21
    sumof: 13 + 21 = 34
    sumof: 21 + 34 = 55
    sumof: 34 + 55 = 89

