---
title: Dot Product

---

# Dot Product

Dot product (atau **hasil kali titik**) adalah operasi matematika antara dua **vektor** yang menghasilkan **angka skalar** (bukan vektor lagi).

### Rumus Dot Product:

Kalau kamu punya dua vektor:

$$
\vec{A} = (a_1, a_2, \dots, a_n), \quad \vec{B} = (b_1, b_2, \dots, b_n)
$$

Maka dot product-nya:

$$
\vec{A} \cdot \vec{B} = a_1b_1 + a_2b_2 + \dots + a_nb_n
$$

### Contoh:

Misal:

$$
\vec{A} = \begin{bmatrix}2\\ 3 \end{bmatrix}, \quad \vec{B} = \begin{bmatrix} 4\\5 \end{bmatrix}
$$

$$
\vec{A} \cdot \vec{B} = (2)(4) + (3)(5) = 8 + 15 = 23
$$

Makna Dot Product
Kalau hasilnya positif, berarti sudut antar vektor < 90° (arah relatifnya mirip).

Kalau hasilnya nol, berarti vektornya tegak lurus (orthogonal).

Kalau hasilnya negatif, berarti sudut antar vektor > 90° (arah relatifnya berlawanan).

#### Noted

jika hasil dua vektor tersebut adalah 0 maka kedua vektor tersebut memiliki garis yang sejajar dan memiliki sudut 90°

![geogebra-export (1)](https://hackmd.io/_uploads/rJcZ9INMlg.png)


### **Panjang Vektor (Norma Vektor)**

**Panjang vektor**, atau disebut juga **norma** atau **magnitude**, adalah ukuran seberapa "besar" suatu vektor.



### **Rumus Umum Panjang Vektor**

Untuk vektor $\vec{v} = \langle v_1, v_2, ..., v_n \rangle$, panjang (atau norma) vektor ditulis sebagai:

$$
|\vec{v}| = \sqrt{v_1^2 + v_2^2 + \cdots + v_n^2}
$$


### Contoh 

$$
\vec{v} = \langle 3, 4 \rangle
$$

$$
|\vec{v}| = \sqrt{3^2 + 4^2} = \sqrt{9 + 16} = \sqrt{25} = 5
$$



### **Catatan Tambahan**

* Norma vektor **selalu bernilai positif** atau nol (tidak pernah negatif).
* Jika panjang vektor = 0, berarti itu **vektor nol** $\vec{0}$.
* Panjang ini penting buat normalisasi (membuat vektor satuan), menghitung jarak, sudut antar vektor, dll.


