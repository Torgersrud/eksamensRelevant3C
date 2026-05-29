Oppgave 7 Gitt et system av første ordens differensialligninger

$$\mathbf{y}' = \mathbf{f}(x, \mathbf{y}), \qquad \mathbf{y}(x_0) = \mathbf{y}_0.$$

Vi har sett på flere mulige måter å løse slike ligninger numerisk, i denne oppgaven velger vi «trapes-metoden», gitt ved

$$\mathbf{y}_{n+1} = \mathbf{y}_n + \frac{h}{2} \left[ \mathbf{f}(x_n, \mathbf{y}_n) + \mathbf{f}(x_{n+1}, \mathbf{y}_{n+1}) \right]$$
 (\*)

der h er skrittlengden og  $x_{n+1} = x_n + h$ . Vi antar at  $\mathbf{y}_n$  er kjent, og (\*) brukes til å finne en tilnærmelse til  $\mathbf{y}_{n+1}$ . Metoden er implisitt, siden funksjonen  $\mathbf{f}$  også beregnes i den ukjente løsningen  $\mathbf{y}_{n+1}$ . Vi ender altså med et ikke-lineært ligningssystem som må løses med hensyn på  $\mathbf{y}_{n+1}$  for hvert skritt.

La y = y(x) være funksjonen som tilfredstiller den andre ordens differensialligningen

$$y'' = \sin y$$
,

med startbetingelser  $y(0) = \frac{\pi}{2}$ , y'(0) = 0.

Skriv om ligningen til et system av første ordens differensialligninger. Hva blir startverdiene for dette systemet?

Sett h=0.1 og sett opp det ikke-linære ligningssystemet du får når du ønsker å utføre det første skrittet med trapesmetoden for dette systemet.
