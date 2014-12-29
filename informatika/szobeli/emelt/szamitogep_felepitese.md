> A Neumann által megfogalmazott elvek, és ezek hatása a számítógépek fejődésére. A Neumann-elvű számítógép elvi felépítése, az egyes részegységek feladata.
> A ma használatos számítógépek elvi felépítése és a Neumann elvek.

Neumann általl megfogalmazott elvek, és ezek hatása a számítógép fejlődésre:

 - Szekvenciális működés: az utásításokat sorrendben hajtja végig, egyszerre csak egyet.
 - Kettes számrendszeren használata: Kétállapotú elemekkel a kétféle számjegy könnyen modellezhető (Hatása:  a mechanikus részek elvételével jelentősen csökkentek a méretek.)
 - Belső memória használata: tárolja a feldolgozás alatt álló adatokat és végrehajtandó program utasításokat
 - Univerzális legyen a számítógép: különféle szoftverekkel különböző feladatok ellátására alkalmas

Ezeken az 1946-ban pulbikált elveken alapulnak a mai számítógépek nagy része is.

A Neumann-elvű számítógép elvi felépítése, az egyes részegységek feladata:

 - Memória: a feldolgozást vezérlő program és a feldolgozandó adatok tárolóhelye működés közben.
 - Cache: gyorsítótár, a memóriából idekerül a feldolgozandó tartalom
 - CU:  Vezérlőegység, ez az utasítás regiszterek tartalma alapján a többi egység működését vezérli
 - Regiszterek: a CU itt tárolja az éppen végrehajtott utasításokat
 - ALU: számoló és logikai egység
 - Bemeneti perifériák(eszközök): adatot tartalmazó egység, amit a gép beolvas
 - Kimeneti perifériák: adatot kiíró egységek

Két fő funckionális egység a számítógépben: központi egység(CPU) és periféria. Az első ami a tevékenységeket irányítja,
az utóbbi ami biztosítja a kapcsolatot a központi egység és annak környezete / a felhasználó között.

A ma használatos számítógépek elvi felépítése és a Neumann elvek:

 - CPU: központi feldolgozó egység
 - Busz rendszer: kapcsolatot teremt a CPU és a memiróa/egyes perifériák között (vezetékek, vezérlő áramkörök)
 - Memória: végrehajtás alatt tárolja a programot és a szükséges adatokat; ROM - Csak olvasható; RAM - Ítható és olvasható
 - Merevlemez: elsődleges háttértár, a programokat és adatokat tartalmazza (nem felhasználás közben, lsd. Memória)
 - Optikai lemez: legelterjedtebb cserélhető lemehezes háttértároló
 - Egyéb:
   + Alaplap:  kisegítő áramkörök, órajelgenerátor, buszrendszerek, csatoló felületek egységbe foglalása
   + Tápegység: a számítógép egyes részeit árammal látja el
   + Ház: egybe foglalja a számítógépet

> A mai (személyi) számítógépek részei és ezek jellemző paramétereinek bemutatása. Az egyes részek funkciói.

> Központi feldolgozóegység, jellemző értékek.

Közismertebb nevén processzor. Többmillió tranzisztorból áll.
Feladatai:

 - a program utasításainak értelmezése és végrehajtása
 - ezek alapján a gép részegységeinek vezérlése
 - az adodó számítási műveletek elvégzése

Részei:

 - CU (vezérlőegység): értelmezi a program utasításait, előállítja a végrehajtáshoz szükséges vezérlőjeleket
 - ALU (aritmetikai és logikai egység): aritmetikai és logikai műveleketek elvégzése
 - Regiszterek (fajtái):
   + Programszámláló: (végrehajtásnál a következő utasítás címét tartalmazza
   + Veremtár mutató: alprogramok hívásánál a visszatérési címet és a CPU állapotát tartalmazó veremre mutat
   + Akkumulátr: Általános célú regiszter, utasítások használják (pl. aritmetikai eredmények ide kerülnek).
 - Gyorsítótár: A többi, különböző sebességgel működő eszközzel való adatcserénél használatos átmeneti tár, gyorsítja a műveleteket.
 - Belső órajel: Feladatok elvégzésének gyorsaságát biztosítja, manapság 3GHz is lehet.
 - Külső órajel: A frekvencia, amivel a processzor a környezetével kommunikál, manapság 800 MHz is lehet.

A processzor lehet 32 vagy 64 bites, ez a legnagyobb adatméretet jelöli, amivel a processzor dolgozhat.

> Memória: memóriafajták, jellemzők és felhasználási területük.

RAM (közvetlen hozzáférésű memória) - Operatív memória.
Az éppen futó programok és az általuk használt adatok tárolása. A már nem szükséges adatok helyére újat ír. Megcímzett rekeszekben tárolja az egyes adatelemeket.
A megcímezhető tartomány függ a mikroprocesszortól; Pl.: 32 bites címzés esetén maximum 4GB memória megcímzése lehetséges.
A RAM működése dinamukis; áramkörrel folyamatosan frissíti tartalmát, mp-nként akár több százszor is kiolvassa majd újraírja a tárolt adatokat.
Hozzáférési idő: a tárolócella címzése és a neki megfelelő adat megjelnése között eltelt idő (dinamikus RAM-nál: 90ns). Feszültség hiányában törlődnek róla az adatok. Legfőbb jellemző paraméterei:

 - Típus: DDR, DDR-II, DDR-III
 - Kapacitás: 512 MB, 1 GB, 2GB
 - Órajel: 533MHz, 667MHz, 800MHz (hozzáférés üteme)

ROM - Csak olvasható memória
Számítógép bekapcsolásakor a hardverkomponensek ellenőrzéséhez szükséges adatok, az operációs rendszer betöltését végző programok tárolása.
Kicsi kapacitás, megbízható tároló, tartalmát csak ritkán kell módosítani. RAM-mal ellentétben nem igényel áramellátást az adatok megőrzéséhez.
Fajtái:

 - ROM: Csak olvasható, ált. gyári beállításokkal rendelkezik.
 - PROM: Egyszer írható, egyébként csak olvasható tároló. Írás speciális eszközökkel.
 - EPROM: Újraírható tároló, törlése UV fénnyel történik. Írás speciális eszközökkel.
 - EEPROM: Újraírható tároló, elektronikusan törölhető és írható.
 - flash: Hasonló az EEPROMHOZ, de nem byte-onként, hanem 512  blokkonként kezelhetőek az adatok. Pendrive-ok,  mp3 lejátszo, fényképezőgépek, telefonok.

> Buszrendszer, interfészek, tápegység, hűtés, ház: típusok, jellemzők.

Buszrendszer

Azonos feladatot ellátó vezetékcsoportok, egyes vezetékein csak két feszültségszint jelenhet meg. Vezetékek számával a busz mérete is nő.
Egy busz erén keresztül egy bitnyi információ továbbítható egyszerre. A CPU ezekkel a csatornákkal csatlakozik az operatív tárhoz és a periféria vezérlőkhöz.

Ezen CPU és buszok 3 nagy csoportja:

 - Adatbusz: Ez teszi lehetővé az adatcserét.
 - Címbusz: A címzéssel foglalkozik. (RAM)
 - Vezérlőbuszok: Számítógép működését vezérlő és összehangoló vezetékek

Interfészek(illesztőegységek)

Fizikailag és logikailag összekötik a CPU-t és a perifériákat. Típusai:

 - Soros illesztők/port: bitekénti adatátvitelre alkalmas (pl. egér illesztése)
 - Párhuzamos illesztők/port: egyszerre 8 bit átvitelére alkalmas (pl. nyomtató illesztése)

Tápegység (PSU):

A számítógép működéséhez szükséges feszültségeket állítja elő. Fajtái:

 - Külső tápegység (pl: Commodore 64)
 - AT: operációs rendszer nem tudja vezérelni
 - ATX: Az alaplap folyamatosan kap egy alacsony feszültséget, így lehetséges a szoftveres leállítása, és a külső, hardveres indítása.
 - BTX: Még nem elterjedt (?)

Hűtés:

A számítógép egyes részei (tápegység, processzor, egyéb) hőt termelnek. Hűtőberendezés szükséges az elvezetéshez. Fajtái:

 - Léghűtéses: A processzora felszerelt hűtőborda, elvonja a hőt és kivezeti a ventillátoron keresztül.
 - Vízhűtéses: A hűteni kívánt egységre vizet cirkuláló csöveket szerelnek.

Kevésbé elterjedtek:

 - Peltier hűtés: Peltier elemre kerül a  hűtő egység. Az elem az egyik oldalára vezető a hőt, a másik hideg marad
 - Hidrogénes hűtés, hőcsöves hűtés, folyékony nitrogénes hűtés

Ház:

Részegységek komplex, működő halmazát tartalmazza. Lényeges jellemzői:

 - Méret: meghajtóhelyek
 - Tápegység: (lsd. feljebb)
 - Külső csatlakozások (USB, kártyaolvasók, stb.)
 - Alaplap:közör kapcsolódási felület a számítógép egyes részegységei számára

> A perifériák jelentősége, csoportosítása (bemeneti és kimeneti eszközök). A manapság használatos perifériák besorolása az egyes csoportokba.
> A főbb perifériák bemutatása és jellemző paraméterértékei: monitor, nyomtató, háttértárak, egér, billentyűzet.

> A ma jellemzően használatos monitorfajták (CRT, LCD, TFT) és ezek működési elve. A monitorokkal kapcsolatos fogalmak: felbontás, frissítési frekvencia, képátló, képpont.
> A monitortípusok összehasonlítása a felhasználási terület szempontjából.

CRT(Cathode Ray Tube): A CRT monitorban egy katódsugárcső található, elektronágyúval az egyik végén, foszforral bevont képernyővel a másik végén.
Az elektronágyú elektronnyalábot lő ki, ezt elektromágneses térrel térítik el. Az elektronnyaláb a foszforborításba ütközik és felvillan, majd elhalványodik.
Ha elég gyorsan követik egymást az elektronnyalábok, akkor az a pont nem halványodik el.
Tehát az elektronágyúk írnak a képernyőre a számítógép utasításának megfelelően, balról jobbra, egy másodperc alatt többször is frissítve a képpontokat.
Az első monitorok egyetlen szín árnyalatait tudták megjeleníteni (monokróm): a fekete-fehér mellett a borostyán sárga és a zöld színűek is elterjedtek voltak.

LCD(Liquid Crystal Display):
Az LCD , azaz a folyadékkristályos kijelző lelke egy folyadékristály réteg, melyen polarizált fény halad keresztül.
A látható fény (nem polarizált) először áthalad egy ún. polárszűrőn, melynek következtében az polarizálódik (a fény rezgései csak egy síkban történnek).
Az ember szabad szemmel nem tudja megkülönböztetni egymástól a polarizált és a nem polarizált fényt.
A kijelzőben az immár polarizált fény áthalad a folyadékkristályt tartalmazó rétegen, melyet két elektród közé teszünk.
Az áthaladás után a polarizált fény síkja 90 fokkal elfordul a folyadékkristállyal való kölcsönhatás következtében.
Amennyiben feszültséget kapcsolunk a folyadékkristályos rétegre, akkor nem a polarizált fény síkja nem fordul el.
A különleges rétegen áthaladó polarizált fény ismét egy polárszűrőre esik, melyen csak akkor halad át, ha a fény síkja a fentire merőleges.
Ha áthalad rajta, akkor az alul elhelyezkedő tükörről visszaverődve a kijelzőn világosságot látunk.
Amennyiben a folyadékkristályos rétegre, vagy annak egy részére feszültséget kapcsolunk, a kijelzőn sötétséget észlelünk.
A folyadékkristályos réteg kiképzésétől függően számokat, betűket, rajzokat is meg lehet jeleníteni a kijelzőn.

TFT(Thin Film Transistor): Az LCD technológián alapuló TFT minden egyes képpontja egy saját tranzisztorból áll, amely aktív állapotban elő tud állítani egy világító pontot.
Az ilyen kijelzőket gyakran aktív-mátrixos LCD-nek is szokás nevezni.
Felbontás: Megadja, hogy a képernyő hány képpontból áll.(pl: Full HD:1920*1080)
Frissítési frekvencia: Megadja, hogy egy másodpercen belül hányszor frissül a képernyőn megjelenített kép.(Általánoss értékek pl.: 60Hz, 75-110Hz)
Képátló: A képernyő egyik sarkától a szemközti sarkáig terjedő távolság, hüvelykben (1 inch = 2,54 cm) mérik.
Képpont(pixel): A képpont a legkisebb megcímezhető illetve szerkeszthető alkotóeleme a képnek vagy képernyőnek.

> A ma jellemzően használatos nyomtatási technológiák jellemzői. A nyomtatók működési elve (tűs, tintasugaras, lézer). A nyomtatókkal és a nyomatással kapcsolatos fogalmak.
> A nyomtatók összehasonlítása a felhasználási területük szempontjából. A ma jellemzően használatos háttértárak. A technológiák ismertetése (mágneses elvű, optikai).
> Az egyes eszközök felépítése, működése.
> Az adatok tárolásának fizikai megvalósítása. A winchesterek üzembe helyezése, működése közben fellépő fizikai problémák, ezek megelőzése, javítási lehetőségei.

> A ma jellemzően használatos adattárolók fajtái és ezek jellemzői (CD, CD-ROM, CDR, CDRW és DVD lemezek).

Optikai tárak:speciáilis felületű műanyag korongról az olvasó egység lézersugár segítségével, fényvisszaverődés elvével olvas.

 - CD: Audió és videó anyagok tárolására, lejátszására használták.
 - CD-ROM: Hosszabb élettartam, nagyobb tárolási sűrűség, kapacitáshoz mérten alacsony ár, cserélhető és hordozható (Átlag kapacitás: 650MB)
 - CD-R: Írható lemez, íráskor lézersugár égető az adatokat jelentő lyukakat
 - CD-RW: Újraírható lemez, az adatok nem égnek be a lemezbe, kémiai változással tárolódnak az adatok
 - DVD: Nagyobb adatsűrűség; sokkal nagyobb kapacitás, már filmek és jobb minőségű mutlimédiás fájlok tárolására is alkalmas. Lehetséges a két oldalas és atöbb réteges írás. Fajtái:
   + DVD5: Egy réteg egy oldalon (kapacitás: 4,7GB)
   + DVD9: Két réteg egy oldalon (8,5GB)
   + DVD10 Egy-egy réteg két oldalon (9,4GB)
   + DVD17 Két-két réteg két oldalon (17GB)
 - Blu Ray Disc: Vörös lézerfény helyett kékkel olvas, kisebbb a hullámhossza, kisebb felületre koncentrálható; nagyobb adatsűrűség


> A számítógép részeinek és a perifériáinak fizikai karbantartása (tisztítása, szállítása, tárolása).

A gépházat időről időre éremes kitisztítani.
A ventillátor a levegővel együtt port is beszív a gépházba, ami leülepszik az alkatrészekre. Pára lecsapódhat rá, ami rövidzárlatot okozhat.
Billentyűzet, monitor és egér tisztiása saját kezűleg elvégezhető. Görgős egérnél a  mozgást érzékelő hengerekre is rá mehet a kosz.

> A (személyi) számítógépek részeinek összekapcsolása, és a számítógép üzembe helyezése. Az üzembe helyezés és biztonságos működtetés feltételei.

 - Kicsomagolás: Hűvős, párás időben kicsomagolás után várni, hogy a páracseppek megszáradjanak.
 - Csatlakoztatások: Csatlakozók a mintor és a számítógép hátoldalán. Mindent oda kell dugni, ahova erőlködés nélkül, simán belemegy ( ͡° ͜ʖ ͡°)
 - Úgy készülnek, hogy csak a hozzá tartozó foglalatba lehessen bedugni (Tűk lyukak elhelyezése, méret)
 - Tápfeszültség ellátás: A számítógépet és a monitort csatlakoztatni kell a hálózathoz (?)
 - Adatkapcsolatok: A számítógép egyes részeinek csatlakoztatása (perifériák).
   + Bekapcsolás:
   + Perifériák bekapcsolása (monitor, nyomtató)
   + Számítógép bekapcsolása a megfelelő gombbal (Power)
 - Power LED bekapcsolt állapotban végig világít, a Hard disk LED jelzi, hogy dolgozik a merevlemez.

> A hálózatok kialakításának jelentősége. A hálózatok csoportosítása kiterjedtség szerint. A hálózatok topológiája, a topológiák jellemzése.
> A hálózati kialakításhoz szükséges eszközök, ezek jellemzői (hálózati közeg, hálózati kártya, kapcsolók, útválasztók, jelerősítők).

A tárolt adatokkal folgalkozó gépek számának növekedésével felmerült a gépek közötti kapcsolat kiépítésének ötlete.
Hálózat: Számítógépek összekapcsolása az egymás közti kommunikáció, szoftver és hardver erőforrás megosztás érdekében. Háttértárak és nyomtatók megosztása költségkímélő.
Állományok megosztása, gyors információ csere lehetséges.

 - Központi gép (szerver): Ezen fut a hálózati operációs rendszer, felügyeli a hálózat működését
 - Hálózati operációs renszer: Felhasználók kezelése (nyilvántartés, bejelentkezés, stb.), biztosítja fájlok és erőforrások megosztását, kapcsolat fenttartása a külvilággal (pl. internet)
 - (rendszerre példa:Linux, Windows NT stb.)
 - Munkaállomások: Számítógépek, melyekkel a hálózat felhasználói elérik annak szolgáltatásait. Saját operáációs rendszer van rajtuk (DOS, Windows, stb.).
 - Vezetékek, szerelvények: Fizikai kapcsolat a gépek között (jelátviteli közeg)

Gépek viszonya egymással:

 - Szerver-kliens (kiszolgáló-ügyfél): A szerver szolgáltatást nyújt a kliensnek, leggyakoribb modell (pl.: honlapok).
 - Host-terminál (vendéglátó-terminál): Telefonvonallal vannak összekötve, a host az elérhető adatokat tárolja, a terminálról kérhető le az információ.
 - Peer to peer: a gépek egyenrangúak, mindegyik egyszerre szerver és munkaállomás

Csoportosísát kiterjedtség szerint:

 - LAN (Local Area Network) - kis kiterjedésű, lokális hálózat. Egyedi kábelezés, gyors adatátvitel. 1métertől néhány kilométerig terjedhet.
   + WLAN - Vezeték nélküli helyi hálózat (hordozható eszközöknél használatos)
 - MAN (Metropolitan Area Network) - városi méretű, város nagyságrendű hálózat. Települések összefogására, világhálózatok kiindlási pontjaihoz való belépés biztosításaként használatos.
 - WAN (Wide Area Network) - pár kilométertől kezdve az egész Földre kiterjedhet. Átviteli eszköz lehet telefonvonal, műhold, mikrohullám, stb. Több LAN-t és MAN-t magába foglalhat. Ilyen az internet is.

Hálózati topolóógáknak nevezzük a különböző összeköséi módokat. Topológiák és jellemzésük:

 - Sín: A gépeket egy főkábel segítségével kötjük össze. Ehhez kapcsolodnak az egyes gépek. Koax kábel esetén ügyeljünk a mindkét oldali lezárásra.
 - Gyűrű: Hasonló a sín topológiához, a sín két végpontja össze van kötve.
 - Csillag: A gépek egyénileg csatlakoznak egy központi egységhez. Egy gép megsérülése esetén csak a többi nem esik ki a kommunikációból.
 - Fa: Hasonló a csillag topológiához, egy hálózat több csomópontból álló ágat is tartalmazhat. (pl. Iskolákban)
 - Teljes Hálózat: Minden eszköz csatlakozik minden eszközhöz. Ez a legbiztonságosabb elrendezés. Csak véges számú eszköz lehet tagja, többet nehéz kivitelezni fizikailag és gazdasági szempontból.
 - Celluláris hálózat: Vezeték nélküli eszközök (pl: mobil) használják.

A hálózati kialakításhoz szükséges eszközök, ezek jellemzői (hálózati közeg, hálózati kártya, kapcsolók, útválasztók, jelerősítők). Hardver feltételek:

 - Számítógépek: Legalább kettő, az egyik kiszolgáló, munkaállomásként ez ritkán használható. A többi gép a munkaállomás.
 - Hálózati kártya: A hálózatra való kapcsolódásért és azon keresztül történő kommunikációért felelős. 10-100Mbites a megszokott. Lehetséges csatlakozófelület a PCI, USB és PCMIA.
 - Szabvány szerint készülnek, mindegyik tud mindegyikkel kommunikálni, driver szükséges.
 - Vezeték: Átvivő közeg elemei:
   + Koaxiális kábel: középen tömör rézhuzal, szigetelőréteg veszi körül, amin pedig árnyékolás található. Képes alap- és szélessávú átvitelre.
     T elosztóval vagy vámpír csatlakozóval történik a megcsapolás(?).
     Jó, mert nagy szávsélesség, nagy távolság, zajérzéketlenség, azonban lehallgatható, sérülékeny kiépítés, nehézkés szerelhetőség. Telepítése és karbanttartása szaktudást igényel
   + Sodort érpár: Két szigetelt, egymással összecsavart rézhuzal. Lehet árnyékolt és árnyékolatlan (STP és UTP).
     Jó mert könnyen szerelhető, felépíthető és bővíthető, de zajérzékeny, limitált sávszélesség valamint lehallgatható.
   + Optikai kábel: Üvegszálban haladó fénysugár megléte vagy hiánya hordozza az információt. A fény visszaverődik a szálon belül, nem "szökhet" ki.
     Jó mert érzéketlen az elektromágneses zavarokra, nagy sávszélesség, erősítés nélkül is nagy távra vihető, nem hallgatható le, de drága, nehéz javítani.
   + Infravörös, lézer, mikrohullámú, rádióhullámú és műhöldas átvitel: Speciális igények kielégítésére szolgáló megoldások (távirányító, TV csatornák, stb.)
   + Struktúrált kábelezés: Univerzális, a különböző kábelezési előírásokra is megfelel.
 - Csatlakozók:(üres?)
 - Aktív eszközök (hub, switch) - útvonalválasztók
   + aktív "HUB", telefonközpont, médiakonverter a központi egységben. Ezek manapság egy központi szerkénybe kerülnek, bővíthetőek.
   + Repeater: jelerősítő, újradigitalizálja a jeleket útközben, adat torzulása ellen véd
   + Bridge: hálózati szegmensek közti elválasztás, ellenőrzi a CRC értéket
   + Router: bridge+útvonalválasztás, különböző típusú hálózatok összekötése
   + Gateway: Protokoll átalakító
   + Modem - analóg csatornán való lassú üzenettovábbítás
   + switch: A csomagokat csak a kiindulási és a beérkezési állomás között továbbítja (nem küldi szét mindenhova az adatokat). Kevésbé terhelődik mint a hub.

Szoftver feltételek:

 - Egyenrangú hálózatnál a kapcsolatban álló gépek kliensként és szerverként is működnek, az operációs rendszerbe be vannak építve a szükséges szolgáltatásaok.
 - Kliens-szerver hálózatoknál a szerveren hálózati operációs rendszer szükséges (pl. Win XP, Linux) a kiszolgálóra, hogy teljesíthetőek legyenek a kliens kérései.
   A kliensen tetszőleges rendszer futhat.

> A matematikai logika szerepe az informatikában. A logikai alapműveletek és azok alkalmazása különböző feladatok megoldása során. Igazságtáblák (ÉS, VAGY, NEM, Kizáró VAGY).
> Logikai kifejezések kiértékelése, egyenértékűsége, tagadása.
