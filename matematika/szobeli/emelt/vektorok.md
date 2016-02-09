*Fogalma:* az irányított szakaszt vektornak nevezzük

 - független számpárral/számhármassal/szám n-essel megadott mennyiség (vektor dimenziói)
   + a vektorok igazi létjogosultságát a fizika igényelte
   + a valós számok is felfoghatóak egydimenziós vektorként
     - komplexek kétdimenziósként

*Definíció:* a vektor abszolút értéke a vektort meghatározó irányított szakasz hossza

*Definíció:* két vektor egyirányú, ha a két vektor párhuzamos, és azonos irányba mutat

*Definíció:* két vektor egyenlő, ha egyirányúak és abszolút értékük is egyenlő

*Vektorműveletek:* összeadás, kivonás, nullvektor, ellentett vektor

*Vektorok összege* annak az eltolásnak a vektora, amellyel helyettesíthető az a vektorral és a b vektorral történő egymásutánja

*Vektorösszeadás tulajdonságai:*
 - kommutatív: [latex inline] a + b = b + a [/latex]
 - asszociatív: [latex inline] \(a + b) + c = a + (b + c) [/latex]

*Különbségvektor* az a vektor, amelyhez a b vektort adva az a vektort kapjuk

*Definíció:* egy nullvektortól különböző a vektor tetszőleges [latex inline] \lambda [/latex] valós számmal (skalárral) vett szorzata egy olyan vektor, amelynek abszolút értéke [latex inline] |\lambda| * |a| [/latex] és [latex inline] \lambda > 0 [/latex] esetén a-val egyirányú, [latex inline] \lambda < 0 [/latex] esetén a-val ellentétes irányú

*Skalárral vett szorzat:*

 - disztributív: [latex inline] \alpha * a + \beta * a = ( \alpha + \beta ) * a [/latex]
 - asszociatív: [latex inline] \alpha * ( \beta * a) = ( \alpha * \beta ) * a [/latex]

*Két vektor skaláris szorzata:* az a szám, ami a két vektor nagyságának és a közbezárt szögük koszinuszának a szorzatával egyezik meg

 - disztributív
 - nem asszociatív
 - kommutatív [latex inline] \overline{a} * \overline{b} = \overline{b} * \overline{a} [/latex]

*Vektoriális szorzás:* két vektor szorzatán értjük azt a vektort, amelynek nagysága a két vektor hosszának és az általuk bezárt szög szinuszának a szorzata

 - iránya merőleges a két vektor által meghatározott síkra
 - nem kommutatív

*Vegyes szorzat:* három vektor vegyes szorzata megadja az általuk kifeszített paralelepipedon térfogatát. determinánssal számolható

## Vektorok felbontása:

 - ha két vektor párhuzamos, egy számmal (skalár) szorzással egyik a másikból felírható
 - ha két vektor nem párhuzamos, akkor független vektorok, egyik a másikból nem fejezhető ki
 - ha egy síkban két nem párhuzamos vektort rögzítünk, akkor a sík bármely vektora előállítható ezek lineáris kombinációjaként
   - több dimenzióban is működik, 3-ban 3-mal, n-ben n-nel

*Lineáris kombináció:* tetszőleges a, b vektorokkal és [latex inline] \alpha [/latex], [latex inline] \beta [/latex] valós számokkal képzell [latex inline] v = \alpha * a + \beta * b [/latex] vektort az a és b vektorok lináris kombinációjának nevezzük

a lináris kombinációban szereplő a és b vektorokat bázisvektoroknak nevezzük

## Vektorok koordinátái

a síkbeli derékszögű koordináta-rendszerben a bázisvektorok az origóból kiinduló egymásra merőleges egységvektorok, melyek az origótól kifelé mutatnak

*Definíció:* a derékszögű koordináta-rendszerben egy vektor koordinátáinak nevezzük az origó kezdőpontú, vele egyenlő helyvektor végpontjának koordinátáit [latex inline] \overline{a}(a_1, a_2) [/latex]

*Tétel:* vektor koordinátáinak kiszámítása kezdő- és végpontjának segítségével: [latex inline] A(a_1, a_2), B(b_1, b_2) \to AB(b_1-a_1, b_2-a_2) [/latex]

## Vektorműveletek koordinátákkal:

 - összeg: [latex inline] \overline{a} + \overline{b} =  (a_1 + b_1, a_2 + b_2) [/latex]
 - különbség: [latex inline] \overline{a} - \overline{b} = (a_1 - b_1, a_2 - b_2) [/latex]
 - számszoros: [latex inline] \lambda * \overline{a} (\lambda * a_1, \lambda * a_2) [/latex]
 - 90°-os elforgatás
   + +90° [latex inline] \overline{a}(a_1, a_2) \to \overline{a}'(-a_2, a_1) [/latex]
   + -90° [latex inline] \overline{a}(a_1, a_2) \to \overline{a}"(a_2, -a_1) [/latex]

Tetszőleges két vektor skalárszorzata: [latex inline] \overline{a} * \overline{b} = |\overline{a}| * |\overline{b}| * cos \alpha [/latex]

![Skaláris szorzat](http://i.imgur.com/OVEBj1A.png)

két vektor szorzata akkor és csak akkor 0, ha merőlegesek egymásra
 - bizonyítás

vektor → 1 soros mátrix

## Alkalmazások

 - szögfüggvények
 - addíciós tételek bizonyítása
 - két vektor vektoriális szorzatának nagysága pralelogramma területe
 - eltolás transzformáció

### Fizika

 - vektormennyiségek: v, a F, p, E, B
 - munka → skalárszorzat
 - vektoriális szorzat → lorentz erő, forgatónyomaték
 - mátrixok mint adatkezelés
