mi az állomány?

miért van szükség könyvtárakra? pc, 80-as évek eleje, hajlékonylemeznek nevezett mágneses adathordozó (floppy) 160-360 KB-os kapacitással, pl 1-2 KB-os szöveges állományból elfér legfeljebb néhány száz db: ez még áttekinthető, lehet minden ‬„egy kupacban”

merevlemezek: ugyancsak a pc-korszak kezdetén 10-20-30 MB, ma 1 TB: öt nagyságrend, az állományok száma is három-négy nagyságrenddel nő [miért nem öt nagyságrendet írtam?], százezer-egymillió állomány egy adathordozón: rendszerezni kell

(eredetileg) fához hasonló szerkezet: könyvtárak (mappák); gyökérkönyvtár és alkönyvtárak

#### állományrendszerek (file system, fs)

mágneses adathordozón (hajlékonylemezen, merevlemezen), optikai tárolón (cd-n, dvd-n), elektronikus eszközökön (pendrive-on) sokféle formában tárolhatók az adatok (az állományok és a rendszerezésükre szolgáló könyvtárak, a továbbiakban ezeket együtt is nevezzük állománynak)

az állományrendszer a felhasználó elől rejtve van, általában nem sok ismerete van róla, de sok teendő értő elvégzéséhez, sok jelenség magyarázatához, sok korlátozás megértéséhez érdemes lehet néhány dolgot tudnia

természetesnek tartjuk, hogy minden állománynak van neve, nem ritkán elolvassuk a méretére vonatkozó információt, esetleg a hozzárendelt dátumot [mire utal ez?], de az idő múlásával (az operációs rendszer összetettebbé válásával, a háttértárak kapacitásának növekedésével) egyre több és többféle adat szól magukról az adatokról (nevezhetjük ezeket metaadatoknak), így válnak egyre bonyolultabbá a filerendszerek is

### néhány kiragadott példa (csak a pc történetére szorítkozva)

- elképzelhető állományrendszer könyvtárak nélkül (ilyen volt a dos 1.0)

- könyvtárszerkezet a unix mintájára a dos 2.0-s változatától

- dos alatt egyszerű filerendszer (file allocation table: fat) mindössze 8+3-as állománynevekkel (a mai napig gyakori a háromkarakteres kiterjesztés; csak ennek a korlátnak köszönhető a jpeg/jpg kettősség)

- a dos egyfelhasználós rendszer: nincsenek jogosultságok (nincs rájuk szükség)

- a windows megjelenésével a fastruktúra hamar bonyolódik: ismét csak a unix mintájára linkek (parancsikonok)

- a windows többfelhasználós rendszer: tárolni kell a felhasználók állományokhoz, könyvtárakhoz fűződő jogosultságait (melyik felhasználó mit tehet az adatokkal: olvasás, módosítás, törlés stb) – ez önmagában elég ok a fat fs elvetéséhez, helyette ntfs (new technology fs a 90-es évek második felétől)

- létezik más állományrendszer a pc-ken is: például a a linuxok jellegzetes állományrendszere az extended fs (ext2, ext3, ext4)

### kitekintés (ismét csak kiragadott példákkal)

- van állományrendszer, ahol az állományoknak több verziójuk lehet (a Digital Equipment Corporation VAX gépeinek VMS nevű operációs rendszere): *jegyzet.txt;1* az eredeti, *jegyzet.txt;17* a tizenhetedik [mire utalhat a *jegyzet.txt;-1* ?]

- a Macintosh gépeinek felhasználóbarát működéséhez nagyban hozzájárul a bonyolult (sokféle metaadatot tároló) filerendszer (ez éppúgy érvényes a legrégebbi Apple gépekre, mint az OS X-et futtató maiakra)

### korlátozások

említettük már: látszólag az operációs rendszertől (valójában az általa használt a állományrendszertől) függnek az állományok, könyvtárak elnevezésére vonatkozó szabályok

hagyományosan két rész: név és kiterjesztés; utóbbi utal a tartalomra, illetve annak formájára (kép, ezen belül pl bmp, png, jpg stb), ezzel szoros összefüggésben arra, hogy milyen alkalmazásokkal lehet ezekhez hozzáférni

kerülendő:
- szóköz (körülményes a használata például a parancssorban)
- írásjelek (némelyiknek fenntartott szerepe van [melyeknek?], mások használata nehézkes a parancssorban)
- ékezetes betűk (különböző operációs rendszerekben, különbző filerendszerekben másként jelenhetnek meg)
- nagybetűk (unix/linux megkülönbözteti a kisbetűktől, dos/windows nem különbözteti meg)

### jogosultságok

állományok esetén például
- olvasás
- írás
- futtatás

könyvtárak esetén például
- olvasás (azaz listázás)
- írás (azaz tartalom módosítása) [mit jelenthet ez?]
- belépés

#### állomány- és könyvtárműveletek

könyvtárak esetén például
- létrehozás
- törlés
- átnevezés/mozgatás [miért említhetjük ezeket együtt? és mikor van lényeges különbség a kettő között?]
- másolás
- belépés

állományok esetén például
- létrehozás
- törlés
- átnevezés/mozgatás
- másolás
- megnyitás (olvasásra vagy írásra, azaz megtekintésre vagy szerkesztésre)

[a fenti műveletek közül melyeket végezhetjük el az operációs rendszerrel? a többit miért nem?]

### hogyan végezhetjük ezeket a műveleteket?

három korszak, három megközelítésmód (részletesebben másik tételben):
1. parancssor (mkdir/md, rmdir/rd, illetve rm/del, mv/move, cp/copy, cd/cd)
2. szöveges keretrendszer (norton commander az ős; midnight commander; free commander, total commander)
3. grafikus felületen

### speciális feladatok

nem ritkán szükséges törölt állomány (gyakran véletlenül törölt állomány) helyreállítása:
- lehetővé tehetné a filrendszer (nem ez a jellemző)
- speciális könyvtár (kuka, lomtár, trashbin stb)
- trükközés: hátha nem írtunk még a törölt adatok helyére

karbantartás: például töredezettségmentesítés [miért van erre szükség?]
