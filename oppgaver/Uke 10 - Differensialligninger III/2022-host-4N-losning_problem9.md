### Problem 9.

We are given the following embedded Runge-Kutta pair:

$$\begin{array}{c|ccccccccccccccccccccccccccccccccccc$$

The first row of b coefficients gives a second order accurate method, and the second row gives a method of order three. The pair is applied to the ODE

$$y' = -y^2$$
,  $y(0) = 1$ .

- a) Let the initial step size be  $h_0 = 0.2$  and perform one step with the highest order method.
- b) Let  $y_1$ ,  $\hat{y}_1$  denote the solutions after one step with stepsize  $h_0 = 0.2$  with the lowest, respectively the highest order method, both starting from  $y(0) = y_0 = 1$ .

Compute the local error estimate  $\hat{\epsilon}_1 = |y_1 - \hat{y}_1|$ .

c) Comparing  $\hat{\epsilon}_1$  with the tolerance tol =  $10^{-3}$ , check if the first step is acceptable, and if not, compute a new stepsize  $h_{\text{new}}$ . Use the pessimist factor (safety factor) P = 0.8.
