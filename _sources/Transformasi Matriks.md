---
title: Transformasi Matriks

---

# Transformasi Matriks
Transformasi matriks adalah cara untuk mengubah satu vektor menjadi vektor lain menggunakan perkalian matriks.

Fungsi seperti ini disebut transformasi matriks dan merupakan bagian dari kelas fungsi yang disebut transformasi linear.

Matriks bisa dianggap sebagai alat untuk mentransformasikan vektor, baik dari segi arah maupun panjangnya.

Visualisasi transformasi ini membantu memahami bagaimana vektor berubah—terutama berguna dalam dimensi rendah dan aplikasi seperti grafik komputer.

Secara umum, jika ada matriks A dan vektor x, maka hasil transformasinya adalah y = A * x.

Ringkasan 5.1.1: Matriks – Perkalian Vektor
Untuk menyederhanakan, pembahasan fokus pada vektor di ruang 2 dimensi (ℝ²).

Untuk hasil transformasi tetap di ℝ², matriks yang digunakan harus berbentuk persegi (2×2).

Contoh dilakukan dengan beberapa vektor dan satu matriks, kemudian hasilnya dibandingkan sebelum dan sesudah dikalikan matriks.

Konsep ini membuka jalan untuk memahami transformasi yang lebih kompleks, seperti mengubah vektor 2D menjadi vektor 3D dengan matriks 3×2.

Contoh 5.1.1: Mengalikan Vektor dengan Matriks
Misalkan A adalah matriks, dan 𝑥, 𝑦, serta 𝑧 adalah vektor-vektor yang diberikan seperti di bawah ini:
$𝐴=  \begin{bmatrix} 1\ 3 \\ 4\ 2 \end{bmatrix}$, $\vec{x}= \begin{bmatrix}1 \\ 1\end{bmatrix}$, $\vec{y}=\begin{bmatrix}−1 \\ 1\end{bmatrix},\vec{z}=\begin{bmatrix}3 \\ −1\end{bmatrix}$ 

Soal: Gambar 𝑥, 𝑦, dan 𝑧, serta hasil perkalian matriksnya: A𝑥, A𝑦, dan A𝑧.

Penyelesaian: Mudah untuk dihitung:
$A\vec{x}=\begin{bmatrix}5\\6\end{bmatrix},A\vec{y}=\begin{bmatrix}3\\−2\end{bmatrix},A\vec{z}=\begin{bmatrix}−1\\10\end{bmatrix}$ 
Vektor-vektor tersebut digambarkan pada Gambar 5.1.2.

Penjelasan Tambahan:
Ada beberapa hal penting yang perlu diperhatikan:

Setiap vektor yang dikalikan dengan A menghasilkan vektor dengan panjang yang berbeda (dalam contoh ini, semuanya jadi lebih panjang).

Untuk dua vektor (𝑦 dan 𝑧), arah hasilnya juga berubah.

Menariknya, arah dari 𝑥 tidak berubah setelah dikalikan oleh A. Mengapa bisa begitu? Jawabannya akan dibahas di Bagian 7.1, saat membahas konsep eigenvektor.

Poin-poin Penting:
Matriks berbeda mempengaruhi vektor dengan cara yang berbeda.

Ada yang selalu memperpanjang vektor.

Ada yang memendekkan vektor.

Ada yang hanya mempengaruhi arah tanpa mengubah panjang.

Kadang perubahan arah hanya terjadi pada sebagian vektor, bukan semua.

Maka dari itu, kita perlu pendekatan yang sistematis untuk memahami bagaimana suatu matriks mempengaruhi berbagai vektor—bukan sekadar menebak atau mencoba satu per satu.

Kesimpulan dan Strategi:
Untuk memahami efek transformasi matriks, kita bisa mulai dari teknik yang sudah dikenal:

Bandingkan hasil transformasi dari vektor- vektor yang kita sudah tahu.

Perhatikan polanya—arah, panjang, perubahan yang terjadi.

Contoh ini menunjukkan bahwa tidak semua vektor berubah arah setelah dikalikan dengan matriks.

Contoh 5.1.1: Mengalikan Vektor dengan Matriks
Diberikan matriks A dan vektor 
𝑥⃗,𝑦⃗,𝑧⃗
 , setelah dikalikan dengan A, panjang vektor berubah dan arah bisa berubah. Menariknya, terkadang arah vektor tetap, seperti 
𝑥⃗  dan 𝐴𝑥⃗
  yang tetap searah. Ini membuka konsep "eigenvectors" (akan dibahas di Bab 7.1). Matriks bisa memperbesar, memperkecil, atau tidak mengubah panjang/direksi vektor tergantung jenisnya.

Contoh 5.1.3: Menggabungkan Penjumlahan dan Perkalian Matriks
Diberikan vektor 
𝑥⃗  dan 𝑦⃗
 , serta matriks A. Ketika kamu menjumlahkan dua vektor dan kemudian mengalikannya dengan A, hasilnya sama dengan mengalikan masing-masing vektor dengan A lalu menjumlahkannya:
𝐴(𝑥⃗+𝑦⃗)=𝐴𝑥⃗+𝐴𝑦⃗
 
Ini adalah sifat distributif dari perkalian matriks. Ilustrasinya menggunakan garis putus-putus untuk menekankan bentuk paralelogram (aturan penjumlahan vektor).

Contoh 5.1.5: Menggambarkan Efek dari Perkalian Matriks
Tiga vektor 
𝑥⃗,𝑦⃗,𝑧⃗
  jika dikalikan dengan A, salah satu menjadi vektor nol. Artinya, A mengubah vektor ke arah yang sama (kolinear). Ini bisa menunjukkan properti khusus dari A yang membuat beberapa vektor menjadi sejajar atau nol setelah dikalikan.

5.1.2: Transformasi dari Bidang Kartesius
Setiap titik di bidang Kartesius bisa dipandang sebagai vektor. Jika semua vektor dalam bidang dikalikan dengan matriks A, bentuk grid akan berubah: garis lurus tetap lurus, dan garis lengkung tetap lengkung (tapi mungkin melengkung lebih tajam atau datar).

Contoh 5.1.7: Memvisualisasikan Transformasi Matriks
Untuk memahami bagaimana A mengubah bidang Kartesius, digunakan unit square (persegi satuan). Setiap sudut persegi dikalikan dengan A, dan hasilnya membentuk bentuk baru. Ini membantu memahami bagaimana A bekerja terhadap semua titik (bukan cuma satu vektor). Digunakan juga metode cepat dengan membuat matriks B yang isinya adalah titik-titik dan dikalikan dengan A.

🔹 Ringkasan Singkat (Kesimpulan Bab 5.1):
Matriks bisa digunakan untuk mentransformasikan vektor.

Perkalian matriks bisa mengubah arah dan panjang vektor.

Ada properti penting seperti distributif: 
𝐴(𝑥⃗+𝑦⃗)=𝐴𝑥⃗+𝐴𝑦⃗

Visualisasi membantu memahami bagaimana matriks mempengaruhi ruang/vektor.

Untuk memahami efek pada seluruh bidang, kita bisa melihat bagaimana matriks mempengaruhi unit square.

Contoh 5.1.1: Mengalikan Vektor dengan Matriks
Ketika vektor dikalikan dengan matriks A, hasilnya adalah vektor baru dengan panjang yang berbeda (biasanya lebih panjang), dan arahnya juga bisa berubah. Menariknya, dalam salah satu kasus, arah tidak berubah sama sekali. Ini akan dibahas lebih lanjut di bab tentang eigenvectors.

Matriks yang berbeda mempengaruhi vektor secara berbeda: bisa memperbesar atau memperkecil panjang, mengubah arah, atau bahkan tidak mengubah sama sekali.

Contoh 5.1.3: Menambahkan dan Mengalikan Matriks
Menunjukkan bahwa hasil perkalian A(x + y) sama dengan Ax + Ay. Ini menampilkan sifat distributif perkalian matriks terhadap penjumlahan vektor. Grafik menunjukkan bahwa bentuk hasil akhir tetap mencerminkan jumlah dari hasil sebelumnya.

Contoh 5.1.5: Menunjukkan Pengaruh Matriks terhadap Vektor
Beberapa vektor seperti x bisa berubah menjadi nol setelah dikalikan dengan matriks tertentu (disebut null vector). Vektor-vektor lain bisa menjadi sejajar atau membentuk garis yang sama setelah transformasi.

Bagian 5.1.2: Transformasi Bidang Kartesius
Dengan memahami bagaimana vektor unit (seperti titik-titik di kuadran) berubah setelah dikalikan dengan matriks, kita bisa mengerti bagaimana seluruh bidang berubah. Misalnya, sebuah persegi bisa berubah menjadi jajaran genjang setelah dikalikan dengan matriks.

Contoh 5.1.7–5.1.10: Visualisasi Transformasi
Matriks bisa meregangkan, memutar, atau mengubah bentuk persegi menjadi bentuk lain.

Garis lurus tetap menjadi garis lurus setelah transformasi (meskipun bentuknya bisa miring).

Transformasi seperti rotasi atau refleksi dapat dilakukan tergantung bentuk matriks A.

Bahkan transformasi seperti rotasi 90° bisa dilakukan hanya dengan satu matriks.

Ringkasan Umum Bab 5.1: Transformasi Matriks
Matriks x Vektor = Mengubah arah dan panjang vektor.

Sifat Distributif: A(x + y) = Ax + Ay.

Transformasi Geometris: Matriks bisa mengubah bentuk bidang (rotasi, refleksi, skala).

Garis Lurus Tetap Lurus: Walau bentuk berubah, struktur geometris tetap terjaga.

Visualisasi: Membantu memahami dengan menggambar hasil transformasi.

Nol Vektor: Beberapa vektor bisa hilang (menjadi 0) setelah transformasi tertentu.

Inti dari Transformasi Matriks
Matriks transformasi mengubah posisi titik-titik di bidang 2D.

Setiap kolom dalam matriks menunjukkan ke mana arah sumbu x dan y (atau vektor 𝑒⃗1e  1​  dan 𝑒⃗2e  2​ ) setelah ditransformasi.

Jika kamu ingin tahu bentuk baru dari sebuah titik, tinggal kalikan matriksnya dengan titik tersebut.

🟩 Cara Menyusun Matriks Transformasi
Untuk membuat matriks:

Transformasikan vektor 
𝑒⃗1=[1,0] → ini jadi kolom pertama.

Transformasikan 
𝑒⃗2=[0,1] → ini jadi kolom kedua.

Contoh:

Flip sumbu x & stretch 2x ke kanan

$𝐴=\begin{bmatrix}2 \ 0 \\ 0 \ −1\end{bmatrix}$
🟨 Gunakan Matriksnya
Kalau ada titik (2,3) dan kamu punya matriks 𝐴
A, hasil transformasinya tinggal: $𝐴⋅\begin{bmatrix}2\\3\end{bmatrix}$
🟥 Beberapa Matriks Umum
Stretch horizontal: $\begin{bmatrix}𝑘 \ 0 \\ 0 \ 1\end{bmatrix}$

Rotasi 90° searah jarum jam: $\begin{bmatrix}0 \ 1 \\ −1 \ 0\end{bmatrix}$

Refleksi terhadap sumbu x: $\begin{bmatrix}1 \ 0 \\ 0 \ −1\end{bmatrix}$

⚠️ Hati-hati: Urutan Penting!
Kalau kamu gabung dua transformasi, urutan perkalian berpengaruh!

𝐴2⋅𝐴1≠𝐴1⋅𝐴2
Konsep Utama: Matriks sebagai Transformasi Linier
Transformasi Linier mengubah posisi titik di bidang 2D (seperti rotasi, refleksi, skala).

Matriks 2×2 bisa mewakili transformasi linier.
Contoh:
$𝐴=\begin{bmatrix}𝑎 \ 𝑏 \\ 𝑐 \ 𝑑\end{bmatrix}$
📌 Makna Kolom Matriks
Kolom pertama menunjukkan ke mana vektor 
𝑒⃗1= $\begin{bmatrix}1 \\ 0\end{bmatrix}$ dipetakan.

Kolom kedua menunjukkan ke mana 
𝑒⃗2= $\begin{bmatrix}0 \\ 1\end{bmatrix}$ dipetakan.

Jadi, kamu bisa membentuk matriks transformasi cukup dengan melihat transformasi dua vektor dasar itu.

📌 Cara Membentuk Matriks dari Transformasi
Misal:

𝑒⃗1→ $\begin{bmatrix}3 \\ 1\end{bmatrix}$
𝑒⃗2→$\begin{bmatrix}2 \\ 4\end{bmatrix}$

Maka:

$𝐴=\begin{bmatrix}3 \ 2 \\ 1 \ 4\end{bmatrix}$
📌 Aplikasi Matriks
Untuk menerapkan transformasi ke titik 
𝑣⃗=[𝑥𝑦]v =[ xy​], tinggal kalikan:

$𝐴⋅\vec{v}$
 
📌 Gabungan Transformasi
Kalau ada dua transformasi berturut-turut (misal 𝐴 lalu 
𝐵), maka hasil gabungan:


$B⋅A$
Urutan penting! Transformasi pertama ditulis di kanan.

## Jawaban

### Soal 1

Diketahui vektor: $[ \vec{x} = \begin{bmatrix} 1 \ 1 \end{bmatrix}$, $\quad \vec{y}$ = $\begin{bmatrix} -1 \ 2 \end{bmatrix} ]$ 
Matriks $( A ): [ A = \begin{bmatrix} 1 & -1 \\ 2 & 3 \end{bmatrix} ]$
Hitung hasil perkalian matriks dengan vektor: 
$[ A \vec{x}$ = $\begin{bmatrix} (1 \times 1) + (-1 \times 1) \\ (2 \times 1) + (3 \times 1) \end{bmatrix}$ = $\begin{bmatrix} 0 \\ 5 \end{bmatrix} ]$
$[ A \vec{y} = \begin{bmatrix} (1 \times -1) + (-1 \times 2) \\ (2 \times -1) + (3 \times 2) \end{bmatrix}$ = $\begin{bmatrix} -3 \\ 4 \end{bmatrix} ]$
Jadi, hasilnya untuk Soal 1:
- $( A \vec{x} = \begin{bmatrix} 0 \ 5 \end{bmatrix} )$
- $( A \vec{y} = \begin{bmatrix} -3 \ 4 \end{bmatrix} )$

### Soal 2

Diketahui :
$[ \vec{x} = \begin{bmatrix} 1 \ 1 \end{bmatrix}$, $\quad \vec{y}$ = $\begin{bmatrix} -1 \ 2 \end{bmatrix} ]$ 
Matriks $( A ): [ A = \begin{bmatrix} 2 & 0 \\ -1 & 3 \end{bmatrix} ]$
Hitung hasil perkalian matriks dengan vektor:
$[ A \vec{x} = \begin{bmatrix} (2 \times 1) + (0 \times 1) \\ (-1 \times 1) + (3 \times 1) \end{bmatrix} = \begin{bmatrix} 2 \\ 2 \end{bmatrix} ]$
$[ A \vec{y} = \begin{bmatrix} (2 \times -1) + (0 \times 2) \\ (-1 \times -1) + (3 \times 2) \end{bmatrix} = \begin{bmatrix} -2 \\ 7 \end{bmatrix} ]$
Jadi, hasilnya untuk Soal 2:
- $( A \vec{x} = \begin{bmatrix} 2 \ 2 \end{bmatrix} )$
- $( A \vec{y} = \begin{bmatrix} -2 \ 7 \end{bmatrix} )$

### soal 5

Diketahui: [ $A = \begin{bmatrix} a & b \\ c & d \end{bmatrix}$ ] 
Vektor yang diberikan: $[ \vec{x} = \begin{bmatrix} x_1 \\ y_1 \end{bmatrix}, \quad \vec{y} = \begin{bmatrix} x_2 \\ y_2 \end{bmatrix} ]$
Hasil transformasi: $[ A \vec{x} = \begin{bmatrix} a x_1 + b y_1 \\ c x_1 + d y_1 \end{bmatrix} ]
[ A \vec{y} = \begin{bmatrix} a x_2 + b y_2 \\ c x_2 + d y_2 \end{bmatrix} ]$
Kesimpulan untuk Soal 5:
Hasil transformasi dari matriks $A$ terhadap vektor $\vec{x}$ dan $\vec{y}$ dapat dihitung dengan formula di atas.


### soal 6

Diketahui: $B = \begin{bmatrix} p & q \\ r & s \end{bmatrix}$ 
Vektor yang diberikan: $\vec{u} = \begin{bmatrix} u_1 \\ v_1 \end{bmatrix}, \quad \vec{v} = \begin{bmatrix} u_2 \\ v_2 \end{bmatrix}$ 
Hasil transformasi: 
$B \vec{u} = \begin{bmatrix} p u_1 + q v_1 \\ r u_1 + s v_1 \end{bmatrix}$
$B \vec{v} = \begin{bmatrix} p u_2 + q v_2 \\ r u_2 + s v_2 \end{bmatrix}$
Kesimpulan untuk Soal 6: Transformasi dari matriks $B$ terhadap vektor $\vec{u}$ dan $\vec{v}$ menggunakan metode perkalian matriks dan vektor sesuai dengan formula di atas.



