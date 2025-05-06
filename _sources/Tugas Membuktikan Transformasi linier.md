---
title: Tugas Membuktikan Transformasi linier

---

Untuk membuktikan bahwa $T(v_1,v_2) = (v_1+v_2,v_1)$ adalah transformasi linier, kita perlu memeriksa dua properti utama dari transformasi linier:

1. Preservasi Penjumlahan: $T(\mathbf{u} + \mathbf{v})$ = $T(\mathbf{u}) + T (\mathbf{v})$
2. Preservasi Perkalian Skalar: $T(c *\mathbf{v})$ = $c *T(\mathbf{v})$ , untuk setiap skalar \( c \)

Misalkan kita punya dua vektor dalam $\mathbb{R}^2$:
$\mathbf{u}$ = $(u_1, u_2)$, $\quad \mathbf{v}$ = $(v_1, v_2)$

### 1. Preservasi Penjumlahan:

$T(\mathbf{u} + \mathbf{v})$ = $T((u_1 + v_1, u_2 + v_2))$

Dengan menerapkan definisi \( T \), kita mendapatkan:
$T(u_1+v_1, u_2+v_2) = ((u_1+v_1) + (u_2+v_2), u_1+v_1)$

Di sisi lain, jika kita menerapkan \( T \) ke masing-masing vektor, kita mendapatkan:

$T(\mathbf{u}) + T(\mathbf{v}) = (u_1+u_2, u_1) + (v_1+v_2, v_1) = ((u_1+u_2) + (v_1+v_2), u_1+v_1)$

Karena kedua sisi sama, maka properti pertama terpenuhi.

### 2. Preservasi Perkalian Skalar:
Misalkan ( c \) adalah suatu skalar, maka:

$T(c \mathbf{v}) = T(c v_1, c v_2)$

Dengan definisi \( T \), kita mendapatkan:

$T(c v_1, c v_2) = ((c v_1 + c v_2), c v_1)$

Di sisi lain, jika kita menerapkan \( c \) pada \( T(\mathbf{v}) \), kita mendapatkan:

$c *T(v_1, v_2) = c (v_1+v_2, v_1) = (c v_1 + c v_2, c v_1)$

Karena kedua sisi sama, properti kedua terpenuhi.


Karena kedua properti transformasi linier telah terbukti benar, maka $T(v_1,v_2) = (v_1+v_2,v_1) \)$ adalah transformasi linier
