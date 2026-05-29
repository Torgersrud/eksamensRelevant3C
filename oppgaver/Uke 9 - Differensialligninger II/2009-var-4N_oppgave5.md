#### Oppgave 5

a) Gitt et system av ordinære differensialligninger

(5) 
$$y_1' = -y_2, \\ y_2' = y_1,$$

med initialbetingelsen

$$y_1(0) = 1, \quad y_2(0) = 0.$$

Finn en tilnærming til løsningen av systemet (5)  $\mathbf{y}(t) = [y_1(t), y_2(t)]^T$ , når t = 0.2, ved bruk av den implisitte trapesmetoden, gitt av

(6) 
$$\mathbf{y}^{(i+1)} = \mathbf{y}^{(i)} + \frac{h}{2} \left[ \mathbf{f}(t_i, \mathbf{y}^{(i)}) + \mathbf{f}(t_{i+1}, \mathbf{y}^{(i+1)}) \right], \quad t_i = t_0 + ih.$$

Bruk h = 0.2, dvs  $\mathbf{y}^{(1)} \approx \mathbf{y}(0.2)$ .

b) Vis at for systemet (5), med de gitte initialbetingelsene, er

$$\|y(t)\|_2 = 1$$
, for  $t \ge 0$ 

hvor  $\|\boldsymbol{y}\|_2 = \sqrt{y_1^2 + y_2^2}$ . Dvs. lengden  $\|\boldsymbol{y}\|_2$  er konstant lik en.

c) Vis at

$$\|\boldsymbol{y}^{(i+1)}\|_2 = \|\boldsymbol{y}^{(i)}\|_2$$
, for  $i = 0, 1, 2, \dots$ 

der  $\boldsymbol{y}^{(i)}$  er gitt av trapesmetoden (6) andvendt på ligningssystemet (5). Dvs. trapesmetoden bevarer lengden,  $\|\boldsymbol{y}^{(i)}\|_2$ .

Hint:

$$\begin{bmatrix} 2 & h \\ -h & 2 \end{bmatrix}^{-1} = \frac{1}{4+h^2} \begin{bmatrix} 2 & -h \\ h & 2 \end{bmatrix}$$
