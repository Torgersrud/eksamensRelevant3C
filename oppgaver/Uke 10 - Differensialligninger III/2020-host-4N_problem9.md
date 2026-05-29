## Problem 9 [8 points]

There are four versions of this exercise, each with a different RK-method.

We are given the following python code, in which one step of a Runge–Kutta method is implemented.

#### Version I:

```
def onestep(f, x, y, h):
k1 = f(x, y)
k2 = f(x+h/4, y+h*k1/4)
k3 = f(x+h, y+h*(k1+k2)/2)
y_next = y + h*(2*k2/3+k3/3)
x_next = x + h
return x_next, y_next
```

#### Version II:

```
def onestep(f, x, y, h):
k1 = f(x, y)
k2 = f(x+h/2, y+h*k1/2)
k3 = f(x+h, y+h*(k1+k2)/2)
y_next = y + h*(k1/3+k2/3+k3/3)
x_next = x + h
return x_next, y_next
```

### Version III:

```
def onestep(f, x, y, h):
k1 = f(x, y)
k2 = f(x+2*h/3, y+2*h*k1/3)
k3 = f(x+h, y+h*(k1+k2)/2)
y_next = y + h*(5*k1/12+k2/4+k3/3)
x_next = x + h
return x_next, y_next
```

### Version IV:

```
def onestep(f, x, y, h):
k1 = f(x, y)
k2 = f(x+3*h/4, y+3*h*k1/4)
k3 = f(x+h, y+h*(k1+k2)/2)
y_next = y + h*(4*k1/9+2*k2/9+k3/3)
x_next = x + h
return x_next, y_next
```

Write down the Butcher tableau of the method, and determine the method's order.