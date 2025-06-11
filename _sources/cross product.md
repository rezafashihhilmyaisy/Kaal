---
title: cross product

---

## Cross Product




### Definisi Hasil Kali Silang

Misalkan

$$
\vec{u} = \begin{bmatrix} u_1 \\ u_2 \\ u_3 \end{bmatrix} \quad \text{dan} \quad \vec{v} = \begin{bmatrix} v_1 \\ v_2 \\ v_3 \end{bmatrix}
$$

adalah vektor-vektor di $\mathbb{R}^3$. **Hasil kali silang** dari $\vec{u}$ dan $\vec{v}$, dinotasikan sebagai $\vec{u} \times \vec{v}$, adalah vektor:

$$
\vec{u} \times \vec{v} = 
\begin{bmatrix}
u_2 v_3 - u_3 v_2 \\
-(u_1 v_3 - u_3 v_1) \\
u_1 v_2 - u_2 v_1
\end{bmatrix}.
$$

---

**Cross product** (perkalian silang) adalah operasi dalam matematika vektor yang mengambil dua vektor dalam ruang tiga dimensi dan menghasilkan vektor ketiga yang **tegak lurus (normal)** terhadap kedua vektor asal.

---

### 🔹 Definisi Formal

Jika ada dua vektor:

$$
\vec{A} = \begin{bmatrix} A_x \\ A_y \\ A_z \end{bmatrix}, \quad
\vec{B} = \begin{bmatrix} B_x \\ B_y \\ B_z \end{bmatrix}
$$

Maka **cross product** ditulis sebagai:

$$
\vec{A} \times \vec{B} = \begin{bmatrix}
A_y B_z - A_z B_y \\
A_z B_x - A_x B_z \\
A_x B_y - A_y B_x
\end{bmatrix}
$$

Hasilnya adalah vektor baru yang:

* Arahnya tegak lurus terhadap $\vec{A}$ dan $\vec{B}$
* Panjangnya sama dengan:

$$
|\vec{A} \times \vec{B}| = |\vec{A}| \cdot |\vec{B}| \cdot \sin(\theta)
$$

di mana $\theta$ adalah sudut antara $\vec{A}$ dan $\vec{B}$

---

### 🔹 Sifat-Sifat Penting

* Tidak komutatif:

  $$
  \vec{A} \times \vec{B} \neq \vec{B} \times \vec{A}
  \quad \text{(bahkan, } \vec{A} \times \vec{B} = -(\vec{B} \times \vec{A})\text{)}
  $$
* Kalau dua vektor sejajar (sudut 0° atau 180°), hasil cross product = 0
* Sering dipakai dalam fisika untuk menentukan arah gaya, momen, atau bidang

---

### 🔹 Contoh

Misalnya:

$$
\vec{A} = \begin{bmatrix}1 \\ 0 \\ 0\end{bmatrix}, \quad
\vec{B} = \begin{bmatrix}0 \\ 1 \\ 0\end{bmatrix}
$$

$$
\vec{A} \times \vec{B} = \begin{bmatrix}
0 \cdot 0 - 0 \cdot 1 \\
0 \cdot 0 - 1 \cdot 0 \\
1 \cdot 1 - 0 \cdot 0
\end{bmatrix}
= \begin{bmatrix}
0 \\
0 \\
1
\end{bmatrix}
$$

Jadi hasilnya adalah vektor di arah sumbu-z, tegak lurus terhadap vektor A dan B.

Berikut adalah penulisan ulang dari isi gambar contoh perhitungan hasil kali silang:

---

### Contoh Menghitung Hasil Kali Silang

Misalkan

$$
\vec{u} = \begin{bmatrix} 2 \\ -1 \\ 4 \end{bmatrix}, \quad \vec{v} = \begin{bmatrix} 3 \\ 2 \\ 5 \end{bmatrix}.
$$

Temukan $\vec{u} \times \vec{v}$, dan verifikasi bahwa hasil kali silang ini tegak lurus terhadap baik $\vec{u}$ maupun $\vec{v}$.

---

### Solusi

Menggunakan **definisi**:

$\vec{u} \times \vec{v} =
\begin{bmatrix}
(-1)(5) - (4)(2) \\
-((2)(5) - (4)(3)) \\
(2)(2) - (-1)(3)\end{bmatrix}=\begin{bmatrix}-13 \\2 \\7\end{bmatrix}.$$

---


Berikut adalah penulisan ulang dari isi gambar verifikasi hasil kali silang tegak lurus terhadap kedua vektor:

---

### Verifikasi Ortogonalitas

Untuk memastikan bahwa $\vec{u} \times \vec{v}$ tegak lurus terhadap $\vec{u}$ dan $\vec{v}$, kita hitung **dot product** (hasil kali titik) berikut:

$$
(\vec{u} \times \vec{v}) \cdot \vec{u} =
\begin{bmatrix}
-13 \\
2 \\
7
\end{bmatrix}
\cdot
\begin{bmatrix}
2 \\
-1 \\
4
\end{bmatrix}
=(-13)(2) + (2)(-1) + (7)(4)= -26 - 2 + 28 = 0.
$$

$$
(\vec{u} \times \vec{v}) \cdot \vec{v} =
\begin{bmatrix}
-13 \\
2 \\
7
\end{bmatrix}
\cdot
\begin{bmatrix}
3 \\
2 \\
5
\end{bmatrix}
=(-13)(3) + (2)(2) + (7)(5)= -39 + 4 + 35 = 0.$$

---

Karena hasil dot product keduanya adalah nol, maka dapat disimpulkan bahwa
$\vec{u} \times \vec{v}$ **tegak lurus terhadap $\vec{u}$ dan $\vec{v}$**. ✅

Berikut adalah penulisan ulang dari isi gambar tersebut tentang **menggunakan determinan untuk mencari hasil kali silang**:

---

### Menggunakan Determinan untuk Menemukan Perkalian Silang

Pertama, kita bentuk array $3 \times 3$ seperti berikut:

$$
\begin{vmatrix}
\vec{i} & \vec{j} & \vec{k} \\
u_1 & u_2 & u_3 \\
v_1 & v_2 & v_3 \\
\end{vmatrix}
$$

Lalu, hasil kali silang dari $\vec{u} \times \vec{v}$ dapat dihitung menggunakan determinan minor sebagai berikut:

$\vec{u} \times \vec{v} =\begin{vmatrix}u_2 & u_3 \\v_2 & v_3 \\\end{vmatrix}\vec{i}$
-
$\begin{vmatrix}u_1 & u_3 \\v_1 & v_3 \\\end{vmatrix} \vec{j}
+\begin{vmatrix}
u_1 & u_2 \\v_1 & v_2 \\\end{vmatrix}\vec{k}$

Atau secara eksplisit:

$$\vec{u} \times \vec{v}=
(u_2v_3 - u_3v_2)\vec{i}
-(u_1v_3 - u_3v_1)\vec{j}+(u_1v_2 - u_2v_1)\vec{k}$$

---





pertama kita membentuk array 3x3 seperti yang ditunjukkan dibawah ini

![image](https://hackmd.io/_uploads/rya0ZRIQgx.png)



## soal 1

rumus:

$$
\text{Luas} = |\vec{u} \times \vec{v}|
$$

Untuk vektor dua dimensi:

$$
\vec{u} = \begin{bmatrix} 1 \\ 2 \end{bmatrix}, \quad \vec{v} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}
$$

Maka hasil perkalian silang (cross product) dalam 2D:

$$
|\vec{u} \times \vec{v}| = |(1)(1) - (2)(2)| = |1 - 4| = |-3| = 3
$$

### Jawaban:

Luas jajaran genjang tersebut adalah 3 satuan luas.

## soal 2


Diberikan:

$$
\vec{u} = \begin{bmatrix} 2 \\ 0 \end{bmatrix}, \quad \vec{v} = \begin{bmatrix} 0 \\ 3 \end{bmatrix}
$$

Rumus luas jajaran genjang di 2D:

$$
\text{Luas} = |\vec{u} \times \vec{v}| = |u_1 v_2 - u_2 v_1|
$$

Substitusi nilainya:

$$
\text{Luas} = |2 \cdot 3 - 0 \cdot 0| = |6 - 0| = \boxed{6}
$$

 Jadi, luas jajaran genjangnya adalah 6 satuan luas.

## soal 3

### Langkah-langkah:

1. Buat dua vektor dari titik-titik sudut:

   $$
   \vec{AB} = B - A = (1, 3, -1) - (0, 0, 0) = (1, 3, -1)
   $$

   $$
   \vec{AC} = C - A = (2, 1, 1) - (0, 0, 0) = (2, 1, 1)
   $$

2. Hitung **perkalian silang** $\vec{AB} \times \vec{AC}$:

$$
\vec{AB} \times \vec{AC} = 
\begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
1 & 3 & -1 \\
2 & 1 & 1 \\
\end{vmatrix}
= \mathbf{i}(3 \cdot 1 - (-1) \cdot 1) - \mathbf{j}(1 \cdot 1 - (-1) \cdot 2) + \mathbf{k}(1 \cdot 1 - 3 \cdot 2)
$$

$$
= \mathbf{i}(3 + 1) - \mathbf{j}(1 + 2) + \mathbf{k}(1 - 6)
= 4\mathbf{i} - 3\mathbf{j} - 5\mathbf{k}
$$

Jadi:

$$
\vec{AB} \times \vec{AC} = (4, -3, -5)
$$

3. Hitung **panjang vektor hasil cross product**:

$$
|\vec{AB} \times \vec{AC}| = \sqrt{4^2 + (-3)^2 + (-5)^2} = \sqrt{16 + 9 + 25} = \sqrt{50}
$$

4. Luas segitiga adalah setengah dari luas jajar genjang:

$$
\text{Luas} = \frac{1}{2} |\vec{AB} \times \vec{AC}| = \frac{1}{2} \sqrt{50} = \frac{\sqrt{50}}{2} = \frac{5\sqrt{2}}{2}
$$

---

### Jawaban akhir:

$$
\boxed{\frac{5\sqrt{2}}{2}}  satuan luas.$$


## soal 4

### Langkah-langkah:

1. Hitung vektor AB dan AC:

$$
\vec{AB} = B - A = (3 - 5, 6 - 2, 2 - (-1)) = (-2, 4, 3)
$$

$$
\vec{AC} = C - A = (1 - 5, 0 - 2, 4 - (-1)) = (-4, -2, 5)
$$

2. Hitung **cross product** $\vec{AB} \times \vec{AC}$:

$$
\vec{AB} \times \vec{AC} =
\begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
-2 & 4 & 3 \\
-4 & -2 & 5 \\
\end{vmatrix}
= \mathbf{i}(4 \cdot 5 - 3 \cdot (-2)) - \mathbf{j}(-2 \cdot 5 - 3 \cdot (-4)) + \mathbf{k}(-2 \cdot (-2) - 4 \cdot (-4))
$$

$$
= \mathbf{i}(20 + 6) - \mathbf{j}(-10 + 12) + \mathbf{k}(4 + 16)
= \mathbf{i}(26) - \mathbf{j}(2) + \mathbf{k}(20)
$$

$$
\Rightarrow \vec{AB} \times \vec{AC} = (26, -2, 20)
$$

3. Hitung **panjang vektor cross product**:

$$
|\vec{AB} \times \vec{AC}| = \sqrt{26^2 + (-2)^2 + 20^2} = \sqrt{676 + 4 + 400} = \sqrt{1080}
$$

4. Luas segitiga adalah:

$$
\text{Luas} = \frac{1}{2} |\vec{AB} \times \vec{AC}| = \frac{1}{2} \sqrt{1080}
= \frac{1}{2} \cdot \sqrt{36 \cdot 30} = \frac{1}{2} \cdot 6\sqrt{30} = 3\sqrt{30}
$$

### Jadi, **luas segitiga tersebut adalah** $\boxed{3\sqrt{30}}$ satuan luas.
