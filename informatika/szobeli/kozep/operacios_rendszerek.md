Mindenek előtt definiálnunk kell az operációs rendszer fogalmát.

Operációs rendszernek nevezzük a számítógépeknek azt az alapprogramját, ami közvetlenül kezeli a hardvert és egységes környezetet biztosít a futtatandó alkalmazásoknak. (pl. szövegszerkesztők, játékok).

Majd beszélnünk kell az operációs rendszerek feladatiról.

1.	Feladatai:
- A perifériák tesztelése, a gépi erőforrások kezelése
- Programok indítása, működtetése
- A gépi erőforrás-megosztás a futó programok között
- Adatok kezelése
- Programok és adatok biztonságos megőrzése
- A működési zavarok jelzése
- Párbeszédes kapcsolattartás a gép kezelőjével

Ezek után csoportosítanunk kell az operéciós rendszereket (felület, felhasználók száma, processzor idejének kihasználása).

- Kezelői felület szerint:
o	Szöveges (MS DOS, UNIX)
o	Grafikus (Windows 95, Windows NT, OS/2)
- A felhasználók száma szerint:
o	Egy felhasználós (DOS, WIN 9x)
o	Több felhasználós (LINUX, UNIX)
- Processzorkezelés szerint:
o	Egy feladatos (DOS)
o	Több feladatos (WIN 9X, WIN NT, UNIX)
- Elterjedtebbek:
o	Microsoft Windows, Linux, Mac OS, Mac OS X


Állományokról és könyvtárszerkezetről is essen pár szó.

A számítógépes munka során háttértárolókat kezelünk, amin partíciók vannak. Egy-egy partíción több ezer állományt tárolnak. A partíciót az áttekinthető felhasználás érdekében mappákra osztjuk. Mappa minden operációs rendszerben van. Minden rendszerre jellemző, hogy a valamilyen szempont szerint összetartozó fájlok kerülnek egy mappába. A mappaszerkezet hierarchikus, azaz egy mappában nemcsak állományok, de újabb mappák is lehetnek.

Könyvtárak és állományok műveletei általánosságban.
Könyvtár:

- Mappa: Az adathordozókon tárolt fájlok rendezett
halmaza, amiket a számítógépes katalógus tárol.
- Neve: A kis- és nagybetűket a Windows-rendszer nem
különbözteti meg, a Linux-rendszer – mint az operációs
rendszerek viszont igen.
- Gyökérkönyvtár: Formázás során
keletkezik. Ebben a mappában található meg az összes mappa és állomány. Neve kötött, a Windows rendszerben vissza per jel.
- Aktuális katalógus: A lemez- és állományműveletek
egyszerűbbé tételéhez az operációs rendszer feltételezi, hogy a katalógusszerkezet egyik eleme kitüntetett szerepet tölt be: a műveletek ebben értelmezettek. Ez az aktuális katalógus. A katalógusműveletek egyikével lehet ezt változtatni, a kérdéses meghajtóval végzett munka legelső lépésekkor az azon levő katalógusszerkezet alapkatalógusa az aktuális katalógus. A Linux-rendszerben ilyen fogalom nincs.
- Alkatalógus: A bármely katalógusból nyíló katalógus az
adott mappában: ez az alkatalógus.
- Szülőkatalógus: Az a katalógus, amelyből a fenti mint
alkatalógus nyílik. A katalógusszerkezetben az alapkatalógus kivételével minden katalógusnak van szülőkatalógusa.

1.	Következő műveleteket végezhetünk mappákkal:

- Készítés: Új mappa jön létre, ez a meglévő
mappaszerkezethez az aktuális katalógusból kapcsolódik. A FÁJL -> Új -> Mappa elemével lehet létrehozni.
Valamennyi rendszerben közös, hogy a mappa neve az adott almappában egyéni legyen.
- Átnevezés: Létező mappa nevének megváltoztatása csak
akkor lehetséges, ha a célnév nem foglalt.
A FÁJL -> Átnevezés paranccsal lehet megváltoztatni a mappanevet.
- Törlés: Fejletlenebb rendszerekben a mappatörlés előtt ki
kellett törölni a mappának a tartalmát is. Windows-rendszerekben a törlést a DEL gombbal végezhetjük, vagy Jobb egérgomb -> Törlés
- A mappa listázása, megjelenítése: A mappaablak
fejlécében lehet a megjelenítés módját megválasztani.

2. Fontosabb WINDOWS mappák
- Windows: Idekerülnek be a windows telepítése során
minden operációs rendszerrel kapcsolatos fájlok és mappák. Itt találhatók a számítógép hardverelemeinek a driverei. Ezen kívül még itt található a súgó és több windows alkalmazás is.
- Program Files: az operációs rendszer alá telepített
programokat találhatjuk itt.
- Documents and Settings: ebben a mappában találhatóak
meg a számítógép felhasználóinak fájlai, dokumentumai és beállításai. Minden felhasználónak saját Dokumentum mappája van, melyben megtalálható a Képek, Zene és Videók mappa is.






Állomány:
- Állomány fogalma: A számítógépen lévő információ
tárolási egysége a  fájl. Más megfogalmazás szerint a logikailag összefüggő adatok halmazát nevezhetjük állománynak.
- A fájl: A háttértárolón egységen tárolt, névvel és
kiterjesztéssel azonosított adat együttes.
Jellemzői: név, kiterjesztés, méret, dátum…
- Fájl (állomány) kezelési műveletek:
<table border= "4">
<tr><td>FILEMŰVELET</td><td>	WINDOWS INTÉZŐ</td></tr>
<tr><td>megnyitás, futtatás</td><td>	Fájl ikonján duplakattintás az egér bal gombjával</td></tr>
<tr><td>keresés</td><td>	Start/keresés vagy aktuális ablak Keresés gomb az eszköztárban</td></tr>
<tr><td>mozgatás</td><td>	Egér balgombbal áthúzás a célhelyre vagyJobb gomb/Kivágás és a célhelyen Jobb gomb/Beillesztés</td></tr>
<tr><td>másolás</td><td>	Fájl/Küldés vagy Ctrl gomb+egér balgombbal áthúzás a célhelyre vagy Jobb gomb/Másolás és a célhelyen Jobb gomb/Beillesztés</td></tr>
<tr><td>átnevezés</td><td>	Fájl/Átnevezés vagy Jobb gomb/Átnevezés vagy Két lassú kattintás a néven/új név beírása</td></tr>
<tr><td>törlés</td><td>	Fájl/Törlés vagy Egér jobb gomb/Törlés vagy Delete gomb a billentyűzeten</td></tr>
<tr><td>visszaállítás</td><td>	Szerkesztés/Visszavonás vagy Lomtár/Fájl visszaállítása</td></tr>
<tr><td>jellemző beállítása</td><td> Fájl/Tulajdonságok vagy Jobb gomb/ Tulajdonság</td></tr>
<tr><td>szöveges állomány létrehozása</td><td>	Fájl/Új/Szöveges dokumentum</td></tr>
<tr><td>nyomtatás</td><td> Fájl/Nyomtatás vagy Egér jobb gomb/Nyomtatás</td></tr>
<tr><td>mentés</td><td>	Fájl/Mentés az aktuális dokumentum ablakban</td></tr>
</table>

3. Kiterjesztési típusai:
- ASCII-be kódolt állományok (.UUE, Base64, BTOA, .BOO, .HQX);
- szalagarchívumok (.tar);
- tömörített állományok (.Z, .zip, .arj, SFX .exe, .gz, .sit);
- futtatható programok(.exe)
- szövegek, dokumentumok (.RTF, .PS, .EPS, TEX, .HTM/.HTML, .PDF);
- képek (.GIF, .JPG/.JPEG, .PNG);
- hangok és zenék (.VOC, .VAW, .AU, .AIF/.AIFF, .AIFC, MIDI, .MPA, .MPA2, MP3, .RA/.RAM);
- animációk (.DL, .GL, .FLI, .FLC);
- filmek es videók (.MPEG/.MPG, .AVI, .QT/.MOV);
- virtuális valóság (VRML/.WRL).
