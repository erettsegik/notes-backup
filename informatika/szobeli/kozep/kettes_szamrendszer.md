## Általánosan:

A tízes számrendszer a számok ábrázolásának legelterjedtebb módja. Sőt a hétköznapi ember számára nem is létezik másik számrendszer. Ennek az oka lehet az, hogy egy embernek 10 ujja van, viszont például a nyelvekben ezekre ellenpéldákat találhatunk ugyanis mind a németben, mind az angolban 12-től van ismétlődés. Illetve az időben vagy a fokmérésben sem a 10-es számrendszer terjedt el, hanem a 60-as.

Az informatikában a 2-es számrendszert használjuk, mert így tudunk adatokat könnyen tárolni és továbbítani. Ez azért van, mert az áramnak is két féle állapota van: van áram vagy nincs áram. Illetve a mágneses háttértárnál is két pólus van É-i és D-i. Viszont a 2-es számrendszer nagyon hosszú számokat eredményez és a hétköznapi életben bonyolult lenne a használata. Ahhoz hogy a számrendszerekben nem jártas ember is könnyen értelmezni tudja a sok 0-ást és 1-est, ezeket át kell tudnunk váltani 10-es számrendszerbe. A kettes számrendszerben 2 számjegy van, a helyi értékek pedig a természetes számok 2. hatványai.

Átváltás: 2 --> 10:
<table style="margin:auto">
<tr>
<td>16</td>
<td>8</td>
<td>4</td>
<td>2</td>
<td>1</td>
<td colspan="2">=1*16+0*8+0*4+2*1+1*1= 1910</td>
</tr>
<tr>
<td>1</td>
<td>0</td>
<td>0</td>
<td>1</td>
<td>1</td>
</tr>
</table>

Átváltás: 10 --> 2:
<table style="margin:auto">
<tr>
<td rowspan="2" style="vertical-align: top">372=</td>
<td>256</td>
<td>128</td>
<td>64</td>
<td>32</td>
<td>16</td>
<td>8</td>
<td>4</td>
<td>2</td>
<td>1</td>
</tr>
<tr>
<td>1</td>
<td>0</td>
<td>1</td>
<td>1</td>
<td>1</td>
<td>0</td>
<td>1</td>
<td>0</td>
<td>0</td>
</tr>
<tr>
<td>Maradék:</td>
<td>116</td>
<td>-</td>
<td>52</td>
<td>20</td>
<td>4</td>
<td>-</td>
<td>0</td>
<td>-</td>
<td>-</td>
</tr>
</table>

A számítógépekben 1 byte-on (8bit) 0-tól 255-ig ábrázolhatjuk a természetes számokat. A számítógépek egyik legalapvetőbb művelete az inkrementálás, ami az 1-el való növelés.

Néhány példa:
<table style="margin:auto; width: 75%">
<tr>
<td>0000 --> 0001</td>
<td>0011 --> 0100</td>
</tr>
<tr>
<td>0101 --> 0110</td>
<td>1111 --> 10000</td>
</tr>
</table>

## Negatív számok:

Ha negatív számokat szeretnénk ábrázolni, akkor a legkézenfekvőbb megoldás az lenne, ha lenne egy előjel bit ami megmondaná. hogy az adott szám: pozitív, ha az előjel bit: 0 vagy negatív, ha az előjel bit: 1. pl: 00001111 --> 15, 10001111 --> -15

Ez a megoldás azonban két okból is rossz megoldás az egyik ok az, hogy így 2 db 010 lenne, mert a 000000000 és az 100000000 is 0-lenne. A fő baj viszont az hogy nem működne mindig az inkrementálás. 10000001 (-1) –et inkrementálva 10000010 (-2)-et kapnánk. Ezért, hogy mindig működjön az inkrementálás egy kicsit bonyolultabb lesz a megoldás:
<table style="margin:auto">
<tr>
<td>1</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>-128</td>
</tr>
<tr>
<td>1</td>
<td>1</td>
<td>1</td>
<td>1</td>
<td>1</td>
<td>1</td>
<td>1</td>
<td>0</td>
<td>-2</td>
</tr>
<tr>
<td>1</td>
<td>1</td>
<td>1</td>
<td>1</td>
<td>1</td>
<td>1</td>
<td>1</td>
<td>1</td>
<td>-1</td>
</tr>
<tr>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
</tr>
<tr>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>1</td>
<td>1</td>
</tr>
<tr>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>1</td>
<td>0</td>
<td>2</td>
</tr>
<tr>
<td>0</td>
<td>1</td>
<td>1</td>
<td>1</td>
<td>1</td>
<td>1</td>
<td>1</td>
<td>1</td>
<td>127</td>
</tr>
</table>

Így már minden esetben működik az inkrementálás és az egész számokat ábrázolni tudjuk 8bit-en -128-tól 127-ig. Amikor az -110-et inkrementáljuk akkor valójában 100000000-at kéne kapnunk de mivel a számítógép 8 biten dolgozik azt az 1-est nem jeleníti meg hasonló eset a hétköznapi életben például a villanyóránál. Ezt túlcsordulásnak nevezzük. Ha jobban megfigyeljük, az első bit mutatja az előjelét a számnak, ha 0 az első bit, akkor vagy 0 vagy pozitív a szám, ha pedig 1 akkor negatív a szám.
A negatív számokat azonban nem lehet olyan könnyen átváltani, mint a pozitívokat. Ha egy negatív, 10-es számrendszerbeli számot akarunk átváltani a következő a teendő: Először vegyük a szám -1 szeresét, váltsuk át úgy mintha egy pozitív számot váltanánk át, majd ezt a számot regáljuk (az 1-esek helyére nullákat írunk a 0-ások helyére 1-eseket). Majd végül ezt a 2-es számrendszerbeli számot inkrementáljuk.
Ha egy 2-es számrendszerbeli számot szeretnénk átváltani 10-es számrendszerbe, akkor ugyanez a teendőnk csak visszafele kell végigmennünk a lépéseken és inkrementálás helyett dekrementálnunk kell, ami az 1-el való csökkentés.
Törtek:
A törteket 10-es számrendszerben egy tizedesvesszővel (12,34) jelöljük. Ezek alapján a 2-es számrendszerben a törteket egy kettedes vesszővel (10,01) jelöljük. 2-es számrendszerből a szokásos módon váltjuk 10-esbe a számokat.
8	4	2	1	,	1/2	1/4	1/8	=2,2510
0	0	1	0		0	1	0
10-es számrendszerből 2-esbe akkor legkönnyebb az átváltás, ha a nevező 2 valamelyik hatványa. Könnyebb átváltás az, hogy átváltjuk a számlálóban lévő számot majd odébb toljuk a kettedes vesszőt.
A k/l nem egyszerűsíthető tört 10-es számrendszerbeli alakja véges, ha az l= 2m*5n. Ugyanígy a 2-es számrendszerben k/l nem egyszerűsíthető tört alakja véges, ha l=2m. Ez a két állítás visszafelé is igaz. Például az 1/10-ed 2-es számrendszerben végtelen tizedes tört, ami azt eredményezi, hogy a számítógép nem tud vele pontosan számolni.
A törtek ábrázolására 2 féle módszert használhatunk a számítástechnikában. Az egyik a fixpontos ábrázolás, amikor a kettedes vesszőt adott helyen rögzítjük.
				,
Ebben az esetben a legkisebb szám 1/16-od, a legnagyobb pedig 15 egész 15/16, a számítás pontossága 1/16. Mintha a 10-es számrendszerben 1/10000 és 9999,9999 között 1/10000 pontossággal számolnánk. Ezt nevezzük abszolút pontosságnak. A relatív pontosság pedig azt mutatja, hogy hány százalékos a pontosság.
A lebegőpontos ábrázolás esetén a számokat normál alakra hozzuk a 10-es számrendszerben: n*10k, kettes számrendszerben pedig: n*2k. Ahol az n-t mantisszának nevezzük, a k-t pedig karakterisztikának. A 8 bitből mondjuk 5-öt lefoglal a mantissza, 3-at pedig a karakterisztika.
