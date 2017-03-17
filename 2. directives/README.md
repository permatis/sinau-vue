## 2. Directives
Pada latihan kedua ini yaitu menampilkan atau memanipulasi data didalam element. Maksudnya menampilkan nilai didalam attribut dan atau menampilkan text didalam element.

* copy file `example.html`. 
* kemudian kita membuat element input yang didalamnya ditambahkan attribut `v-text`. Atrribut `v-text` inilah yang dinamakan **directive**. Directive menggunakan prefix `v-` merupakan attribut khusus yang mengindikasikan menggunakan vue. Directive ini akan menerapkan perilaku reaktif khusus untuk merender DOM. Attribut `v-text` merupakan salah satu dari macam directive yang ada di vue.

Berikut ini adalah beberapa directive beserta fungsinya di latihan 2. 
*. Directive `v-text` digunakan untuk menampilkan text didalam element. Sama halnya menggunakan double bracket / mustache `{{ property }}` didalam element.
* Directive `v-html` digunakan untuk menampilkan text didalam element namun akan merender jika didalam text tersebut terdapat element. Berbeda halnya dengan `v-text` akan menampilkan sama seperti nilainya.
* Directive `v-show` digunakan untuk menampilkan nilai jika nilainya true. Directive `v-show` ini akan menambahkan attribut `style=display:none` ketika nilainya false. Begitu juga sebaliknya, jika nilainya true maka attribut `style=display:none` akan hilang.
* Directive `v-if` dan `v-else` digunakan untuk menampilkan nilai jika nilainya true atau sebaliknya false. Directive `v-if` dan `v-else` ini akan menghilangkan element tersebut jika nilainya false. Begitu juga sebaliknya akan ditampilkan jika nilainya true.
* Directive `v-pre` digunakan menampilkan nilai asli dari dalam element. Tidak merender jika didalamnya terdapat mustache.
* Directive `v-once` digunakan untuk merender hanya satu kali. Nilai tidak dapat diubah.
* Directive `v-cloak` digunakan ketika ingin membuat style pada nilai tersebut karena dapat dikombinasikan dengan CSS seperti `[v-cloak]: { display:none }`. Nilai dalam property yang sudah di kompilasi didalam ViewModel akan rekompile. 
* Directive `v-model` digunakan ketika menggunakan input dan form binding. Jadi memanipulasi nilai pada inputan. 
* Directive `v-bind` digunakan ketika menambahkan sebuah nilai kedalam attribut. Berbeda dengan `v-model` yang hanya digunakan dalam inputan namun dapat memanipulasi nilai. 
* Directive `v-for` digunakan untuk membuat perulangan dari property yang sudah dikompilasi didalam ViewModel. Sama seperti perulangan pada pemogramanan lainnya. Penulisannya yaitu ` alias in dataArray`
* Directive `v-on` digunakan untuk handling event listener di element. Sebuah tipe event dilambangkan oleh argumen. Expression dapat menjadi sebuah nama method atau barisan pernyataan. atau sederhananya ketika expression tersebut dapat dirubah.