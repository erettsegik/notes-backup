A számítógép, már csak a neve miatt is azt a benyomást kelti, hogy számításokkal foglalkozik, pedig az adatfeldolgozás legalább ilyen fontos felhasználási területe (németül korábban Rechner a *számolni* igéből; franciául ordinateur a *rendez* igéből).

### A számítástechnika kezdetei

A kutatások szerint az ősemberek első számolóeszközei a kavicsok (latinul calculus -> kalkulátor), fadarabok, zsinórra kötött csomók lehettek. Ezek a primitív eszközök nemcsak kifejezték, hanem tárolták is a mennyiségeket. Az emberek kezdettől fogva törekedtek olyan eszközök előállítására, amelyek magát a számolást teszik könnyebbé. Az első számológép az abakusz lehetett.

Napier a 17. században feltalálta a róla elnevezett számolópálcákat, melyeknek segítségével a szorzás és osztás művelete gyorsabban elvégezhetővé vált. (Ezen kívül ő állította össze az első logaritmustáblázatot.)

Ezek az eszközök azonban még nem voltak igazi számítógépek, hiszen nem voltak képesek automatikus működésre.

### Mechanikus számítógépek

1623\.  Schickard megépítette az első komolyabb mechanikus számológépet, ennek működése fogaskerekeken alapult; mind a négy alapműveletet tudta.

1642\.  Pascal köztárcsák segítségével megoldotta a helyiértékek közti átvitelt. Ez a gép már nyolcjegyű számokkal is tudott számolni. Hátránya: csak összeadni és kivonni tudott. Ez az első mechanikus számológép, ami tömeggyártásra került. Pascalról elneveztek egy programozási nyelvet is.

1673\.  Leibniz továbbfejlesztette Pascal gépét váltótárcsák, ill. két regiszter (ideiglenes tartalmú, feldolgozásra alkalmas tárolóegység) beépítésével, így már szorozni és osztani is tudott.

1810\.  Jacquard elkészítette a lyukkártya által vezérelt szövőgépet.
(lyukkártya: a kártyán meghatározott módon elhelyezett lyukak információt hordoznak)
A kártyák cseréjével tetszés szerinti mintázatú szövetet tudott ugyanazzal a géppel előállítani.

1820\.  Thomas megépítette Leibniz gépének továbbfejlesztését, az aritmometert. Ő volt az első ember, aki felvetette egy automata programvezérelt gép (számítógép) megépítését.

1848\.  Boole kidolgozott az állításokon végzett műveletek leírására egy algebrarendszert (Boole-algebra). Ezzel megalapozta a logika formális leírását: nem csak a tagadás, az *és*, a *vagy* matematikai szimbólumait vezette be, hanem –ami ennél sokkal több– matematikailag kezelhetővé tette a *ha… akkor…* típusú mondatokat. (állítások: olyan mondatok, amelyek egyértelműen igazak vagy hamisak, azaz két –logikainak mondott– érték valamelyikét vehetik fel: igazat vagy hamisat, binárisan kódolva: 1-et vagy 0-t) A Boole-algebra a mai digitális számítógép matematikai alapja.

1887\.  Hollerith egy lyukkártyákat használó statisztikai [a tízévenként tartott népszámlálás adatainak feldolgozására alkalmas – talán érdemes lenne akár csak nagyságrendileg említeni a lakosság számát] gépet készített, amely hatalmas adatmennyiség feldolgozására képes. A lyukkártyák egydolláros nagyságúak voltak, mert a pénz számlálására már voltak megfelelő gépek. Ezzel könnyedén –mindössze négy hét alatt– elvégezte az Egyesült Államok 1890-es népszámlálási adatainak feldolgozását (kézi feldolgozással ez több mint egy évtizedig tartott volna). Ennek sikere láttán alapította meg a saját cégét, amelyből aztán 1924-ben megalakult az IBM.

1936\.  Turing programozhatóautomata-elmélete: bebizonyította, hogy ha egy gép el tud végezni néhány alapműveletet, akkor megfelelően programozva bármilyen számításra képes.

### Elektromechanikus számítógépek

XX. század.  A II. világháborúban hadi célokra használták a számítógépeket, leginkább ballisztikai számításokra (lövedékek röppályája), titkosított üzenetek megfejtésére és atombomba-szimulációra. Angliában eredetileg amerikai tervezésű számítógépeket használtak a németek rejtjelezett üzeneteinek megfejtésére és egyéb katonai feladatokra.
Mindezek tekinthetők példaként a számítógép előzményeire, de a mai számítógép elődjének megépítése Neumann Jánoshoz köthető.

### Elektronikus számítógépek

#### Neumann-elv (1945. június)

1945-ben Neumann János (1903-1957) magyar származású tudós kidolgozta saját elveit az ideális számítógép működéséhez, ezek a Neumann-elvek. A legtöbb számítógépet napjainkban is ezen elvek alapján készítik el.

#### Neumann-elvek:

- a gép legyen univerzális: alkalmasság bármilyen adatfeldolgozási feladatra (Turing-elvű)
- kettes (bináris) számrendszer használata
- teljesen elektronikus működés (azaz nincsenek mechanikus, elektromechanikus alkatrészek)
- belső memória (operatív tár) használata az adatok és a programok tárolására (korábban nem volt nyilvánvaló, hogy ez a kettő együtt, egy helyen tárolható)
- soros utasítás-végrehajtás (az utasítások végrehajtása időben egymás után történik)
- központi vezérlőegység alkalmazása

#### Számítógép-generációk

Az elektronikus számítógépek megjelenésétől kezdve a számítógépeket generációkba soroljuk.

##### 1. generáció (1946-1959)
- ENIAC (1946)
  - ez az első programozható, elektronikus, digitális számítógép
  - tízes számrendszerben működött
  - a programot lyukkártyákra lyukasztották
- EDVAC (1949)
  - Neumann János készítette saját elvei alapján
  - ez az első belső programvezetésű, elektronikus, digitális, univerzális számítógép
  - a memória tárolta benne az adatokat és a programokat
  - az ALU-t és a CU-t egyesítették, ezt CPU-nak hívják (ALU: aritmetikai és logikai egység, matematikai és logikai műveleteket hajt végre; CU: vezérlőegység, a processzor munkáját ütemezi; CPU: központi feldolgozóegység/processzor, utasításokat értelmez és hajt végre)
  - a lyukkártyát felváltotta egy mágnesdrót
  - adatkivitelre nyomtatót használtak

Ebben a generációban elektroncsöveket alkalmaztak. A gépek nagyon nagyméretűek és nagyon drágák voltak. Néhány ezer művelet/mp a teljesítményképesség, nagy az energia-felhasználás, a gyakori hibák miatt magas a karbantartási költség.

##### 2. generáció (1959-1964)

A 2. generáció a tranzisztor feltalálásával és elterjedésével kezdődik. A tranzisztor egy félvezetőeszköz, amit elektronikus áramkörben használnak erősítési és kapcsolási célokra. Az elektroncsöveket felváltják a tranzisztorok, így a gépek mérete lényegesen csökken, a számítási sebesség növekszik (1 millió művelet másodpercenként).
- megjelentek az első magas szintű programozási nyelvek (Fortran, Cobol, Algol)
- memóriaként mágnestárakat használtak

##### 3. generáció (1964-1975)

A 3. generációt az integrált áramkör elterjedésétől számítjuk. Az integrált áramkör egy félvezető lapra felvitt kisméretű áramkör. Felhasználásukkal tovább csökkent a számítógépek mérete.
- különvált a hardver és a szoftver
- megjelent a BASIC programozási nyelv  (általános célú, készítette Kemény János és Thomas Kurtz)
- megjelentek az első grafikus monitorok
- elterjedtek a nyomtatók
- a 70-es évek végén megjelent az egér
- a számítógépek ára tovább csökkent
- az első operációs rendszerek születése

##### 4. generáció (1970-es évek közepétől)

A 4. generáció a mikroprocesszor feltalálásával kezdődik. A mikroprocesszor elterjedésével a gépek mérete ugyancsak tovább csökken, beindul a miniatürizálás.
- megalkották a merevlemezt
- 1980-as években megjelentek, s rohamosan elterjedtek a PC-k,
- 1981-ben bemutatták az  első IBM PC-t, 1500 dollárba [szerintem 3000] került, ami akkoriban még egy amerikai mérnöknek is többhavi fizetése volt, de még így is olcsónak számított, 160 kB floppyval rendelkezett
- bemutatták a World Wide Web (WWW) technológiát
- a processzorok teljesítménye exponenciálisan nőtt (Moore-törvény: integrált áramkörökben lévő tranzisztorok száma 18 hónaponként megduplázódik, a processzorok teljesítménye viszont nem csupán a tranzisztorok számától függ)

##### 5. generáció (jelen és jövő)

- nem Neumann-elvű gépek kifejlesztése (párhuzamos utasítás-végrehajtás)
- mesterséges intelligencia

Ezek a gépek már komplex problémákat tudnának alkotó módon megoldani. Ennek a fejlesztésnek a végső célja az igazi mesterséges intelligencia létrehozása lenne. Az egyik aktívan kutatott terület a párhuzamos feldolgozás, azaz amikor sok áramkör egyidejűleg különböző feladatokat old meg. A párhuzamos feldolgozás alkalmas lehet akár az emberi gondolkodás utánzására is.
