# Taylor Series

Aproksimasi sebuah fungsi f(x) pada titik a dirumuskan sebagai berikut

$$
f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(a)}{n!} (x-a)^n
$$

$$
f(x) = f(a) + f'(a)(x-a) + \frac{f''(a)}{2!} (x-a)^2 + \frac{f'''(a)}{3!} (x-a)^3
$$

# Maclaurin Series

Deret Taylor yang diaproksimasi pada titik a = 0

$$
f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(0)}{n!}x^n
$$

$$
f(x) = f(0) + f'(0)x + \frac{f''(0)}{2!}x^2 + \frac{f'''(0)}{3!}x^3
$$

## Contoh

### Fungsi Eksponensial

$$
e^x = \sum_{n=0}^{\infty}\frac{x^n}{n!}
$$

### Logaritma Natural

$$
ln(1-x) = -\sum_{n=1}^{\infty}\frac{x^n}{n}
$$

$$
ln(1+x) = \sum_{n=1}^{\infty}(-1)^{n+1}\frac{x^n}{n}
$$

### Deret Geometris `|x| < 1`

$$
\frac{1}{1-x} = \sum_{n=0}^{\infty} x^n
$$

$$
\frac{1}{(1-x)^2} = \sum_{n=1}^{\infty} nx^{n-1}
$$

$$
\frac{1}{(1-x)^3} = \sum_{n=2}^{\infty}\frac{(n-1)n}{2} x^{n-2}
$$

### Fungsi Trigonometri

$$
sin(x) = \sum_{n=0}^{\infty}\frac{(-1)^n}{(2n + 1)!}x^{2n+1}
$$

$$
cos(x) = \sum_{n=0}^{\infty}\frac{(-1)^n}{(2n)!}x^{2n}
$$

### Fungsi Hiperbolik

$$
sinh(x) = \sum_{n=0}^{\infty}\frac{x^{2n+1}}{(2n + 1)!}
$$

$$
cosh(x) = \sum_{n=0}^{\infty}\frac{x^{2n}}{(2n)!}
$$

