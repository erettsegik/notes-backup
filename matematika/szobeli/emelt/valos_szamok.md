﻿Ajánlott nyitómondat:

A valós számokat a természetes számoktól szeretném első körben felépíteni és csak utána kifejteni a tétel többi részét.

## TERMÉSZETES SZÁMOK

[latex]x^3[/latex]

jele: [latex inline]\natural x^2[/latex]

#### definíció1:

A véges halmazok számosságát természetes számoknak nevezzük 5[/latex],

- ha  AnB= 0   |AuB| = |A| + |B|
- ha  AnB= 0   |AxB| = |A| * |B|

#### definíció2:(*Peano-axiómák*)

Az N halmazt a természetes számok halmazának nevezzük, ha teljesülnek rá:
1. 1 eleme [latex inline]\mathbb{N}[/latex]-nek
2. n eleme [latex inline]\mathbb{N}[/latex]-nek => n+ eleme [latex inline]\mathbb{N}[/latex]-nek
3. nem létezik n eleme [latex inline]\mathbb{N}[/latex]-nek : n+ = 1
4. bármely n,m eleme [latex inline]\mathbb{N}[/latex]-nek : n+ = m+ => n=m
5. [latex inline]\mathbb{N}'[/latex] részhalmaza [latex inline]\mathbb{N}[/latex]-nek és [latex inline]\mathbb{N}'[/latex]-ban igaz az első 3 axióma, akkor [latex inline]\mathbb{N}'=\mathbb{N}[/latex]
(teljes indukció)
- egyetlen TELJES axióma rendszer. 
neutrális elem(a nulla) nem tartozik hozzá a peano axiómák szerint, bár elfogadott bizonyos körökben az is, ha hozzávesszük.  


### Műveletek a természetes számok halmazán:

összeadás, szorzás (nincs inverzük)

0 → az összeadásra nézve neutrális elem

1 → a szorzásra nézve neutrális elem

Term. számok halmaza ([latex inline]\mathbb{N}[/latex]) + 0 + negatív Term. számok ([latex inline]\mathbb{N}[/latex]-) = az egész számok halmazával ([latex inline]\mathbb{Z}[/latex])

A szorzás invertálhatósága érdekében jöttek létre a racionális számok. → osztás 

jele: [latex inline]\mathbb{Q}[/latex]

mindig elvégezhető: összeadás, kivonás, szorzás, osztás, hatványozás

A számok jelentős része nem írható fel két racionális szám hányadosaként, ezért tovább bővítjük a számok halmazát az irracionális számokra ([latex inline]\mathbb{Q}[/latex]*)

*Tétel*: Léteznek irracionális számok.


*Bizonyítás:*

Tfh.: [latex inline]\sqrt{2}[/latex] eleme [latex inline]\mathbb{Q}[/latex]-nak

[latex inline]\sqrt{2} = p/q [/latex]   |   [latex inline] q≠0   p,q[/latex] eleme [latex inline]\mathbb{Z}[/latex]-nek

[latex inline]\sqrt{2} * q = p[/latex]

[latex inline]2*q^2 = p^2[/latex]  (NINCS 2 olyan négyzetszám, hogy az egyik 2x-ese a másiknak)

  |                 |

PÁROS = PÁROS

  |                 |

tehát q is osztható 4-gyel ( q páros ) = p is páros, úgyhogy p2 osztható 4-gyel

bal oldal= 2 páratlan hatványa

jobb oldal = 2 páros hatványa

NEM IGAZ --> tehát  [latex inline]\sqrt{2}[/latex] eleme [latex inline]\mathbb{Q}[/latex]*-nak

Nevezetes irracionális számok: [latex inline]e, pi, fi … [/latex]

A racionális számok és az irracionális számok halmazának úniója ([latex inline]\mathbb{Q}u\mathbb{Q}*=R[/latex]) egyenlő a valós számok halmazával 
Bármely két racionális szám között van irracionális szám, és bármely két irracionális szám között is.
minden alapműveletre működik kivéve a negatívból való gyökvonást.


## Komplex számok halmaza:

#### Komplex számok halmazán értjük:

[latex inline]\mathbb{C}[/latex] { [latex inline]a+b*i[/latex] | a, b eleme R-nek, [latex inline]i=\sqrt{-1}[/latex] }

( [latex inline]i = \sqrt{-1}[/latex] – imaginiárius egység, tehát [latex inline]\sqrt{-20} = \sqrt{20} * \sqrt{-1}= \sqrt{20} * i[/latex] )
a komplex számokat koordináta rendszerben ábrázoljuk, nem számegyenesen. 

[latex inline]a+b*i[/latex], forma

0-val való osztás esetére a komplex számok bővíthetőek [latex inline]+∞, -∞[/latex] - re


### Átvezető a számelméletre:

A végére szeretnék áttérni a Matematika számelmélet témakörére. Ez a témakör az amivel a legrégebb óta foglalkozik a matematika.
pitagoreusi iskola → számokkal foglalkoztak

pl.: barátságos számok, tökéletes számok

igazi alkalmazása ennek a területnek a 20. században alakult ki: kriptográfia

Oszthatósági szabályok:

1. : Minden egész szám osztható 1-gyel.
2. : Azok a számok oszthatók 2-vel, amelyeknek utolsó számjegye(egyes helyiértéken álló) osztható 2-vel.
3. : Azok a számok oszthatók 3-mal, amelyeknek a számjegyeinek összege is osztható 3-mal.
4. : Azok a számok oszthatók 4-gyel, amelyeknek az utolsó két számjegyéből képzett kétjegyű szám is osztható 4-gyel.
5. : Azok a számok oszthatók 5-tel, amelyeknek utolsó számjegye is osztható 5-tel.
6. : Azok a számok oszthatók 6-tal, amelyek 2-vel és 3-mal is oszthatóak.
7. : 7-tel úgy vizsgálhatjuk meg az oszthatóságot, hogy a szám első számjegyétől utolsó előtti számjegyéig képzett számból kivonjuk az utolsó számjegy dupláját(2-szeresét).
Ha az így kapott szám osztható 7-tel akkor az eredeti is. Ha még az így kapott számról sem tudjuk megállapítani, hogy osztható-e 7-tel, akkor ugyanezt a tendenciát kell folytatni amíg olyan számot nem kapunk amiről biztosan meg tudjuk állapítani, hogy osztható 7-tel.
Pl.: 315 -> 31-(2*5)=21. 21 osztható 7-tel, tehát 315 is.
8. : Azok a számok oszthatók 8-cal, amelyeknek az utolsó három számjegyéből képzett háromjegyű szám is osztható 8-cal.
9. : Azok a számok oszthatók 9-cel, amelyeknek számjegyeinek összege is osztható 9-cel.
10. : Azok a számok oszthatók 10-zel, amelyeknek utolsó számjegye is osztható 10-zel, magyarul 0-ra végződik.
11. : 11-gyel úgy vizsgálhatjuk meg az oszthatóságot, hogy a szám első számjegyétől utolsó előtti számjegyéig képzett számból kivonom az utolsó számjegyet. Ha az így kapott szám osztható 11-gyel, akkor az eredtei is. Ugyanúgy mint a 7-tel való oszthatóságnál itt is lehet ismételni ezt a folyamatot, ha még mindig megállapíthatatlan az oszhatóság.
Pl.: 5258-> 525-8=517-> 51-7=44 44 osztható 11-gyel, tehát 5258 is.

*Prímszámok definiálása:* Azokat a természetes számokat, amelyeknek pontosan két osztójuk van, prímszámoknak nevezzük.

*Számelmélet alaptétele:* Bármely egész szám felírható véges sok prímszám szorzataként és az a felbontás a tényezők sorrendjétől eltekintve és az egység szorzót figyelmen kívül hagyva egyértelmű.

*Fermat-sejtés később tétel:* [latex inline]a^n+b^n=c^n[/latex] ahol [latex inline]a,b,c,n ϵ Z[/latex] , [latex inline]\mathbb{N}>2[/latex] esetén nincs triviális megoldás

*Számrendszerek:* komolyabb algebrai fejlődéshez kell, plusz informatikában van nagy jelentősége,
hinduktól származtatjuk

### Alkalmazások:

- csekkeken a sorszám ellenőrzés
- kriptográfiában→szuperszámítógépek
- számrendszerek→info
- filozófia, számmisztika

## Ajánlott bizonyítások: