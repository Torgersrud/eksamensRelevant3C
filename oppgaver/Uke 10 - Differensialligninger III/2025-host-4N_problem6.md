## Problem 6 Numerical methods for ODEs (10 points)

a) Rewrite the following initial value problem (IVP) as a first order system with initial value

$$x'''(t) - 2x''(t) - x'(t) + 2x(t) = 1 - 2t, \quad x(0) = x'(0) = 1, \ x''(0) = 0.$$

b) Consider the first order IVP

$$x'(t) = 1 + t - x(t), \quad t > 0, \quad x(0) = x_0 = 0.$$

- i) Use the explicit Euler method with a general step size h to compute the first three approximations  $x_1, x_2, x_3, \ldots$
- ii) Deduce an expression for  $x_n$  in terms of  $t_n = nh$ .
- iii) Use the result to guess the exact solution of the IVP.
- c) Show that the Runge–Kutta method with Butcher tableau

$$\begin{array}{c|cccc}
0 & 0 & 0 \\
1 & \frac{1}{2} & \frac{1}{2} \\
\hline
& \frac{1}{2} & \frac{1}{2}
\end{array}$$

is equivalent to the trapezoidal rule

$$x_{n+1} = x_n + \frac{1}{2}h(f(t_{n+1}, x_{n+1}) + f(t_n, x_n)).$$
