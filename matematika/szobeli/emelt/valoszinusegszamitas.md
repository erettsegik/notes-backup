Pascal megbízásra foglalkozott szerencsejátékokkal. Játékelmélet.

*Definíció:* A valószínűség egy 0 és 1 közötti pozitív valós szám.

### Eseményalgebra:

*Definíció:* Az A esemény komplementere az az esemény, amely akkor következik be, amikor A nem következik be.

*Definíció:* Az A és B események összege az az esemény, amely akkor következik be, amikor A vagy B bekövetkezik. A+B

*Definíció:* Az A és B események szorzata az az esemény, amely akkor következik be, amikor A és B bekövetkezik. A*B

*Definíció:* Az A és B események egymást kizárják, ha egyszerre nem következhetnek be.

A halmazműveletekhez hasonlóan működnek.

### Kombinatorikai modell:

*Definíció:* Ha elvégzünk n-szer egy kísérletet, és ebből az A esemény k-szor következik be, akkor az A esemény relatív gyakorisága a k/n hányados.

*Definíció:* Ha sokszor elvégzünk egy kísérletet, akkor megfigyelhetjük, hogy egy A esemény relatív gyakorisága egy szám körül ingadozik. Ezt a számot nevezzük az A esemény valószínűségének. P(A)

*Definíció:* A valószínűség kiszámításának klasszikus modelljét akkor alkalmazhatjuk, ha egy kísérletnek véges sok kimenetele van és ezek valószínűsége egyenlő. Ekkor az A esemény valószínűsége: P(A)= kedvező/összes

### A valószínűségszámítás axiómái:

 - Tetszőleges A esemény esetén [latex inline] 0 \leq P(A) \leq 1 [/latex]
 - Biztos esemény valószínűsége 1, lehetetlen eseményé 0
 - Ha A és B egymást kizáró események, akkor [latex inline] P(A + B) = P(A) + P(B) [/latex]
 - Ha A és B tetszőleges esemény, akkor [latex inline] P(A + B) = P(A) + P(B) - P(A * B) [/latex]
 - [latex inline] P(A) + P(\overline{A}) = 1 [/latex]

*Feltételes valószínűség:* Az A esemény B-re vonatkozó feltételes valószínűsége: [latex inline] P(A | B) = \frac{P(A * B)}{P(B)}

 - Ez annak a valószínűsége, hogy az A esemény bekövetkezik, feltéve, hogy a B esemény bekövetkezik.

*Definíció:* A binomiális eloszlás olyan kísérletnél fordul elő, amelynek csak két kimenetele lehetséges: az A és p valószínűséggel bekövetkezik, vagy 1-p valószínűséggel nem következik be.

*Tétel:* Binomiális eloszlásnál ha a kísérletet n-szer ismételjük, akkor annak a valószínűsége, hogy az A esemény k-szok következik be éppen:
[latex] P(\xi = k) = {n \choose k} * p^k * (1 - p)^{n - k}  \text{,ahol } k \leq n. [/latex]

 - Binomiális eloszlásra vezetnek a visszatevéses mintavétel esetei, ahol n elem közül p valószínűséggel választunk valamilyen tulajdonsággal rendelkezőt oly módon, hogy a kivett elemet az újabb húzás előtt visszatesszük.

*Definíció:* A visszatevés nélküli mintavétel eloszlását hipergeometrikus eloszlásnak nevezzük.

*Tétel:* Hipergeometrikus eloszlásnál legyen N db elemünk, amelyből M db elem rendelkezik egy adott A tulajdonsággal, N-M db pedig nem. Kiválasztunk véletlenszerűen visszatevés nélkül n db-ot. Annak a valószínűsége, hogy a kihúzott n db elem közül k db rendelkezik az A tulajdonsággal:

[latex] P(\xi = k) = \frac{{M \choose k} * {N - M \choose n - k}}{{N \choose n}}  \text{,ahol } k \leq n. [/latex]

#### Bayes-tétel:

Arra jó, hogy ha az egyik esemény a másikra vonatkozó feltételes valószínűségét ismerem akkor meg tudjam fordítani.

[latex] P(B_k | A) = \frac{P(A | B_k) * P(B_k)}{\sum_{i=1}^{n} P(A | B_i) * P(B_i)} [/latex]

*Alkalmazások:*

 - amit a kombinatorikában többé-kevésbé
 - Bayes tétel alapján sok spamszűrő működik -> szóelemzés
 - Gyakorisági elemzés
 - Kódfejtés
