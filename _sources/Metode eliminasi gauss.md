---
title: Metode eliminasi gauss

---

# Metode eliminasi gauss
## pengertian metode gauss
Eliminasi Gauss adalah suatu metode untuk mengoperasikan nilai-nilai di dalam matriks sehingga menjadi matriks yang lebih sederhana lagi. Dengan melakukan operasi baris sehingga matriks tersebut menjadi matriks yang baris. Ini dapat digunakan sebagai salah satu metode penyelesaian persamaan linear dengan menggunakan matriks. Caranya dengan mengubah persamaan linear tersebut ke dalam matriks teraugmentasi dan mengoperasikannya. Setelah menjadi matriks baris, lakukan substitusi balik untuk mendapatkan nilai dari variabel-variabel tersebut.

### penyelesaian

2𝑥+𝑦−𝑧=8
−3𝑥−𝑦+2𝑧=−11
−2𝑥+𝑦+2𝑧=−3

1. Langkah 1: Bentuk matriks augmented

2 1 -1    | 8
-3 -1 2   |-11
-2 1 2    |-3

2. Langkah 2: Eliminasi baris pertama

- Kita kalikan baris pertama dengan 3 dan tambahkan ke baris kedua:

$R_2 => R_2+3 R_1$

- Kita kalikan baris pertama dengan 2 dan tambahkan ke baris ketiga:

$R_3=>R_3+2 R_1$

Hasilnya:

2 1 -1  |8
0 2 -1  |13
0 3 0   |13

3. Langkah 3: Eliminasi baris kedua

- Kita kalikan baris kedua dengan 3 dan dan tambahkan ke baris kedua:

$R_2 => R_2+3 R_1$

- Kita kalikan baris pertama dengan 2 dan tambahkan ke baris ketiga:

$R_3 => R_3+2 R_1$

Hasilnya:

2 1 -1  |8 
0 2 -1  |13
0 3 0   |13

4. Langkah 3: Eliminasi baris kedua

- Kita kalikan baris kedua dengan 3 dan kurangkan dari baris ketiga:

$R_3=>R_3-2R_2$

Hasilnya:

2 1 -1  |8
0 2 -1  |13
0 0 1.5 |1.5

5. Langkah 4: Bentuk eselon baris atas

- Kita bagi baris ketiga dengan 1.5 untuk mendapatkan elemen pivot 1:

$R_{3} = R_{3}/1.5$

Hasilnya:

2 1 -1 8 
0 2 -1 13
0 0 1  1

6. Langkah 5: Substitusi balik (back substitution)

z = 1, y = 13 - (- 1 . 1) = 14, x = 8 - 1/2 . 14 = 1

Jadi, solusi dari sistem persamaan linear ini adalah:

x = 1 , y = 7 , z = 1

hasil dari grafis geogebra
![geogebra-export](https://hackmd.io/_uploads/B1wCc8QjJx.png)
[https://www.geogebra.org/classic/k7aht8zx](https://)