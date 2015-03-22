Számsorozatokkal már az ókori görögök is foglalkoztak. Ismerték a számtani sorozat összegzésének módját, az első n négyzetszám összegének a kiszámítását. A sorozatok vizsgálata vezetett el később a differenciál- és integrálszámításhoz.

*Számsorozat definíció:* A számsorozat olyan függvény, amelynek értelmezési tartománya pozitív egész számok halmaza, értékkészlete pedig valamilyen számhalmaz.

*Monotonitás:* Az [latex inline]{a_n}[/latex] sorozat szigorúan monoton növekvő(csökkenő), ha minden pozitív egész n-re teljesül, hogy [latex inline] a_n < a_{n+1} (a_n>a_{n+1}) [/latex]. Sima monotonitás esetén az egyenlőség is megengedett.

 - Monoton sorozat határesete a konstans sorozat

*Korlátosság:* Egy [latex inline]{a_n}[/latex] sorozatnak K felső(alsó) korlátja, ha  minden pozitív egész n-re teljesül. hogy [latex inline] a_n \leq K(k \leq a_n) [/latex] Ilyenkor a sorozat felülről(alúlról) korlátos. Egy sorozatot korlátosnak nevezünk, ha alulról és felülről is korlátos.

*Konvergencia:* Az [latex inline]{a_n}[/latex] sorozat konvergens és határértéke az A szám, ha minden pozitív [latex inline]\epsilon[/latex] számhoz létezik olyan N pozitív egész, hogy a sorozat [latex inline]a_N[/latex] utáni tagjai mind az A szám [latex inline]\epsilon[/latex] sugarú környezetébe esnek, vagyis minden pozitív [latex inline]\epsilon[/latex] számhoz létezik olyan N pozitív egész, hogy minden n>N esetén [latex inline]|a_n - A| < \epsilon [/latex].Jelölése: [latex inline] \lim_{x \to \infty} a_n = A [/latex]

 - A nem konvergens sorozatokat *divergensnek* nevezzük.

*Tétel:* Felülről korlátos szigorúan monoton növekvő sorozat konvergens.

*Torlódási pont:* Az a pont amelynek bármely környezete tartalmaz sorozatbeli pontot.

#### Sorozatok közti műveletek:

- [latex inline] <a_n> \pm <b_n> = <a_n+b_n> [/latex]
- [latex inline] c \in [/latex] ℝ , [latex inline] c * <a_n> = <c * a_n> [/latex]
- [latex inline] <a_n> * <b_n>=<a_n * b_n>
- [latex inline] b_n \neq 0 , \frac{<a_n>}{<b_n>} = < \frac{a_n}{b_n} > [/latex]

### Nevezetes számsorozatok:

 - Számtani sorozat
   + n-edik elem: [latex inline] a_n=a_1+(n - 1) * d [/latex]
   + első n tag összege: [latex inline] S_n = \frac{a_1 * n + a_n}{2}
   + Az első n tag összegtételének bizonyítása itt jó választás lehet.
 - Mértani sorozat
   + n-edik elem: [latex inline] a_n=a_1*q^{n-1} [/latex]
   + első n tag összege: [latex inline] S_n = \frac{a_1 * q^n - 1}{q - 1} , q \neq 1 [/latex]
   + Az első n tag összegtételének bizonyítása itt jó választás lehet.

- *Fibonacci sorozat:*
   + Az első két elem a 0, 1 az összes további elem az előtte lévő kettő összege.
     Képletként:
     [latex] f(n) = 0 , \text{ha } n = 0[/latex]
     [latex] f(n) = 1 , \text{ha } n = 1[/latex]
     [latex] f(n) = F_{n-1} + F_{n-2} , \text{ha } n \geq 0[/latex]

Fibonacci a nyuszik szaporodásának problémájától jutott el a sorozatig.

*Tétel:* A Fibonacci sorozat minden 3. eleme páros.

*Tétel:* Fibonacci sorozat minden 4. eleme osztható 3-al.

*Tétel:* A Fibonacci sorozat bármely két szomszédos tagja relatív prím

[latex inline] \frac{f_n}{f_m} = \frac{n}{m} [/latex], a tagok akkor osztják egymást, ha sorszámaik is

*Tétel:* Számpárainak a hányadosa az aranymetszés irracionális számához konvergál

*Tétel:* két Fibonacci típusú sorozat összege és különbsége is fibonacci típusú

 - A fenti tételek egyikét érdemes ebből az anyagrészbő bizonyítani

itt érdemes megemlíteni a következő rekurzív sorozatot: [latex inline] (1 + \frac{1}{n})^n [/latex] aminek a határértéke egy irracionális szám az e.
[latex] \lim_{x \to \infty}(1 + \frac{1}{n})^n = e[/latex]

 - a sorozat tul.: szigorúan monoton növekvő, és felülről korlátos

### Sorok:

[latex inline] <a_n> [/latex]

[latex inline] S_1= a_1 [/latex]

[latex inline] S_2= a_1 + a_2 [/latex]

[latex inline] S_n = \sum_{i = 1}^n a_i [/latex]

[latex inline] <S_n> [/latex] : sor a részletösszegek sorozata

 - ha [latex inline] <S_n> [/latex] sorozat konvergens akkor a határértékét a sor összegének nevezzük
   [latex] \sum_{i = 1}^n a_i = \lim_{n \to \infty} S_n = S [/latex]

*Mértani sor összege:* [latex inline] S = \frac{a_1}{q - 1} [/latex]

*Zenon:* Akhilleusz és a teknősbéka versenye, a köztük lévő távolság feleződik, ezért Akhilleusz nem nyerhet mivel előnyt adott a teknősnek, megoldás a sorok.

#### Sorok közti műveletek:
[latex] \sum(a_n \pm b_n) = \sum a_n \pm \sum b_n [/latex]
[latex] \sum(a_n * b_n) = \sum a_n * \sum b_n [/latex]
[latex] \sum\frac{a_n}{b_n} = \frac{\sum a_n}{\sum b_n} [/latex]

### Alkalmazások:

- Mértani sorozat: kamatos kamat
- Fibonacci sorozat: természet/művészet + kapocs aranymetszéshez(építészet, fényképészet, zene)
- Sorok: Zenon agóriák
- prímszámok reciprokai
