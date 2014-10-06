> Az analóg és a digitális jel fogalma, példák felhasználásukra. Az analóg és digitális jel különbsége és jellemzői. Az analóg jelek digitalizálhatósága. A mintavételezés törvénye.
> A digitalizált adattárolás pontossága – minőségi problémák, korlátok.

Jelek csoportosítása értékkészlet és értelmezési tartomány szerint:

 - analóg jel: értelmezési tartománya és értékkészlete is folytonos
 - időtartományban diszkrét jel: a jel értelmezési tartománya diszkrét, értékkészlete folytonos (pl. óránként leolvasott hőmérő)
 - amplitúdóban diszkrét jel: az értelmezési tartománya folytonos, az értékkészlete diszkrét (pl. tápegység állítható kimeneti feszültsége)
 - digitális jel: értelmezési tartománya és értékkészlete is diszkrét

Az analóg és a digitális jel fogalma, példák felhasználásukra

 - Az analóg jel:
 - Értékkészlete és értelmezési tartománya folytonos. Értéke tetszőleges értéket vehet fel, folyamatosan változik. Bármikor leolvashatő, valosághű adatot ad.
 - Például: sebességmérő, hagyományos feszültségmérők, hagyományos hőmérő(higanyszál), barométer, hidraulika
 - Digitális jel: Valamely változó jelenségnek, vagy fizikai mennyiségnek diszkrét (azaz nem folytonos), megszámlálhatóan felaprózott, s így számokkal felírt értékein alapul.
 - Például: digitális fényképezők, számítógép, digtális hőmérő, digitális óra

Különbség és jellemzők:

A digitális rendszerek sokkal inkább (bináris) számokat használnak bevitelhez, feldolgozáshoz, átvitelhez, tároláshoz, vagy megjelenítéshez.
Az analóg rendszerek inkább az értékek folytonos spektrumát használják, vagy a nem-numerikus szimbólumokat, mint a betűk, vagy ikonok.
Az analógnál az apró ingadozásoknak, hullámzásoknak is van jelentésük.

Mintavétel törvénye:

Shannon mintavételi törvénye szerint annak a feltétele, hogy a minták helyesen tükrözzék a spektrum legnagyobb frekvenciájú komponensét az, hogy
a mintavételi frekvencia legalább kétszerese legyen a spektrum legmagasabb frekvenciájának.

Analóg jelek digitalizálhatósága, a digitalizált adattárolás pontosága, minőségi problémák, korlátok:

Digitalizálás során az analóg jelekből számjegyekkel reprezentálható jeleket állítunk elő, melyet a számítógép is értelmezni tud.
Az eredeti függvényből lépésközzel mintát veszünk, és a két lépés közötti változó értéket egyetlen értékkel helyettesítünk.
Ez csak egy megközelítő érték, hiszen a digitális jel csak adott értékeket vehet föl. Minél több értéket vehet fel a digitalizálás során, annál közelebbi értéket kaphatunk.
Az értéktartomány megadását hívjuk kvantálásnak. Több mintavételezés kisebb lépésekkel szintén javíthat a jel pontosságán.
A digitalizálás közben adatvesztés történik, ezért az eredeti analóg jel nem alakítható vissza a digitális jelből.

> Az analóg jelek digitalizálásának lépései. A hang, a kép és a film digitalizálhatósága. A digitalizálás eszközei.

Az analóg jelek digitalizálásának lépései:

 - Mintavételezés: Az eredeti függvényből lépésközzel mintát veszünk, és a két lépés közötti változó értéket egyetlen értékkel helyettesítünk.
 - Kvantálás: Az értékkészlet megadása, amelyből a digitális jel megadott, az eredeti jel értékét megközelítő értéket vesz fel.
 - Kódolás: A mintavételezett jelet a kódoló egységgel a kvantálással kapott értékhez bináris jelsorozatot rendelünk.
   + PCM - minden kvantáláshoz egyedi kód
   + DPCM - a megelőző mintához viszonyítótt eltéréshez rendelünk kódot
   + Előrejelzéses DPCM - a megelőző mintasorozat alapján várható értéktéől való eltérést írja le.

> Az adat és az adatmennyiség fogalma az informatikában. Az informatikában használt mértékegységek és ezek jellemzői. A bináris számábrázolás módszere és jelentősége az informatikában.
> A bináris karakterábrázolás formái, kódtáblák felépítése, jellemzői (ASCII, UNICODE).

Az adat és adatmennyiség fogalma:

 - Adat: Egy objektum egy meghatározott változojánának értéke; számmal leírható, számítástechnikai eszközzel rögzíthető, feldolgozható, megjeleníthető.
 - Adatmennyiség: Az a mennyiség, mérőszám és mértékegység, amely a jelek számát méri egy választott jelrendszerben. Szokásos egysége a bit, amely egy darab bináris jel adatmennyisége.

Az informatikában használt mértékegységek és ezek jellemzői:

Az információtartalom egysége a bit. Az információ két féle lehet (0, 1/HAMIS, IGAZ). Ez önmagában kevés, többszörösét használjuk. Nyolc bit alkot egy byte-ot.
A byte többszörösei: kiB, MiB, GiB, TiB, PiB (peta-), EiB(exa-). Váltoszám: 1024

A bináris számábrázolás módszere és jelentősége:

 - Fixpontos számábrázolás: Egész számok ábrázolása. Egy byte-on, azon belül 8 biten ábrázoljuk kettes számrendszerben a számot. Egy bájton 0-tól 255-ig ábrázolhatók a számok.
 - Előjeles szám esetében az első tag jelenti az előjelet, 0 a pozitívot, 1 a negatívot jelenti, ekkor -127 és 127 közötti értékek adhatóak meg.
 - Lebegőpontos számábrázolás: Valósz számok. A matetatikában is használt normálalak elven alapul.
 - Minden tizedes törtet fel írunk "egy nulla" egész alakú szám és 10 valamelyik hatványának szorzataként. 32 biten ábárzoljuk.

A számítógép minden műveletet számokkal végez. A számítógépek erre a kettes számrendszert használják; a 0-át és 1-et (HAMIS/IGAZ) könnyebb volt úgy fizikailag előállítani,
hogy a gép különbséget tudjon tenni a kettő között és megértse azt. Egyszerűen tud vele számításokat elvégezni.

A bináris karakterábrázolás formái, kódtáblák felépítése, jellemzői (ASCII, UNICODE):

Karakterek lehetnek: betűk, számjegyek, speciális jelek (pl.: felkiáltó jel (!), dollár jel($))
Minden karakternek megfelel egy 8 bites bináris kód, tehát egy karakter egy bájtot foglal. (Pl.: nagy "A" betű a bináris 65 (01000001))
A kódokat az ASCII tábla tartalmazza (szabványos amerikai kód információcserére). 256 karakter kódját tartalmazza. Nemzeti karakterek miatt külön kódlapokat hoztak létre.
Az UNICODE a XEROX által kifejlesztett új karakterkódolási módszer, amely már 16 biten ábrázolja a karaktereket. Ez 65536 különböző karaktert jelent.
Ez elegendő a világ összes nyelvének ábrázolására.

> A digitális képek tárolása, képformátumok és azok jellemzői (raszteres és vektoros). A színek kódolásának módjai (RGB, CMYK). Alapfogalmak: pixel, felbontás, színmélység.

A digitális kép tárolása, színek kódolásának módjai(RGB, CMYK):

A digitalizálás eredményét két jellemző határozza meg: a mintavételezés gyakorisága (felbontás), és a mért értékek kvantálása (színmélység).
A mintavételezés sűrűségét a felbontás adja meg, másszóval az, hogy milyen sűrűn vizsgáljuk a képpontokat. A pixelt a kép további részekre nem bontható egységes színű részének tekintjük.
Egy-egy pixelt a színével jellemezzük. A képponthoz rendelt színkódok számosságát a színmélységgel adjuk meg.
Erre a kódólásra a két legelterjedtebb módszer az RGB (Red Green Blue) és a CMYK (Cyan Magenta Yellow blacK/Karbon).
Az előbbit használják a monitorok, utóbbit nyomtatandó/nyomtatott képekhez használják.
Az RGB (összegző) additív színkeverés: a három alapszínt jelentő fénysugár különböző arányú keverésével állítja elő a képet. Általában egy ilyen arányt 24 biten, összetevőnként 1-1 bájton jelezzük.
A CMYK szubsztraktív (kivonó) színkeverés: Az egyes alapszíneket jelentő festékek bizonyos színeket elnyelnek a visszavert fényből.
A CMY szín elegendő lenne a fekete szín előállításához, de sosem tökéletes. Ehhez a színkeveréshez 32 biten tároljuk a színeket.

Pixel, felbontás, színmélység(Ezek definiálását beírtam a fenti szövegbe is)

 - Pixel: Nem osztható képpont, egy pixel elhelyezkedését(koordináta) és információ tartalmát(szín) határozza meg.
 - Felbontás: A képet alkotó pontoszlopok és pontsorok száma (pl. 640x360). Mértékegysége a képpont/hüvelyk. Mintavételezésnél ez jelenti a gyakoriságot.
 - Színmélység: a pontok színét leíró bitsorozat hossza, azaz a képernyőn megjeleníthető színek száma

Digitális képek formátuma és jellemzői:

 - Rraszteres (bitképes):  egyes képpontok információit tároljuk, és nem figyeljük, mit ábrázol a kép. Nagyobb kép nagyobb file méretet eredményez. A képet pontonként tároljuk.
 - Nagyításkor romlik a minőség. Pl.: .bmp, .png, .jpeg.
 - Vektoros: Matematikai formulákkal írjuk le a kép tartalmát/amit a kép ábrázol. Nagyobb kép nem jelent nagyobb file méretet, a kép csak geometrikus alakzatokból épül fel, függvényekkel leírható. Nagyításkor nem romlik a minőség. Pl.: .wmf, .swf (böngészőknél)

> A digitális hang tárolása, formátumok és azok jellemzői.

Digitalizálás során két tényező fontos: mintavételezési frekvencia, ami a mintavételezés gyakoriságát jelöli, és a kvantálás,
amely a minták amplitúdójának folytonos értékkészletét diszkrétté alakítja. Az első adja meg, hogy másodpercenként hány mintavétel legyen
(pl. Egy CD minőségű hangfájlnál ez a szám 44100, jelölése (44100)kHz. A kvantálás minőségét bitekben mérjük. Pl.: 16 bit az 65536 értéket vehet fel.
Formátumok:

 - Hullámformás tárolás: Sztereo hangot is tud tárolni, tároláshoz nem kell átalakítás, viszont a fájl mérete nagy lesz. Pl.: .wav, .pcm
 - Lehet tömöríteni a kapott fájlt, adatvesztéssel jár, csak az emberi fül által érzékelhető frenkvencián tárol adatokat. Pl.: .mp3, .mpeg
 - Ezen kívül vannak MIDI fájlok: utasításokat tartalmaznak, hardvereszközökkel lejátszható, egy szabvány hangszerkészletből építkezik.
