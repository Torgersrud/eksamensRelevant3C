**Problem 4** You are given the problem

$$u''' + (3 - u')u'' + 2u = 0$$

$$u(0) = 1$$

$$u'(0) = 2$$

$$u''(0) = 5.$$
(1)

a) Write the problem as a system of equations.

Heun's method can be viewed as a predictor-corrector combination of Euler's method and the trapezoidal rule.

Backward Euler is given by

$$u_{n+1} = u_n + h f(t_{n+1}, u_{n+1}).$$

Give a method using Euler's method as a predictor and backward Euler as a corrector.

b) Apply one step of the method you obtained in a) to (??). Use h = 0.1. If you did not manage to find the method in a), use Heun's method instead.