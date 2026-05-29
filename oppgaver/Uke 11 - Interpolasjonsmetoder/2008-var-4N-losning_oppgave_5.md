#### Oppgave 5

a) Vi lager Newtons divided difference interpolation tabell

| $x_j$ | $f_j = f(x_j)$ | $f[x_j, x_{j+1}]$ | $f[x_j, x_{j+1}, x_{j+2}]$ | $f[x_j,\ldots,x_{j+3}]$ | $f[x_j,\ldots,x_{j+4}]$ |
|-------|----------------|-------------------|----------------------------|-------------------------|-------------------------|
| 0     | 1              |                   |                            |                         |                         |
|       |                | 5                 |                            |                         |                         |
| 0.25  | 2.25           |                   | 12                         |                         |                         |
|       |                | 11                |                            | 16                      |                         |
| 0.5   | 5              |                   | 24                         |                         | 0                       |
|       |                | 23                |                            | 16                      |                         |
| 0.75  | 10.75          |                   | 36                         |                         |                         |
|       |                | 41                |                            |                         |                         |
| 1     | 21             |                   |                            |                         |                         |

og man får

$$P(x) = 1 + 5x + 12x(x - 0.25) + 16x(x - 0.25)(x - 5)$$

som forenkler seg til

$$P(x) = 16x^3 + 4x + 1.$$

**b)** Vi har

$$\int_0^1 P(x) dx = \int_0^1 (16x^3 + 4x + 1) dx$$
$$= \left[ 16\frac{x^4}{4} + 4\frac{x^2}{2} + x \right]_0^1$$
$$= 7.$$

Simpsons regel gir

$$\int_0^1 P(x) dx \approx S_n = \frac{\Delta x}{3} (P(0) + 4P(0.25) + 2P(0.5) + 4P(0.75) + P(1))$$
$$= \frac{0.25}{3} (1 + 4 \cdot 2.25 + 2 \cdot 5 + 4 \cdot 10.75 + 21)$$
$$= 7.$$

Feilestimat for feilen er gitt av

$$\left| \int_{a}^{b} f(x) \, dx - S_{n} \right| \le \frac{f^{4}(c)(b-a)^{5}}{180n^{2}}$$

for noen  $c \in [0, 1]$ . Siden P har graden 3 har vi $P^{(4)}(x) = 0$ . Det vil si at feilen blir null for P. Den degree of precision til Simpsons metode er lik 3 og metoden gir den eksakte verdien av integralet til P.
