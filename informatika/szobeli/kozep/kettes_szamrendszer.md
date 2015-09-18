## A számrendszerekről általánosságban

A tízes számrendszer a számok ábrázolásának legelterjedtebb módja; a hétköznapi ember számára nem is létezik másik számrendszer. Ennek kézenfekvő oka lehet, hogy az embernek tíz ujja van, ugyanakkor sok nyelv utal arra, hogy nem mindig és nem mindenütt volt kizárólagos a tízes csoportosítás (twelve, thirteen; zwölf, dreizehn – seize, dix-sept – septemdecim, duodeviginti; quatre-vingt, quatre-vingt-dix); az időmérés és a szögmérés ősi 12-es, 60-as tagolása is ezt erősíti.

## A kettes számrendszerről

Az informatikában a kettes számrendszert használjuk, mert így tudunk adatokat könnyen tárolni és továbbítani: az általánosan elterjedt informatikai eszközökben az áramnak kétféle állapotára építünk (van vagy nincs), illetve a mágneses háttértáraknál is a kétféle pólus meglétét használjuk ki (északi vagy déli pólus).

Ugyanakkor a kettes számrendszer nagyon hosszú számokat eredményez, ezért az így megadott számokat rövidebben (gyakran 16-os, esetleg nyolcas számrendszerben) írjuk le; a hétköznapi élettel való kapcsolatteremtéshez pedig ismernünk kell a kettes-tízes, illetve tízes-kettes átváltást.

A kettes számrendszerben két számjegy van, a helyiértékek pedig a kettő természetes kitevőjű (illetve, amint látni fogjuk, valójában egész kitevőjű) hatványai.

### Átváltás

#### 2 --> 10:

| 16 | 8 | 4 | 2 | 1 |
|:--:|:-:|:-:|:-:|:-:|
|  1 | 0 | 0 | 1 | 1 |

1 \* 16 + 0 \* 8 + 0 \* 4 + 2 \* 1 + 1 \* 1 = 19

#### 10 --> 2:

| 372 =    | 256 | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
|:--------:|:---:|:---:|:--:|:--:|:--:|:-:|:-:|:-:|:-:|
|          | 1   | 0   | 1  | 1  | 1  | 0 | 1 | 0 | 0 |
| Maradék: | 116 | -   | 52 | 20 | 4  | - | 0 | - | - |

A számítógépeken 1 byte-on (8 biten) 0-tól 255-ig ábrázolhatjuk a természetes számokat. A számítógépek egyik legalapvetőbb művelete az inkrementálás, azaz az 1-gyel való növelés; ennek nagy jelentősége lesz a negatív számok ábrázolásának megértésében.

Néhány példa erre:

|               |                |
|:-------------:|:--------------:|
| 0000 --> 0001 | 0011 --> 0100  |
| 0101 --> 0110 | 1111 --> 10000 |

### Negatív számok

Ha negatív számokat szeretnénk ábrázolni, akkor a legkézenfekvőbb megoldásnak az tűnik, hogy van egy előjelbit, amely megmutatja, hogy az adott szám pozitív (ha az előjelbit 0), illetve negatív (ha az előjelbit 1): például 00001111 --> 15, 10001111 --> -15

Ez a megoldás azonban két okból is célszerűtlen. Egyfelől így két különböző (formájú) nulla lenne, hiszen a 00000000 és az 10000000 is azt jelölné. Ennél sokkal nagyobb baj azonban, hogy így az inkrementálás nem működnék (pontosabban csak a pozitív számok esetén működnék a megszokott módon): 10000001-et (-1-et) inkrementálva 10000010-t (-2-t) kapnánk. Ezért annak érdekében, az inkrementálás egységes módon működjék a különböző előjelű számok esetén, egy kicsit bonyolultabb lesz a megoldás:

|   |   |   |   |   |   |   |   |      |
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:----:|
| 1 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | -128 |
| 1 | 1 | 1 | 1 | 1 | 1 | 1 | 0 | -2   |
| 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | -1   |
| 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0    |
| 0 | 0 | 0 | 0 | 0 | 0 | 0 | 1 | 1    |
| 0 | 0 | 0 | 0 | 0 | 0 | 1 | 0 | 2    |
| 0 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 127  |

Így már minden esetben működik az inkrementálás; ahogy a fenti táblázat mutatja, 8 biten -128-tól 127-ig tudjuk ábrázolni az egészeket.

(Amikor az 1111111-et (a -1-et) inkrementáljuk, akkor valójában 100000000-at kellene kapnunk, de mivel a számítógép (ebben az egyszerű esetben) 8 biten dolgozik, az élen álló 1-est nem jeleníti meg. Hasonló helyzetet látunk tehát, mint a hétköznapi életben például egy hagyományos villanyóránál. Ezt a jelenséget túlcsordulásnak nevezzük.)

Ha jobban megfigyeljük, az első bit megmutatja a szám előjelét: ha ez 0, akkor 0 vagy pozitív a szám, ha pedig 1, akkor negatív a szám.

A pozitív számok átváltása ezek után kézenfekvő (úgy dolgozunk, ahogyan korábban felvázoltuk).

A negatív számokat azonban nem lehet olyan könnyen átváltani, mint a pozitívokat. Ha egy negatív, 10-es számrendszerbeli számot akarunk átváltani, a következő a teendő. Először vegyük a szám -1 szeresét, váltsuk át úgy, mintha egy pozitív számot váltanánk át, majd ezt a számot negáljuk (a 0-k helyére 1-eseket írunk, az 1-esek helyére 0-kat), végül ezt a 2-es számrendszerbeli számot inkrementáljuk.

Ha egy 2-es számrendszerbeli számot szeretnénk átváltani 10-es számrendszerbe, akkor ugyanez a teendőnk, csak visszafelé kell végigmennünk a lépéseken, és inkrementálás helyett dekrementálnunk kell (ez az 1-gyel való csökkentés művelete).

### Törtek

Tízes számrendszerben a (tizedes)törtekben egy tizedesvesszővel választjuk el az egész részt és a tört részt: 12,34. Ennek mintájára a 2-es számrendszerben a (kettedes)törtekben kettedesvessző áll: 10,01

Kettes számrendszerből a szokásos módon váltjuk 10-esbe a számokat:

| 8 | 4 | 2 | 1 | &nbsp; | 1/2 | 1/4 | 1/8 |
|:-:|:-:|:-:|:-:|:-:|:---:|:---:|:---:|
| 0 | 0 | 1 | 0 | , | 0   | 1   | 0   |

= 2,25

Tízes számrendszerből kettesbe akkor legkönnyebb az átváltás, ha a nevező kettő valamelyik (pozitív egész kitevős) hatványa. Ilyenkor az a legegyszerűbb eljárás, hogy átváltjuk a számlálóban lévő számot, majd odébbtoljuk a kettedesvesszőt.

A k/l nem egyszerűsíthető tört 10-es számrendszerbeli alakja véges, ha l=2^m*5^n. Ugyanígy a 2-es számrendszerben k/l nem egyszerűsíthető tört alakja véges, ha l=2^m. Ez a két állítás visszafelé is igaz. Ennek furcsa következménye például az, hogy 1/10 kettes számrendszerben végtelen tizedes tört, ami azt eredményezi, hogy a számítógép nem tud vele pontosan számolni.

#### Törtek a számítógépen

A törtek ábrázolására kétféle módszert használhatunk a számítástechnikában.

Az egyik a fixpontos ábrázolás, amikor a kettedesvesszőt adott helyen rögzítjük.

| &nbsp; | &nbsp; | &nbsp; | &nbsp; | ,  | &nbsp; | &nbsp; | &nbsp; | &nbsp; |
|:-:|:-:|:-:|:-:|:--:|:-:|:-:|:-:|:-:|

Ebben az esetben a legkisebb szám (8 biten) az 1/16-od, a legnagyobb pedig 15 egész 15/16, a számítás pontossága 1/16. Ez éppen olyan, mintha a tízes számrendszerben 0,0001 és 9999,9999 között 1/10000 pontossággal számolnánk. Ilyenkor tehát az abszolút pontosság állandó, ennek azonban nem sok értelme van: sokkal célszerűbb, ha a relatív pontosság állandó (azaz a hiba az ábrázolt számnak mindig ugyanannyi százaléka lehet, ami úgy érhető el, ha a hiba és az ábrázolt szám nagyságrendjének különbsége állandó).

Ezt a másik módszerrel, a lebegőpontosnak mondott számábrázolással érhetjük el; ez lényegében a tízes számrendszerből ismert normálalak megfelelője. Ahogyan 10-es számrendszerben felírhatjuk a számot: m x 10^k alakban, úgy 2-es számrendszerben m x 2^k lesz a normálalak, ahol m-et mantisszának nevezzük, k-t pedig karakterisztikának. Egyszerű esetben például 8 bitből 5-öt lefoglalhat a mantissza, 3-at pedig a karakterisztika (a valóságban mindkettő hosszabb, azaz a szám –éppen úgy, mint a legtöbb egész típus–
több byte-os).

### Műveletek

Egyszerű műveletek elvégzése kettes számrendszerben:

#### Összeadás

Hasonlóan a tízes számrendszerhez, itt is egymás alá kell írni azt a két számot, amelyet össze szeretnénk adni. Így gyakorlatilag öt eset lehetséges:

|           |                                                     |
|:---------:|:---------------------------------------------------:|
| 0 + 0     | = 0                                                 |
| 1 + 0     | = 1                                                 |
| 0 + 1     | = 1                                                 |
| 1 + 1     | = 10 (a 0-t leírjuk, az 1-et továbbvisszük)         |
| 1 + 1 + 1 | = 11 (az 1-et leírjuk, a másik 1-est továbbvisszük) |

Ez negatív számokkal is működik; ez a kettes komplemens ábrázolás legfőbb előnye.

#### Szorzás

A tízes számrendszerben a legalapvetőbb szorzás a tízzel való szorzás, ugyanígy a kettes számrendszerben a kettővel való szorzás a legfontosabb. A kettes számrendszerben a kettővel való szorzás ugyanúgy működik, mint a tízes számrendszerben, azaz egy nullát írunk a szám végére:

|         |   |      |
|:-------:|:-:|:----:|
| 111 × 2 | = | 1110 |
