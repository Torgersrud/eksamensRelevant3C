## Problem 6 Quadrature rules [15 pts]

a) It is known that the quadrature rule MR[f](a,b) defined by the midpoint rule satisfies the error estimate

$$|MR[f](a,b) - \int_a^b f(x)dx| \le \frac{7M}{24}(b-a)^3,$$

where  $M = \max_{x \in [a,b]} |f''(x)|$ . Which degree of exactness has this quadrature rule and why?

**b)** Show that the corresponding composite midpoint rule CMR[f](a,b,m) defined on m equally spaced subintervals satisfies an estimate for the quadrature error of the form

$$|CMR[f](a, b, m) - \int_{a}^{b} f(x)dx| \leq M(b - a)\frac{7h^{2}}{24},$$

where  $h = \frac{b-a}{m}$  and M is defined as in **b**).
- c) Consider the the integral  $\int_0^1 \cos(x) dx$ . Find the number of intervals m which guarantees that the quadrature error for the composite midpoint rule is below  $10^{-3}$ .
- d) Write down a Python code snippet, which for given function f, interval endpoints a, b and number of intervals m uses the composite midpoint rule to compute the integral  $\int_a^b f(x)dx$  numerically.
