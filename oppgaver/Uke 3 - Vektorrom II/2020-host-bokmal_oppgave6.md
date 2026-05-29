For å simulere proteinene som danner taggene til koronaviruset SARS-CoV-2 bruker forskere overgangsalgoritmer (for eksempel i prosjektet Folding@Home ved Stanford).

De trenger din hjelp til å teste om algoritmen de har implementert fungerer som den skal, og har derfor forenklet utregningene slik at du kan gjøre dem for hånd.

Proteinet S kan innta tre ulike tilstander, A, B og C. Hvert mikrosekund, altså hvert $10^{-6}$-sekund, kan den bytte tilstand.

- Gitt at S er i tilstand A, og man venter et mikrosekund så er det: (x-1)/x sannsynlighet for at S fortsatt er i tilstand A, 1/x sannsynlighet for at S går til tilstand B, 0 sannsynlighet for at S går til tilstand C.
- Gitt at S er i tilstand B, og man venter et mikrosekund så er det: 0 sannsynlighet for at S går til A, (y-1)/y sannsynlighet for at S fortsatt er i tilstand B, 1/y sannsynlighet for at S går til tilstand C.
- Gitt at S er i tilstand C, og man venter et mikrosekund så er det: 1/3 sannsynlighet for at S går til A, 1/3 sannsynlighet for at S går til tilstand B, 1/3 sannsynlighet for at S fortsatt er i tilstand C.

a) Finn den stokastiske matrisen M som representerer hvordan S endrer tilstander for hvert mikrosekund.

b) Er M regulær?

c) Gitt at S ligger i tilstand A, hva er sannsynligheten for at S ligger i tilstand B to (2) mikrosekunder senere?

d) Forskerene simulerer at proteinet S får endre tilstand fritt, slik det vil, i et helt sekund. Estimer sannsynligheten for at S er i hver av de 3 tilstandene på slutten av sekundet. Hvilken tilstand er det mest sannsynlig at S vil være i?
