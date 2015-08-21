A kombinatorika alapja világunk és a matematika több fontos területének, például a valószínűségszámítés, játékelmélet stb.
fun fact: Pascal megbízásra foglalkozott szerencsejátékkal.

### Kombinatorika

#### Permutáció:

Egy adott n elem különböző egy sorba rendezését permutációnak nevezzük.
 - *Ismétlés nélküli:* ha nincsenek egyforma elemek
   - Tétel: n-elemű halmaz ismétlés néküli permutációi:
   [latex] P_n = n * (n - 1) * (n - 2) * ... * 2 * 1 = n! [/latex]
 - *Ismétléses:* ha vannak egymással megegyező elemek
   - Tétel: n-elem között v-féle egymással megegyező elemek száma: [latex inline] k_1, k_2, k_3, ... , k_r [/latex]
   [latex] P_n^(k_1, k_2, ... , k_r) = \frac{n!}{k_1! * k_2! * ... * k_r!} [/latex]

#### Variáció:

Ha n elemből minden lehetséges módon kiválasztunk k elemet és permutáljuk őket.
 - *Ismétlés nélküli:*
  - Tétel: Az n elem k-ad osztályú ismétlés nélküli variációinak száma:
  [latex] P_n^k = \frac{n!}{(n-k)!} [/latex]
 - *Ismétléses:*
  - Tétel: Az n elem k-ad osztályú ismétléses variációinak száma:[latex inline] n^k [/latex]

#### Kombináció:

Az n egymástól különböző elemből k db-ot minden lehetséges módon kiválasztunk úgy, hogy a kiválasztott elemek sorrendjére nem vagyunk tekintettel.
 - *Ismétlés nélküli:*
  - Tétel: Az n elem k-ad osztályú ismétlés nélküli kombinációinak száma:
  [latex] C_{n,k} = \frac{n * (n - 1) * (n - 2) * ... * (n - k + 1)}{k * (k - 1) * ... * 2 * 1} = \frac{n!}{k!(n-k)!} = \binom{n}{k} [/latex]
 - *Ismétléses:* ahol a kiválsztás sorrendje továbbra sem számít, de a már kiválasztott elemeket újra kiválaszthatjuk
  - Tétel: Az n elem k-ad osztályú ismétléses kombinációinak száma:
  [latex] C_{n,k}^i = \binom{n + k - 1}{k} [/latex]

#### Binomiális tétel:

[latex] \(a+b)^2 = a^2 + 2 a b + b^2 [/latex]

[latex] \(a+b)^3 = a^3 + 3 a^2 b + 3 a b^2 + b^3 [/latex]

[latex] \(a+b)^n = \binom{n}{0} a^n b^0 + \binom{n}{1} a^{n-1} b^1  + \binom{n}{2} a^{n-2} b^2 + ... + \binom{n}{n-1} a^{1} b^{n-1} + \binom{n}{n} a^{0} b^n [/latex]

 - [latex inline] \binom{n}{k} [/latex] binomiális együttható.

### Gráfok:

 - *Gráf:* gráfpontok, és élek
 - *Hurokél:* él aminek ugyanaz a kezdő és végpontja
 - *Izolált pont:* nincs él
 - *Többszörös él:* két csúcs között több él van
 - *Egyszerű gráf:* ha nincs benne hurokél, vagy többszörös él

 *Tétel:* Legalább 2 csúcsú egyszerű gráfban van 2 azonos fokú  csúcs.

 - *Fokszám:* csúcsból kiinduló élek száma

 *Tétel:* a pontok fokszámának összege az élek számának a kétszerese

 - *Összefüggő gráf:* ha bármely pontjából el lehet jutni bármelyik pontjába
 - *Teljes gráf:* n eleme pozitív számok esetén, n pontú gráf melynek minden pontjából egy él vezet a többibe

 *Tétel:* n pontú teljes gráf éleinek a száma [latex inline] \frac{n * (n-1)}{2} [/latex]  

 *Tétel:* n pontú teljes gráfban a fokszámok összege [latex inline] n * (n-1) [/latex]

 - *Út:* olyan élek sora amely egy ponton sem halad át 1-nél többször
 - *Vonal:* minden él csak egyszer szerepel(élsorozat)
 - *Kör:* út amelynek kezdő és végpontja megegyezik
 - *Euler-vonal:* olyan zárt vonal amely nem alkalmaz kört

 *Euler-tétel:* Egy gráf akkor és csak akkor Euler-gráf, ha összefüggő és minden csúcsának fokszáma páros

 - *Fa:* olyan összefüggő gráf amely nem tartalmaz kört

 *Tétel:* A fa bármely két csúcsát egyetlen út köti össze

##### Alkalmazások:
 - szerencsejáték
 - biztosítási szakemberek munkájában
 - kockázat elemzésnél
 - játékelméletnél - Neumann János
 - vállalati stratégiák
 - gazdasági folyamatok elemzésénél
 - genetikai tanácsadásnál
 - Gráfok - Erdős Pál
 - közlekedés szervezése

A gráfelméletnek az utóbbi 20 évben a kiterjesztése a hálózat elmélet. Az let minden területét érinti, főleg az internet(közösségi háló), orvostudomány, biológia.
