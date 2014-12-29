> Az operációs rendszer fogalma, feladata, fajtái. Az operációs rendszer működési struktúrája (rendszermag, indítófájl, külső és belső parancsok rendszere, opcionális kiegészítések).
> Az operációs rendszer feladatából következő jellemző működési területek (memóriakezelés, folyamatvezérlés, megszakítás-kezelés, kommunikáció a perifériákkal).
> Több feladat párhuzamos végzésének szervezése. Az operációs rendszer telepítése.

Operációs rendszer (operating system): Olyan program , mely betölti és vezérli a számítógépen futó programokat, alkalmazásokat, elosztja, ütemezi az erőforrásokat, kezeli a hardvert, biztosítja a felhasználó és a számítógép közötti kommunikációt.

Az operációs rendszer feladatai:

 - A kernel feladatai:
   + Programok, folyamatok futásának kezelése
   + Indítás, futási feltételek biztosítása, leállítás
   + Memória-hozzáférés biztosítása
   + Processzor idejének elosztása
   + Virtuális gép mutatása a nemkívánt taszkok felé (pontosabban a hardver által biztosított lehetőségek szoftver-kiegészítései)
   + Háttértárolók kezelése
   + Rendszerhívások kiszolgálása
   + Fájlrendszer
 - A shell feladatai
   + Kapcsolattartás a felhasználóval (felhasználói felület)
   + Alkalmazások futásának kezelése (indítás, futási feltételek biztosítása, PIT leállítás)

Az operációs rendszerek csoportosítása:

 - Felhasználók száma szerint:
   + Egy felhasználós: Mobiltelefonok operációs rendszerei
   + Több felhasználós: Windows, OSX, Linux
 - Párhuzamosan futtatható programok, folyamatok száma szerint:
   + Monoprogramozott(egyfeladatos): MS-DOS
   + Multiprogramozott(többfeladatos):Windows XP
 - Felhasználói felület szerint:
   + Karakteres (CLI: Command Line Interface): MS-DOS, UNIX
   + Grafikus (GUI: Graphic User Interface):    OSX, Windows
 - Jogállás szerint:
   + Nyílt forráskódú: Linux
   + Zárt forráskódú: OSX, Windows
 - Cél szerint:
   + Univerzális: OSX, Windows, Linux
   + Speciális: mosógép,mp3-player operációs rendszere
 - Sínrendszer szerint(Hány bites)
   + 16 bites: MS-DOS
   + 32 bites: Windows XP
   + 64 bites: OSX, Windows 7

Az operációs rendszer működési struktúrája:
Az operációs rendszer két fő részből áll, kernelből és shellből. A kettő közti kapcsolatot a programozási interfészek látják el.

 - Kernel(rendszermag):
   + Végzi a hardver irányítását
   + Párhuzamosan futtatja a programokat, és meghatározza a futó programok,folyamatok processzoridejét
   + Megakadályozza, hogy a felhasználó közvetlenül elérhesse a hardvert
   + Rendszerhívások segítségével érhető el, a programok így utasítják a műveletek végrehajtására.
   + A kernel fontos részei az eszközkezelők (driverek), a fájlrendszervezérlők ,a hálózat-, processzor-, memóriakezelés, stb. programjai
 - Shell(parancsértelmező):
   + Feladata a kapcsolattartás a felhasználóval, a felhasználó által adott parancsok átkonvertálása a kernel által értelmezhető rendszerhívásokká
   + Biztosítja a programok számára a futási feltételeket

> Az operációs rendszer betöltődésének folyamata. A számítógép kikapcsolásának módjai, az operációs rendszer feladatai a kikapcsolás során.
> Az operációs rendszerek tipikus hibaüzenetei, hibajelenségei, ezek elhárítási módja.

> Hardver eszközök üzembe helyezése, beállítása (konfigurálása), eltávolítása.

> A szoftverek telepítése, beállítása, eltávolítása. Szoftverek futtatása és leállítása, memória felszabadításának kérdései.

> Az operációs rendszerek által használt állományszervezési, -nyilvántartási módszerek.
> A lemezkezelés és a leggyakrabban használt operációs rendszerek fájlrendszerének ismerete, legfontosabb tulajdonságai (pl.: FAT, FAT32, NTFS, EXT stb.).

> A könyvtárszerkezet felépítésének ismerete. A könyvtárakról tárolt tulajdonságok. A könyvtárműveletek: létrehozás, törlés, másolás, áthelyezés, átnevezés, listázás, könyvtárváltás.

> Az állományok típusai. Az állományok elnevezésének formai követelményei, rendszerfüggő szintaktikai megkötések. Az állományokról tárolt tulajdonságok. Az állományok társítása.
> Az állományok fizikai tárolásának szervezése. Az elérési útvonal megadásának formái.

> Az állományokkal végzett műveletek ismerete (létrehozás, másolás, áthelyezés, törlés, mentés, nyomtatás, megnyitás). Az állományokkal végzett műveletek fizikai megvalósítása.
> Keresés háttértárakon, a keresési feltételek (helyettesítő karakterek használata). A parancsok paraméterezett futtatása. A kapcsolók és a paraméterek szerepe, néhány példa > használatukra.

> A háttértárak karbantartása (formázás, partícionálás, töredezettség-mentesítés), a karbantartás fontossága.

> A tömörítés lényege és elve. Tömörítési módszerek (veszteséges és veszteségmentes). A kép, a hang, a video és egyéb állományok tömörítésének jellemzői.
> Általános tömörítő programok működésének ismerete. Az állományok és a könyvtárak tömörítésének és kicsomagolásának megvalósítása.
> Az önkicsomagoló, méretre darabolt, védett állományok létrehozása, kibontása. Egy állomány hozzáfűzése létező tömörített állományhoz.

> Az operációs rendszerek segédprogramjai (fájlkezelés, archiválás, vírusvédelem, tűzfal, multimédia stb.). A segédprogramok létjogosultsága, szolgáltatásai, jellemzői.
> Néhány segédprogram bemutatása.

> Vírusirtó program használatának ismerete. Vírusellenőrzés a háttértárakon és a memóriában.

> A vírusvédelem kialakítása a számítógépen. Aktív vírusvédelem. A vírusvédelem gyenge pontjai, hiányosságai (pl. emberi tényező).

> A számítógépes hálózatok működéséhez szükséges szoftverek. A szerver operációs rendszerének jellemző többletfunkciói.
> A hálózati kommunikáció logikai felépítése (a szerver-kliens és az egyenrangú hálózatok). A helyi hálózatokhoz kapcsolódás feltételei és megvalósítása.
> A hálózati szolgáltatások elérésének módjai, az eszközhasználat feltételei. A felhasználók azonosítása, jogosultságok kezelése.
