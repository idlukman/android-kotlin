# Perulangan

**Looping** atau dalam bahasa indonesia di sebut dengan **perulangan** merupakan fungsi pada pemrograman untuk mempermudah penulisan kode program yang tanpa harus menulis program tersebut berulang-ulang pada bahasa pemograman android menggunakan kotlin.

<p>Berikut ini ada tiga macam jenis dari struktur kontrol pengulangan yaitu :</p>

1. while
2. do-while
3. for-loops

Cara penulisannya hampir sama dengan java namun ada beberapa perbedaan yang harus kalian ketahui. Struktur kontrol Pengulangan merupakan sebuah pernyataan dari Kotlin yang mengizinkan kita untuk mengeksekusi **blok code** atau **statement** secara berulang-ulang sesuai dengan jumlah tertentu yang diinginkan.

##### 1. Perulangan while

Pengulangan pernyataan memungkinkan kita untuk menentukan bahwa kode yang harus mengulangi tindakan sementara beberapa kondisi tetap benar

```json
while (kondisi) {
       // Pernyataan atau Statement
}
```

<p>Contoh program :</p>

```json
fun main(args: Array<String>){
    var angka = 0
    while(angka <= 5){
        println("Sukses")
        angka++
    }
}
```

![Foto](https://4.bp.blogspot.com/-pTkMSw6J8dI/WUUIDg--6VI/AAAAAAAAB4Q/XkWFW-G6rOM3lPFsXdV3d_q38OpMbMd8QCLcBGAs/s1600/Kotlin-Looping-Example1-min.jpg)

Jika kita jalankan, pernyataan yang terdapat pada pernyataan while akan terus dieksekusi hingga kondisi menjadi false, perintah **angka++** digunakan agar nilai pada variable angka terus bertambah 1 hingga kondisi pada while menjadi false dan program dihentikan.

Program tersebut akan mencetak kata “Berhasil” sebanyak 5 kali, Perlu kalian ingat jika bagian **angka++** dihilangkan, akan menghasilkan pengulangan yang terus menerus **(infinite loop)**. Pastikan agar kalian memberikan pernyataan yang membuat pengulangan berhenti pada suatu kondisi.

##### 2. Perulangan do-while

Peryataan do-while sama dengan pernyataan while yaitu untuk mengeksekusi pernyataan berulang-ulang selama kondisi true.

```json
do {
   // Pernyataan atau Statement
} while ( kondisi )
```

Perbedaannya, pernyataan pada pernyataan **_do_** akan dieksekusi terlebih dahulu sebelum dievaluasi kondisinya pada Pernyataan **_while_**, jika kondisi pada Peryataan **_while_** bernilai true, maka pernyataan pada **_do_** akan di eksekusi lagi secara berulang-ulang sampai bernilai false dan program dihentikan.

<p>Contoh Program sederhana dengan menggunakan do-while, seperti berikut ini : </p>

Menggunakan **[While](https://while.org)**.

```json
var angka = 0
    while(angka > 5){ //Menghasilkan Nilai False
        println("Sukses")
    }
```

<p>Jika kita jalankan, hasilnya akan seperti ini :</p>

![Foto](https://4.bp.blogspot.com/-LLnVnyvq3Z4/WUUqINF8aeI/AAAAAAAAB4k/RFHvvZgxzEEK-9O_0sUUvTW_Mqym4LYtACLcBGAs/s1600/Kotlin-Looping-Example3-min.jpg)

Menggunakan **[Do-While](https://do-while.org)**.

```json
var angka = 0
    do{
        println("Sukses")
    }while (angka > 5) //Menghasilkan Nilai False
```

<p>Jika kita jalankan, hasilnya akan seperti ini :</p>

![Foto](https://4.bp.blogspot.com/-oO1nMUuzEm8/WUUqChC0agI/AAAAAAAAB4g/r8VYOn6rxnYO0HawlfndMlSjakeDANGlACEwYBhgL/s1600/Kotlin-Looping-Example2-min.jpg)

Coba kalian perhatikan, pada program yang menggunakan while tidak akan menampilkan Output karena pernyataan pada statement while akan dieksekusi jika kondisi bernilai true, Jika pada do-while, pernyataan akan tetap di eksekusi walaupun bernilai false, itu karena, do-while akan mengeksekusi peryataan terlebih dahulu sebelum mengevaluasi kondisinya.

##### 3. Perulangan For

Penggunaan for loop pada kotlin lebih simple dan mudah dibandingkan dengan Java, kita bisa menggunakan for untuk mengeksekusi pernyataan secara berulang-ulang, tetapi penggunaannya lebih simple dibandingkan while dan do-while.

> for (variable(single/multiple variable) in expression) Pernyataan

atau

```json
for (variable(single/multiple variable) in expression) {
      // Pernyataan
}
```

Pada contoh berikut ini, misalnya kita ingin mencetak kata "Sukses" sebanyak 7 kali, maka kita tidak memerlukan kondisi true, seperti pada while dan do-while, seperti ini :

```json
fun main(args: Array<String>){
    for (data in 1..7) println("Sukses")
}
```

<p> Kita Jalankan Program tersebut : </p>

![Foto](https://3.bp.blogspot.com/-naLowm54Aqc/WUWerM_8-oI/AAAAAAAAB44/HzT9NXOJNccQxk5d9GX3UbAKFyAz3WsmACLcBGAs/s1600/Kotlin-Looping-Example4-min.jpg)

Disana terdapat sebuah variable Integer bernama data (Kalian bisa mengganti namanya sesuai keinginan), jadi program akan melooping sesuai dengan range atau jumlah item pada expression yang diberikan, dan expression tersebut menjadi suatu nilai dari variable item.

<p> Variable item akan mempunyai nilai dari expression, kita juga bisa mencetak veriable tersebut seperti ini : </p>

```json
fun main(args: Array<String>){
    for (data in 1..7) println(data)
}
```

<p> Hasilnya akan seperti berikut ini : </p>

![Foto](https://1.bp.blogspot.com/-DTb0dDZ3Wk4/WUWezQ28uPI/AAAAAAAAB48/srofjPVrJB41D6rJOzmPa-s9bSc4u_GagCLcBGAs/s1600/Kotlin-Looping-Example5-min.jpg)

Coba perhatikan gambar diatas, jika kita panggil data tersebut, nilai yang terdapat di sebelah kanan in akan keluar, itu artinya nilai tersebut bisa kita panggil melalui variable data, dan akan melooping sesuai dengan jumlah atau range pada nilai/expression tersebut.

</p> Jika masih belum paham, mari kita ke contoh berikutnya, Disini kita akan membuat sebuah List, dimana pada list tersebut akan kita isi beberapa item, lalu kita akan mencetak semua item tersebut menggunakan for loop, Seperti berikut ini : </p>

```json
fun main(args: Array<String>){
    val teman: List<String> = listOf("Wildan","Azis","Alvians","Ferdi")
    for(data in teman){
        data.let { println(it) }
    }
}
```

<p> Jika kita jalankan, hasilnya akan seperti gambar dibawah ini : </p>

![Foto](https://3.bp.blogspot.com/-8_bo9T5yjwY/WUXyga-zVJI/AAAAAAAAB5M/UoCM8uXMCGkqDtjSAumhQXNvePvHXMGTACLcBGAs/s1600/Kotlin-Looping-Example6-min.jpg)

Coba perhatikan, Program akan melooping sesuai jumlah item pada list yang terdapat pada variable teman, dikarenakan pada list tersebut berjumlah 4 item yaitu **"WIldan", "Azis", "Alvians", "Ferdi"**. Jadi program akan melooping sebanyak 4 kali.

Fungsi **[let](https://let.org)** yaitu untuk Memanggil blok fungsi yang ditentukan dengan nilai **[this](https://this.org)** sebagai argumennya dan mengembalikan hasilnya, lalu kita akan mencetak semua item pada list tersebut melalui variable data, dengan menggunakan fungsi **[it](https://it.org)**.
