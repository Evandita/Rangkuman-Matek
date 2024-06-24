# First Order ODE (Ordinary Differential Equation)

## Definisi

1. Differential Equation

        Persamaan yang mengandung variabel turunan

2. Order

        Turunan tertinggi pada sebuah ODE

3. ODE & PDE

        Ordinary Differential Equation merupakan persamaan turunan yang hanya memiliki satu variabel, sedangkan Partial Differential Equation memiliki lebih dari satu variabel

4. Linear Differential Equations

        Persamaan turunan yang derajat polinomial variabelnya 1

5. Solution

   - General  Solution

        ```
        Solusi yang memenuhi persamaan ODE
        ```   

    - Actual Solution
     
        ```
        Solusi yang memenuhi persamaan ODE dan initial condition
        ```

6. Initial Condition

        Hasil dari sebuah persamaan ODE untuk suatu kondisi awal

7. Initial Value Problem

        Berisikan kumpulan Initial Condition untuk mencari Actual Solution

8. Explicit Solution

        Bentuk solusi yang dituliskan dalam format y = ...

9. Implicit Solution

        Bentuk solusi yang tidak memenuhi format Explicit Solution

10. Interval of Validity

        Interval yang diperbolehkan agar explicit solution valid

## Bentuk persamaan First Order ODE dan cara penyelesaiannya


### Linear Differential Equation


$$
y' + p(t)y = g(t)
$$

Cara Penyelesaian:

1. Mencari U(t)

$$
u(t)=e^{\\int_{}^{}p(t)dt}
$$

2. Mengkalikan persamaan LDE dengan U(t)

$$
e^{\\int_{}^{}p(t)dt} y' + e^{\\int_{}^{}p(t)dt}p(t)y=e^{\\int_{}^{}p(t)dt}g(t)
$$

3. Menyederhanakan persamaan

$$
(u(t)y(t))' = u(t) g(t)
$$

4. Mengintegralkan kedua sisi

$$
\\int_{}^{} (u(t)y(t))'dt = \\int_{}^{}u(t)g(t)dt
$$

5. Menyelesaikan integral untuk mendapatkan **General Solution**

6. Mensubstitusi IVP untuk mendapatkkan **Actual Solution**

7. Mencari Interval Penyelesaian untuk **Explicit Solution**

### Separable Differential Equations

$$
N(y) dy = M(x) dx
$$

Cara Penyelesaian:

1. Mengintegralkan kedua ruas

$$
\\int N(y) dy = \\int M(x)dx
$$

2. Menyederhanakan persamaan untuk mendapatkan **General Solution**

3. Mensubstitusi IVP untuk mencari **Actual Solution**

4. Mencari Interval Penyelesaian untuk **Explicit Solution**

### Exact Differential Equations

$$
M(x,y)+N(x,y)\\frac{dy}{dx}=0
$$

Cara penyelesaian:

1. Verifikasi bahwa sifat berikut benar

$$
M_{y} = N_{x}
$$

2. Mencari integral dari M(x,y) terhadap x

$$
\\psi =\\int M dx +h(y)
$$

3. Turunkan psi terhadap y

$$
\\psi_{y} + h'(y) = N
$$

4. Cari nilai dari h'(y)

$$
h'(y) = N - \\psi_{y}
$$

5. Cari nilai dari h(y)

$$
h(y) = \\int h'(y)dy + k
$$

6. Substitusi h(y) ke persamaan psi    

$$
\\psi =\\int M dx + \\int h'(y)dy = c
$$

7. Substitusi Initial Value untuk mencari c
8. Ubah bentuk implicit menjadi explicit untuk mencari IVP

### Bernoulli Differential Equations

$$
y' + p(x)y = q(x)y^{n}
$$

1. Bagi kedua ruas dengan y^n

$$
y^{-n}y' + p(x)y^{1-n} = q(x)
$$

2. Misalkan sebuah variabel baru `v` sebagai berikut

$$
v = y^{1-n}
$$

$$
v' = (1-n)y^{-n}y'
$$

3. Substitusi `v` pada persamaan awal

$$
\\frac{1}{1-n}v' + p(x)v=q(x)
$$

4. Kalikan kedua ruas dengan (1-n)

$$
v' + (1-n)p(x)v=(1-n)q(x)
$$

5. Selesaikan persamaan tersebut menggunakan cara `Linear ODE`

6. Substitusi nilai `v` dengan y kembali 