---
title: Tugas Refleksi Satu Titik

---

 Tugas Refleksi Satu Titik


``` import numpy as np
import matplotlib.pyplot as plt

def reflect_x_equals_a(point, a):
    """Refleksi terhadap garis x = a"""
    x, y = point
    return (2 * a - x, y)

def reflect_y_equals_b(point, b):
    """Refleksi terhadap garis y = b"""
    x, y = point
    return (x, 2 * b - y)

def reflect_y_equals_x(point):
    """Refleksi terhadap garis y = x"""
    x, y = point
    return (y, x)

# Titik awal
point = (3, 4)

# Menerapkan refleksi terhadap berbagai garis
point_x_reflected = reflect_x_equals_a(point, 2)
point_y_reflected = reflect_y_equals_b(point, 2)
point_xy_reflected = reflect_y_equals_x(point)

# Visualisasi
fig, ax = plt.subplots(figsize=(6, 6))
ax.set_xlim(0, 5)
ax.set_ylim(0, 5)
ax.axvline(2, color='gray', linestyle='--', label="x = 2")
ax.axhline(2, color='gray', linestyle='--', label="y = 2")
ax.plot([0, 5], [0, 5], color='gray', linestyle='--', label="y = x")

# Plot titik
ax.scatter(*point, color='blue', label="Titik Awal")
ax.scatter(*point_x_reflected, color='red', label="Refleksi x = 2")
ax.scatter(*point_y_reflected, color='green', label="Refleksi y = 2")
ax.scatter(*point_xy_reflected, color='purple', label="Refleksi y = x")

ax.legend()
ax.set_title("Transformasi Refleksi dari Titik")
ax.set_xlabel("X")
ax.set_ylabel("Y")
plt.grid()
plt.show()
```






![image](https://hackmd.io/_uploads/HymqCkPxee.png)

Grafik yang dihasilkan dari kode Python menunjukkan bagaimana satu titik direfleksikan terhadap tiga garis: ( x = 2 ), ( y = 2 ), dan ( y = x ).
Elemen pada Grafik
- Titik Awal (Biru): Ini adalah titik yang akan direfleksikan, dengan koordinat (3,4).
- Garis Refleksi (Putus-Putus):
- ( x = 2 ) (Garis vertikal berwarna abu-abu).
- ( y = 2 ) (Garis horizontal berwarna abu-abu).
- ( y = x ) (Garis diagonal berwarna abu-abu).
- Titik Refleksi:
- Refleksi terhadap ( x = 2 ) → (Merah) (1,4).
- Refleksi terhadap ( y = 2 ) → (Hijau) (3,0).
- Refleksi terhadap ( y = x ) → (Ungu) (4,3).
Cara Interpretasi
- Refleksi terhadap ( x = 2 ):
- Koordinat x berubah sesuai rumus ( x' = 2a - x ), sehingga dari (3,4) menjadi (1,4).
- Y tetap sama karena refleksi terhadap garis vertikal tidak mempengaruhi koordinat y.
- Refleksi terhadap ( y = 2 ):
- Koordinat y berubah dengan rumus ( y' = 2b - y ), sehingga dari (3,4) menjadi (3,0).
- X tetap sama karena refleksi terhadap garis horizontal tidak mempengaruhi koordinat x.
- Refleksi terhadap ( y = x ):
- Koordinat ( (x,y) ) ditukar, sehingga dari (3,4) menjadi (4,3).
Kesimpulan
Grafik ini memperlihatkan bagaimana refleksi titik berfungsi dalam geometri koordinat. Dengan melihat titik awal dan hasil refleksi, kita bisa memahami bagaimana setiap refleksi mempengaruhi koordinat. Jika ingin bereksperimen dengan titik lain, cukup ubah nilai titik awal di kode Python.
Semoga penjelasannya jelas! Jika ingin tambahan visualisasi atau ada pertanyaan lebih lanjut, beri tahu saya. 

Cara Interpretasi
- Refleksi terhadap ( x = 2 ):
- Koordinat x berubah sesuai rumus ( x' = 2a - x ), sehingga dari (3,4) menjadi (1,4).
- Y tetap sama karena refleksi terhadap garis vertikal tidak mempengaruhi koordinat y.
- Refleksi terhadap ( y = 2 ):
- Koordinat y berubah dengan rumus ( y' = 2b - y ), sehingga dari (3,4) menjadi (3,0).
- X tetap sama karena refleksi terhadap garis horizontal tidak mempengaruhi koordinat x.
- Refleksi terhadap ( y = x ):
- Koordinat ( (x,y) ) ditukar, sehingga dari (3,4) menjadi (4,3).



