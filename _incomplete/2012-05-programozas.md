A kapott forrásfájl valahogy így néz ki:

    1 7 14
    3 3 10
    1 1 3
    1 2 3

Első lépésként importáljuk a *csv* modult, amely jelentősen megkönnyíti
a dolgunkat a beolvasásnál.

    import csv

Ezután definiálunk két függvényt, az első csupán arra szolgál, hogy a feladatok
sorszámait egyszerűbben írhassuk ki,
a második viszont visszaadja a megkapott összegeket a távolság függvényében.

    def _(x):
      print('\n\n{}. feladat\n'.format(x))

    def fizetes(x):
      if x < 3:
        return 500
      elif x < 6:
        return 700
      elif x < 11:
        return 900
      elif x < 21:
        return 1400
      else:
        return 2000

Most következik a fájl beolvasása. Ehhez a *csv* modul *reader* függvényét
használjuk, amely egy listába menti el a fájl sorait, amelyeken belül
további allistákat hozhat létre attól függően, hogy mit adtunk meg delimiter
paraméternek, illetve hogy milyen szerkezetű a forrásfájlunk.

Ebben az esetben a fájlunkban szóközökkel vannak elválasztva az adatok, ezért
a *reader* függvény egy olyan listát fog létrehozni, amely annyi elemű, ahány
soros a fájlunk, és minden egyes eleme egy újabb lista, amelyben az egy sorban
található számok szerepelnek egymás után.

A *reader* által visszaadott objektummal azonban nem tudunk rendesen dolgozni,
mert miután kiolvasunk belőle egy adatot, az eltűnik belőle.
Ezért a tartalmát átmásoljuk a fuvarok listába (ami tehát ugyanígy listák
listája lesz), majd ezt még rendezzük (alapértelmezés szerint az első érték,
azaz a nap sorszáma alapján).

    fajl = csv.reader(open('tavok.txt'), delimiter = ' ')

    fuvarok = [[int(adat) for adat in sor] for sor in fajl]

    fuvarok.sort()

Az így kapott adatszerkezettel rendkívül egyszerű dolgozni, az első két feladat
megoldható egy-egy rövid *print()* utasítással. A legelső fuvar a rendezés után a
listánk legelején, azaz a 0. pozícióban fog elhelyezkedni, ennek a sornak kell
a kilométer értékét kiírnunk, ami pedig a harmadik adat, azaz a második sorszámú
elem.

    _(2)

    print(fuvarok[0][2], 'km')

A következő feladat megoldása szinte ugyanez, csak itt a legutóbbi fuvar hosszát
kérdezik, ezért a lista legutolsó elemére van szükségünk, amit legegyszerűbben
úgy kaphatunk meg, hogy a -1. elemére hivatkozunk (úgy képzelhető el, mintha
hátulról számoznánk a listát -- hasonlóan működik a -2, -3, ... index is).

    _(3)

    print(fuvarok[-1][2], 'km')

Ahhoz, hogy meghatározzuk, melyik napokon nem dolgozott a futár, először
létrehozunk egy halmazt, amely az összes nap sorszámát tartalmazza (1-7-ig),
majd ebből a halmazból kivonjuk azt a halmazt, amely azoknak a napoknak a
sorszámait tartalmazza, amelyeken dolgozott.

    _(4)

    napok = set(range(1, 8))
    dolgozottNapok = set()

    for fuvar in fuvarok:
      if fuvar[0] not in dolgozottNapok:
        dolgozottNapok.add(fuvar[0])

    szabadnapok = napok - dolgozottNapok

    print('A következő napokon nem dolgozott a futár: ', szabadnapok)

Úgy kapjuk meg a legtöbb fuvar napját, hogy egyesével az összes napra eltároljuk
a fuvarok mennyiségét, majd ezek közül kiválasztjuk a legnagyobbat.

Az egyszerűség kedvéért ezt egy nyolcelemű listában tároljuk, melynek a 0. eleme
végig változatlan marad, és nem is törődünk vele, csak az 1-7-ig tartó sorszámok
lesznek fontosak.

Végigiterálunk az összes fuvaron, és a megfelelő sorszámú mezőhöz minden esetben
hozzáadunk egyet, majd miután a ciklus végigfutott, kiírjuk a legnagyobb elemhez
tartozó sorszámot.

    _(5)

    fuvarokSzama = [0]*8

    for fuvar in fuvarok:
      fuvarokSzama[fuvar[0]] += 1

    print('A legtöbb fuvar a(z) {}. napon volt'.format(fuvarokSzama.index(max(fuvarokSzama))))

Hasonlóan az előző feladathoz, egy nyolcelemű listában összegezzük az egyes
napokra eső fuvarok hosszát, majd az összes naphoz (tehát a nulladik sorszámot
nem vesszük figyelembe) tartozó számot kiírjuk.

    _(6)

    napiKm = [0]*8

    for fuvar in fuvarok:
      napiKm[fuvar[0]] += fuvar[2]

    for nap in range(1, 8):
      print('{}. nap: {} km'.format(nap, napiKm[nap]))

Innentől kezdve mindegyik feladatban használni fogjuk a program legelején
elkészített *fizetes()* függvényt. Ha látjuk, hogy több feladat is hasonló
válaszokat vár, de legalább is részfeladatokban egyeznek, akkor érdemes lehet
függvényt írni, ezzel nem csak a kódunk lesz áttekinthetőbb, de sokszor a
megírásra fordítandó idő is a töredékére csökken.

Ahhoz, hogy a függvényt a beolvasott adatra alkalmazni tudjuk, először egész
számmá kell azt alakítani, a python eredetileg szövegként olvassa be.

    _(7)

    tavolsag = input('Adjon meg egy tetszőleges távolságot (km-ben): ')

    print('Az ezért járó díjazás {} Ft'.format(fizetes(int(tavolsag))))

A fájlba íráskor is hasznos lesz a függvényünk, az összes fuvarra vonatkozóan ki
kell írnunk a fuvar díját.

Fontos észben tartani, hogy míg a *print()* alapértelmezés szerint sortöréssel
zárja a kiíratást, fájlba írás esetén (legalábbis a file.*write* funkció
használatakor) nekünk kell a sorok végére írnunk a *\n*-t, azaz a sortörést.

    _(8)

    f = open('dijazas.txt', 'w')

    for fuvar in fuvarok:
      f.write('{}. nap {}. út: {} Ft\n'.format(fuvar[0], fuvar[1], fizetes(fuvar[2])))

    f.close()

Az utolsó feladatban is csupán a függvényünket kell az összes fuvarra
alkalmazni, és a kapott értékeket összeadni.

    _(9)

    ossz = 0

    for fuvar in fuvarok:
      ossz += fizetes(fuvar[2])

    print('A futár heti keresete {} Ft'.format(ossz))
