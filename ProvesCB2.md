## Proves de caixa negra:



**Calculeu la partició equivalent i valors per les classes d'equivalència vàlides i no vàlides:**

| Paràmetres | Condicions | Classes valides | Classes no vàlides |
| ----------- | ----------- | ----------- | ----------- |
| Preu | num entre 0,1-50 | 0,1<= preu <=50 | Preu < 0,1, Preu > 50, o no num = false |
| Diners | num entre 0-50  | num entre 0-50 | 0 < diners < 50 | diners < 0, diners > 50, o no num = false|


| Paràmetre entrada | Regla a aplicar | Classes vàlides | Classes no vàlides |
| ----------- | ----------- | ----------- | ----------- |
| diners | És un número? + rang valors (0..50) | 1. 0 <= diners <= 50 | 2. diners < 0 <br> 3. diners > 50 <br> 4. no és un número.|
| preu | És un número? + rang valors (0,1..50) | 5. 0,1 <= preu <= 50 | 6. preu < 0 <br> 7. preu > 50 <br> 8. no és un número.|

<br>
<br>
<br>

### Classes d'equivalència:


<br>
### Classes d'equivalència vàlides (1 i 5):

Ara haurem de dissenyar els casos de prova per cobrir totes les classes vàlides (1).

| diners | preu | Classe vàlida coberta| Resultat |
| ----------- | ----------- | ----------- | ----------- |
| 10 | 9 | 1, 5 | 1 |

<br>
### Classes d'equivalència no vàlides:

Ara generarem proves per cobrir totes les calsses de proves no vàlides (2 a 4 i 6 a 8).


| diners | preu | Classe vàlida coberta| Resultat |
| ----------- | ----------- | ----------- | ----------- |
| -10 | 11 | 2 | -1 |
| 60 | 2 | 3 | -1 |
| cinquanta | 4 | 3 | Error |
| 10 | -1 | 6 | -1 |
| 10 | 100 | 7 | -1 |
| 10 | sis | 8 | Error |

<br>

### Anàlisi dels valors límits:

| Paràmetre entrada | Regla a aplicar | Classes vàlides | Classes no vàlides |
| ----------- | ----------- | ----------- | ----------- |
| diners | És un número? + rang valors (0..50) | 9. diners = 0<br> 10. diners = 1<br> 11. diners = 50<br> 12. diners = 49 | 13. diners = -1 <br> 14. diners = 51 |
| preu | És un número? + rang valors (0,1..50) | 15. preu = 0,1<br> 16. preu = 1<br> 17. preu = 50<br> 18. preu = 49| 19. preu = -1<br> 20. preu = 51 |

Ara haurem de dissenyar els casos de prova per cobrir totes les classes vàlides (9 a 12 i 15 a 18).
<br>


| diners | preu | Classe vàlida coberta| Resultat |
| ----------- | ----------- | ----------- | ----------- |
| 0 | 5 | 9 | -1 |
| 1 | 5 | 10 | -1 |
| 50 | 5 | 11 | 45 |
| 49 | 5 | 12 | 44 |
| 10 | 0,1 | 15 | 9,90 |
| 10 | 1 | 16 | 9 |
| 10 | 50 | 17 | -1 |
| 10 | 49 | 18 | -1 |



I els casos no vàlids (13, 14, 19 i 20):

| diners | preu | Classe vàlida coberta| Resultat |
| ----------- | ----------- | ----------- | ----------- |
| -1 | 5 | 13 | -1 |
| 51 | 5 | 14 | -1 |
| 5 | -1 | 19 | -1 |
| 5 | 51 | 20 | -1 |
