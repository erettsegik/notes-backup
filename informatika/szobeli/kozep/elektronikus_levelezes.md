### Alapfogalmak, összevetés a hagyományos levelezéssel

A levelezés mint kommunikációs forma az offline kommunikáció körébe tartozik, mert nem szükséges egyszerre mindkét fél együttes jelenléte.

Az elektronikus levelezés leginkább a papíralapú levelezéséhez hasonlít. Postafiókos levelezésnél két adatot kell a borítékra írnunk: egy irányítószámot és egy postafiókszámot. Például elegendő címzettként annyit írni a borítékra, hogy 1751 Pf. 85. Az 1751 egyértelműen meghatároz egy postahivatalt hazánkban, a Pf. 85 pedig a kérdéses postahivatal egyik fiókját jelöli meg. A papíralapú világban tehát a cím két fő részre osztható fel.

Az elektronikus világban is két fő részből áll az e-mail cím, amelyet fióknév@tartománynév formában adunk meg. Az irányítószám megfelelője a tartománynév: ez egy elektronikus postahivatalt, azaz egy (levelek fogadására alkalmas) kiszolgálót jelent az interneten. Ezen belül a fióknév azt a postafiókot azonosítja, ahová a postásnak (vagyis a levelet fogadó kiszolgálónak) el kell helyeznie küldeményt. Formailag szabályos e-mail címek például: rendeles@etterem.hu, pulyka.sonka@bolt.hu, kifli@mail.pekseg.hu.

Ahogyan a fenti példák is szemléltik, a címnek kötelező eleme a @-jel: ez választja el a címzés két fő részét. [A rész-egész, speciális-általános, tartalmazott-tartalmazó sorrend ―éppen úgy, mint a hagyományos levelek esetén― szokatlan a magyar anyanyelvű felhasználó számára, de megfelel az indoeurópai nyelvekben megszokottnak.] A fióknév rész lehet egytagú vagy többtagú: az ultraviola fióknév mellett szabályos az ultra.viola és az ultra_viola is (kevéssé ismert érdekesség, hogy ezek a gmail esetében ugyanazon fiókban végződnek). A tartománynév  (az internetes nevezéktannak megfelelően) lehet kéttagú vagy lehet többtagú (pédául a @bme.hu egy hálózatot azonosít, a @mkt.bme.hu egy alhálózatot, az @f-labor.mkt.bme.hu az alhálózaton elhelyezkedő kiszolgálót); egytagú viszont sosem lehet (ismét csak az internet hálózatainak, illetve kiszolgálóinak elnevezésére vonatkozó szabályok szerint).

#### Nézzük meg, hogyan jut el Viktor levele Mónihoz

A viktor@kifli. hu címről kell eljutni a levélnek a moni@sonka hu címre. Viktor megírja levelét és kattint a küldés gombra. Fontos tudni, hogy ekkor a levél a helyi levelező program elküldendő üzeneteket tároló mappájába kerül. A levél a küldés/fogadás megindítása után indul útjára. Lehet, hogy ehhez a művelethez egy gombra kell kattintanunk, vagy lehet automatikus is. Ha elküldtük, akkor levelünk hamarosan szolgáltatónk (levélküldő) kiszolgálójára kerül. A kiszolgáló a tartománynév alapján eldönti, hogy tovább kell-e küldeni a levelet vagy sem. A példa szerinti esetben a kifli.hu tartomány (levélküldő) kiszolgálója felveszi a kapcsolatot a sonka.hu tartomány (levélfogadó) kiszolgálójával és továbbküldi a levelet. Következőként a sonka.hu kiszolgálója elhelyezi a levelet a címzett postafiókjába. Fontos tudni, hogy egyes esetekben a címzett gépén csak akkor fog megjelenni a levél, ha ő is kezdeményez egy küldés/fogadást.

Több helyen is hiba csúszhat a levelek kézbesítésébe. Ha elrontjuk a címzett tartománynevét, akkor már saját kiszolgálónk jelzi a hibát. Ha a címzett fióknevét rontjuk el, akkor már a címzett kiszolgálója fog jelezni. Ezek a visszajelzések legtöbbször automatikusak, de természetesen csak elküldés után jelenhetnek meg.

A sikeres kézbesítésről és az olvasásról is kérhetünk visszaigazolást. A kézbesítési visszaigazolás automatikus. Az olvasási visszaigazolás esetén a címzett egy kérdést kap, hogy szeretné-e elküldeni a feladó kérésére az olvasási visszaigazolást.

### A levelezőprogram beállítása

Tekintsük át, hogy milyen adatokat kell megadnunk programunk megfelelő működéséhez. Helytelen beállításokkal olyan helyzetet is teremthetünk, hogy például magunk nem tudunk levelet küldeni, de tudjuk fogadni a nekünk írt leveleket. Elsőként tudnunk kell, hogy milyen a kiszolgálónk típusa, azaz milyen módon kapcsolódik levelezőprogramunk a kiszolgálóhoz. Ez leggyakrabban az SMTP/POP3 típusú kapcsolat. A kimenő leveleket kezelő SMTP és a bejövő leveleket kezelő POP3 szerverek nem mindig azonosak. Ha otthon kell ezt beállítanunk, akkor ezeket az adatokat általában az az előfizetői szerződésből, illetve használati útmutatóból tudhatjuk meg.

Az internetszolgáltató gyakran ad postafiók-szolgáltatást is, de választhatunk tőle független levelezőszolgáltatót is. Ez utóbbi sok esetben nem nyújt SMTP szolgáltatást; ilyenkor az internetszolgáltató SMTP-szolgáltatását kell használnunk. Ekkor persze más-más felhasználónév és jelszó tartozik az SMTP-, illetve a POP3-szerverekhez.

A POP3-szerverhez minden esetben tartozik felhasználónév és  jelszó (miért is?); az SMTP-szolgáltatás működhetnék azonosítás nélkül is, de ez igen ritka: az SMTP-szerverek jellemzően csak az általuk ismert felhasználók leveleit továbbítják, hogy elkerüljék a levélszemét átvételét és továbbítását.

### Levél írása
Levél küldésénél az egyetlen kötelező adat a Címzett. A Tárgy sorát is illik kitölteni; az üres tárgyú levél könnyen végezheti a levélszemét között. A Címzett és a Másolatot kapó címzett között a kézbesítés szempontjából igazából nincs különbség. A címzett(ek) (To:) és a másolatot kapók (Cc: a carbon copy rövidítéseként) kölcsönösen látják egymást, de egyikük sem látja a titkos másolatot kapó (Bcc: blind carbon copy) címzett(ek)et. (Különbség lehet viszont a válasz küldésekor – micsoda?)

Ha fontos, hogy egy iratot olyan formában lásson a címzett, ahogyan mi megírtuk, akkor ne a levél törzsét formázzuk. A megfelelő programmal készítsük el a dokumentumot és a terméket csatoljuk levelünkhöz. Mellékletet legtöbbször egy gemkapocs-ikonra való kattintás után helyezhetünk el a levélben. Jó tudni, hogy több mellékletet is csatolhatunk egy levélhez, de mappaszerkezetet nem. Ha a fájlokat a mappaszerkezet megtartásával szeretnénk elküldeni, akkor előbb tömörítsünk, majd a tömörített állományt csatoljuk. Érdemes tudni, hogy nem minden melléklet lesz használható a címzett gépén: a csatolt állomány olvasásához a címzett(ek)nek rendelkezniük kell a megfelelő programmal (ennek megfelelően célszerű szabványos, széles körben elterjedt dokumentumformátumot választani, például pdf-et). Ezen kívül az is lehetséges, hogy a biztonsági szempontból veszélyforrást jelentő mellékletekhez nem enged hozzáférni a levelezőprogram.

Ha szeretnénk felhívni a címzett figyelmét levelünkre, akkor megjelölhetjük, a Sürgős jelzővel. Ennek nincs hatása a levél kézbesítésére, a címzett figyelmének felhívására használatosak.

Alapértelmezett beállítások szerint elküldött üzeneteinkből egy másolat marad gépünkön is, a megfelelő mappában.

Jó tudni, hogy a levelezőprogramban általában meghatározhatjuk a levél formátumát. Ez lehet például html, txt (egyes rendszerekben akár rtf is). Html esetén a weblapoknál megszokott formázásokat használhatjuk; az rtf választása a szövegszerkesztésből tűnhet ismerősnek; némely szövegszerkesztő ismeri ezt a formátumot. A txt formátum esetén nem formázható a szöveg, és például képek sem helyezhetők el a szövegtörzsben, csak a mellékletként (de a fent írtak szerint ez a helyes forma – miért is?).

### Beérkezett üzenetek kezelése

Sok levelezőrendszer már alaphelyzetben több mappában helyezi el a leveleket. Ilyen lehet a Beérkezett üzenetek, az Elküldött levelek, a Postázandó üzenetek vagy a Törölt elemek. Ezek mellett sok más (alapértelmezett) mappára láthatunk példát: így az Outlook a Piszkozatok mappában tárolja a félbehagyott, a Levélszemét mappában a kéretlennek ítélt leveleket. Ezen kívül persze magunk is létrehozhatunk mappákat az üzeneteket rendszerezéséhez. Alapértelmezés szerint a nekünk irt üzenetek a Beérkezett üzenetek nevű mappában fognak megjelenni.

Az üzenetek listájában láthatjuk például a feladót, tárgyat, érkezési időt és méretet (és azon további információkat, amelyeket kiválasztunk); ennek megfelelően sokféle szempont szerint rendezhetjük, illetve szűrhetjük a levelek listáját.

Csukott boríték jelölheti az olvasatlan üzeneteket, egy gemkapocs pedig azokat a leveleket, amelyekhez melléklet tartozik. Gyakori, hogy a mappák listájában néhány név, s mellettük egy szám félkövéren jelenik meg: ezekben a mappákban olvasatlan üzenetek (is) vannak, zárójelek között ezek száma jelenik meg. Általában a kiválasztott üzenetre duplán kattintva olvashatjuk el annak tartalmát.

Egy másik részben látjuk a levél törzsét, felette a fejléc-információkat. Láthatjuk a feladót, a tárgyat, de sosem látjuk a titkos másolatot kapó személy(ek) címét. Az ablak címsorában megjelenhetik, hogy milyen formátumú levélről van szó. Ha a levélhez melléklet is tartozik és szeretnénk ezt megtekinteni, akkor kattintsunk rá duplán.

Programunk általában rákérdez, hogy a mellékletet megnyitni vagy menteni szeretnénk (természetesen a megnyitás is letöltéssel, s valószínűleg tárolással is jár). Biztonsági okokból fontos, hogy ismeretlen mellékletet pusztán kíváncsiságból ne nyissunk meg. Ha több mellékletet is tartalmaz az üzenet, akkor sem kell egyesével menteni ezeket. Általában a Fájl menü megfelelőpontjának kiválasztása után csoportosan menthetjük az üzenet mellékleteit.

Egy üzenetet letörölhetünk egérkattintással vagy billentyű(kombináció) leütésével. Megjegyzendő, hogy üzenetünk ekkor általában a törölt elemek tárolására szolgáló mappába kerül; a végleges törléshez innen is törölni kell.

### Válasz, továbbítás

A beérkezett üzenetekre válaszolhatunk új üzenettel, de hasznosabb, ha a beépített válaszolási lehetőséget használjuk; ezen kívül továbbíthatjuk a levelet más(ok)nak. A válaszadás kétféle lehetőségét, illetve a továbbítás funkcióját gyakran tévesen értelmezik, ezért érdemes tisztázni a Válasz, a Válasz mindenkinek és a Továbbítás közti különbséget.

Ha a *Válasz* gombra kattintunk, akkor automatikusan a levél eredeti feladója lesz a címzett és a levél tárgya kiegészül a Re: előtaggal; ezeket az automatikusan ajánlott lehetőségeket természetesen módosíthatjuk.

A *Válasz mindenkinek* gombra kattintva a tárgy szintén a Re: előtaggal egészül ki; különbség a címzettnél lesz: ilyenkor az eredeti levél feladója, összes címzettje és másolatot kapója lesz a válasz címzettje (kivéve természetesen a titkos másolatot kapókat). Jó tudni, hogy a válaszokban automatikusan nem jelenik meg az eredeti levél melléklete, hiszen akitől kaptuk, annak valószínűleg megvan.

*Továbbítás* esetén a címzettet nekünk kell megadni, az eredeti tárgy az Fw: előtaggal egészül ki, az újabb levél törzsében pedig megjelenik az eredeti levél törzse és fejléc-információi. Ilyenkor az eredeti levél melléklete automatikusan része lesz a továbbított levélnek is. Ezeket igény szerint módosíthatjuk, hozzáírhatunk, illetve törölhetünk belőlük. Alapértelmezés szerint a készülő levél formátuma az eredeti levél formátumával fog megegyezni, de ezen igényeink szerint módosíthatunk.

Érdekességként megemlíthetjük, hogy egyik lehetőségként a továbbító/válaszoló sorait eltérő színnel jelölhetik a levelezőprogramok.

Érdemes megemlíteni a válasz egy speciális esetét, a Házon kívül választ: távollétünk idején automatikus Házon kívül (Out of Office) válasszal értesíthetjük a beérkező levelek küldőjét. Az automatikus választ kaphatja mindenki, de koncentrálhatunk csak adott felhasználókra: például a listáról érkező levelekre, de a vírusok által küldött levelekre sem célszerű elküldeni a házon kívül választ. Ezt a fajta választ a szolgáltatónak támogatni kell, hiszen gépünk általában nincs bekapcsolva távollétünk idején.

### A levélszemét

Az elektronikus levelezés bosszantó mellékhatásaként rengeteg kéretlen levelet (spamet) kaphatunk, ezek egy része ráadásul vírust, ártó kódot is tartalmazhat. A legtöbb szolgáltató ajánl spamszűrő szolgáltatást, de a levelező programok is beépítetten biztosíthatnak levélszemét-szűrési lehetőséget. Egy beépített logika próbálja osztályozni az üzeneteket, ennek működését úgy pontosíthatjuk, hogy magunk is levélszemétnek minősíthetünk egy üzenetet. Ha egy feladótól a továbbiakban már nem szeretnénk levelet kapni, akkor hozzáadhatjuk a letiltott feladók listájához, másfelől viszont biztonságosnak is minősíthetünk egy feladót a levelei tartalmától függetlenül.

A megfelelő (fekete- és fehér)listákat kiegészíthetjük például kollégánk listájával importálás és exportálás segítségével. Jó tudni, hogy alapértelmezés szerint a levélszemétszűrőn fennakadt levél csak a levélszemét mappába kerül, ahonnan kézzel kell törölnünk (vagy egy idő után a program törli). Ha egy feladó a tiltott és a megbízható feladók között is szerepel, akkor végeredményben levelei megbízhatónak minősülnek. [Ilyen általánosításból már rengeteget kigyomláltam, illetve helyesbítettem az előző bekezdésekben; itt látszik az, hogy a redmondi szemüveggel –vagy inkább szemellenzővel– ellátott forrás mennyire keveset lát a világból. Ha a feleletben ilyen állítások hangzanak el, vissza fogok kérdezni. Valóban? Hány levelezőprogram ismeretében állítod ezt? Konkrétan mely levelezőprogramokat láttad, amelyek így viselkednek?]. Hasznos tudni, hogy a tiltott feladók közé felvehetünk @spamkuldo.hu formájú elemet is. Ekkor a kérdéses tartomány minden levele kéretlennek minősül.

A Spam eredetileg egy olcsó (sokak szerint ehetetlen) konzerv volt az Egyesült Államokban; a szó jelentésváltozásában és elterjedésében jelentős szerepet játszott egy Monty Python-jelenet. [A levélszemét elterjedéséhez pedig nagyban hozzájárult az Egyesült Államok alkotmányának még 1791-ből származó, lényegében korlátlan szólászabadságot biztosító első kiegészítése.]

### Digitális aláírás

Ha fontos tudni, hogy útközben nem módosult egy üzenet, akkor lássuk el digitális aláírással. Ehhez előbb egy tanúsítványt kell szereznünk valamely hiteles szolgáltatótól. Ez általában fizetős szolgáltatás, de rövidebb ideig érvényes tanúsítványt ingyen is szerezhetünk.

Ha aláírt levelet szeretnénk, akkor írjuk azt meg a szokásos módon, majd például Outlook esetén kattintsunk a Beállítások fülre, válasszuk a Biztonsági beállítások pontot és kérjünk digitális aláírást.

Lényeges, hogy a digitális aláírás sértetlenséget és hitelességet igazol, míg a hagyományos aláírás csak udvariassági formula.

### Webes felületű levelezőprogramok

Érdemes szólni a webes felületű levelező programokról is. Gyakorlatilag már ezek is nyújtják a kliensprogramok szolgáltatásait. A webes felület nagy előnye, hogy használatához nem kell semmilyen egyéb program, elegendő a böngészőnk. Ebből adódóan nem kell a kliensprogramoknál látott beállításokkal bajlódnunk, és a világ bármely részén a jól megszokott felület fogad miket. Számtalan ingyenes szolgáltatót találunk az interneten, és egy rövid regisztráció után már használhatjuk is a választott e-mail címünket. Természetesen a választott fióknevünknek egyedinek kell lenni a szolgáltatónál. Egyre több internetszolgáltató is biztosít már online webes elérést az internet-előfizetők számára adott e-mail címeknek.

Vegyük észre, hogy a mappák közül hiányzik a postázandó üzenetek nevű. Ez a mappa a kliensprogramoknál azokat a leveleket tartalmazza, amelyek a levelező kiszolgálónk felé való továbbításra várakoznak. Webes felület esetén erre nincs is szükség, hiszen közvetlenül a kiszolgálón dolgozunk. A webes felület esetén is használhatjuk a megszokott szolgáltatásokat. Ilyen például a spamszűrés, blokkolhatunk adott feladókat, megadott feltételeknek megfelelő leveleket továbbíthatunk egy másik címre, mappákba csoportosíthatjuk leveleinket stb.

Fontos megemlíteni, hogy a kliensprogramok a saját gépünkön tárolják a leveleket [ez nem így van, de már nem javítgatok többet – nem is kell, lásd a következő bekezdést], míg a webes felületű levelezők a kiszolgálón. Ez persze azt is jelenti, hogy webes felület használata esetén mindenképpen élő internetkapcsolat kell a levelek olvasásához, írásához.

Szolgáltatótól függően lehetséges ugyanannak az e-mail címnek a használata webes felületen és POP3-IMAP/SMTP kliensprogrammal is. A kliensprogramoknál megadhatjuk, hogy a már letöltött leveleket távolítsa el a kiszolgálóról (POP3) vagy sem (IMAP). Alapértelmezés szerint a letöltött levelek (POP3 esetén) a kiszolgálóról törlődnek, tehát a webes felületen keresztül később már nem lesznek elérhetők.
