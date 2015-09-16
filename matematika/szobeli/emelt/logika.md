A matematikai logika elemei?

A logikai szita formula kettő, illetve három halmaz esetében:

 - |A ⋃ B| = |A| + |B| - |A ⋂ B|
 - |A ⋃ B ⋃ C| = |A| + |B| + |C| - |A ⋂ B| - |A ⋂ C| - |B ⋂ C| + |A ⋂ B ⋂ C|

## Logikai műveletek:

Logikai függvény értelmezési tartománya bármi lehet, értékkészlete kételemű halmaz {igaz; hamis}

Negáció (tagadás) – komplementer halmaz:
[latex] P = 1 \to !P = 0 [/latex]

Konjunkció („és” kapcsolat) – két halmaz metszete (két állítás metszete):

| A | B | A * B |
|:-:|:-:|:-----:|
| 0 | 0 |   0   |
| 1 | 0 |   0   |
| 0 | 1 |   0   |
| 1 | 1 |   1   |

Diszjunkció(vagy) – két halmaz uniója

| A | B | A + B |
|:-:|:-:|:-----:|
| 0 | 0 |   0   |
| 1 | 0 |   1   |
| 0 | 1 |   1   |
| 1 | 1 |   1   |

Implikáció:

| A | B | A → B |
|:-:|:-:|:-----:|
| 0 | 0 |   1   |
| 1 | 0 |   0   |
| 0 | 1 |   1   |
| 1 | 1 |   1   |

A fentiek szerint hamis állításból következhet hamis, hamisból következhet igaz, igazból nem következhet hamis, igazból következhet igaz állítás. Ez tulajdonképpen a "Ha..., akkor..." kijelentésnek felel meg.

Ekvivalencia:

| A | B | A ↔ B |
|:-:|:-:|:-----:|
| 0 | 0 |   1   |
| 1 | 0 |   0   |
| 0 | 1 |   0   |
| 1 | 1 |   1   |

*de Morgan féle azonosságok*:

 - A *halmazelméletben* a következők:
   ![DeMorgan azonosságok](http://i.imgur.com/iRtcdCe.png)
   ![DeMorgan azonosságok](http://i.imgur.com/PCTNS7L.png)
 - *Logikában* pedig:

 - Arisztotelészi logika (3-as elv)
   + minden dolog azonos önmagával
   + semmi sem azonos önmaga ellentétjével
   + egy dolog és tagadása közül egy igaz
  - Szillogizmus: amikor 2 állításból jön a konklúzió
 - Szókratész ember. Minden ember halandó. Tehát Szókratész halandó. "Arisztotelész"
 - Állítás megfordítása: pl. a paralelogramma átlói felezik egymást
   + megfordítható: négyszög átlója ami felezi egymást paralelogramma
 - Szükséges feltétel, elégséges feltétel
   + Szükséges de nem elégséges feltétel: ahhoz, hogy egy négyszög paralelogramma legyen, szükséges 2 párhuzamos oldal
   + Elégséges, de nem szükséges feltétel: 2 egyenlő és felező átló
