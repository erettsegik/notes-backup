*Periféria:* a számítógép központi egységéhez kívülről csatlakoztatható eszközök, az adatok be- és kivitelét (megjelenítését) szolgálják. Három csoportjuk van: bemeneti egységek (input), kimeneti egységek (output), ki- és bemeneti egységek.

*Kimenetei (output) egységek:* a számítógépbe bevitt, illetve a gép által tárolt és/vagy feldolgozott adatokat ezek segítségével tekinthetjük meg, kizárólag az adatok megjelenítését szolgálják. Legfontosabbak a monitor és a nyomtató, de megemlíthetjük ezek mellett például a rajzgépet is.

### Monitorok

Ma a számítógép fő kimeneti egysége. A monitoron megjelenő képet képpontok (pixelek – picture element) alkotják, ezek sűrűségétől és méretétől függ a monitor minősége. Általában VGA, DVI vagy HDMI kábel köti össze a számítógéppel (pontosabban azon belül a videokártyával).

Kezdetben a (monokrómnak nevezett) monitorok a fekete mellett egy színt jeleníthettek meg (fehéret, zöldet, borostyánsárgát), később már 16-, illetve 256-féle szín megjelenítésére is képesek voltak. A VGA-szabványtól kezdődően jelentek meg a (mai értelemben is) színes  monitorok.

A megjelenítés *kétféle üzemmódban* történhet:
- szöveges üzemmód: ilyenek voltak az első monitorok, csak karaktereket lehet rajtuk megjeleníteni
- grafikus üzemmód: nem csak karakterek megjelenítésére képes, a teljes képernyőt betölti a grafikus felület, külön kezeli a képpontokat – mára ez szinte kizárólagossá vált

A mai operációs rendszerek általában grafikus megjelenítésűek, de például linux esetén máig nem kevesen használnak szöveges üzemmódot a grafikus üzemmód mellett (kiszolgálók esetén pedig gyakran kizárólagos a szöveges mód), s windows rendszerű gépeken is nyitható szöveges módú parancsablak.

A ma elterjedt monitorok *három fő típusa:*

- *crt (cathode ray tube):* katódsugárcsöves monitorok (mint a régebbi televíziók). A képcső hátuljában elhelyezett elektronágyú elektronsugarakat lövell ki a képcső elejére, melyet foszfor alapú réteg fed. Erős elektromágnesek térítik el az elektronsugarakat, így azok a képcső elejének különböző részeit találják el. Ha az elektronnyaláb eléri a képcső elülső részét, a foszforborításba ütközik, amely felvillan, majd elhalványul (ha tehát az elekronnyaláb elég gyorsan visszajut ugyanarra a pontra, akkor a pont folyamatosan világít). Az elektronnyaláb balról jobbra, illetve felülről lefelé haladva egy másodperc alatt többször is frissíti a képpontokat.

- *lcd/tft:* Az lcd folyadékkristályos képernyő, az első ilyen monitor a 60-as években jelent meg. Fizikai alapja a folyadékkristály átlátszóságának változása elektromos tér hatására. A gyártás tökéletlensége miatt előfordulhatnak „beragadt” képpontok, ez a pixelhiba. A tft az lcd-technika továbbfejlesztése, jobb minőségű képet eredményez, grafikus munkákhoz ajánlják, sok azonban a selejtes kijelző.

- *pdp (plazma display panel):* plazmakijelző, működése azon alapul, hogy két üveglap közé ionizált neon- vagy argongázt zárnak, melyek mozgó elektronok hatására fényt bocsájtanak ki. Előnye a nagy képátló, hátránya a magas ár.

A monitorok *főbb paraméterei:*
- *megjelenítő típusa:* a fentiek szerint crt, lcd stb
- *képátló:* a kijelző egyik sarkától a szemközti sarkáig terjedő távolság, inchben szokás megadni
- *képarány:* a kijelző oldalhosszúságainak aránya, korábban jellemző módon 4:3, manapság a multimédia előretörésével egyre inkább 16:9 [miért?]
- *kontraszt:* a részletgazdagságot jellemző tulajdonság, értéke a legfényesebb és a legsötétebb pixel fényerejének hányadosa
- *válaszidő:* az lcd monitorok jellemzője, ezredmásodpercben mérik; az az idő, ami alatt egy képpont fényereje megváltozik; 12 ms-tól lassú válaszidőről beszélhetünk
- *fényerő:* a kijelző fényessége, pl 250 cd/m^2
- *felbontás:* a pixelek száma, pl: 1920x1080, 1366x768, 1024x768, 640x480 stb
- *megjelenő színek száma:* a megjeleníthető színárnyalatok száma, ma jellemző módon 16,7 millió
- *látószög:* megadja, hogy milyen szögből látható a kijelzőn megjelenő információ
- *frekvencia:* megadja, hogy másodpercenként hányszor frissülnek a képpontok, Hertzben mérik, ma 60 és 130 Hertz közötti értékek a megszokottak, körülbelül 65-70 Hz felett nem érzékelhető a vibrálás

### Nyomtatók.

A legegyszerűbb eszköz arra, hogy munkánkat papíron is viszontláthassuk (ez volt a korai, monitor nélküli számítógépek adatmegjelenítő egysége).

A nyomtatott kép minőségét az egységnyi nyomtatási területre eső képpontok dpi-vel megadott maximális száma határozza meg. Jó minőségű nyomtatásról 300 dpi (pontosabban 300 dpi x 300 dpi) felett beszélhetünk.

A nyomtatott szövegben az egy hüvelyk hosszon elhelyezkedő karakterek száma a cpi. A nyomtatási sebességet korábban a karakter/másodperc értéket leíró cps, ma sokkal inkább a lap/perc mértékegységgel mérhetjük.

*Fajtái:*

- *különböző technológiájú (láncos, írókorongos, íróhengeres) sornyomtatók:* egyszerre egy egész sort nyomtatnak
  - rögzített jelkészlet (például csak az angol abc nagybetűi, számjegyek és a legfontosabb írásjelek)
  - meglepően gyors, de
  - rendkívül hangos működés

- *Gömbfejes és margarétafejes nyomtatók:* gyári fejen lévő fix karakterkészletet tudják alkalmazni, mint az írógépek
  - lassan, de
  - viszonylag szépen nyomtatnak

- *Mátrixnyomtatók:* az írógép továbbfejlesztett változatának tekinthetjük, a legrégebbi széles körben elterjedt nyomtatótípus. Az írásjelek képét az írófejben egymás alatt elhelyezhedő 9 vagy 24 tű segítségével, egymás alatt  pontokból alakítja ki. A tűk mágneses tér hatására mozdulnak ki, rugó húzza vissza őket a helyükre.
  - romban rögzített vagy ramba letölthető (tehát módosítható) jelkészlet
  - nagyon korlátozott grafikai képességek
  - viszonylag lassú működés
  - elfogadható zajszint
  - meglehetősen gyenge minőség (kopik a tű, fogy a festék a szalagból: egyenletlen a fedés)
  - mai napig használják, leginkább a többpéldányos nyomtatási képessége miatt (indigós papír, számlanyomtatás)

- *Tintasugaras nyomtatók:* az otthoni felhasználók körében a legelterjedtebb; nyomtatáskor egy kisméretű tintaágyú mikroszkopikus méretű tintacseppeket lő a papírra, egy karaktert sokkal több pontból alakítanak ki, mint a mátrixnyomatók, ennek megfelelően
  - nagyon csendes működés
  - nyomtatvány szintű íráskép, akár foto-realisztikus fénykép nyomtatása
  - általában nyomott áron adott készülék (rövid élettartammal)
  - igen drága kellékanyaggal

- *Lézernyomtatók:* működési elvük a fénymásolóéhoz hasonló. A szelénnel bevont hengernek fény hatására megváltoznak az elektromágneses tulajdonságai; a hengert végigpásztázó, „fel-felvillanó” lézer rajzolja fel a nyomtatandó kép egy sorát, s mikor ez a rész érintkezésbe kerül a festékport (tonert) tartalmazó rekesszel, az elektromos töltés miatt a toner rátapad a hengerre. Továbbgördülve a festék rákerül a papírra, majd beégetéssel rögzül azon.
  - csendes működés
  - kifogástalan minőség
  - drágább készülék
  - olcsóbb üzem
