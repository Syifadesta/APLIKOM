# Syifa Desta Rumaisha_22305141020_Plot 3D
Nama  : Syifa Desta R


NIM   : 22305141020


Kelas : Matematika E 2022


# Menggambar Plot 3D dengan EMT

Ini adalah pengenalan plot 3D di Euler. Kita membutuhkan plot 3D untuk
memvisualisasikan fungsi dari dua variabel.


Euler menggambar fungsi tersebut menggunakan algoritma pengurutan
untuk menyembunyikan bagian di latar belakang. Secara umum, Euler
menggunakan proyeksi pusat. Standarnya adalah dari kuadran x-y positif
menuju titik asal x=y=z=0, tetapi sudut=0° terlihat dari arah sumbu y.
Sudut pandang dan ketinggian dapat diubah.


Euler dapat merencanakan


* 
permukaan dengan bayangan dan garis level atau rentang level,

* 
awan poin,

* 
kurva parametrik,

* 
permukaan implisit.


Plot 3D dari suatu fungsi menggunakan plot3d. Cara termudah adalah
dengan memplot ekspresi dalam x dan y. Parameter r mengatur kisaran
plot di sekitar (0,0).


\> aspect(1.5); plot3d("x^2+sin(y)",r=pi):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-001.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-001.png)

\>aspect(1.5); plot3d("x^2+sin(y)",0,10,0,2\*pi):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-002.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-002.png)

\>aspect(1.5); plot3d("x^2+sin(y)",-5,5,0,2\*pi):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-003.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-003.png)

\>aspect(1.5); plot3d("x^2+sin(y)",-5,5,0,6\*pi):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-004.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-004.png)

\>aspect(1.5); plot3d("x^2+sin(y)",-2,7,0,5\*pi):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-005.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-005.png)

\>aspect(1.5); plot3d("x^2\*sin(y)",-5,5,0,2\*pi):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-006.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-006.png)

\>aspect(1.5); plot3d("x^2-sin(y)",-5,5,0,2\*pi):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-007.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-007.png)

\>aspect(1.5); plot3d("x^2\*(1+sin(y))",-5,5,0,6\*pi):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-008.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-008.png)

\>aspect(1.5); plot3d("x^3+sin(y)",-5,5,0,2\*pi):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-009.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-009.png)

# Fungsi dua Variabel

Untuk grafik fungsi, gunakan


* 
ekspresi sederhana dalam x dan y,

* 
nama fungsi dari dua variabell

* 
atau matriks data.


Standarnya adalah kisi kawat yang diisi dengan warna berbeda di kedua
sisi. Perhatikan bahwa jumlah default interval grid adalah 10, tetapi
plot menggunakan jumlah default 40x40 persegi panjang untuk membangun
permukaan. Ini bisa diubah.


* 
n=40, n=[40,40]: jumlah garis kisi di setiap arah

* 
grid=10, grid=[10,10]: jumlah garis grid di setiap arah.


Kami menggunakan default n=40 dan grid=10.


\>plot3d("x^2+y^2"):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-010.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-010.png)

\>plot3d("x^3+y^3"):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-011.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-011.png)

Interaksi pengguna dimungkinkan dengan &gt;parameter pengguna. Pengguna
dapat menekan tombol berikut.


* 
kiri, kanan, atas, bawah: putar sudut pandang

* 
+,-: memperbesar atau memperkecil

* 
a: menghasilkan anaglyph (lihat di bawah)

* 
l: beralih memutar sumber cahaya (lihat di bawah)

* 
spasi: reset ke default

* 
kembali: akhiri interaksi


\>plot3d("exp(-x^2+y^2)",\>user, ...  
\>     title="Turn with the vector keys (press return to finish)"):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-012.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-012.png)

\>plot3d("exp(-x^3+y^4)",\>user, ...  
\>     title="Turn with the vector keys (press return to finish)"):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-013.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-013.png)

\>plot3d("exp(x^5+y^2)",\>user, ...  
\>     title="Turn with the vector keys (press return to finish)"):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-014.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-014.png)

Rentang plot untuk fungsi dapat ditentukan dengan


* 
a,b: rentang-x

* 
c,d: rentang-y

* 
r: persegi simetris di sekitar (0,0).

* 
n: jumlah subinterval untuk plot.


Ada beberapa parameter untuk menskalakan fungsi atau mengubah tampilan
grafik.


fscale: skala ke nilai fungsi (defaultnya adalah &lt;fscale).


skala: angka atau vektor 1x2 untuk skala ke arah x dan y.


bingkai: jenis bingkai (default 1).


\>plot3d("exp(-(x^2+y^2)/5)",r=10,n=80,fscale=4,scale=1.2,frame=3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-015.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-015.png)

\>plot3d("exp(-(x^2+y^2)/3)",r=10,n=80,fscale=4,scale=1.2,frame=3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-016.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-016.png)

\>plot3d("exp(-(x^2+y)/5)",r=10,n=80,fscale=4,scale=1.2,frame=3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-017.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-017.png)

Tampilan dapat diubah dengan berbagai cara.


* 
jarak: jarak pandang ke plot.

* 
zoom: nilai zoom.

* 
sudut: sudut terhadap sumbu y negatif dalam radian.

* 
tinggi: ketinggian tampilan dalam radian.


Nilai default dapat diperiksa atau diubah dengan fungsi view(). Ini
mengembalikan parameter dalam urutan di atas.


\>view


    [5,  2.6,  2,  0.4]

Jarak yang lebih dekat membutuhkan lebih sedikit zoom. Efeknya lebih
seperti lensa sudut lebar.


Dalam contoh berikut, sudut=0 dan tinggi=0 terlihat dari sumbu y
negatif. Label sumbu untuk y disembunyikan dalam kasus ini.


\>plot3d("x^2+y",distance=3,zoom=2,angle=0,height=0):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-018.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-018.png)

\>plot3d("x^3+y^2",distance=2,zoom=2,angle=0,height=0):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-019.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-019.png)

\>plot3d("x+y",distance=3,zoom=1,angle=0,height=0):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-020.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-020.png)

Plot terlihat selalu ke pusat kubus plot. Anda dapat memindahkan pusat
dengan parameter tengah.


\>plot3d("x^4+y^2",a=0,b=1,c=-1,d=1,angle=-20°,height=20°, ...  
\>     center=[0.4,0,0],zoom=5):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-021.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-021.png)

\>plot3d("x^6+y^3",a=0,b=1,c=-1,d=1,angle=60°,height=15°, ...  
\>     center=[0.6,0,0],zoom=4):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-022.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-022.png)

\>plot3d("x^3+y^2",a=0,b=1,c=-1,d=1,angle=90°,height=45°, ...  
\>     center=[0.5,0,0],zoom=5):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-023.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-023.png)

Plot diskalakan agar sesuai dengan kubus satuan untuk dilihat. Jadi
tidak perlu mengubah jarak atau zoom tergantung pada ukuran plot.
Namun, label mengacu pada ukuran sebenarnya.


Jika Anda mematikannya dengan scale=false, Anda harus berhati-hati,
agar plot tetap pas dengan jendela plot, dengan mengubah jarak pandang
atau zoom, dan memindahkan bagian tengahnya.


\>plot3d("5\*exp(-x^2-y^2)",r=2,<fscale,<scale,distance=13,height=50°, ...  
\>     center=[0,0,-2],frame=3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-024.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-024.png)

\>plot3d("5\*exp(-x^2-y^2)",r=1,<fscale,<scale,distance=15,height=30°, ...  
\>     center=[0,0,-2],frame=3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-025.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-025.png)

\>plot3d("3\*exp(-x^2-y^2)",r=1,<fscale,<scale,distance=15,height=70°, ...  
\>     center=[0,0,2],frame=3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-026.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-026.png)

Sebuah plot kutub juga tersedia. Parameter polar=true menggambar plot
polar. Fungsi tersebut harus tetap merupakan fungsi dari x dan y.
Parameter "fscale" menskalakan fungsi dengan skala sendiri. Jika
tidak, fungsi diskalakan agar sesuai dengan kubus.


\>plot3d("1/(x^2+y^2+1)",r=5,\>polar, ...  
\>   fscale=2,\>hue,n=100,zoom=4,\>contour,color=gray):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-027.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-027.png)

\>plot3d("1/(x^2+y^2)",r=5,\>polar, ...  
\>   fscale=2,\>hue,n=100,zoom=3,\>contour,color=blue):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-028.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-028.png)

\>plot3d("1/(x^2+y^2+2)",r=5,\>polar, ...  
\>   fscale=2,\>hue,n=100,zoom=5,\>contour,color=black):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-029.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-029.png)

\>function f(r) := exp(-r/2)\*cos(r); ...  
\>   plot3d("f(x^2+y^2)",\>polar,scale=[1,1,0.4],r=2pi,frame=3,zoom=4):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-030.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-030.png)

\>function f(r) := exp(r/2)\*cos(r); ...  
\>   plot3d("f(x^2+y^2)",\>polar,scale=[1,1,0.4],r=2pi,frame=2,zoom=4):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-031.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-031.png)

\>function f(r) := exp(-r/2)\*cos(r); ...  
\>   plot3d("f(x^2+y^2)",\>polar,scale=[1,1,0.4],r=pi,frame=3,zoom=4):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-032.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-032.png)

Rotasi parameter memutar fungsi dalam x di sekitar sumbu x.


* 
rotate=1: Menggunakan sumbu x

* 
rotate=2: Menggunakan sumbu z


\>plot3d("x^2+1",a=-1,b=1,rotate=true,grid=5):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-033.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-033.png)

\>plot3d("x^3+2",a=-1,b=1,rotate=true,grid=5):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-034.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-034.png)

\>plot3d("x^4+3",a=-1,b=1,rotate=true,grid=6):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-035.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-035.png)

\>plot3d("x","x^2+y^2","y",r=2,zoom=3.5,frame=3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-036.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-036.png)

\>plot3d("x","x^2+y^2","y",r=2,zoom=2.5,frame=3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-037.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-037.png)

\>plot3d("x","x^2+y","y",r=2,zoom=3,frame=-3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-038.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-038.png)

# Plot Kontur

Untuk plot, Euler menambahkan garis grid. Sebagai gantinya
dimungkinkan untuk menggunakan garis level dan rona satu warna atau
rona berwarna spektral. Euler dapat menggambar tinggi fungsi pada plot
dengan bayangan. Di semua plot 3D, Euler dapat menghasilkan anaglyph
merah/sian.


-&gt; hue: Menyalakan bayangan cahaya alih-alih kabel.


-&gt; kontur: Memplot garis kontur otomatis pada plot.


- level=... (atau level): Sebuah vektor nilai untuk garis kontur.


Standarnya adalah level="auto", yang menghitung beberapa garis level
secara otomatis. Seperti yang Anda lihat di plot, level sebenarnya
adalah rentang level.


Gaya default dapat diubah. Untuk plot kontur berikut, kami menggunakan
grid yang lebih halus untuk 100x100 poin, skala fungsi dan plot, dan
menggunakan sudut pandang yang berbeda.


\>plot3d("exp(-x^2-y^2)",r=2,n=100,level="thin", ...  
\>    \>contour,\>spectral,fscale=1,scale=1.1,angle=45°,height=20°):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-039.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-039.png)

\>plot3d("exp(x^2-y^2)",r=2,n=100,level="thin", ...  
\>    \>contour,\>spectral,fscale=1,scale=1.1,angle=90°,height=15°):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-040.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-040.png)

\>plot3d("exp(x\*y)",angle=100°,\>contour,color=green):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-041.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-041.png)

\>plot3d("exp(x\*y)",angle=120°,\>contour,color=blue):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-042.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-042.png)

Bayangan default menggunakan warna abu-abu. Tetapi rentang warna
spektral juga tersedia.


-&gt; spektral: Menggunakan skema spektral default


- color=...: Menggunakan warna khusus atau skema spektral


Untuk plot berikut, kami menggunakan skema spektral default dan
menambah jumlah titik untuk mendapatkan tampilan yang sangat halus.


\>plot3d("x^2+y^2",\>spectral,\>contour,n=100):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-043.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-043.png)

\>plot3d("x^4+y^3",\>spectral,\>contour,n=100):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-044.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-044.png)

Alih-alih garis level otomatis, kita juga dapat mengatur nilai garis
level. Ini akan menghasilkan garis level tipis alih-alih rentang
level.


\>plot3d("x^2-y^2",0,1,0,1,angle=220°,level=-1:0.2:1,color=redgreen):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-045.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-045.png)

\>plot3d("x^4-y^4",0,1,0,1,angle=110°,level=-1:0.2:1,color=blue):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-046.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-046.png)

\>plot3d("x^4-y^3",0,1,0,1,angle=100°,level=-1:0.2:1,color=red):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-047.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-047.png)

\>plot3d("x^2-y^2",0,5,0,5,angle=220°,level=-1:0.1:1,color=redgreen):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-048.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-048.png)

\>plot3d("x^2-y^2",0,5,0,5,angle=100°,level=-1:0.1:1,color=redgreen):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-049.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-049.png)

\>plot3d("x^2-y^2",-5,5,5,5,level=-1:0.2:1,color=redgreen):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-050.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-050.png)

Dalam plot berikut, kami menggunakan dua pita level yang sangat luas
dari -0,1 hingga 1, dan dari 0,9 hingga 1. Ini dimasukkan sebagai
matriks dengan batas level sebagai kolom.


Selain itu, kami melapisi kisi dengan 10 interval di setiap arah.


\>plot3d("x^2+y^3",level=[-0.1,0.9;0,1], ...  
\>     \>spectral,angle=30°,grid=10,contourcolor=gray):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-051.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-051.png)

\>plot3d("x^4+y^5",level=[-0.1,0.9;0,1], ...  
\>     \>spectral,angle=60°,grid=10,contourcolor=gray):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-052.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-052.png)

Dalam contoh berikut, kami memplot himpunan, di mana


$$f(x,y) = x^y-y^x = 0$$Kami menggunakan satu garis tipis untuk garis level.


\>plot3d("x^y-y^x",level=0,a=0,b=6,c=0,d=6,contourcolor=red,n=100):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-054.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-054.png)

\>plot3d("x^2y-2y^x",level=0,a=0,b=6,c=0,d=6,contourcolor=green,n=100):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-055.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-055.png)

\>plot3d("x^-y-y^x",level=0,a=0,b=6,c=0,d=6,contourcolor=green,n=100):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-056.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-056.png)

Dimungkinkan untuk menunjukkan bidang kontur di bawah plot. Warna dan
jarak ke plot dapat ditentukan.


\>plot3d("x^2+y^4",\>cp,cpcolor=green,cpdelta=0.2):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-057.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-057.png)

\>plot3d("x^3+y^6",\>cp,cpcolor=black,cpdelta=0.2):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-058.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-058.png)

\>plot3d("x^2+y^4",\>cp,cpcolor=red,cpdelta=0.5):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-059.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-059.png)

Berikut adalah beberapa gaya lagi. Kami selalu mematikan frame, dan
menggunakan berbagai skema warna untuk plot dan grid.


\>figure(2,2); ...  
\>   expr="y^3-x^2"; ...  
\>   figure(1);  ...  
\>     plot3d(expr,<frame,\>cp,cpcolor=spectral); ...  
\>   figure(2);  ...  
\>     plot3d(expr,<frame,\>spectral,grid=10,cp=2); ...  
\>   figure(3);  ...  
\>     plot3d(expr,<frame,\>contour,color=gray,nc=5,cp=3,cpcolor=greenred); ...  
\>   figure(4);  ...  
\>     plot3d(expr,<frame,\>hue,grid=10,\>transparent,\>cp,cpcolor=gray); ...  
\>   figure(0):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-060.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-060.png)

\>figure(2,2); ...  
\>   expr="x^2 - y^2"; ...  
\>   figure(1);  ...  
\>     plot3d(expr,<frame,\>cp,cpcolor=spectral); ...  
\>   figure(2);  ...  
\>     plot3d(expr,<frame,\>spectral,grid=10,cp=2); ...  
\>   figure(3);  ...  
\>     plot3d(expr,<frame,\>contour,color=gray,nc=5,cp=3,cpcolor=greenred); ...  
\>   figure(4);  ...  
\>     plot3d(expr,<frame,\>hue,grid=10,\>transparent,\>cp,cpcolor=gray); ...  
\>   figure(0):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-061.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-061.png)

\>figure(2,2); ...  
\>   expr="x^3 - y^2"; ...  
\>   figure(1);  ...  
\>     plot3d(expr,<frame,\>cp,cpcolor=spectral); ...  
\>   figure(2);  ...  
\>     plot3d(expr,<frame,\>spectral,grid=10,cp=2); ...  
\>   figure(3);  ...  
\>     plot3d(expr,<frame,\>contour,color=gray,nc=5,cp=3,cpcolor=greenred); ...  
\>   figure(4);  ...  
\>     plot3d(expr,<frame,\>hue,grid=10,\>transparent,\>cp,cpcolor=gray); ...  
\>   figure(0):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-062.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-062.png)

Ada beberapa skema spektral lainnya, bernomor dari 1 hingga 9. Tetapi
Anda juga dapat menggunakan warna=nilai, di mana nilai


* 
spektral: untuk rentang dari biru ke merah

* 
putih: untuk rentang yang lebih redup

* 
kuningbiru,ungu hijau,birukuning,hijaumerah

* 
birukuning, hijau ungu, kuning biru, merah hijau


\>figure(3,3); ...  
\>   for i=1:9;  ...  
\>     figure(i); plot3d("x^2+y^2",spectral=i,\>contour,\>cp,<frame,zoom=4);  ...  
\>   end; ...  
\>   figure(0):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-063.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-063.png)

\>figure(4,4); ...  
\>   for i=1:9;  ...  
\>     figure(i); plot3d("x^3+y^3",spectral=i,\>contour,\>cp,<frame,zoom=4);  ...  
\>   end; ...  
\>   figure(0):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-064.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-064.png)

\>figure(3,3); ...  
\>   for i=1:10;  ...  
\>     figure(i); plot3d("x^4-y^4",spectral=i,\>contour,\>cp,<frame,zoom=4);  ...  
\>   end; ...  
\>   figure(0):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-065.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-065.png)

Sumber cahaya dapat diubah dengan l dan tombol kursor selama interaksi
pengguna. Itu juga dapat diatur dengan parameter.


* 
cahaya: arah untuk cahaya

* 
amb: cahaya sekitar antara 0 dan 1


Perhatikan bahwa program tidak membuat perbedaan antara sisi plot.
Tidak ada bayangan. Untuk ini, Anda perlu Povray.


\>plot3d("-x^2-y^2", ...  
\>     hue=true,light=[0,1,1],amb=0,user=true, ...  
\>     title="Press l and cursor keys (return to exit)"):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-066.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-066.png)

\>plot3d("x^2+y^2", ...  
\>     hue=true,light=[0,1,1],amb=0,user=true, ...  
\>     title="Press l and cursor keys (return to exit)"):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-067.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-067.png)

Parameter warna mengubah warna permukaan. Warna garis level juga dapat
diubah.


\>plot3d("-x^2-y^2",color=rgb(0.2,0.2,0),hue=true,frame=false, ...  
\>     zoom=3,contourcolor=red,level=-2:0.1:1,dl=0.01):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-068.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-068.png)

\>plot3d("x^2-y^2",color=rgb(0.2,0.2,0),hue=true,frame=false, ...  
\>     zoom=3,contourcolor=green,level=-2:0.1:1,dl=0.01):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-069.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-069.png)

\>plot3d("x^2+y^2",color=rgb(0.2,0.2,0),hue=true,frame=false, ...  
\>     zoom=3,contourcolor=blue,level=-2:0.1:1,dl=0.01):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-070.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-070.png)

\>plot3d("x^2+y^4",color=rgb(0.2,0.2,0),hue=true,frame=false, ...  
\>     zoom=3,contourcolor=yellow,level=-2:0.1:1,dl=0.01):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-071.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-071.png)

\>plot3d("x^2+y^3",color=rgb(0.2,0.2,0),hue=true,frame=false, ...  
\>     zoom=2,contourcolor=green,level=-2:0.1:1,dl=0.01):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-072.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-072.png)

Warna 0 memberikan efek pelangi khusus.


\>plot3d("x^2/(x^2+y^2+1)",color=0,hue=true,grid=10):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-073.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-073.png)

\>plot3d("x^3/(x^3+y^3+1)",color=0,hue=true,grid=10):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-074.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-074.png)

\>plot3d("x^4/(x^4+y^4-1)",color=0,hue=true,grid=10):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-075.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-075.png)

\>plot3d("x/(x+y-1)",color=0,hue=true,grid=10):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-076.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-076.png)

Permukaannya juga bisa transparan.


\>plot3d("x^2+y^2",\>transparent,grid=10,wirecolor=red):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-077.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-077.png)

\>plot3d("x^3+y^3",\>transparent,grid=15,wirecolor=yellow):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-078.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-078.png)

\>plot3d("x+y^3",\>transparent,grid=15,wirecolor=green):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-079.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-079.png)

\>plot3d("x^5-y^3",\>transparent,grid=15,wirecolor=blue):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-080.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-080.png)

\>plot3d("x^5-y^2",\>transparent,grid=13,wirecolor=red):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-081.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-081.png)

\>plot3d("x^7+y^3",\>transparent,grid=20,wirecolor=blue):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-082.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-082.png)

\>plot3d("x^8-y^4",\>transparent,grid=15,wirecolor=green):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-083.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-083.png)

\>plot3d("x^10-y^5",\>transparent,grid=15,wirecolor=yellow):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-084.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-084.png)

\>plot3d("x^7+y^3",\>transparent,grid=15,wirecolor=black):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-085.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-085.png)

# Plot Implisit

Ada juga plot implisit dalam tiga dimensi. Euler menghasilkan
pemotongan melalui objek. Fitur plot3d termasuk plot implisit.
Plot-plot ini menunjukkan himpunan nol dari suatu fungsi dalam tiga
variabel.


Solusi dari


$$f(x,y,z) = 0$$dapat divisualisasikan dalam potongan sejajar dengan bidang x-y-, x-z-
dan y-z.


* 
implisit=1: potong sejajar dengan bidang y-z

* 
implisit=2: potong sejajar dengan bidang x-z

* 
implisit=4: potong sejajar dengan bidang x-y


Tambahkan nilai-nilai ini, jika Anda suka. Dalam contoh kita plot


$$M = \{ (x,y,z) : x^2+y^3+zy=1 \}$$\>plot3d("x^2+y^3+z\*y-1",r=5,implicit=3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-088.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-088.png)

\>plot3d("x^3+y^3+z\*y-2",r=5,implicit=4):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-089.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-089.png)

\>plot3d("x^2+y^2+4\*x\*z+z^3",\>implicit,r=2,zoom=2.5):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-090.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-090.png)

\>plot3d("x^4+y^4+5\*x\*z+z^2",\>implicit,r=2,zoom=3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-091.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-091.png)

\>plot3d("x^7+y^2+3\*x\*z+z^4",\>implicit,r=2,zoom=2):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-092.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-092.png)

\>plot3d("x^5+y^9-3\*x\*z+z^5",\>implicit,r=2,zoom=2.5):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-093.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-093.png)

\>plot3d("x^4+y^5+5\*x\*z+z^2",\>implicit,r=2,zoom=2):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-094.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-094.png)

\>plot3d("x^2-y^2+4\*x\*z+z^3",\>implicit,r=2,zoom=2):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-095.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-095.png)

# Merencanakan Data 3D

Sama seperti plot2d, plot3d menerima data. Untuk objek 3D, Anda perlu
menyediakan matriks nilai x-, y- dan z, atau tiga fungsi atau ekspresi
fx(x,y), fy(x,y), fz(x,y).


$$\gamma(t,s) = (x(t,s),y(t,s),z(t,s))$$Karena x,y,z adalah matriks, kita asumsikan bahwa (t,s) melalui sebuah
kotak persegi. Hasilnya, Anda dapat memplot gambar persegi panjang di
ruang angkasa.


Anda dapat menggunakan bahasa matriks Euler untuk menghasilkan
koordinat secara efektif.


Dalam contoh berikut, kami menggunakan vektor nilai t dan vektor kolom
nilai s untuk membuat parameter permukaan bola. Dalam gambar kita
dapat menandai daerah, dalam kasus kita daerah kutub.


\>t=linspace(0,2pi,180); s=linspace(-pi/2,pi/2,90)'; ...  
\>   x=cos(s)\*cos(t); y=cos(s)\*sin(t); z=sin(s); ...  
\>   plot3d(x,y,z,\>hue, ...  
\>   color=blue,<frame,grid=[10,20], ...  
\>   values=s,contourcolor=red,level=[90°-24°;90°-22°], ...  
\>   scale=1.4,height=50°):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-097.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-097.png)

\>t=linspace(0,2pi,180); s=linspace(-pi/2,pi/2,90)'; ...  
\>   x=cos(s)\*cos(t); y=cos(s)\*sin(t); z=sin(s); ...  
\>   plot3d(x,y,z,\>hue, ...  
\>   color=blue,<frame,grid=[15,30], ...  
\>   values=s,contourcolor=green,level=[90°-24°;90°-22°], ...  
\>   scale=1.4,height=50°):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-098.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-098.png)

\>t=linspace(0,2pi,180); s=linspace(-pi/2,pi/2,90)'; ...  
\>   x=cos(s)\*cos(t); y=cos(s)\*sin(t); z=sin(s); ...  
\>   plot3d(x,y,z,\>hue, ...  
\>   color=blue,<frame,grid=[10,20], ...  
\>   values=s,contourcolor=red,level=[90°-20°;90°-18°], ...  
\>   scale=1.4,height=50°):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-099.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-099.png)

Berikut adalah contoh, yang merupakan grafik fungsi.


\>t=-1:0.1:1; s=(-1:0.1:1)'; plot3d(t,s,t\*s,grid=10):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-100.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-100.png)

\>t=-1:0.5:1; s=(-1:0.5:1)'; plot3d(t,s,t\*s,grid=10):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-101.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-101.png)

\>t=-2:0.2:2; s=(-2:0.2:2)'; plot3d(t,s,t\*s,grid=15):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-102.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-102.png)

\>t=-1:0.1:1; s=(-1:0.1:1)'; plot3d(t,s,t\*s,grid=11):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-103.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-103.png)

Namun, kita bisa membuat segala macam permukaan. Berikut adalah
permukaan yang sama dengan fungsi


$$x = y \, z$$\>plot3d(t\*s,t,s,angle=180°,grid=10):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-105.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-105.png)

\>plot3d(t\*s,t,s,angle=90°,grid=16):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-106.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-106.png)

\>plot3d(t\*s,t,s,angle=270°,grid=5):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-107.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-107.png)

\>plot3d(t\*s,t,s,angle=45°,grid=7):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-108.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-108.png)

\>plot3d(t\*s,t,s,angle=60°,grid=10):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-109.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-109.png)

Dengan lebih banyak usaha, kami dapat menghasilkan banyak permukaan.


Dalam contoh berikut, kita membuat tampilan bayangan dari bola yang
terdistorsi. Koordinat biasa untuk bola adalah


$$\gamma(t,s) = (\cos(t)\cos(s),\sin(t)\sin(s),\cos(s))$$dengan


$$0 \le t \le 2\pi, \quad \frac{-\pi}{2} \le s \le \frac{\pi}{2}.$$Kami mendistorsi ini dengan sebuah faktor


$$d(t,s) = \frac{\cos(4t)+\cos(8s)}{4}.$$\>t=linspace(0,2pi,320); s=linspace(-pi/2,pi/2,160)'; ...  
\>   d=1+0.2\*(cos(4\*t)+cos(8\*s)); ...  
\>   plot3d(cos(t)\*cos(s)\*d,sin(t)\*cos(s)\*d,sin(s)\*d,hue=1, ...  
\>     light=[1,0,1],frame=0,zoom=5):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-113.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-113.png)

\>t=linspace(0,2pi,270); s=linspace(-pi/2,pi/2,80)'; ...  
\>   d=1+0.2\*(cos(4\*t)+cos(8\*s)); ...  
\>   plot3d(cos(t)\*cos(s)\*d,sin(t)\*cos(s)\*d,sin(s)\*d,hue=1, ...  
\>     light=[1,0,1],frame=0,zoom=5):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-114.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-114.png)

Dalam percobaan saya ini ternyata dengan fungsi tersebut dapat
membentuk sebuah bunga.


berikut beberapa bentuk contohnya


\>t=linspace(0,pi,320); s=linspace(-pi/2,pi/2,150)'; ...  
\>   d=1+5\*(cos(2\*t)+cos(4\*s)); ...  
\>   plot3d(cos(t)\*cos(s)\*d,sin(t)\*cos(s)\*d,sin(s)\*d,hue=1, ...  
\>     light=[1,0,1],frame=0,zoom=5):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-115.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-115.png)

\>t=linspace(0,pi,320); s=linspace(-pi/2,pi/2,150)'; ...  
\>   d=1+7\*(cos(2\*t)+cos(4\*s)); ...  
\>   plot3d(cos(t)\*cos(s)\*d,sin(t)\*cos(s)\*d,sin(s)\*d,hue=1, ...  
\>     light=[1,0,1],frame=0,zoom=5):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-116.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-116.png)

\>t=linspace(0,pi,260); s=linspace(-pi/2,pi/2,120)'; ...  
\>   d=1+10\*(cos(3\*t)+cos(7\*s)); ...  
\>   plot3d(cos(t)\*cos(s)\*d,sin(t)\*cos(s)\*d,sin(s)\*d,hue=1, ...  
\>     light=[1,0,1],frame=0,zoom=5):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-117.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-117.png)

\>t=linspace(0,pi,260); s=linspace(-pi/2,pi/2,120)'; ...  
\>   d=1+15\*(cos(7\*t)+cos(8\*s)); ...  
\>   plot3d(cos(t)\*cos(s)\*d,sin(t)\*cos(s)\*d,sin(s)\*d,hue=1, ...  
\>     light=[1,0,1],frame=0,zoom=5):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-118.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-118.png)

\>t=linspace(0,pi,270); s=linspace(-pi/2,pi/2,180)'; ...  
\>   d=1+15\*(cos(10\*t)+cos(12\*s)); ...  
\>   plot3d(cos(t)\*cos(s)\*d,sin(t)\*cos(s)\*d,sin(s)\*d,hue=1, ...  
\>     light=[1,0,1],frame=0,zoom=5):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-119.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-119.png)

Tentu saja, titik cloud juga dimungkinkan. Untuk memplot data titik
dalam ruang, kita membutuhkan tiga vektor untuk koordinat titik-titik
tersebut.


Gayanya sama seperti di plot2d dengan points=true;


\>n=500;  ...  
\>     plot3d(normal(1,n),normal(1,n),normal(1,n),points=true,style="."):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-120.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-120.png)

\>n=1000;  ...  
\>     plot3d(normal(1,n),normal(1,n),normal(1,n),points=true,style="--"):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-121.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-121.png)

\>n=1000;  ...  
\>     plot3d(normal(1,n),normal(1,n),normal(1,n),points=true,style=".."):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-122.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-122.png)

\>n=500;  ...  
\>     plot3d(normal(1,n),normal(1,n),normal(1,n),points=true,style="\*\*"):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-123.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-123.png)

Dimungkinkan juga untuk memplot kurva dalam 3D. Dalam hal ini, lebih
mudah untuk menghitung titik-titik kurva. Untuk kurva di pesawat kami
menggunakan urutan koordinat dan parameter wire=true.


\>t=linspace(0,8pi,500); ...  
\>   plot3d(sin(t),cos(t),t/10,\>wire,zoom=3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-124.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-124.png)

\>t=linspace(0,7pi,1000); ...  
\>   plot3d(sin(t),cos(t),t/6,\>wire,zoom=3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-125.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-125.png)

\>t=linspace(0,8\*pi,1000); ...  
\>   plot3d(sin(t),cos(t),t/5,\>wire,zoom=3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-126.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-126.png)

\>t=linspace(0,8\*pi,3000); ...  
\>   plot3d(sin(t),cos(t),t/10,\>wire,zoom=3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-127.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-127.png)

\>t=linspace(0,4pi,1000); plot3d(cos(t),sin(t),t/2pi,\>wire, ...  
\>   linewidth=3,wirecolor=blue):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-128.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-128.png)

\>t=linspace(0,4pi,4000); plot3d(cos(t),sin(t),t/2pi,\>wire, ...  
\>   linewidth=3,wirecolor=red):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-129.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-129.png)

\>t=linspace(0,4pi,4000); plot3d(cos(t),sin(t),t/pi,\>wire, ...  
\>   linewidth=3,wirecolor=red):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-130.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-130.png)

\>X=cumsum(normal(3,1000)); ...  
\>    plot3d(X[1],X[2],X[3],\>anaglyph,\>wire):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-131.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-131.png)

\>X=cumsum(normal(5,100)); ...  
\>    plot3d(X[1],X[2],X[3],\>anaglyph,\>wire):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-132.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-132.png)

\>X=cumsum(normal(6,600)); ...  
\>    plot3d(X[1],X[2],X[3],\>anaglyph,\>wire):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-133.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-133.png)

EMT juga dapat memplot dalam mode anaglyph. Untuk melihat plot seperti
itu, Anda memerlukan kacamata merah/sian.


\> plot3d("x^2+y^3",\>anaglyph,\>contour,angle=30°):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-134.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-134.png)

\>plot3d("x^2+y^2",\>anaglyph,\>contour,angle=60°):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-135.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-135.png)

\> plot3d("x^3-y^3",\>anaglyph,\>contour,angle=75°):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-136.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-136.png)

\> plot3d("x^4+y^5",\>anaglyph,\>contour,angle=60°):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-137.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-137.png)

\> plot3d("x^2+y^7",\>anaglyph,\>contour,angle=90°):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-138.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-138.png)

\> plot3d("x^5-y^3",\>anaglyph,\>contour,angle=80°):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-139.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-139.png)

\> plot3d("x^2+y^8",\>anaglyph,\>contour,angle=180°):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-140.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-140.png)

\> plot3d("x^9-y^6",\>anaglyph,\>contour,angle=30°):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-141.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-141.png)

Seringkali, skema warna spektral digunakan untuk plot. Ini menekankan
ketinggian fungsi.


\>plot3d("x^2\*y^3-y",\>spectral,\>contour,zoom=3.2):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-142.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-142.png)

\>plot3d("x^3\*y^4+y",\>spectral,\>contour,zoom=3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-143.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-143.png)

\>plot3d("x^6\*y^3-y",\>spectral,\>contour,zoom=2.5):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-144.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-144.png)

\>plot3d("x^9\*y^4+y",\>spectral,\>contour,zoom=2.5):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-145.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-145.png)

\>plot3d("x^3\*y^9+3y",\>spectral,\>contour,zoom=3.2):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-146.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-146.png)

Euler juga dapat memplot permukaan berparameter, ketika parameternya
adalah nilai x-, y-, dan z dari gambar kotak persegi panjang dalam
ruang.


Untuk demo berikut, kami mengatur parameter u- dan v-, dan
menghasilkan koordinat ruang dari ini.


\>u=linspace(-1,1,10); v=linspace(0,2\*pi,50)'; ...  
\>   X=(3+u\*cos(v/2))\*cos(v); Y=(3+u\*cos(v/2))\*sin(v); Z=u\*sin(v/2); ...  
\>   plot3d(X,Y,Z,\>anaglyph,<frame,\>wire,scale=2.3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-147.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-147.png)

\>u=linspace(-1,1,10); v=linspace(0,2\*pi,100)'; ...  
\>   X=(4+u\*cos(v/2))\*cos(v); Y=(4+u\*cos(v/2))\*sin(v); Z=u\*sin(v/2); ...  
\>   plot3d(X,Y,Z,\>anaglyph,<frame,\>wire,scale=2.3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-148.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-148.png)

\>u=linspace(-1,1,10); v=linspace(0,4\*pi,70)'; ...  
\>   X=(5-u\*cos(v/2))\*cos(v); Y=(5-u\*cos(v/2))\*sin(v); Z=u\*sin(v/2); ...  
\>   plot3d(X,Y,Z,\>anaglyph,<frame,\>wire,scale=2.3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-149.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-149.png)

Berikut adalah contoh yang lebih rumit, yang megah dengan kacamata
merah/sian.


\>u:=linspace(-pi,pi,160); v:=linspace(-pi,pi,400)';  ...  
\>   x:=(4\*(1+.25\*sin(3\*v))+cos(u))\*cos(2\*v); ...  
\>   y:=(4\*(1+.25\*sin(3\*v))+cos(u))\*sin(2\*v); ...  
\>    z=sin(u)+2\*cos(3\*v); ...  
\>   plot3d(x,y,z,frame=0,scale=1.5,hue=1,light=[1,0,-1],zoom=2.8,\>anaglyph):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-150.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-150.png)

\>u:=linspace(-pi,pi,160); v:=linspace(-pi,pi,500)';  ...  
\>   x:=(4\*(2+.25\*sin(3\*v))+cos(u))\*cos(2\*v); ...  
\>   y:=(4\*(2+.25\*sin(3\*v))+cos(u))\*sin(2\*v); ...  
\>    z=sin(u)+2\*cos(3\*v); ...  
\>   plot3d(x,y,z,frame=0,scale=1.5,hue=1,light=[1,0,-1],zoom=3,\>anaglyph):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-151.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-151.png)

\>u:=linspace(-pi,pi,170); v:=linspace(-pi,pi,700)';  ...  
\>   x:=(5\*(1+.25\*sin(3\*v))+cos(u))\*cos(2\*v); ...  
\>   y:=(5\*(1+.25\*sin(3\*v))+cos(u))\*sin(2\*v); ...  
\>    z=sin(u)+2\*cos(3\*v); ...  
\>   plot3d(x,y,z,frame=0,scale=1.5,hue=1,light=[1,0,-1],zoom=2,\>anaglyph):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-152.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-152.png)

\>u:=linspace(-pi,pi,160); v:=linspace(-pi,pi,400)';  ...  
\>   x:=(4\*(1+.75\*sin(3\*v))+cos(u))\*cos(4\*v); ...  
\>   y:=(4\*(1+.75\*sin(3\*v))+cos(u))\*sin(4\*v); ...  
\>    z=sin(u)+2\*cos(3\*v); ...  
\>   plot3d(x,y,z,frame=0,scale=1.5,hue=1,light=[1,0,-1],zoom=2.8,\>anaglyph):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-153.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-153.png)

# Plot Statistik

Plot bar juga dimungkinkan. Untuk ini, kita harus menyediakan


* 
x: vektor baris dengan n+1 elemen

* 
y: vektor kolom dengan n+1 elemen

* 
z: matriks nilai nxn.


z bisa lebih besar, tetapi hanya nilai nxn yang akan digunakan.


Dalam contoh, pertama-tama kita menghitung nilainya. Kemudian kita
sesuaikan x dan y, sehingga vektor berpusat pada nilai yang digunakan.


\>x=-1:0.1:1; y=x'; z=x^2+y^2; ...  
\>   xa=(x|1.1)-0.05; ya=(y\_1.1)-0.05; ...  
\>   plot3d(xa,ya,z,bar=true):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-154.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-154.png)

\>x=-1:0.1:1; y=x'; z=x^3+y^3; ...  
\>   xa=(x|1.1)-0.05; ya=(y\_1.1)-0.05; ...  
\>   plot3d(xa,ya,z,bar=true):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-155.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-155.png)

\>x=-1:0.5:1; y=x'; z=x^2-y^2; ...  
\>   xa=(x|1.1)-0.05; ya=(y\_1.1)-0.05; ...  
\>   plot3d(xa,ya,z,bar=true):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-156.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-156.png)

\>x=-1:0.3:1; y=x'; z=x^4+y^4; ...  
\>   xa=(x|1.1)-0.05; ya=(y\_1.1)-0.05; ...  
\>   plot3d(xa,ya,z,bar=true):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-157.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-157.png)

Dimungkinkan untuk membagi plot permukaan menjadi dua atau lebih
bagian.


\>x=-1:0.1:1; y=x'; z=x+y; d=zeros(size(x)); ...  
\>   plot3d(x,y,z,disconnect=2:2:20):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-158.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-158.png)

\>x=-1:0.5:1; y=x'; z=x+y; d=zeros(size(x)); ...  
\>   plot3d(x,y,z,disconnect=2:2:20):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-159.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-159.png)

\>x=-2:0.2:2; y=x'; z=x+y; d=zeros(size(x)); ...  
\>   plot3d(x,y,z,disconnect=2:2:10):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-160.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-160.png)

\>x=-3:0.3:3; y=x'; z=x+y; d=zeros(size(x)); ...  
\>   plot3d(x,y,z,disconnect=2:2:30):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-161.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-161.png)

Jika memuat atau menghasilkan matriks data M dari file dan perlu
memplotnya dalam 3D, Anda dapat menskalakan matriks ke [-1,1] dengan
scale(M), atau menskalakan matriks dengan &gt;zscale. Ini dapat
dikombinasikan dengan faktor penskalaan individu yang diterapkan
sebagai tambahan.


\>i=1:20; j=i'; ...  
\>   plot3d(i\*j^2+100\*normal(20,20),\>zscale,scale=[1,1,1.5],angle=-40°,zoom=1.8):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-162.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-162.png)

\>i=1:20; j=i'; ...  
\>   plot3d(i\*j^2+100\*normal(20,20),\>zscale,scale=[1,1,2],angle=-50°,zoom=1.8):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-163.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-163.png)

\>Z=intrandom(5,100,6); v=zeros(5,6); ...  
\>   loop 1 to 5; v[#]=getmultiplicities(1:6,Z[#]); end; ...  
\>   columnsplot3d(v',scols=1:5,ccols=[1:5]):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-164.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-164.png)

# Permukaan Benda Putar

\>plot2d("(x^2+y^2-1)^3-x^2\*y^3",r=1.3, ...  
\>   style="#",color=red,<outline, ...  
\>   level=[-2;0],n=100):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-165.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-165.png)

\>ekspresi &= (x^2+y^2-1)^3-x^2\*y^3; $ekspresi


$$\left(y^2+x^2-1\right)^3-x^2\,y^3$$Kami ingin memutar kurva jantung di sekitar sumbu y. Berikut adalah
ungkapan, yang mendefinisikan hati:


$$f(x,y)=(x^2+y^2-1)^3-x^2.y^3.$$Selanjutnya kita atur


$$x=r.cos(a),\quad y=r.sin(a).$$\>function fr(r,a) &= ekspresi with [x=r\*cos(a),y=r\*sin(a)] | trigreduce; $fr(r,a)


$$\left(r^2-1\right)^3+\frac{\left(\sin \left(5\,a\right)-\sin \left(  3\,a\right)-2\,\sin a\right)\,r^5}{16}$$Hal ini memungkinkan untuk mendefinisikan fungsi numerik, yang
memecahkan r, jika a diberikan. Dengan fungsi itu kita dapat memplot
jantung yang diputar sebagai permukaan parametrik.


\>function map f(a) := bisect("fr",0,2;a); ...  
\>   t=linspace(-pi/2,pi/2,100); r=f(t);  ...  
\>   s=linspace(pi,2pi,100)'; ...  
\>   plot3d(r\*cos(t)\*sin(s),r\*cos(t)\*cos(s),r\*sin(t), ...  
\>   \>hue,<frame,color=red,zoom=4,amb=0,max=0.7,grid=12,height=50°):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-170.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-170.png)

Berikut ini adalah plot 3D dari gambar di atas yang diputar di sekitar
sumbu z. Kami mendefinisikan fungsi, yang menggambarkan objek.


\>function f(x,y,z) ...


    r=x^2+y^2;
    return (r+z^2-1)^3-r*z^3;
     endfunction
</pre>
\>plot3d("f(x,y,z)", ...  
\>   xmin=0,xmax=1.2,ymin=-1.2,ymax=1.2,zmin=-1.2,zmax=1.4, ...  
\>   implicit=1,angle=-30°,zoom=2.5,n=[10,60,60],\>anaglyph):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-171.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-171.png)

# Plot 3D Khusus

Fungsi plot3d bagus untuk dimiliki, tetapi tidak memenuhi semua
kebutuhan. Selain rutinitas yang lebih mendasar, dimungkinkan untuk
mendapatkan plot berbingkai dari objek apa pun yang Anda suka.


Meskipun Euler bukan program 3D, ia dapat menggabungkan beberapa objek
dasar. Kami mencoba memvisualisasikan paraboloid dan garis
singgungnya.


\>function myplot ...


      y=0:0.01:1; x=(0.1:0.01:1)';
      plot3d(x,y,0.2*(x-0.1)/2,<scale,<frame,>hue, ..
        hues=0.5,>contour,color=orange);
      h=holding(1);
      plot3d(x,y,(x^2+y^2)/2,<scale,<frame,>contour,>hue);
      holding(h);
    endfunction
</pre>
Sekarang framedplot() menyediakan frame, dan mengatur tampilan.


\>framedplot("myplot",[0.1,1,0,1,0,1],angle=-45°, ...  
\>     center=[0,0,-0.7],zoom=6):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-172.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-172.png)

Dengan cara yang sama, Anda dapat memplot bidang kontur secara manual.
Perhatikan bahwa plot3d() menyetel jendela ke fullwindow() secara
default, tetapi plotcontourplane() mengasumsikan itu.


\>x=-1:0.02:1.1; y=x'; z=x^2-y^4;

\>function myplot (x,y,z) ...  
\>  
<pre class="udf">      zoom(2);
      wi=fullwindow();
      plotcontourplane(x,y,z,level="auto",<scale);
      plot3d(x,y,z,>hue,<scale,>add,color=white,level="thin");
      window(wi);
      reset();
    endfunction
</pre>
\>myplot(x,y,z):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-173.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-173.png)

# Animasi

Euler dapat menggunakan frame untuk menghitung animasi terlebih
dahulu.


Salah satu fungsi yang memanfaatkan teknik ini adalah rotate. Itu
dapat mengubah sudut pandang dan menggambar ulang plot 3D. Fungsi
memanggil addpage() untuk setiap plot baru. Akhirnya itu menjiwai
plot.


Silakan pelajari sumber rotasi untuk melihat lebih detail.


\>function testplot () := plot3d("x^2+y^3"); ...  
\>   rotate("testplot"); testplot():


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-174.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-174.png)

*Menggambar Povray


Dengan bantuan file Euler povray.e, Euler dapat menghasilkan file
Povray. Hasilnya sangat bagus untuk dilihat.


Anda perlu menginstal Povray (32bit atau 64bit) dari
  <a href="http://www.povray.org/, dan meletakkan sub-direktori "bin" dari Povray ke jalur lingkungan, atau mengatur variabel "defaultpovray" dengan path lengkap yang menunjuk ke "pvengine.exe".">http://www.povray.org/, dan meletakkan sub-direktori "bin" dari Povray ke jalur lingkungan, atau mengatur variabel "defaultpovray" dengan path lengkap yang menunjuk ke "pvengine.exe".</a>


Antarmuka Povray dari Euler menghasilkan file Povray di direktori home
pengguna, dan memanggil Povray untuk mengurai file-file ini. Nama file
default adalah current.pov, dan direktori default adalah eulerhome(),
biasanya c:\Users\Username\Euler. Povray menghasilkan file PNG, yang
dapat dimuat oleh Euler ke dalam buku catatan. Untuk membersihkan
file-file ini, gunakan povclear().


Fungsi pov3d memiliki semangat yang sama dengan plot3d. Ini dapat
menghasilkan grafik fungsi f(x,y), atau permukaan dengan koordinat
X,Y,Z dalam matriks, termasuk garis level opsional. Fungsi ini memulai
raytracer secara otomatis, dan memuat adegan ke dalam notebook Euler.


Selain pov3d(), ada banyak fungsi yang menghasilkan objek Povray.
Fungsi-fungsi ini mengembalikan string, yang berisi kode Povray untuk
objek. Untuk menggunakan fungsi ini, mulai file Povray dengan
povstart(). Kemudian gunakan writeln(...) untuk menulis objek ke file
adegan. Terakhir, akhiri file dengan povend(). Secara default,
raytracer akan dimulai, dan PNG akan dimasukkan ke dalam notebook
Euler.


Fungsi objek memiliki parameter yang disebut "look", yang membutuhkan
string dengan kode Povray untuk tekstur dan hasil akhir objek. Fungsi
povlook() dapat digunakan untuk menghasilkan string ini. Ini memiliki
parameter untuk warna, transparansi, Phong Shading dll.


Perhatikan bahwa alam semesta Povray memiliki sistem koordinat lain.
Antarmuka ini menerjemahkan semua koordinat ke sistem Povray. Jadi
Anda dapat terus berpikir dalam sistem koordinat Euler dengan z
menunjuk vertikal ke atas, a nd x,y,z sumbu dalam arti tangan kanan.


Anda perlu memuat file povray.


\>load povray;


Pastikan, direktori bin Povray ada di jalurnya. Jika tidak, edit
variabel berikut sehingga berisi path ke povray yang dapat dieksekusi.


\>defaultpovray="C:\\Program Files\\POV-Ray\\v3.7\\bin\\pvengine.exe"


    C:\Program Files\POV-Ray\v3.7\bin\pvengine.exe

Untuk kesan pertama, kami memplot fungsi sederhana. Perintah berikut
menghasilkan file povray di direktori pengguna Anda, dan menjalankan
Povray untuk ray tracing file ini.


Jika Anda memulai perintah berikut, GUI Povray akan terbuka,
menjalankan file, dan menutup secara otomatis. Karena alasan keamanan,
Anda akan ditanya, apakah Anda ingin mengizinkan file exe untuk
dijalankan. Anda dapat menekan batal untuk menghentikan pertanyaan
lebih lanjut. Anda mungkin harus menekan OK di jendela Povray untuk
mengakui dialog awal Povray.


\>pov3d("x^2+y^2",zoom=3);


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-175.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-175.png)

\>pov3d("x^3+y^3",zoom=3);


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-176.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-176.png)

Kita dapat membuat fungsi menjadi transparan dan menambahkan hasil
akhir lainnya. Kami juga dapat menambahkan garis level ke plot fungsi.


\>pov3d("x^2+y^3",axiscolor=red,angle=20°, ...  
\>     look=povlook(blue,0.2),level=-1:0.5:1,zoom=3.8);


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-177.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-177.png)

\>pov3d("x^2+y^4",axiscolor=red,angle=25°, ...  
\>     look=povlook(blue,0.2),level=-1:0.5:1,zoom=3.8);


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-178.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-178.png)

Terkadang perlu untuk mencegah penskalaan fungsi, dan menskalakan
fungsi dengan tangan.


Kami memplot himpunan titik di bidang kompleks, di mana produk dari
jarak ke 1 dan -1 sama dengan 1.


\>pov3d("((x-1)^2+y^2)\*((x+1)^2+y^2)/40",r=1.5, ...  
\>     angle=-120°,level=1/40,dlevel=0.005,light=[-1,1,1],height=45°,n=50, ...  
\>     <fscale,zoom=3.8);


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-179.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-179.png)

\>pov3d("((x-1)^3+y^3)\*((x+1)^2+y^2)/40",r=1.5, ...  
\>     angle=-120°,level=1/40,dlevel=0.005,light=[-1,1,1],height=90°,n=50, ...  
\>     <fscale,zoom=3.8);


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-180.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-180.png)

# Merencanakan dengan Koordinat

Alih-alih fungsi, kita dapat memplot dengan koordinat. Seperti pada
plot3d, kita membutuhkan tiga matriks untuk mendefinisikan objek.


Dalam contoh kita memutar fungsi di sekitar sumbu z.


\>function f(x) := x^3-x+1; ...  
\>   x=-1:0.01:1; t=linspace(0,2pi,8)'; ...  
\>   Z=x; X=cos(t)\*f(x); Y=sin(t)\*f(x); ...  
\>   pov3d(X,Y,Z,angle=40°,height=20°,axis=0,zoom=4,light=[10,-5,5]);


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-181.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-181.png)

\>function f(x) := x^4+x+1; ...  
\>   x=-1:0.01:1; t=linspace(0,2pi,8)'; ...  
\>   Z=x; X=cos(t)\*f(x); Y=sin(t)\*f(x); ...  
\>   pov3d(X,Y,Z,angle=40°,height=20°,axis=0,zoom=4,light=[10,-5,5]);


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-182.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-182.png)

Dalam contoh berikut, kami memplot gelombang teredam. Kami
menghasilkan gelombang dengan bahasa matriks Euler.


Kami juga menunjukkan, bagaimana objek tambahan dapat ditambahkan ke
adegan pov3d. Untuk pembuatan objek, lihat contoh berikut. Perhatikan
bahwa plot3d menskalakan plot, sehingga cocok dengan kubus satuan.


\>r=linspace(0,1,80); phi=linspace(0,2pi,80)'; ...  
\>   x=r\*cos(phi); y=r\*sin(phi); z=exp(-5\*r)\*cos(8\*pi\*r)/3;  ...  
\>   pov3d(x,y,z,zoom=5,axis=0,add=povsphere([0,0,0.5],0.1,povlook(green)), ...  
\>     w=500,h=300);


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-183.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-183.png)

\>r=linspace(0,1,80); phi=linspace(0,pi,80)'; ...  
\>   x=r\*cos(phi); y=r\*sin(phi); z=exp(-5\*r)\*cos(8\*pi\*r)/3;  ...  
\>   pov3d(x,y,z,zoom=5,axis=0,add=povsphere([0,0,0.5],0.1,povlook(green)), ...  
\>     w=500,h=300);


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-184.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-184.png)

Dengan metode bayangan canggih dari Povray, sangat sedikit titik yang
dapat menghasilkan permukaan yang sangat halus. Hanya di perbatasan
dan dalam bayang-bayang triknya mungkin menjadi jelas.


Untuk ini, kita perlu menambahkan vektor normal di setiap titik
matriks.


\>Z &= x^2\*y^3


    
                                     2  3
                                    x  y
    

Persamaan permukaannya adalah [x,y,Z]. Kami menghitung dua turunan ke
x dan y ini dan mengambil produk silang sebagai normal.


\>dx &= diff([x,y,Z],x); dy &= diff([x,y,Z],y);


Kami mendefinisikan normal sebagai produk silang dari turunan ini, dan
mendefinisikan fungsi koordinat.


\>N &= crossproduct(dx,dy); NX &= N[1]; NY &= N[2]; NZ &= N[3]; N,


    
                                   3       2  2
                           [- 2 x y , - 3 x  y , 1]
    

Kami hanya menggunakan 25 poin.


\>x=-1:0.5:1; y=x';

\>pov3d(x,y,Z(x,y),angle=10°, ...  
\>     xv=NX(x,y),yv=NY(x,y),zv=NZ(x,y),<shadow);


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-185.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-185.png)

Berikut ini adalah simpul Trefoil yang dilakukan oleh A. Busser di
Povray. Ada versi yang ditingkatkan dari ini dalam contoh.


Lihat: Contoh\Trefoil Simpul | Simpul trefoil


Untuk tampilan yang bagus dengan tidak terlalu banyak titik, kami
menambahkan vektor normal di sini. Kami menggunakan Maxima untuk
menghitung normal bagi kami. Pertama, ketiga fungsi koordinat sebagai
ekspresi simbolik.


\>X &= ((4+sin(3\*y))+cos(x))\*cos(2\*y); ...  
\>   Y &= ((4+sin(3\*y))+cos(x))\*sin(2\*y); ...  
\>   Z &= sin(x)+2\*cos(3\*y);


Kemudian kedua vektor turunan ke x dan y.


\>dx &= diff([X,Y,Z],x); dy &= diff([X,Y,Z],y);


Sekarang normal, yang merupakan produk silang dari dua turunan.


\>dn &= crossproduct(dx,dy);


Kami sekarang mengevaluasi semua ini secara numerik.


\>x:=linspace(-%pi,%pi,40); y:=linspace(-%pi,%pi,100)';


Vektor normal adalah evaluasi dari ekspresi simbolik dn[i] untuk
i=1,2,3. Sintaks untuk ini adalah &amp;"expression"(parameters). Ini
adalah alternatif dari metode pada contoh sebelumnya, di mana kita
mendefinisikan ekspresi simbolik NX, NY, NZ terlebih dahulu.


\>pov3d(X(x,y),Y(x,y),Z(x,y),axis=0,zoom=5,w=450,h=350, ...  
\>     <shadow,look=povlook(gray), ...  
\>     xv=&"dn[1]"(x,y), yv=&"dn[2]"(x,y), zv=&"dn[3]"(x,y));


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-186.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-186.png)

Kami juga dapat menghasilkan grid dalam 3D.


\>povstart(zoom=4); ...  
\>   x=-1:0.5:1; r=1-(x+1)^2/6; ...  
\>   t=(0°:30°:360°)'; y=r\*cos(t); z=r\*sin(t); ...  
\>   writeln(povgrid(x,y,z,d=0.02,dballs=0.05)); ...  
\>   povend();


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-187.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-187.png)

Dengan povgrid(), kurva dimungkinkan.


\>povstart(center=[0,0,1],zoom=3.6); ...  
\>   t=linspace(0,2,1000); r=exp(-t); ...  
\>   x=cos(2\*pi\*10\*t)\*r; y=sin(2\*pi\*10\*t)\*r; z=t; ...  
\>   writeln(povgrid(x,y,z,povlook(red))); ...  
\>   writeAxis(0,2,axis=3); ...  
\>   povend();


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-188.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-188.png)

# Objek Povray

Di atas, kami menggunakan pov3d untuk memplot permukaan. Antarmuka
povray di Euler juga dapat menghasilkan objek Povray. Objek-objek ini
disimpan sebagai string di Euler, dan perlu ditulis ke file Povray.


Kami memulai output dengan povstart().


\>povstart(zoom=4);


Pertama kita mendefinisikan tiga silinder, dan menyimpannya dalam
string di Euler.


Fungsi povx() dll. hanya mengembalikan vektor [1,0,0], yang dapat
digunakan sebagai gantinya.


\>c1=povcylinder(-povx,povx,1,povlook(red)); ...  
\>   c2=povcylinder(-povy,povy,1,povlook(green)); ...  
\>   c3=povcylinder(-povz,povz,1,povlook(blue)); ...  
\>  
String berisi kode Povray, yang tidak perlu kita pahami pada saat itu.


\>c1


    cylinder { &lt;-1,0,0&gt;, &lt;1,0,0&gt;, 1
     texture { pigment { color rgb &lt;0.564706,0.0627451,0.0627451&gt; }  } 
     finish { ambient 0.2 } 
     }

Seperti yang Anda lihat, kami menambahkan tekstur ke objek dalam tiga
warna berbeda.


Itu dilakukan oleh povlook(), yang mengembalikan string dengan kode
Povray yang relevan. Kita dapat menggunakan warna Euler default, atau
menentukan warna kita sendiri. Kami juga dapat menambahkan
transparansi, atau mengubah cahaya sekitar.


\>povlook(rgb(0.1,0.2,0.3),0.1,0.5)


     texture { pigment { color rgbf &lt;0.101961,0.2,0.301961,0.1&gt; }  } 
     finish { ambient 0.5 } 
    

Sekarang kita mendefinisikan objek persimpangan, dan menulis hasilnya
ke file.


\>writeln(povintersection([c1,c2,c3]));


Persimpangan tiga silinder sulit untuk divisualisasikan, jika Anda
belum pernah melihatnya sebelumnya.


\>povend;


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-189.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-189.png)

Fungsi berikut menghasilkan fraktal secara rekursif.


Fungsi pertama menunjukkan, bagaimana Euler menangani objek Povray
sederhana. Fungsi povbox() mengembalikan string, yang berisi koordinat
kotak, tekstur, dan hasil akhir.


\>function onebox(x,y,z,d) := povbox([x,y,z],[x+d,y+d,z+d],povlook());

\>function fractal (x,y,z,h,n) ...  
\>  
<pre class="udf">     if n==1 then writeln(onebox(x,y,z,h));
     else
       h=h/3;
       fractal(x,y,z,h,n-1);
       fractal(x+2*h,y,z,h,n-1);
       fractal(x,y+2*h,z,h,n-1);
       fractal(x,y,z+2*h,h,n-1);
       fractal(x+2*h,y+2*h,z,h,n-1);
       fractal(x+2*h,y,z+2*h,h,n-1);
       fractal(x,y+2*h,z+2*h,h,n-1);
       fractal(x+2*h,y+2*h,z+2*h,h,n-1);
       fractal(x+h,y+h,z+h,h,n-1);
     endif;
    endfunction
</pre>
\>povstart(fade=10,<shadow);

\>fractal(-1,-1,-1,2,4);

\>povend();


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-190.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-190.png)

Perbedaan memungkinkan memotong satu objek dari yang lain. Seperti
persimpangan, ada bagian dari objek CSG Povray.


\>povstart(light=[5,-5,5],fade=10);


Untuk demonstrasi ini, kami mendefinisikan objek di Povray, alih-alih
menggunakan string di Euler. Definisi ditulis ke file segera.


Koordinat kotak -1 berarti [-1,-1,-1].


\>povdefine("mycube",povbox(-1,1));


Kita dapat menggunakan objek ini di povobject(), yang mengembalikan
string seperti biasa.


\>c1=povobject("mycube",povlook(red));


Kami menghasilkan kubus kedua, dan memutar dan menskalakannya sedikit.


\>c2=povobject("mycube",povlook(yellow),translate=[1,1,1], ...  
\>     rotate=xrotate(10°)+yrotate(10°), scale=1.2);


Kemudian kita ambil selisih kedua benda tersebut.


\>writeln(povdifference(c1,c2));


Sekarang tambahkan tiga sumbu.


\>writeAxis(-1.2,1.2,axis=1); ...  
\>   writeAxis(-1.2,1.2,axis=2); ...  
\>   writeAxis(-1.2,1.2,axis=4); ...  
\>   povend();


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-191.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-191.png)

# Fungsi Implisit

Povray dapat memplot himpunan di mana f(x,y,z)=0, seperti parameter
implisit di plot3d. Namun, hasilnya terlihat jauh lebih baik.


Sintaks untuk fungsinya sedikit berbeda. Anda tidak dapat menggunakan
output dari ekspresi Maxima atau Euler.


\>povstart(angle=70°,height=50°,zoom=4);


Buat permukaan implisit. Perhatikan sintaks yang berbeda dalam
ekspresi.


\>writeln(povsurface("pow(x,2)\*y-pow(y,3)-pow(z,2)",povlook(green))); ...  
\>   writeAxes(); ...  
\>   povend();


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-192.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-192.png)

# Objek Jala

Dalam contoh ini, kami menunjukkan cara membuat objek mesh, dan
menggambarnya dengan informasi tambahan.


Kami ingin memaksimalkan xy di bawah kondisi x+y=1 dan menunjukkan
sentuhan tangensial dari garis level.


\>povstart(angle=-10°,center=[0.5,0.5,0.5],zoom=7);


Kami tidak dapat menyimpan objek dalam string seperti sebelumnya,
karena terlalu besar. Jadi kita mendefinisikan objek dalam file Povray
menggunakan #declare. Fungsi povtriangle() melakukan ini secara
otomatis. Itu dapat menerima vektor normal seperti pov3d().


Berikut ini mendefinisikan objek mesh, dan langsung menulisnya ke
dalam file.


\>x=0:0.02:1; y=x'; z=x\*y; vx=-y; vy=-x; vz=1;

\>mesh=povtriangles(x,y,z,"",vx,vy,vz);


Sekarang kita mendefinisikan dua cakram, yang akan berpotongan dengan
permukaan.


\>cl=povdisc([0.5,0.5,0],[1,1,0],2); ...  
\>   ll=povdisc([0,0,1/4],[0,0,1],2);


Tulis permukaan dikurangi dua cakram.


\>writeln(povdifference(mesh,povunion([cl,ll]),povlook(green)));


Tulis dua persimpangan.


\>writeln(povintersection([mesh,cl],povlook(red))); ...  
\>   writeln(povintersection([mesh,ll],povlook(gray)));


Tulis titik maksimum.


\>writeln(povpoint([1/2,1/2,1/4],povlook(gray),size=2\*defaultpointsize));


Tambahkan sumbu dan selesaikan.


\>writeAxes(0,1,0,1,0,1,d=0.015); ...  
\>   povend();


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-193.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-193.png)

# Anaglyph di Povray

Untuk menghasilkan anaglyph untuk kacamata merah/sian, Povray harus
berjalan dua kali dari posisi kamera yang berbeda. Ini menghasilkan
dua file Povray dan dua file PNG, yang dimuat dengan fungsi
loadanaglyph().


Tentu saja, Anda memerlukan kacamata merah/sian untuk melihat contoh
berikut dengan benar.


Fungsi pov3d() memiliki sakelar sederhana untuk menghasilkan
anaglyphs.


\>pov3d("-exp(-x^2-y^2)/2",r=2,height=45°,\>anaglyph, ...  
\>     center=[0,0,0.5],zoom=3.5);


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-194.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-194.png)

Jika Anda membuat adegan dengan objek, Anda perlu menempatkan generasi
adegan ke dalam fungsi, dan menjalankannya dua kali dengan nilai yang
berbeda untuk parameter anaglyph.


\>function myscene ...


      s=povsphere(povc,1);
      cl=povcylinder(-povz,povz,0.5);
      clx=povobject(cl,rotate=xrotate(90°));
      cly=povobject(cl,rotate=yrotate(90°));
      c=povbox([-1,-1,0],1);
      un=povunion([cl,clx,cly,c]);
      obj=povdifference(s,un,povlook(red));
      writeln(obj);
      writeAxes();
    endfunction
</pre>
Fungsi povanaglyph() melakukan semua ini. Parameternya seperti di
povstart() dan povend() digabungkan.


\>povanaglyph("myscene",zoom=4.5);


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-195.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-195.png)

# Mendefinisikan Objek sendiri

Antarmuka povray Euler berisi banyak objek. Tapi Anda tidak terbatas
pada ini. Anda dapat membuat objek sendiri, yang menggabungkan objek
lain, atau objek yang sama sekali baru.


Kami mendemonstrasikan sebuah torus. Perintah Povray untuk ini adalah
"torus". Jadi kami mengembalikan string dengan perintah ini dan
parameternya. Perhatikan bahwa torus selalu berpusat di titik asal.


\>function povdonat (r1,r2,look="") ...


      return "torus {"+r1+","+r2+look+"}";
    endfunction
</pre>
=Inilah torus pertama kami.


\>t1=povdonat(0.8,0.2)


    torus {0.8,0.2}

Mari kita gunakan objek ini untuk membuat torus kedua, diterjemahkan
dan diputar.


\>t2=povobject(t1,rotate=xrotate(90°),translate=[0.8,0,0])


    object { torus {0.8,0.2}
     rotate 90 *x 
     translate &lt;0.8,0,0&gt;
     }

Sekarang kita menempatkan objek-objek ini ke dalam sebuah adegan.
Untuk tampilan, kami menggunakan Phong Shading.


\>povstart(center=[0.4,0,0],angle=0°,zoom=3.8,aspect=1.5); ...  
\>   writeln(povobject(t1,povlook(green,phong=1))); ...  
\>   writeln(povobject(t2,povlook(green,phong=1))); ...  
\>  
&gt;povend();


memanggil program Povray. Namun, jika terjadi kesalahan, itu tidak
menampilkan kesalahan. Karena itu Anda harus menggunakan


  &gt;povend(&lt;keluar);  

jika ada yang tidak berhasil. Ini akan membiarkan jendela Povray
terbuka.


\>povend(h=320,w=480);


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-196.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-196.png)

Berikut adalah contoh yang lebih rumit. Kami memecahkan


lateks: Ax \le b, \quad x \ge 0, \quad c.x \to \text{Max.}


dan menunjukkan titik layak dan optimal dalam plot 3D.


\>A=[10,8,4;5,6,8;6,3,2;9,5,6];

\>b=[10,10,10,10]';

\>c=[1,1,1];


Pertama, mari kita periksa, apakah contoh ini memiliki solusi sama
sekali.


\>x=simplex(A,b,c,\>max,\>check)'


    Variable or function A not found.
    Error in:
    x=simplex(A,b,c,&gt;max,&gt;check)' ...
               ^

Ya, sudah.


Selanjutnya kita mendefinisikan dua objek. Yang pertama adalah pesawat


$$a \cdot x \le b$$\>function oneplane (a,b,look="") ...


      return povplane(a,b,look)
    endfunction
</pre>
Kemudian kita mendefinisikan persimpangan semua setengah ruang dan
kubus.


\>function adm (A, b, r, look="") ...


      ol=[];
      loop 1 to rows(A); ol=ol|oneplane(A[#],b[#]); end;
      ol=ol|povbox([0,0,0],[r,r,r]);
      return povintersection(ol,look);
    endfunction
</pre>
Kita sekarang dapat merencanakan adegannya.


\>povstart(angle=120°,center=[0.5,0.5,0.5],zoom=3.5); ...  
\>   writeln(adm(A,b,2,povlook(green,0.4))); ...  
\>   writeAxes(0,1.3,0,1.6,0,1.5); ...  
\>  
Berikut ini adalah lingkaran di sekitar optimal.


\>writeln(povintersection([povsphere(x,0.5),povplane(c,c.x')], ...  
\>     povlook(red,0.9)));


    Variable or function A not found.
    Error in:
    ... 20°,center=[0.5,0.5,0.5],zoom=3.5); writeln(adm(A,b,2,povlook( ...
                                                         ^

Dan kesalahan ke arah yang optimal.


\>writeln(povarrow(x,c\*0.5,povlook(red)));


    Cannot combine a 1x51 and a 1x3 matrix for +!
    Try "trace errors" to inspect local variables after errors.
    povarrow:
        o1=povcylinder(x,x+v,d);

Kami menambahkan teks ke layar. Teks hanyalah objek 3D. Kita perlu
menempatkan dan memutarnya menurut pandangan kita.


\>writeln(povtext("Linear Problem",[0,0.2,1.3],size=0.05,rotate=125°)); ...  
\>   povend();


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-198.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-198.png)

# LATIHAN - LATIHAN SOAL Fungsi Dua Variabel atau Lebih

 Grafik dari fungsi f dengan dua variabel yang dimaksud adalah grafik  

dari persamaan z = f(x,y). Biasanya grafik ini berupa permukaan dan
karena setiap (x,y) di daerah asal hanya berpadanan dengan satu nilai
z, maka setiap garis tegaklurus bidang-xy memotong permukaan pada
paling banyak satu titik.


Soal :


1. Grafik merupakan sebuah paraboloida f(x,y) = y^2-x^2


2. z = -4x^3y^2


3. z = xy exp(-x^2-y^2)


4. z = x - 1/8x^3 - 1/3y^2


\>aspect(1.5); plot3d("y^2-x^2"):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-199.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-199.png)

\>aspect(1.5); plot3d("-4x^3\*y^2"):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-200.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-200.png)

\>plot3d("x\*y\*exp(-x^2-y^2)",r=2,<fscale,<scale,distance=13,height=20°, ...  
\>     center=[0,0,-0.2],frame=3):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-201.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-201.png)

\>aspect(1.5); plot3d("x-1/8\*x^3-1/3\*y^2"):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-202.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-202.png)

\>plot3d("sin(x)\*cos(y)"):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-203.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-203.png)

Membuat Talang (Perosotan pada kolam renang)


Dalam membuat perosotan kolam renang ini saya belum bisa membuat
secara bagus, karena perosotan yang saya buat masih kurang jadi dan
bentuknya pun masih dari arah kiri ke kanan, bahkan terlihat dari sisi
belakang dan  dari samping, belum terlihat dari depan.


\>plot3d("x^3-y^3",\>anaglyph,\>contour,angle=75°):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-204.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-204.png)

\>plot3d("x^3-y^3",\>anaglyph,\>contour,angle=20°):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-205.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-205.png)

\>plot3d("x^3+y^3",\>anaglyph,\>contour,angle=116°):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-206.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-206.png)

\>aspect(1.5); plot3d("x^3+sin(y)",-5,5,0,2\*pi):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-207.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-207.png)

\>aspect(1.5); plot3d("x^3-sin(2y)",-5,5,0,pi):


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-208.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-208.png)

\>load povray;

\>defaultpovray="C:\\Program Files\\POV-Ray\\v3.7\\bin\\pvengine.exe"


    C:\Program Files\POV-Ray\v3.7\bin\pvengine.exe

\>povstart(center=[0,0,1],zoom=3.6); ...  
\>   t=linspace(0,2,1000); r=exp(-t); ...  
\>   x=cos(2\*pi\*20\*t)\*r; y=sin(2\*pi\*10\*t)\*r; z=t; ...  
\>   writeln(povgrid(x,y,z,povlook(red))); ...  
\>   writeAxis(0,2,axis=4); ...  
\>   povend();


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-209.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-209.png)

\>povstart(center=[0,0,1],zoom=3); ...  
\>   t=linspace(0,2,1000); r=exp(-t); ...  
\>   x=cos(pi\*10\*t)\*r; y=sin(pi\*10\*t)\*r; z=t; ...  
\>   writeln(povgrid(x,y,z,povlook(yellow))); ...  
\>   writeAxis(0,2,axis=4); ...  
\>   povend();


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-210.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-210.png)

\>povstart(zoom=3); ...  
\>   x=-1:0.5:1; r=1-(x+1)^3/6; ...  
\>   t=(0°:30°:360°)'; y=r\*cos(t); z=r\*sin(t); ...  
\>   writeln(povgrid(x,y,z,d=0.02,dballs=0.05)); ...  
\>   povend();


![images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-211.png](images/Syifa%20Desta%20Rumaisha_22305141020_Plot%203D-211.png)

# Lebih Banyak Contoh

Anda dapat menemukan beberapa contoh lagi untuk Povray di Euler di
file berikut.


  <a href="Examples/Dandelin Spheres.html">Examples/Dandelin Spheres</a>  

  <a href="Examples/Donat Math.html">Examples/Donat Math</a>  

  <a href="Examples/Trefoil Knot.html">Examples/Trefoil Knot</a>  

  <a href="Examples/Optimization by Affine Scaling.html">Examples/Optimization by Affine Scaling</a>  

