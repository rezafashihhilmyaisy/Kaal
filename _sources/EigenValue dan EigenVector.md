---
title: EigenValue dan EigenVector

---

## EigenValue dan EigenVector

## definisi eigenvalue dan eigenvector

rumus : $Av = \lambda v$



Eigenvalue (nilai eigen) adalah konsep penting dalam aljabar linear yang muncul saat kita mempelajari transformasi linier, khususnya dalam konteks matriks.

Secara sederhana:

 Eigenvalue adalah angka (skalar) yang menunjukkan seberapa besar suatu vektor (disebut eigenvector) diregangkan atau dikompresi oleh suatu transformasi matriks, tanpa mengubah arah vektornya.

### Secara Matematis:

Jika $A$ adalah sebuah matriks persegi (n x n), dan $v$ adalah vektor tak nol, maka $\lambda$ adalah eigenvalue dari $A$ jika:

$$
A \cdot v = \lambda \cdot v
$$

Di sini:

* $A$: matriks
* $v$: eigenvector (vektor tak nol)
* $\lambda$: eigenvalue

### Cara mencarinya:

Biasanya dicari dengan menyelesaikan **persamaan karakteristik**:

$$
\det(A - \lambda I) = 0
$$

Dimana:

* $\det$: determinan
* $I$: matriks identitas
* $\lambda$: variabel eigenvalue

Hasil dari persamaan ini akan berupa satu atau beberapa nilai $\lambda$ — itulah eigenvalue-nya.

### Contoh Singkat:

Misalnya untuk matriks 2x2:

$$
A = \begin{bmatrix} 2 & 1 \\ 1 & 2 \end{bmatrix}
$$

Persamaan karakteristiknya:

$$
\det \left( \begin{bmatrix} 2 & 1 \\ 1 & 2 \end{bmatrix} - \lambda \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix} \right) = 0
\Rightarrow \det \begin{bmatrix} 2 - \lambda & 1 \\ 1 & 2 - \lambda \end{bmatrix} = 0
$$
.

.

Eigenvector (vektor eigen) adalah pasangan dari eigenvalue dalam dunia aljabar linear.

### Pengertian Simpelnya:

Eigenvector adalah vektor tak nol yang arahnya tidak berubah ketika dikenai transformasi oleh suatu matriks — hanya panjang (magnitudonya) yang berubah, tidak arahnya.

### Hubungannya dengan Eigenvalue:

Jika suatu matriks $A$ dan skalar $\lambda$ memenuhi:

$$
A \cdot v = \lambda \cdot v
$$

maka:

* $v$ adalah eigenvector dari matriks $A$
* $\lambda$ adalah eigenvalue yang terkait dengan vektor $v$

Jadi, saat vektor $v$ dikalikan dengan matriks $A$, hasilnya tetap searah dengan $v$, hanya skalanya berubah sebesar $\lambda$.



### Contoh Sederhana:

Misal $A = \begin{bmatrix} 2 & 0 \\ 0 & 3 \end{bmatrix}$

Kita coba vektor $v = \begin{bmatrix} 1 \\ 0 \end{bmatrix}$

$$
A \cdot v = \begin{bmatrix} 2 & 0 \\ 0 & 3 \end{bmatrix} \cdot \begin{bmatrix} 1 \\ 0 \end{bmatrix} = \begin{bmatrix} 2 \\ 0 \end{bmatrix} = 2 \cdot \begin{bmatrix} 1 \\ 0 \end{bmatrix}
$$

Berarti $v$ adalah eigenvector, dan eigenvalue-nya adalah $\lambda = 2$

---

### Intinya:

* Eigenvalue: seberapa besar vektor diregangkan/dipadatkan
* Eigenvector: vektor yang arah transformasinya tidak berubah

Berikut adalah **langkah-langkah sistematis** untuk mencari **eigenvalue** dan **eigenvector** dari sebuah **matriks persegi (n×n)**:



## **Langkah-langkah Mencari Eigenvalue**

Misal: Diberikan matriks $A$

### 1. **Bentuk Persamaan Karakteristik**

Kita mulai dari persamaan:

$$
A \cdot v = \lambda \cdot v
\Rightarrow (A - \lambda I) \cdot v = 0
$$

Agar vektor $v$ tidak nol, maka:

$$
\det(A - \lambda I) = 0
$$

Ini disebut **persamaan karakteristik**, dan hasilnya adalah **persamaan polinomial**.



### 2. **Hitung Determinan**

Cari determinan dari $(A - \lambda I)$, lalu jadikan hasilnya = 0.



### 3. **Selesaikan Persamaan**

Dari hasil di atas, selesaikan untuk menemukan nilai-nilai $\lambda$ — inilah **eigenvalue**-nya.



##  **Langkah-langkah Mencari Eigenvector**

Untuk setiap **eigenvalue** $\lambda$ yang sudah ditemukan:

### 4. **Substitusikan ke (A - λI)v = 0**

Masukkan nilai $\lambda$ ke dalam:

$$
(A - \lambda I) \cdot v = 0
$$

dan selesaikan untuk vektor $v$.


### 5. **Cari Solusi Sistem Persamaan**

Ubah menjadi sistem persamaan linear, dan cari vektor $v$ tak nol yang memenuhi. Vektor inilah **eigenvector** yang sesuai dengan eigenvalue tersebut.

Biasanya solusi ditulis dalam bentuk parameter (misalnya: $v = t \cdot \begin{bmatrix} x \\ y \end{bmatrix}$) karena vektor bisa dikalikan skalar dan tetap jadi eigenvector.

##  **Contoh Singkat:**

Matriks:

$$
A = \begin{bmatrix} 4 & 2 \\ 1 & 3 \end{bmatrix}
$$

### Langkah 1: Bentuk $A - \lambda I$

$$
A - \lambda I = \begin{bmatrix} 4 - \lambda & 2 \\ 1 & 3 - \lambda \end{bmatrix}
$$

###  Langkah 2: Hitung Determinan

$$
\det(A - \lambda I) = (4 - \lambda)(3 - \lambda) - 2 \cdot 1 = \lambda^2 - 7\lambda + 10
$$

###  Langkah 3: Selesaikan

$$
\lambda^2 - 7\lambda + 10 = 0 \Rightarrow (\lambda - 5)(\lambda - 2) = 0
\Rightarrow \lambda = 5 \text{ dan } \lambda = 2
$$

###  Langkah 4: Cari Eigenvector untuk $\lambda = 5$

$$
(A - 5I) = \begin{bmatrix} -1 & 2 \\ 1 & -2 \end{bmatrix}
\Rightarrow \begin{bmatrix} -1 & 2 \\ 1 & -2 \end{bmatrix} \cdot \begin{bmatrix} x \\ y \end{bmatrix} = \begin{bmatrix} 0 \\ 0 \end{bmatrix}
\Rightarrow -x + 2y = 0 \Rightarrow x = 2y
$$

Maka eigenvectornya adalah:

$$
v = \begin{bmatrix} 2 \\ 1 \end{bmatrix} \text{ (atau kelipatannya)}
$$

 **Langkah: Cari Eigenvector untuk λ = 2**

Kita mulai dengan menghitung:

$$
A - \lambda I = A - 2I = \begin{bmatrix} 4 - 2 & 2 \\ 1 & 3 - 2 \end{bmatrix} = \begin{bmatrix} 2 & 2 \\ 1 & 1 \end{bmatrix}
$$

Sekarang kita selesaikan:

$$
(A - 2I) \cdot v = 0
\Rightarrow
\begin{bmatrix} 2 & 2 \\ 1 & 1 \end{bmatrix}
\cdot
\begin{bmatrix} x \\ y \end{bmatrix}
=
\begin{bmatrix} 0 \\ 0 \end{bmatrix}
$$

---

##  **Langkah: Ubah ke Sistem Persamaan Linear**

Dari hasil perkalian matriks:

$$
2x + 2y = 0 \\
x + y = 0
$$

Cukup ambil satu persamaan (karena baris kedua adalah kelipatan dari baris pertama):

$$
x + y = 0 \Rightarrow x = -y
$$



## **Kesimpulan: Eigenvector**

Eigenvector-nya berbentuk:

$$
v = \begin{bmatrix} x \\ y \end{bmatrix} = \begin{bmatrix} -y \\ y \end{bmatrix} = y \cdot \begin{bmatrix} -1 \\ 1 \end{bmatrix}
$$

Jadi:

$$
\text{Eigenvector untuk } \lambda = 2 \text{ adalah } \boxed{\begin{bmatrix} -1 \\ 1 \end{bmatrix}} \text{ (atau kelipatannya)}
$$

##### hasil akhir

$\lambda = 5$ dengan eigenvector $v1 = \begin{bmatrix} 2 \\ 1 \end{bmatrix} \text{ (atau kelipatannya)}$
$\lambda = 2$ dengan eigenvector  $v2 =  \boxed{\begin{bmatrix} -1 \\ 1 \end{bmatrix}} \text{ (atau kelipatannya)}$

```
import numpy as np

# Definisi matriks A
A = np.array([[4, 2], [1, 3]])

# Menghitung eigenvalues dan eigenvectors
eigenvalues, eigenvectors = np.linalg.eig(A)

# Menampilkan hasil
print("Eigenvalues:")
print(eigenvalues)

print("\nEigenvectors:")
print(eigenvectors)
```



![Screenshot 2025-06-16 224834](https://hackmd.io/_uploads/rkKta3a7ll.png)


```
import numpy as np
import matplotlib.pyplot as plt

# Matriks A
A = np.array([[4, 2],
              [1, 3]])

# Hitung eigenvalue dan eigenvector
eigenvalues, eigenvectors = np.linalg.eig(A)

# Titik asal (0, 0) untuk setiap vektor
origin = np.array([[0, 0], [0, 0]])  # shape (2,2)

# Siapkan vektor
vec1 = eigenvectors[:, 0]  # eigenvector 1
vec2 = eigenvectors[:, 1]  # eigenvector 2

# Plotting
plt.figure(figsize=(6, 6))
plt.axhline(0, color='gray', lw=1)
plt.axvline(0, color='gray', lw=1)
plt.grid()
plt.gca().set_aspect('equal')

# Plot eigenvectors (biru)
plt.quiver(*origin, [vec1[0], vec2[0]], [vec1[1], vec2[1]], color=['blue', 'blue'], scale=1, scale_units='xy', angles='xy', label='Eigenvectors')

# Plot hasil transformasi A*v (merah)
Av1 = A @ vec1
Av2 = A @ vec2
plt.quiver(*origin, [Av1[0], Av2[0]], [Av1[1], Av2[1]], color=['red', 'red'], scale=1, scale_units='xy', angles='xy', alpha=0.6, label='A * v')

# Label dan legenda
plt.title("Visualisasi Eigenvector dan Transformasi Matriks A")
plt.xlim(-4, 6)
plt.ylim(-4, 6)
plt.legend()
plt.show()
```
![image](https://hackmd.io/_uploads/Sk57A2pXex.png)

### Definisi ortonormal dan ortogonal

Ortonormal vectors adalah vektor-vektor yang memiliki panjang 1 dan saling tegak lurus satu sama lain.

Dalam matematika ortogonal adalah dua vektor dikatakan ortogonal jika sudut antara keduanya adalah 90 derajat atau tepat lurus.

code dibawah adalah untk ortonormal menjadikan eigenvector menjadi satuan

```
import numpy as np

# Contoh matriks simetris
A = np.array([[4, 1],
              [1, 3]])

# Hitung eigenvalue dan eigenvector
eigenvalues, eigenvectors = np.linalg.eig(A)

print("Eigenvectors sebelum dinormalisasi:")
print(eigenvectors)

# Normalisasi agar jadi ortonormal
def normalize_columns(matrix):
    return matrix / np.linalg.norm(matrix, axis=0)

orthonormal_vectors = normalize_columns(eigenvectors)

print("\nEigenvectors setelah dinormalisasi (ortornomal):")
print(orthonormal_vectors)

# Cek apakah vektor saling ortogonal (dot product antar kolom harus 0)
dot_product = np.dot(orthonormal_vectors[:, 0], orthonormal_vectors[:, 1])
print("\nDot product antar vektor ortonormal:", dot_product)
```
![image](https://hackmd.io/_uploads/SkFyka6Qxe.png)
