#### **Problem 5** Given the differential equation

$$y' = xy^2, y(1) = 0.5.$$

- a) Compute the approximate solution $y_1^H \approx y(1.1)$ by one step of the Heun method with step size h = 0.1.
- b) Compute the approximate solution $y_1^E \approx y(1.1)$ by one step of the Euler method with step size h = 0.1.

Use the result from point a) to find an estimate for the error $y(1.1) - y_1^E$.

Given a user specified tolerance Tol = $10^{-3}$ , will you accept $y_1^E$ as a sufficient accurate solution?

Whether you accept the step or not, what should your next step size be? Use P = 0.8 as the pessimist factor in the step size selection algorithm.

**Hint:** The Euler method is of order 1, the Heun method is of order 2.