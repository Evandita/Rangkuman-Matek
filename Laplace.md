# Laplace

## Bentuk Umum

$$
F(s) = \mathcal{L} \{f(t)\} = \int_{0}^{\infty}e^{-st}f(t)dt
$$

## Sifat

### Linearity

$$
\mathcal{L} \{af(t)+bg(t)\} = aF(s) + bG(s)
$$

Contoh:

$$
\mathcal{L} \{cosh(at)\} = 
\mathcal{L} \{ \frac{1}{2}(e^{at}+e^{-at}) \} =
\frac{1}{2} (\frac{1}{s-a} + \frac{1}{s+a}) =
\frac{s}{s^{2} - a^{2}}
$$

$$
\mathcal{L} \{sinh(at)\} = 
\mathcal{L} \{ \frac{1}{2}(e^{at}-e^{-at}) \} =
\frac{1}{2} (\frac{1}{s-a} - \frac{1}{s+a}) =
\frac{a}{s^{2} - a^{2}}
$$

### Shifting

$$
\mathcal{L} \{e^{at}f(t)\} = F(s-a)
$$

$$
e^{at}f(t) = \mathcal{L}^{-1} \{ F(s-a) \}
$$

### Step Function

$$
\mathcal{L} \{u_{c}(t)f(t-c)\} = e^{-cs} F(s)
$$

contoh:

![](img/ContohStepFunction.png)

### LT of Differential Equation

$$
\mathcal{L} \{f^{n}\} = s^{n}F(s) - s^{n-1}f(0) - s^{n-2}f'(0) - ... - f^{(n-1)}(0)
$$

Contoh:

$$
\mathcal{L} \{y'\} = sY(s) - y(0)
$$

$$
\mathcal{L} \{y''\} = s^{2}Y(s) - sy(0) - y'(0)
$$

### LT of t^n

$$
\mathcal{L} \{t^{n}\} = \frac{n!}{s^{1+n}}
$$

### LT of ty(t)

$$
\mathcal{L}\{ty'\} = -sY'(s)-Y(s)
$$

$$
\mathcal{L}\{t^{2}y'\} = -s^{2}Y'(s)-2sY(s) + y(0)
$$

**Note**: nilai c bergantung saat s -> inf. Jika Y(s) menuju inf, maka c = 0.

### Delta Dirac

$$
\mathcal{L} \{\delta (t-a)\} = \int_{0}^{\infty} e^{-st} \delta (t-a) dt = e^{-as}
$$


## Tabel Laplace `Pendek`

![](img/TabelLaplacePendek.png)


## Tabel Fraction Partial Decompotition

![](img/TabelFractionPartial.png)

## Tabel Laplace `Panjang`

![](img/TabelLaplacePanjang.png)