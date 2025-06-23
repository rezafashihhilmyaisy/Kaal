---
title: Invers Aljabar Matriks

---

# Invers Aljabar Matriks




---

##  1. Pengertian Matriks

Matriks adalah **susunan bilangan** dalam bentuk baris dan kolom yang dituliskan di dalam tanda kurung siku atau biasa.
Contoh matriks ukuran $2 \times 3$:

$$
A = \begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{bmatrix}
$$

Keterangan:

* Ukuran matriks = jumlah baris × jumlah kolom
* Contoh: Matriks $A$ berukuran $2 \times 3$

---

## 2. Jenis-jenis Matriks

1. **Matriks Baris**: Hanya terdiri dari 1 baris. Contoh:

   $$
   A = [1 \ 2 \ 3 ]
   $$

2. **Matriks Kolom**: Hanya terdiri dari 1 kolom. Contoh:

   $$
   A = \begin{bmatrix}
   1 \\
   2 \\
   3
   \end{bmatrix}
   $$

3. **Matriks Persegi**: Jumlah baris = jumlah kolom. Contoh:

   $$
   A = \begin{bmatrix}
   1 & 2 \\
   3 & 4
   \end{bmatrix}
   $$

4. **Matriks Nol**: Semua elemennya 0.

5. **Matriks Identitas**: Matriks diagonal dengan nilai 1. Contoh:

   $$
   I_3 = \begin{bmatrix}
   1 & 0 & 0 \\
   0 & 1 & 0 \\
   0 & 0 & 1
   \end{bmatrix}
   $$

---

##  3. Operasi Dasar Matriks

### a) Penjumlahan dan Pengurangan

Hanya bisa dilakukan jika ukuran matriks **sama**.
Contoh:

$$
A = \begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix},
B = \begin{bmatrix}
5 & 6 \\
7 & 8
\end{bmatrix}
$$

Penjumlahan:

$$
A + B = \begin{bmatrix}
1+5 & 2+6 \\
3+7 & 4+8
\end{bmatrix}
= \begin{bmatrix}
6 & 8 \\
10 & 12
\end{bmatrix}
$$

### b) Perkalian Skalar

$$
k \cdot A = \begin{bmatrix}
k \cdot a_{11} & k \cdot a_{12} \\
k \cdot a_{21} & k \cdot a_{22}
\end{bmatrix}
$$

---

##  4. Perkalian Matriks

Dapat dilakukan jika jumlah kolom matriks pertama = jumlah baris matriks kedua.

Contoh:

$$
A_{2\times3} \times B_{3\times2}
$$

Hasil:

$$
C_{2\times2}
$$

Rumus:

$$
C_{ij} = \sum_{k=1}^{n} A_{ik} \cdot B_{kj}
$$

Contoh:

$$
A = \begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{bmatrix},
B = \begin{bmatrix}
7 & 8 \\
9 & 10 \\
11 & 12
\end{bmatrix}
$$

Hasil:

$$
C = \begin{bmatrix}
1\cdot7 + 2\cdot9 + 3\cdot11 & 1\cdot8 + 2\cdot10 + 3\cdot12 \\
4\cdot7 + 5\cdot9 + 6\cdot11 & 4\cdot8 + 5\cdot10 + 6\cdot12
\end{bmatrix}
$$

---

##  5. Transpos Matriks

Baris dijadikan kolom, dan kolom dijadikan baris.

Contoh:

$$
A = \begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix}
\Rightarrow
A^T = \begin{bmatrix}
1 & 3 \\
2 & 4
\end{bmatrix}
$$

---

##  6. Determinan Matriks

Hanya berlaku untuk matriks persegi.

Contoh $2 \times 2$:

$$
A = \begin{bmatrix}
a & b \\
c & d
\end{bmatrix}
\Rightarrow \text{Det}(A) = ad - bc
$$

Contoh $3 \times 3$: Aturan Sarrus atau ekspansi kofaktor.

---

##  7. Invers Matriks

Hanya untuk matriks persegi dengan $\text{Det}(A) \ne 0$.
Untuk $2 \times 2$:

$$
A = \begin{bmatrix}
a & b \\
c & d
\end{bmatrix}
\Rightarrow A^{-1} = \frac{1}{ad-bc}
\begin{bmatrix}
d & -b \\
-c & a
\end{bmatrix}
$$

---

##  8. Aplikasi Aljabar Matriks

* **Sistem Persamaan Linear** (dapat diselesaikan dengan matriks invers atau metode eliminasi Gauss).
* **Transformasi Geometri** (dalam grafika komputer).
* **Ekonomi** (model input-output).
* **Statistik** (analisis data dengan matriks).

---



---

## 1. Pengertian Invers Matriks

Invers dari sebuah matriks $A$ (dilambangkan $A^{-1}$) adalah matriks yang bila dikalikan dengan $A$ menghasilkan **matriks identitas**:

$$
A \times A^{-1} = A^{-1} \times A = I
$$

---

## 2. Syarat Ada Invers

* Matriks harus **berbentuk persegi** (n×n).
* Determinan $A$ tidak sama dengan nol ( $\text{det}(A) \ne 0$ ).

---

##  3. Invers Matriks $( 2 \times 2 \ )$

Contoh:

$$
A = \begin{bmatrix}
a & b \\
c & d
\end{bmatrix}
$$

Rumus:

$$
A^{-1} = \frac{1}{ad-bc}
\begin{bmatrix}
d & -b \\
-c & a
\end{bmatrix}
$$

---

### Contoh Soal $2 \times 2$:

$A = \begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix}$

1. Hitung determinan:
   $\text{Det}(A) = 1 \times 4 - 2 \times 3 = 4 - 6 = -2$

2. Hitung invers:

$$A^{-1} = \frac{1}{-2}
\begin{bmatrix} 4 & -2 \\-3 & 1\end{bmatrix}$$
=
\begin{bmatrix}
-2 & 1 \\
1.5 & -0.5
\end{bmatrix}
$$

---

##  4. Invers Matriks $3 \times 3$

Untuk matriks:

$$
A = \begin{bmatrix}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33}
\end{bmatrix}
$$

Invers dapat dicari dengan langkah:

1. Hitung **Det(A)**.
2. Hitung **matriks kofaktor** dari masing-masing elemen.
3. Susun matriks kofaktor, buat **matriks adjoin** dengan cara transpose dari matriks kofaktor.
4. Hitung invers:

   $$
   A^{-1} = \frac{1}{\text{Det}(A)} \cdot \text{Adj}(A)
   $$

---

###  Contoh Soal $3 \times 3$

$A = \begin{bmatrix}
1 & 2 & 3 \\
0 & 1 & 4 \\
5 & 6 & 0
\end{bmatrix}$

####  Hitung Determinan $A$

$$
\text{Det}(A) = 1 \cdot (1 \times 0 - 4 \times 6) 
           - 2 \cdot (0 \times 0 - 4 \times 5) 
           + 3 \cdot (0 \times 6 - 1 \times 5)
$$

$$
= 1 \cdot (-24) - 2 \cdot (-20) + 3 \cdot (-5) 
= -24 + 40 - 15 = 1
$$

####  Hitung Matriks Kofaktor

Kofaktor $C_{ij}$ = $(-1)^{i+j}$ dikali determinan submatriks $A$ setelah menghapus baris $i$ dan kolom $j$.

Contoh:

* $C_{11} = +\text{Det} \begin{vmatrix}
  1 & 4 \\
  6 & 0
  \end{vmatrix} = (1)(0) - (4)(6) = -24$

Hitung semua kofaktor hingga dapat matriks kofaktor $C$.

####  Transpos Matriks Kofaktor

Adjoint $A$ = $C^T$

####  Invers

Karena $\text{Det}(A) = 1$,

$$
A^{-1} = \text{Adj}(A)
$$

---

## 5. Metode Lain: Operasi Baris Elementer

Selain dengan metode kofaktor, invers juga dapat dicari dengan metode:

$$
[A|I] \to [I|A^{-1}]
$$

Contoh:

$$
\underbrace{\begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix}}_{A}
\Big| 
\underbrace{\begin{bmatrix}
1 & 0 \\
0 & 1
\end{bmatrix}}_{I}
\to
\underbrace{\begin{bmatrix}
1 & 0 \\
0 & 1
\end{bmatrix}}_{I}
\Big| 
\underbrace{\begin{bmatrix}
-2 & 1 \\
1.5 & -0.5
\end{bmatrix}}_{A^{-1}}
$$

---

# Tugas 

mecari 3 sistem persamaan linier yang hasilnya 1,0,0

$x+2y+3z=1$
$4x+5y+6z=0$
$7x+8y+10z=0$

Sekarang, saya akan menghitung invers dari matriks 
𝐴 dan mengalikannya dengan vektor 𝐵

Hasil dari $A^{-1}$ x $B$ adalah [−0.667,−0.667,1.0]
[−0.667,−0.667,1.0], yang tidak sesuai dengan hasil yang diminta(1,0,0). Saya akan mencoba mencari sistem persamaan lain yang memenuhi syarat.

Hasil dari $A^{-1}$ x $B$ adalah (0.75,0.5,−1.25), yang masih belum sesuai dengan (1,0,0). Saya akan mencoba mencari sistem persamaan yang lebih tepat

Saya telah menemukan sistem persamaan yang memenuhi syarat.

$1x + 2y + 3z = 1$
$0x +1y +4z = 0$
$0x + 0y + 1z = 0$

Dengan sistem ini, Hasil dari $A^{-1}$ x $B$ adalah (1,0,0)