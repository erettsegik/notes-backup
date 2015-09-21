A halmazelmélet a matematika egyik legfiatalabb ága. A 19. század óta foglalkozunk vele Georg Kantornak köszönhetően.

Alapfogalmak: halmaz, halmaz eleme.

Halmaz elemei bármik lehetnek, számok, tárgyak, emberek, adatok, stb. Legtöbbet a matematikában használjuk, melynek több területén is előfordulnak:

 - függvénytanban
 - kombinatorikában
 - geometriában

Egy halmaz megadása történhet:

 - felsorolással: A = {1; 2; 3; 4}
 - tulajdonsággal: B = {négyszögek}; C = {pozitív egész számok 100-ig}
 - képlettel: S = {x | x ϵ N, x < 1000}
 - vagy egyéb módon

*Komplementer halmaz*: Egy A halmaz komplementer halmazának az alaphalmaz azon elemeinek halmazát nevezzük, amelyek az A halmaznak nem elemei. Jele: [latex inline]\overline{A}[/latex].

![Komplementer](http://i.imgur.com/6Zy6sqS.png)

Egy halmazt akkor nevezünk egy másik *részhalmazának*, ha a halmaz összes eleme megtalálható a másikban is. Tehát ha A halmaznak részhalmaza B halmaz, akkor B halmaz minden eleme megtalálható A halmazban.

 - halmaz részhalmazainak száma [latex inline]2^n[/latex]. Ez teljes indukcióval bizonyítható.

*Két halmaz egyenlő*, ha minden eleme egyenlő.

A 0 elemű halmazt *üres halmaznak* nevezzük, jele: ø vagy {}

## Halmazok közti műveletek:

*Unió*: Két halmaz uniója azon elemek halmaza, amelyek legalább az egyik halmaznak elemei. Jele ⋃.

 - *kommutatív művelet:* A ⋃ B = B ⋃ A
 - *asszociatív művelet:* A ⋃ (B ⋃ C) = (A ⋃ B) ⋃ C = A ⋃ B ⋃ C

![Unió](http://i.imgur.com/6Tgq2UN.png)

*Metszet*: Két halmaz metszete mindazon elemek halmaza, amelyek mindkét halmaznak elemei. Jele ⋂.

![Metszet](http://i.imgur.com/xUhQG8t.png)

*Diszjunkt* halmaznak azt nevezzük, ha két halmaz metszete üres halmaz.

*Disztributivitás*: A ⋃ (B ⋂ C) = (A ⋃ B) ⋂ (A ⋃ C) ;  A ⋂ (B ⋃ C) = (A ⋂ B) ⋃ (A ⋂ C)

*Két halmaz különbsége*: Az A és B halmaz különbsége az A halmaz mindazon elemeinek halmaza, amelyek a B halmaznak nem elemei. Jele: A\B.

![Különbség](http://i.imgur.com/p4OhxFZ.png)

*Szimmetrikus differencia*: Az A és B halmaz szimmetrikus differenciája azon elemek halmaza, amelyek A és B halmaz közül pontosan az egyiknek elemei. (Tehát minden olyan elem, ami eleme vagy az A halmaznak vagy a B-nek. – kizáró vagy)

 - A Δ C = (A\C) ⋃ (C\A)

![Szimmetrikus differencia](http://i.imgur.com/ZSndnLQ.png)

*Descartes-szorzat*: Két halmaz Descartes szorzata olyan rendezett elempárok halmaza, ahol az első elem az első halmazból, a második elem a második halmazból származik.

## Halmazok számossága:

Egy *véges halmaz számosságán* elemeinek számát értjük. Jelölés: H halmaz számossága: |H|

Egy halmazt véges halmaznak nevezünk, ha nem létezik olyan valódi részhalmaza, amivel ugyanakkora a számossága (ekvivalens lenne). A nem véges halmazokat végtelennek nevezzük.

Két típusú végtelen lehet:
 - *megszámlálhatóan végtelen*: alef zéró
 - *nem megszámlálhatóan végtelen*: kontinuum számosság

*Kontinuum-sejtés*: Nem létezik olyan halmaz amelynek számossága az alef zéró és a kontinuum végtelen közé esik. Halmazelmélet ma létező legjobb axiómarendszere szerint a kontinuum sejtést sem bebizonyítani, sem megcáfolni nem lehet.

Pl: számhalmazok (ℕ, ℤ, ℝ, ℂ)

## Nevezetes ponthalmazok síkban:

Két adott ponttól egyenlő távolságra lévő pontok halmaza – *egyenes*

Egy egyenestől és egy rá nem illeszkedő ponttól egyenlő távolságra lévő pontok halmaza. – *parabola*

*Parabola:* Adott síkban egy pont és egy rá nem illeszkedő egyenes, és azoknak a pontoknak a halmazát a síkban, amelyek a ponttól és az egyenestől egyenlő távolságra vannak, parabolának nevezzük.

Három adott ponttól egyenlő távolságra lévő pontok halmaza:

- *Háromszög oldalfelező merőlegesei* → háromszög köré írható kör középpontja
  + Itt érdemes az előbbi tétel bizonyítását elmondani ha ezt választottad a tételhez.

Három egyenestől egyenlő távolságra lévő pontok halmaza:

- *Háromszög szögfelezői* → háromszögbe írható kör középpontja
  + Itt érdemes az előbbi tétel bizonyítását elmondani ha ezt választottad a tételhez. → Cheva tételének megemlítése meglepő húzás lehet.

*Ellipszis:* adott síkban két egymásra nem illeszkedő pont és egy a távolságuknál nagyobb pozitív valós szám, azoknak a pontoknak a halmazát a síkban, amelyeknek a két ponttól mért távolságának az összege az adott szám, ellipszisnek nevezzük.

*Hiperbola:* adott a síkban két pont és egy a távolságuknál kisebb pozitív szám, azoknak a pontoknak a halmazát a síkban, amelyeknek a két ponttól mért távolságának a különbségének az abszolút értéke megegyezik az adott számmal, hiperbolának nevezzük.

## Nevezetes ponthalmazok a térben:

*Gömb:* Egy ponttól azonos távolságban lévő pontok halmaza a térben.

*Paraboloid:* Adott a térben egy pont és egy rá nem illeszkedő sík, és azoknak a pontoknak a halmazát a térben, amelyek a ponttól és a síktól egyenlő távolságra vannak, paraboloidnak nevezzük.

*Ellipszoid:* Adott a térben két egymásra nem illeszkedő pont és egy a távolságuknál nagyobb pozitív valós szám, azoknak a pontoknak a halmazát a térben, amelyeknek a két ponttól mért távolságának az összege az adott szám, ellipszoidnak nevezzük.

*Hiperboloid:* Adott a térben két pont és egy a távolságuknál kisebb pozitív valós szám, azoknak a pontoknak a halmazát a térben, amelyeknek a két ponttól mért távolságának a különbségének az abszolút értéke megegyezik az adott számmal, hiperboloidnak nevezzük.

## Alkalmazások:

Matematikai:

 - egyenlőtlenségek (törtes)
 - metszetek (koordináta geometriában)
 - függvények É.T., É.K.-ének megadásakor
 - Descartes szorzat megjelenik a pont koordinátáinál térben

Fizikai:
 - Descartes: 3.;4.;5 dimenzióbeli alkalmazása(hőmérséklet, idő)
 - Logikai áramkörök és/vagy kapcsolások
 - számítógép működésének alapja
 - nyelvészetben
 - kódfejtés
 - jogi érverlésnél: és/vagy (ahol matematikai, vagy hétköznapi „vagy”)
