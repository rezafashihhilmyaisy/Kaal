---
title: Singular Value Decomposition

---

# Singular Value Decomposition

### Apa itu SVD?

Singular Value Decomposition (SVD) adalah teknik faktorisasi matriks yang sangat berguna dalam analisis data dan pengolahan sinyal. SVD memecah matriks menjadi tiga matriks yang lebih sederhana: **U**, **Σ**, dan **V** sehingga \( A = U \Sigma V^T \). 

- **U** adalah matriks ortogonal yang berisi vektor singular kiri.
- **Σ** adalah matriks diagonal yang berisi nilai singular.
- **V** adalah matriks ortogonal yang berisi vektor singular kanan.

SVD sering digunakan dalam berbagai bidang seperti statistik, pembelajaran mesin, pemrosesan gambar, dan sistem rekomendasi.

Rumus dasar dari **Singular Value Decomposition (SVD)** adalah:

$[A = U \Sigma V^T]$

di mana:

- \( A \) adalah matriks asal dengan ukuran \( m \times n \).
- \( U \) adalah matriks ortogonal dengan ukuran \( m \times m \) yang berisi vektor singular kiri.
- \( \Sigma \) adalah matriks diagonal dengan ukuran \( m \times n \) yang berisi nilai singular.
- \( V \) adalah matriks ortogonal dengan ukuran \( n \times n \) yang berisi vektor singular kanan.
- \( V^T \) adalah transpos dari matriks \( V \).

Setiap nilai singular dalam \( \Sigma \) memberikan informasi tentang kontribusi dimensi terhadap struktur data, yang berguna dalam reduksi dimensi dan kompresi data.

Berikut adalah langkah-langkah menghitung **Singular Value Decomposition (SVD)** untuk matriks \( A \):

1. **Hitung Matriks \( A^T A \)** 
   - Transpos matriks \( A \) dan kalikan dengan dirinya sendiri: \( A^T A \).
   - Temukan nilai eigen dan vektor eigen dari \( A^T A \). Vektor eigen ini akan menjadi kolom-kolom matriks **V**.

2. **Hitung Matriks \( A A^T \)** 
   - Kalikan matriks \( A \) dengan transposnya: \( A A^T \).
   - Temukan nilai eigen dan vektor eigen dari \( A A^T \). Vektor eigen ini akan menjadi kolom-kolom matriks **U**.

3. **Hitung Nilai Singular** 
   - Nilai singular adalah akar kuadrat dari nilai eigen yang diperoleh dari langkah sebelumnya.
   - Susun nilai singular dalam matriks diagonal **Σ**.

4. **Susun Matriks SVD** 
   - Matriks **U** berisi vektor eigen dari \( A A^T \).
   - Matriks **Σ** berisi nilai singular dalam bentuk diagonal.
   - Matriks **V** berisi vektor eigen dari \( A^T A \).

Sehingga diperoleh **faktorisasi SVD**: 
$[A = U \Sigma$  V^T ]

menghitung eigenvalue eigenvector, bisaa melakukan matriks transformasi,menghitung svd

### Tugas Soal


$$ A = \begin{bmatrix}
3 & 1 \\ 1 & 3\end{bmatrix}$$

### Langkah 1: Hitung $A^T A$

Karena $A$ simetris, $A^T A = A A$:

$$ A A = \begin{bmatrix}
3 & 1 \\
1 & 3
\end{bmatrix}
\begin{bmatrix}
3 & 1 \\
1 & 3
\end{bmatrix}=\begin{bmatrix}9 + 1 & 3 + 3 \\3 + 3 & 1 + 9\end{bmatrix}=\begin{bmatrix}10 & 6 \\6 & 10\end{bmatrix}$$

### Langkah 2: Temukan nilai eigen dari $A A$

Karakteristik:

$$
\chi(\lambda) = \begin{vmatrix}
10-\lambda & 6 \\
6 & 10-\lambda
\end{vmatrix}
= (10-\lambda)^2 - 36 = \lambda^2 - 20\lambda + 100 - 36 = \lambda^2 - 20\lambda + 64
$$

Akar:

$$
\lambda = \frac{20 \pm \sqrt{20^2 - 4 \times 64}}{2}
           = \frac{20 \pm \sqrt{400-256}}{2}
           = \frac{20 \pm \sqrt{144}}{2}
           = \frac{20 \pm 12}{2}
$$

$$
\lambda_1 = \frac{32}{2} = 16, \qquad \lambda_2 = \frac{8}{2} = 4
$$

### Langkah 3: Nilai Singular $\sigma_i = \sqrt{\lambda_i}$

$\sigma_1 = \sqrt{16} = 4, \qquad \sigma_2 = \sqrt{4} = 2$

### Langkah 4: Hitung V (eigenvektor dari $A^T A$)

* Untuk $\lambda_1 = 16$: $(A A - 16 I)x = 0$

$$
\begin{bmatrix}
-6 & 6 \\
6 & -6
\end{bmatrix}
\Rightarrow x_1 = [1, 1]^T
\Rightarrow v_1 = \frac{1}{\sqrt{2}}\begin{bmatrix}1 \\ 1\end{bmatrix}
$$

* Untuk $\lambda_2 = 4$: $(A A - 4 I)x = 0$

$$
\begin{bmatrix}
6 & 6 \\
6 & 6
\end{bmatrix}
\Rightarrow x_2 = [1, -1]^T
\Rightarrow v_2 = \frac{1}{\sqrt{2}}\begin{bmatrix}1 \\ -1\end{bmatrix}$$

Sehingga:

$$
V = \begin{bmatrix}
1/\sqrt{2} & 1/\sqrt{2} \\
1/\sqrt{2} & -1/\sqrt{2}
\end{bmatrix}
$$

### Langkah 5: Hitung $U = A V \Sigma^{-1}$

$$A v_1 = \begin{bmatrix}3 & 1 \\1 & 3\end{bmatrix}
\frac{1}{\sqrt{2}}\begin{bmatrix}1 \\1\end{bmatrix}=\frac{1}{\sqrt{2}}\begin{bmatrix}3+1 \\1+3\end{bmatrix}=\frac{1}{\sqrt{2}}\begin{bmatrix}4 \\4\end{bmatrix}
=\begin{bmatrix}\frac{4}{\sqrt{2}} \\\frac{4}{\sqrt{2}}\end{bmatrix}\Rightarrow u_1 = \frac{1}{4}\begin{bmatrix}\frac{4}{\sqrt{2}} \\\frac{4}{\sqrt{2}}\end{bmatrix}=\frac{1}{\sqrt{2}}\begin{bmatrix}1 \\1\end{bmatrix}$$

$$A v_2 = \begin{bmatrix}3 & 1 \\1 & 3\end{bmatrix}\frac{1}{\sqrt{2}}\begin{bmatrix}1 \\-1\end{bmatrix}=\frac{1}{\sqrt{2}}\begin{bmatrix}3-1 \\1-3\end{bmatrix}=\frac{1}{\sqrt{2}}\begin{bmatrix}2 \\-2\end{bmatrix}=\begin{bmatrix}\frac{2}{\sqrt{2}} \\-\frac{2}{\sqrt{2}}\end{bmatrix}\Rightarrow u_2 = \frac{1}{2}\begin{bmatrix}\frac{2}{\sqrt{2}} \\-\frac{2}{\sqrt{2}}\end{bmatrix}=\frac{1}{\sqrt{2}}\begin{bmatrix}1 \\-1\end{bmatrix}$$

### ✅ Hasil Final SVD:

$$
A = U \Sigma V^T
$$

dengan:

* $U = \begin{bmatrix}
  1/\sqrt{2} & 1/\sqrt{2} \\
  1/\sqrt{2} & -1/\sqrt{2}
  \end{bmatrix}, \Sigma = \begin{bmatrix}
  4 & 0 \\
  0 & 2
  \end{bmatrix}, V = \begin{bmatrix}
  1/\sqrt{2} & 1/\sqrt{2} \\
  1/\sqrt{2} & -1/\sqrt{2}
  \end{bmatrix}$


