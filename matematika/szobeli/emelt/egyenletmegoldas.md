*Egyenlet definíciója:* két függvényt egyenlővé teszünk. [latex inline]f : A \to B , f(x) = g(x)[/latex]. Azok az A-beli elemek, amelyekre az egyenlőség teljesül, az egyenlet gyökei.

*Osztályozás:* Algebrai és transzcendens

## Transzcendens egyenletek

 - trigonometrikus egyenletek
 - logaritmusos egyenletek
 - exponenciális egyenletek
 - differenciálegyenletek

## Algebrai egyenletek

*Egyismeretlenes egyenletek:*

*Algebrai egyenlet:* Ha egy polinomot nullával egyenlővé teszünk, algebrai egyenletet kapunk. Az egyenlet megoldásai alkotják az egyenlet igazsághalmazát.

*Algebra alaptétele:* n-edfokú egyenletnek pontosan n megoldása van, de n-edfokú egynletnek legfejlebb n darab valós megoldása van. (előfordulhat, hogy két gyök egyenlő)

1. Elsőfokú egyenlet:
   [latex]a * x + b = 0 [/latex]
2. Másodfokú egyenlet:(megoldóképlettel)
   [latex]a*x^2 + b*x + c = 0[/latex]
   [latex] x_{1,2} = \frac{- b \pm \sqrt{b^2 - 4*a*c}}{2*a} [/latex]
3. Harmadfokú egyenlet:
   - [latex inline]ax^3 + bx^2 + cx + d = 0[/latex], a 3 gyök megadható a Cardano-képlet segítségével, bár az eredményeket komplex formában adja meg.
4. Negyedfokú egyenlet:
   - van megoldóképlete.
5. n-ed fokú egyenletek:
   - [latex inline] P(x) = a_n*x^n + a_{n-1}*x^{n-1} + ... + a_2*x^2 + a_1*x + a_0 [/latex]

*Bizonyított állítás (Gelois-Abel tétel):* 5-ödfokútól felfele nem létezik megoldóképlet

A reciprokegyenleteket még meg lehet oldani a 9. fokig.

### Megoldási módszerek

1. *Grafikus megoldás:*
   Az egyenlet, egyenlőtlenség mindkét oldalát egy-egy függvényként ábrázoljuk közös koordináta rendszerben. Az egyenlet megoldása a két grafikon metszéspontjainak x koordinátája.
2. Közelítő értékkel számolás
3. *Mérlegelv / algebrai megoldás:*
   Egy egyenlet megoldáshalmaza nem változik, ha az egyenlet mindkét oldalához ugyanazt a számot hozzáadjuk, vagy ugyanazzal a 0-tól különböző számmal megszorozzuk. (kölcsönösen ekvivalens változtatásokat hajtunk végre)
4. *Értelmezési tartomány vizsgálatával:*
   Megnézzük, hogy az egyenlet két oldalának mi az értelmezési tartománya, és ha nincs közös halmazuk, akkor az egyenletnek sincs megoldása. Pl.: [latex inline] \sqrt{x + 5} = \sqrt{x - 5}
5. *Értékkészlet vizsgálattal:*
   Megnézzük, hogy az egyenlet két oldalának mi az értékkészlete, és az alapján állapítjuk meg, hány gyöke és hol van az egyenletnek. Pl.: [latex inline] |x + 2| + |x - 4| + |x + 6| = 0 [/latex] ; [latex inline]2^x + 2^{-x} = \sin x [/latex]
6. Új változó bevezetésével – Pl.: reciprokegyenleteknél
7. Megoldóképlettel az egyenlet fokától függően

### Gyökvesztés, gyökvonás

 - Pl.: négyzetre emelésnél hamis gyököt hozhatunk létre
 - Pl.: ellipszis egyenletének levezetésénél

*Gyökvesztés:* x-el való leosztás esetén ha x = 0 / vagy gyökvonás esetén ha x = 0.

## Viète formulák

*Másodfokú egyenletnél:* [latex inline] a*x^2 + b*x + c = 0 [/latex]
[latex] x_1 + x_2 = - \frac{b}{a} [/latex]
[latex] x_1 * x_2 = \frac{c}{a} [/latex]

A formula általánosítható n-ed fokú egyenletre:
[latex] x_1 + x_2 + ... + x_n = - \frac{a_{n-1}}{a_n} [/latex]
[latex] x_1 * x_2 * ... * x_n = (-1)^n * \frac{a_0}{a_n}[/latex]

## Alkalmazások

### Koordináta geometriában

 - Egy adott pont rajta van-e egy ...
 - Szélsőérték számítási problémáknál (differenciálszámítással)

### Fizikában

 - *test szabadesése:* másodfokú egyenlet
 - termodinamikai folyamatok leírásában
 - Kirchhoff törvény felírása során (áramerősséget számolunk)

### Informatikában

 - Bármely elemző modellező programban.
 - Képszerkesztő alkalmazásokban
 - stb.
