## Problem 4 Numerical integration (10 points)

a) Consider the quadrature rule

$$\int_{-1}^{1} f(s)ds \approx Q[f] = w_0 f(-1) + w_1 f\left(-\frac{1}{3}\right) + w_2 f\left(\frac{1}{3}\right) + w_3 f(1).$$

Assume that it is exact for all polynomials of degree 3 or lower.

Deduce the values of  $w_0, w_1, w_2, w_3$  and show that

$$w_0 + w_1 = 1$$
 and  $9w_0 + w_2 = 3$ .

b) Use Taylor expansion of the function f at the point  $x_k + \frac{1}{2}h$  to derive the midpoint rule of integration

$$\int_{x_k}^{x_k+h} f(x) \, dx = h f(x_k + \frac{1}{2}h) + \frac{1}{24}h^3 f''(\tilde{\xi}), \qquad x_k < \tilde{\xi} < x_k + h.$$

Hint: You can use the mean value theorem for integrals: If g(x) is continuous and  $w(x) \ge 0$  for all  $x \in [a, b]$ , then

$$\exists \xi \in [a,b] \text{ such that } \int_a^b g(x) w(x) dx = g(\xi) \int_a^b w(x) dx.$$
