### Bináris kép

Bevezetésként érdemes néhány szót ejteni a digitális képek tárolásáról, a különböző fájlformátumokról.

A *bitképes* vagy *pixelgrafikus* tárolás esetén az egyes képpontok információit tároljuk, és nem figyeljük, hogy mit ábrázol, hogy milyen alkotóelemekből tevődik össze a kép. Ilyenkor nagyobb kép nagyobb fájlméretet eredményez.

A *vektoros* tárolás esetén azt is figyeljük, hogy mit ábrázol a kép, és matematikai formulákkal írjuk le a képet. Ekkor a nagyobb kép nem feltétlen jelent nagyobb fájlméretet.

[Hogyan keletkezik a kétféle kép? Milyen tevékenység eredményezi az egyiket, milyen a másikat?]

A bmp kiterjesztésű állományok például rasztergrafikus (bittérképes), az svg kiterjesztésűek pedig vektorgrafikus módon tárolják a képeket. A bittérképes esetben a képet pontonként tároljuk. A vektorgrafikus képek esetén a képet geometrikus alakzatokból építjük fel, függvényekkel írhatjuk le. A pixelgrafikus képek minősége nagyításkor romlik, a vektorgrafikusoké nem. Pixelgrafikus képek esetén a fájl mérete a kép méretétől függ, míg vektoros esetben inkább a kép felépítésétől, összetettségétől.

[érdemes lehet párhuzamot vonni a betűtípusokkal: azok is lehettek pixelesek vagy vektorosak; ennek megfelelően nem lehet vagy lehet őket skálázni (nagyítani)]

Felbontásról, színmélységről itt csak röviden essék szó, főleg arra összpontosíts, hogy hogyan hatnak azok a (tömörítés nélküli) képméretre. Mi történik, ha az x-tengelyen, ha az y-tengelyen, ha mindkettőn megkétszerezzük a képpontok számát; mi történik, ha  a színmélység lesz kétszeres?

A *színek kódolására* a két legelterjedtebb módszer az rgb (vörös-zöld-kék) és a cmyk (Cyan-Magenta-Yellow-blacK, azaz cián-bíbor-sárga-fekete). Az rgb módszerét alapvetően a képet fénysugárzással megjelenítő eszközök, például monitorok alkalmazzák. A cmyk módszer a fényelnyelésen alapul, például a nyomtatásban használjuk.

Az *rgb*-módszert additív (összegző) színkeverésnek is hívják, mert a három alapszínt adó fénysugarak különböző arányú keverésével állítja elő a végeredményt. 24 bites színmélység esetén az egyes összetevők mennyiségét 1-1 byte-on adjuk meg. Az egyik zöld színnek a szokásos jelzése lehet például  #OOAAOO. A nagyobb értékek világosabb színt jelentenek. A színkeverés elvéből adódóan #FFFFFF fehéret ad, #000000 pedig feketét. A három alapszínt azonos mennyiségben tartalmazó színek a szürke valamely árnyalatát határozzák meg.

A *cmyk* módszert szubtraktív (kivonó) színkeverésnek is hívják. Itt a módszer alapja az, hogy az egyes alapszíneket jelentő festékek bizonyos színeket elnyelnek a visszavert fényből. Érdemes megemlíteni, hogy elvileg a cmy színek elegendőek a fekete szín előállításához is, de ez a gyakorlatban nem adna tökéletes eredményt (nem mellesleg rendkívül drága lenne a használata – miért?), ezért alkalmazzák negyedik színként a feketét. A nyomdászatban négyszínnyomásnak is hívják az eljárást. Ha minden színhez 1 bájtot rendelünk, akkor 32 biten tárolhatjuk a színeket. Érdekesség: a black (fekete) megnevezésből azért került a K a rövidítésbe, mert a B a blue (kék) miatt félrevezető lenne.

[Én semmiképpen nem hagynám ki a hsv-modellt, lásd például a gimp színválasztási lehetőségeit.]

[Meg lehetne említeni továbbá az alfa-csatorna szerepét: ez az egyes képpontok átlátszóságát adja meg.]  

Lényeges kérdés, hogy mekkora helyet foglal el a kép az adott háttértáron. Ahogyan korábban említettük, a színmélység és a felbontás növekedésével nő az adatmennyiség, és így egyre nagyobb fájlokat kapunk. A helycsökkentésben játszanak szerepet a különböző *tömörítési* eljárások. Használhatunk veszteséges és veszteségmentes eljárásokat is. Veszteségmentes esetben a tömörített képben az eredeti kép minden információját megtaláljuk. A veszteséges tömörítés alkalmazása esetén a tömörített képben már nincs meg az eredeti kép minden információja. Veszteségmentes tömörítést használ például a gif és a png fájlformátum. Érdemes megemlíteni, hogy a gif esetleges rosszabbnak tűnő minősége abból ered, hogy a formátum csak 256 féle színt kezel. [Akkor ez tényleg veszteségmentes?] A veszteséges eljárásokkal már sokkal nagyobb tömörítési aranyt érhetünk el. A veszteséges tömörítést alkalmazó formátumok egyik tipikus képviselője a közismert jpg/jpeg (Joint Photographic Experts Group). Veszteséges formátum választása esetén eldönthetjük, hogy a minőséget vagy a fájlméretet tekintjük-e fontosabbnak, s a fontosabbat  mennyivel tekintjük fontosabbanak a másiknál.
