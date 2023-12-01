# Syifa Desta Rumaisha_22305141020_Materi Integral Tak Tentu
---

# BAB 4. INTERGAL TAK TENTU (Antiderivatif)

MATERI INTEGRAL TAK TENTU Dibuat Oleh :


NAMA  : SYIFA DESTA RUMAISHA


KELAS : MATEMATIKA E


NIM   : 22305141020


---



CAKUPAN MATERI MELIPUTI DIANTARANYA:


-Defini Integral tak tentu


-Sifat- sifat integral tak tentu


-Integral tak tentu fungsi aljabar, trigonometri, eksponensial,
logaritma, dan komposisi fungsi


-Visualisasi dan kurva fungsi


1. Definisi Intergal Tak Tentu


    Integral tak tentu (indefinite integral) adalah integral yang  

tidak memiliki batas-batas nilai tertentu, sehingga hanya diperoleh
fungsi umumnya saja disertai suatu konstanta C.


    Misalkan diketahui suatu fungsi F(x) yang merupakan fungsi umum  

yang bersifat F'(x)=f(x), maka integral tak tentu merupakan himpunan
anti turunan F(x) dari f(x) pada interval negatif tak hingga sampai
tak hingga yang dinotasikan :


\>$F(x)=('integrate(f(x),x)+c)


Definisi kurva fungsi antiderifatif


      Kurva fungsi antiderivatif adalah kurva yang menggambarkan  

hubungan antara suatu fungsi dan antiderivatifnya. Antiderivatif, juga
dikenal sebagai integral tak tentu. Dalam integral, fungsi
antiderivatif dapat dianggap sebagai "anti turunan" dari fungsi
aslinya.


Contoh :


\>$F(x)=('integrate(3\*x^2,x)+c)

\>$showev('integrate(3\*x^2,x)+c)

\>plot2d(["3\*x^2","x^3","x^3+1","x^3+2","x^3+3"]): //grafik fungsinya, hasil integral, penambahan sebarang konstanta dari hasil integral 


Penyelesaiannya dengan memasukan sebarang nilai C


Contoh :


\>$F(x)=('integrate(x^5,x) +c)

\>$showev('integrate(x^5,x)+c)


$$\int {x^5}{\;dx}+c=\frac{x^6}{6}+c$$\>plot2d(["x^5","x^6/6","(x^6/6)+1","(x^6/6)+2"]):


![images/Syifa%20Desta%20Rumaisha_22305141020_Materi%20Integral%20Tak%20Tentu-002.png](images/Syifa%20Desta%20Rumaisha_22305141020_Materi%20Integral%20Tak%20Tentu-002.png)

---



2. Sifat-sifat Integral Tak Tentu


    Dalam perhitungan, integral tak tentu memiliki sifat-sifat yang  

dapat digunakan. Ada tiga sifat integral tak tentu yaitu sebagai
berikut:


   a. Sifat Pangkat


$$\int x^n dx + c = \frac {x^n+1}{n+1} + c$$\>$showev('integrate(x^n,x)+c)


    Answering "Is n equal to -1?" with "no"

$$\int {x^{n}}{\;dx}+c=\frac{x^{n+1}}{n+1}+c$$ b. Penjumlahan dan Pengurangan  

\>function f(x) &&= f(x)


    
                                     f(x)
    

\>function g(x) &&= g(x)


    
                                     g(x)
    

Penjumlahan


\>$('integrate([f(x)+g(x)],x))=('integrate(f(x),x))+('integrate(g(x),x))


$$\int {\left[ g\left(x\right)+f\left(x\right) \right] }{\;dx}=\int {  g\left(x\right)}{\;dx}+\int {f\left(x\right)}{\;dx}$$Pengurangan


\>$('integrate([f(x)+g(x)],x))=('integrate(f(x),x))-('integrate(g(x),x))


$$\int {\left[ g\left(x\right)+f\left(x\right) \right] }{\;dx}=\int {  f\left(x\right)}{\;dx}-\int {g\left(x\right)}{\;dx}$$c. Konstanta


$$\int k.f(x) dx = k \int f(x) dx$$\>$('integrate(kf(x),x))=(k\*'integrate(f(x),x))


---



3. INTERGAL TAK TENTU FUNGSI ALJABAR


    A. Defnisi  
      Integral tak tentu fungsi aljabar merupakan sebuah operasi  

matematika yang menghasilkan fungsi lain yang turunan parsialnya akan
sama dengan fungsi asal. Dalam konteks fungsi aljabar, integral tak
tentu biasanya melibatkan fungsi-fungsi seperti polinomial,
eksponensial, dan trigonometri, dan menghasilkan fungsi yang mewakili
daerah di bawah kurva fungsi asal terhadap variabel independen.


    B. Rumus-rumus integral fungsi aljabar  



Bentuk pertama


$$\int dx = x + C$$Dalam bentuk pertama bukan berarti tidak ada konstanta yang terlibat
dalam integral tak tentu, tapi ada konstanta yaitu angka 1, di dalam
matematika biasanya angka 1 sebagai konstanta tidak dituliskan.


Bentuk kedua


$$\int k dx = kx + C$$k merupakan konstanta yang berupa sebarang bilangan.


Bentuk ketiga


$$\int kx^n dx = \frac {k}{n+1} x^{n+1} + C$$k dan n merupakan sebarang bilangan bulat, dengan k adalah konstanta
dan n adalah pangkat dari x dengan syarat n tidak sama dengan -1.


Bentuk keempat


$$\int k.f(x) dx = k \int f(x) dx$$ Dengan k merupakan sebarang bilangan bulat.  

Bentuk kelima


Bentuk keenam


$$\int k(ax+b)^n dx = \frac {k}{a(n+1)} (ax+b)^{n+1} + C$$ Dalam bentuk integral keenam hanya berlaku jika angka pada pangkat x  

adalah 1.


    C. Contoh Soal &amp; Kurva  



Soal 1


$$\int 5x^2 dx$$\>$showev('integrate(5\*x^2,x)+c)


$$5\,\int {x^2}{\;dx}+c=\frac{5\,x^3}{3}+c$$\>plot2d(["5\*x^2","(5\*x^3/3)","(5\*x^3/3)+1","(5\*x^3/3)+2"]):


Soal 2


\>function f(x) &&= 4\*x+2


    
                                   4 x + 2
    

\>function g(x) &&= 2\*x+1


    
                                   2 x + 1
    

\>$showev('integrate(f(x)+(g(x)),x)+c)


$$\int {6\,x+3}{\;dx}+c=3\,x^2+3\,x+c$$\>plot2d(["6\*x+3","3\*x^2+3\*x","(3\*x^2+3\*x)+1","(3\*x^2+3\*x)+2"]):


![images/Syifa%20Desta%20Rumaisha_22305141020_Materi%20Integral%20Tak%20Tentu-016.png](images/Syifa%20Desta%20Rumaisha_22305141020_Materi%20Integral%20Tak%20Tentu-016.png)

Soal 3


\>$showev('integrate(x\*sqrt(x+2),x))


$$\int {x\,\sqrt{x+2}}{\;dx}=\frac{2\,\left(x+2\right)^{\frac{5}{2}}  }{5}-\frac{4\,\left(x+2\right)^{\frac{3}{2}}}{3}$$---



4. INTERGAL TAK TENTU FUNGSI NON ALJABAR (transenden)


    4.1 Intergal Tak Tentu Fungsi Trigonometri


        A. Defnisi  
    Integral tak tentu fungsi trigonometri merupakan operasi  

matematika yang digunakan untuk mencari fungsi asal sebelumnya
(biasanya ditambahkan dengan konstanta) yang ketika diambil turunan
akan menghasilkan fungsi trigonometri tersebut.


    Secara umum, integral tak tentu fungsi trigonometri seperti
sin(x), cos(x), atau tan(x) melibatkan berbagai rumus dan teknik
integral yang berbeda tergantung pada jenis fungsi trigonometri yang
terlibat.


        B. Rumus-rumus integral fungsi trigonometri  

![images/Syifa%20Desta%20Rumaisha_22305141020_Materi%20Integral%20Tak%20Tentu-018.png](images/Syifa%20Desta%20Rumaisha_22305141020_Materi%20Integral%20Tak%20Tentu-018.png)

        C. Contoh Soal &amp; Kurva  



Soal 1


\>$showev('integrate(2\*cos(x),x)+c)


$$2\,\int {\cos x}{\;dx}+c=2\,\sin x+c$$\>plot2d(["2\*cos(x)","2\*sin(x)","2\*sin(x)+1","2\*sin(x)+2"]):


![images/Syifa%20Desta%20Rumaisha_22305141020_Materi%20Integral%20Tak%20Tentu-020.png](images/Syifa%20Desta%20Rumaisha_22305141020_Materi%20Integral%20Tak%20Tentu-020.png)

Soal 2


$$\int cos (2x+1) dx$$\>$showev('integrate(cos(2\*x+1),x)+c)


$$\int {\cos \left(2\,x+1\right)}{\;dx}+c=\frac{\sin \left(2\,x+1  \right)}{2}+c$$\>plot2d(["cos(2\*x+1)","sin(2\*x+1)/2","(sin(2\*x+1)/2)+1","(sin(2\*x+1)/2)+2"]):


 4.2 Intergal Tak Tentu Fungsi Eksponensial  

        A. Defnisi  
     Integral dari fungsi eksponensial adalah operasi matematika yang  

digunakan untuk menemukan area di bawah kurva fungsi eksponensial
tertentu. Integral fungsi eksponensial merupakan proses untuk
menemukan fungsi yang, ketika di turunkan, akan menghasilkan fungsi
eksponensial tersebut.


        B. Rumus-rumus integral fungsi eksponensial  



Secara umum, integral dari fungsi eksponensial e^x adalah:


\>$showev('integrate((E^x),x)+ c)


$$\int {e^{x}}{\;dx}+c=e^{x}+c$$di mana "C" adalah konstanta integrasi. Ini berarti hasil dari
integral ini adalah fungsi eksponensial e^x itu sendiri ditambah
dengan konstanta integrasi.


       C. Contoh Soal &amp; Kurva  

Soal 1


$$\int e^{3x} dx$$\>$showev('integrate((E^x)^3,x)+c)


$$\int {e^{3\,x}}{\;dx}+c=\frac{e^{3\,x}}{3}+c$$\> \\plot2d(["(E^x)^3","((E^x)^3)/3","(((E^x)^3)/3)+7"],color=[blue,red,green]):


Soal 2


\>$showev('integrate(x\*(E^x)^2,x)+c)


$$\int {x\,e^{2\,x}}{\;dx}+c=\frac{\left(2\,x-1\right)\,e^{2\,x}}{4}+  c$$\>plot2d(["x\*(E^x)^2","((2\*x-1)E^x^2)/4","(2\*x-1)E^x^2/4 +1"]):


![images/Syifa%20Desta%20Rumaisha_22305141020_Materi%20Integral%20Tak%20Tentu-027.png](images/Syifa%20Desta%20Rumaisha_22305141020_Materi%20Integral%20Tak%20Tentu-027.png)

 4.3 Intergal Tak Tentu Fungsi Logaritma  
        A. Defnisi  
    Integral dari fungsi logaritma adalah operasi matematika yang  

digunakan untuk menemukan area di bawah kurva fungsi logaritma
tertentu.


        B. Rumus integral fungsi logaritma  

$$\int log(x) dx = x log(x) - x + C$$\>$showev('integrate(ln(x),x)+c)


$$\int {\log x}{\;dx}+c=x\,\log x-x+c$$        C. Contoh Soal &amp; Kurva  



Soal 1


\>$showev('integrate(log(2\*x),x)+c)


$$\int {\log \left(2\,x\right)}{\;dx}+c=\frac{2\,x\,\log \left(2\,x  \right)-2\,x}{2}+c$$\>plot2d(["log(2\*x)","(2\*x)log(2\*x)-2\*x/2 +1","(2\*x)log(2\*x)-2\*x/2 +2"]):


![images/Syifa%20Desta%20Rumaisha_22305141020_Materi%20Integral%20Tak%20Tentu-031.png](images/Syifa%20Desta%20Rumaisha_22305141020_Materi%20Integral%20Tak%20Tentu-031.png)

---



5. INTERGAL TAK TENTU FUNGSI KOMPOSISI


   A. Defnisi  
    Integral tak tentu dari fungsi komposisi, juga dikenal sebagai  

"integral tak tentu dari substitusi," adalah teknik integral yang
digunakan untuk mengintegrasikan fungsi yang merupakan hasil dari
komposisi dua fungsi.


  B. Contoh Soal dan kurva  

Soal 1


   f(x)=x+1, g(x)=x+2


\>function f(x) &= x+1


    
                                    x + 1
    

\>function g(x) &= x+2


    
                                    x + 2
    

\>$showev('integrate(f(g(x)),x)+c)


$$\int {x+3}{\;dx}+c=\frac{x^2}{2}+3\,x+c$$\>plot2d(["x+3","((x^2)/2)+3\*x","(((x^2)/2)+3\*x)+1","(((x^2)/2)+3\*x)+2"]):


![images/Syifa%20Desta%20Rumaisha_22305141020_Materi%20Integral%20Tak%20Tentu-033.png](images/Syifa%20Desta%20Rumaisha_22305141020_Materi%20Integral%20Tak%20Tentu-033.png)

# TERIMAKSIH

---

\> 

\> 


