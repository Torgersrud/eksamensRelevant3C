## Problem 3 Numerical methods for ODEs [10 pts]

- a) Verify that the function  $f(x,y) = 2yx^{-4}$  satisfies a Lipschitz condition in the 2nd variable on the domain  $1 \le x < \infty$ ,  $y \in \mathbb{R}$  and determine the associated Lipschitz constant.
- b) For the differential equation y' = f(t, y), we consider the general two-stage *implicit* Runge–Kutta method

$$y_{n+1} = y_n + h \sum_{i=1}^{2} b_i K_i,$$

with the stages

$$K_1 = f(t_n + c_1 h, y_n + h a_{11} K_1 + h a_{12} K_2)$$
   

$$K_2 = f(t_n + c_2 h, y_n + h a_{21} K_1 + h a_{22} K_2),$$

corresponding to the Butcher tableau

$$\begin{array}{c|cccc} c_1 & a_{11} & a_{12} \\ c_2 & a_{21} & a_{22} \\ \hline & b_1 & b_2 \end{array}$$

By applying this method to the scalar-valued differential equation

$$y' = \lambda y$$
,

where  $\lambda$  is a constant, the  $K_1$  and  $K_2$  can be deduced as solution of the linear system

$$\left(\begin{array}{cc} b_{11} & b_{12} \\ b_{21} & b_{22} \end{array}\right) \left(\begin{array}{c} K_1 \\ K_2 \end{array}\right) = \left(\begin{array}{c} \lambda y_n \\ \lambda y_n \end{array}\right).$$

- b1) Describe the matrix B with entries  $\{b_{ij}\}_{1 \leq i,j \leq 2}$  explicitly, in terms of the  $\{ha_{ij}\}_{1 \leq i,j \leq 2}$  and write down its determinant  $\Delta := \det(B)$ .
- b2) Assume that the determinant  $\Delta \neq 0$ . Find explicit formulas for  $K_1$  and  $K_2$  by solving the system

$$B\left(\begin{array}{c} K_1\\ K_2 \end{array}\right) = \left(\begin{array}{c} \lambda y_n\\ \lambda y_n \end{array}\right)$$
