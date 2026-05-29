### **Oppgåve 1** Likningssystemet

$$3x + y + z = 5$$

$$x + 3y - z = 3$$

$$3x + y - 5z = -1$$

er løyst ved to iterasjonsmetodar i Python.

```
def iterasjonEin(x0,y0,z0,n):
    x = x0
    y = y0
    z = z0
    for i in range (0,n):
                                                   \# 0 \le i \le n
        x = 1.0/3.0*(5.0 - y - z)
        y = 1.0/3.0*(3.0 - x + z)
        z = 1.0/5.0*(1.0 + 3.0*x + y)
    return x, y, z
def iterasjonTo(x0,y0,z0,n):
    x = x0
    y = y0
    z = z0
    for i in range (0,n):
                                                   \# \ 0 <= i < n
        x = 1.0/3.0*(5.0 - y - z)
        y = -1.0 - 3.0*x + 5.0*z
        z = -3.0 + x + 3.0*y
    return x,y,z
```

Gjer éin iterasjon med kvar av metodane med $x_0 = y_0 = z_0 = 0,1$ .

Kva for ein iterasjonsmetode er det som er implementert? Kva kan vi sei om konvergensen til disse metodane?
