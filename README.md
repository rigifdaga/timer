**1.2. Understanding how it works.**  

![](1.2.png)  
Dari hasil pengamatan output, dapat kita pahami bahwa fungsi async akan dijalankan di luar dari fungsi utama yang memanggilnya. Sehingga, "hey hey" bisa saja ditampilkan lebih dulu sebelum "howdy!" dan "done!" karena "hey hey" berada di luar fungsi async. Fungsi tersebut akan melanjutkan eksekusi program dan menjalankan `println!("hey hey");` sementara fungsi async masih menunggu hasil dari future.