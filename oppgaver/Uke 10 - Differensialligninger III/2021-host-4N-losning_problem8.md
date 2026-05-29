## Problem 8 Numerical methods for ODE [12 pts]

Consider the following implementation of a 3-stage Runge-Kutta method.

```
def rkm(y0, t0, T, f, Nmax):
      ts = [t0]
      ys = [y0]
3
      dt = (T-t0)/Nmax
5
      while (ts[-1] < T):
6
          t, y = ts[-1], ys[-1]
          k1 = f(t,y)
          k2 = f(t+2/3*dt,y+2/3*dt*k1)
          k3 = f(t+dt,y+dt/2*(k1+k2))
          ys.append(y + dt/4*(k1+3*k2))
13
          ts.append(t + dt)
14
      return np.array(ts), np.array(ys)
```

- a) Extract the Butcher table from the given implementation. Can you simplify the Butcher table and/or implementation code?
- b) Determine the consistency order of the Runge-Kutta method implemented in a).
- c) Now imagine you have run a convergence rate study for three different Runge-Kutta methods, one of which was the method implemented in the code snippet above. You obtained the following tables which tabulate the number of used, equidistant time-steps N against the resulting error.

What are the experimentally observed orders of convergence for each method and which table was likely produced by the method implemented above? Justify your answers!

|   | N   | Error    |   | N   | Error       |   | N   | Error    |
|---|---|----------|---|---|-------------|---|---|----------|
| 0 | 4   | 0.221199 | 0 | 4   | 3.1795 e-02 | 0 | 4   | 0.071203 |
| 1 | 8   | 0.096199 | 1 | 8   | 3.0213 e-03 | 1 | 8   | 0.010207 |
| 2 | 16  | 0.044258 | 2 | 16  | 3.1609e-04  | 2 | 16  | 0.001986 |
| 3 | 32  | 0.021231 | 3 | 32  | 3.5879 e-05 | 3 | 32  | 0.000446 |
| 4 | 64  | 0.010403 | 4 | 64  | 4.2818e-06  | 4 | 64  | 0.000106 |
| 5 | 128 | 0.005141 | 5 | 128 | 5.2306e-07  | 5 | 128 | 0.000026 |

Table 1 Table 2 Table 3
