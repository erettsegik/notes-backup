Mindenekelőtt definiálnunk kell az operációs rendszer fogalmát: operációs rendszernek nevezzük a számítógépeknek azt az alapprogramját, ami közvetlenül kezeli a hardvert és egységes környezetet biztosít a futtatandó alkalmazásoknak (például egy szövegszerkesztőnek éppen úgy, mint egy játékprogramnak).

Beszélnünk kell az operációs rendszerek alapvető feladatairól is.

### Az operációs rendszer fontos feladatai
- a perifériák tesztelése, a gép erőforrásainak kezelése
- a programok indítása és működtetése
- a gép erőforrásainak megosztása a futó programok között [milyen erőforrásokat kell megosztani?]
- az adatok kezelése
- az adatok (ezen belül a programok) biztonságos megőrzése
- a működési zavarok jelzése
- kapcsolattartás a gép felhasználójával

### Csoportosítás a felhasználók és a feladatok száma szerint

Ezek után csoportosítanunk kell az operációs rendszereket; erre több lehetőségünk is van. Fontos szempont például a felhasználók száma, a processzor idejének kihasználása vagy a kapcsolattartás módja a felhasználóval.

- a felhasználók száma szerint:
  - többfelhasználós például
    - a nagyszámítógépeken futó vms
    - a unix és annak késői utódai, a sokféle linux-változat
  - egyfelhasználós például
    - a dos és a korai windows-változatok (a windows 95-ig)

- processzorkezelés szerint:
  - többfeladatos például
    - a unix és leszármazottai
    - a windows 95-től kezdve a windows-változatok
  - egyfeladatos például
    - a dos és a legelső windows-változatok

A mai felhasználó számára furcsa lehet, de az informatika korai időszakában a többfelhasználós rendszer volt természetes. Ez azonban érthető, ha figyelembe vesszük a korabeli gépek akár millió dolláros árát: természetes, hogy egy ilyen drága géppel nem csak egy ember dolgozott. Abban az időben az volt a természetes használati mód, hogy a felhasználók terminálokon (lényegében egy billentyűzettel és egy monitorral) csatlakoztak a számítógéphez (ez nem keverendő össze azzal, amikor önálló működésű számítógépeket hálózatba kötünk). Ezt az üzemmódot a mai felhasználók többsége nem is ismeri, de érdemes megemlíteni, hogy az iskola két termében éppen ez a meghatározó (azzal a nem lényegtelen különbséggel, hogy ezek grafikus terminálok: a korabeli szöveges üzemmódtól eltérően itt grafikus módú a távoli számítógép operációs rendszere, ennek megfelelően a billentyűzet és a képernyő mellé egér is társul).

Az egyfelhasználós rendszer a személyi számítógép megjelenésével vált széles körben elterjedtté: ahogyan az elnevezése is mutatja, a pc-t (illetve annak korai operációs rendszereit) egy ember használatára tervezték; a korabeli technológia és árak mellett nem is tudtak volna néhány ezer dollárért olyan gépet előállítani, amely egyidejűleg több ember munkáját segíthette volna.

Ugyancsak ezeknek a korai gépeknek a technológia korlatai miatt a korai pc-k (illetve operációs rendszereik esetében) kizárólagos volt az egyfeladatos üzemmód: sem a gép teljesítménye, sem a szöveges módú operációs rendszer nem tette lehetővé, hogy a felhasználó ablakok között váltogatva több programot futtathasson.

A személyi használatú pc-n tehát szoros összefüggést figyelhetünk meg a többfeladatosság és a grafikus üzemmód között. Ez a nagyszámítógépeken vagy akár a kiszolgálóként használt pc-ken nem így van: ezeken szöveges üzemmódban is természetes a többfeladatos üzemmód. Azt például könnyű elképzelni, hogy megfelelő billentyűkombinációkkal váltogathatunk egy monitoron több, szöveges módú terminálként működő (virtuális, azaz látszólagos) képernyő között, de a valóságban sokszor erre sincs szükség a többfeladatos működéshez, elegendő például egymás után elindítani az adatbáziskezelő és a webkiszolgáló programot, és máris többfeladatos rendszert látunk.

Amint tudjuk, mára a pc-ken is természetessé vált a többfeladatos operációs rendszer.

A fentiekben szóba került
  - egyfelhasználós és egyfelhasználós rendszer (ilyen a dos és a legelső windows-változatok)
  - egyfelhasználós és többfeladatos rendszer (ilyen a windows 95)
  - többfelhasználós és többfeladatos rendszer (ilyenek a linuxok)

Bizonyos értelemben ezzel kimerítettük a lehetőségeket, hiszen ha a géppel több felhaszáló dolgozik, akkor természetes, hogy azon több feladat is fut; ha nagyon kell, akkor többfelhasználós, de egyfeladatos rendszerként szokták a hálózati operációs rendszereket emlegetni.

### Csoportosítás a felhasználóval való kapcsolattartás módja szerint

Ahogyan említettük, az informatika első néhány évtizedében kizárólagos volt a szöveges üzemmód, a parancssoros működés: így működtek a klasszikus nagyszámítógépek, majd az első időszakban a személyi számítógépek is. Ekkor az operációs rendszer feladatainak végrehajtatásához, a programok indításához is parancsokat kellett kiadni, majd a képernyőre kiírt válaszüzenetekből lehetett tájékozódni az eredményekről (illetve az esetleg felmerült hibákról).

A pc elterjedésével egyre kevésbé volt fenntartható ez a kapcsolattartási forma. Érdemes megemlékezni az ekkor megszülető szöveges keretrendszerekről, mindenekelőtt ezek alighanem leghíresebb képviselőjéről, a dos alatt futó norton commanderről: ez még szöveges módban, de már rendkívül szemléletesen és kényelmesen biztosította (például) az alapvető állomány- és könyvtárműveletek elvégzését. Késői utódai lényegében változatlan megközelítéssel, megegyező billentűkombinációkkal (de természetesen sok új szolgáltatással) végzik a legfontosabb műveleteket (linux alatt ilyen a midnight commander, windows alatt a free commander vagy a total commander).

Gyökeres változást azonban a grafikus felhasználói felületek megjelenése hozott, amelyeknek első –és mai napig legismertebb– képviselői az Apple/Macintosh gépek, illetve a windows operációs rendszert futtató személyi számítógépek. Forradalmian új volt ezekben az egér használata és az ablakok megjelenése (nem véletlenül adta ez windows nevét).  

Összefoglalva tehát
- kezelői felület szerint
  - szöveges üzemmódú például
     - a dos
     - az eredeti unix
  - grafikus üzemmódú például
     - az os/2
     - minden windows
     - minden Apple/Macintosh
