**Lühike vastus:** Allpool on ülesanne täpselt kirjas, seejärel põhjalikud samm‑sammult lahendused, iga sammile on lisatud viide õpikulehelt pärit valemile; lõpus on pikem „õpikuleht“ jada‑valemitega (aritmeetiline, geomeetriline ja üldised jada‑mõisted). **Oluline:** matemaatika inline‑avaldised on $...$ ja ridade kaupa kujutatud `math` plokkides.   [Physics & Maths Tutor](https://pmt.physicsandmathstutor.com/download/Maths/A-level/Pure/Sequences-and-Series-2/Cheat-Sheets/Sequences%20and%20Series.pdf)  [allen.in](https://allen.in/jee/maths/arithmetic-and-geometric-sequence)

### Ülesanne 11. (10 punkti)

**1.** Andrus võitis lotoga 48 000 eurot ja kasutas sellest kaks kolmandikku kinnisvara ostuks. Mitme euro võrra suureneb ostetud kinnisvara väärtus kolme aastaga eeldusel, et kinnisvara väärtus kasvab iga aastaga $2{,}25\%$ võrra?

**2.** Lahendage võrrand $ \log_4(3-x)+\log_4(x+2)=1$.

---

## Lahendused (sammud ja viited õpikulehele)

### Ülesanne 1 — väärtuse kasv
**Ülesande tekst:** $48\,000$ eurot; ostuks kasutatud osa $ \tfrac{2}{3} $; aastane kasv $2{,}25\%$; aeg $3$ aastat.

**Samm 1 — algsumma ostuks.** Kasutame lihtsat korrutamist (õpik: geomeetrilise kasvu rakendamiseks algväärtus).
```math
S_0 = \tfrac{2}{3}\cdot 48000 = 32000
```
*(Valem viide: algväärtuse leidmine; õpikuleht, jada/reaalsed rakendused.)*   [Mathematics LibreTexts](https://math.libretexts.org/Bookshelves/Algebra/College_Algebra_and_Trigonometry_%28Beveridge%29/06%3A_Sequences_and_Series/6.02%3A_Arithmetic_and_Geometric_Sequences)

**Samm 2 — aastane kasvufaktor.** Kui kasv $p=2{,}25\%$, siis kasvufaktor $q=1+p=1{,}0225$. (Õpik: protsendi teisendamine kasvufaktoriks.)   [allen.in](https://allen.in/jee/maths/arithmetic-and-geometric-sequence)

**Samm 3 — kolmeaastane väärtus (geomeetriline kordne kasv).** Kasutame geomeetrilise kasvufunktsiooni $S_n = S_0\cdot q^n$.
```math
S_3 = S_0\cdot 1{,}0225^3
```
*(Valem viide: geomeetrilise jada üldliige $g_n=g_1\cdot q^{n-1}$; siin kordne rakendus ajapikkusega 3.)*   [Physics & Maths Tutor](https://pmt.physicsandmathstutor.com/download/Maths/A-level/Pure/Sequences-and-Series-2/Cheat-Sheets/Sequences%20and%20Series.pdf)  [allen.in](https://allen.in/jee/maths/arithmetic-and-geometric-sequence)

**Samm 4 — kasv eurodes.**
```math
\Delta S = S_3 - S_0 = S_0\bigl(1{,}0225^3-1\bigr)
```
Asendame $S_0=32000$ ja arvutame ligikaudu:
```math
1{,}0225^3 \approx 1{,}0686
```
```math
\Delta S \approx 32000\cdot 0{,}0686 \approx 2195{,}20
```
**Vastus:** kinnisvara väärtus suureneb umbes **$2195{,}20\ \text{€}$** kolme aastaga. (Arvutuslik ligikaudne tulemus; täpsema väärtuse saab kalkulaatoriga.)   [allen.in](https://allen.in/jee/maths/arithmetic-and-geometric-sequence)

---

## Õpikuleht (laiendatud): mis on jada ja peamised valemid
- **Jada (sequence)** on järjestatud elementide rida; **seeria (series)** on nende elementide summa.   [Physics & Maths Tutor](https://pmt.physicsandmathstutor.com/download/Maths/A-level/Pure/Sequences-and-Series-2/Cheat-Sheets/Sequences%20and%20Series.pdf)  [Mathematics LibreTexts](https://math.libretexts.org/Bookshelves/Algebra/College_Algebra_and_Trigonometry_%28Beveridge%29/06%3A_Sequences_and_Series/6.02%3A_Arithmetic_and_Geometric_Sequences)
- **Aritmeetiline jada:** $a_n=a_1+(n-1)d$, summa $S_n=\dfrac{n}{2}(2a_1+(n-1)d)$.   [Physics & Maths Tutor](https://pmt.physicsandmathstutor.com/download/Maths/A-level/Pure/Sequences-and-Series-2/Cheat-Sheets/Sequences%20and%20Series.pdf)
- **Geomeetriline jada:** $g_n=g_1\cdot q^{\,n-1}$, summa $S_n=g_1\cdot\dfrac{1-q^n}{1-q}$ ($q\neq1$), lõpmatu summa $S_\infty=\dfrac{g_1}{1-q}$ kui $|q|<1$.   [allen.in](https://allen.in/jee/maths/arithmetic-and-geometric-sequence)  [Brilliant](https://brilliant.org/wiki/arithmetic-geometric-progression/)

---

### Ülesanne 11. (10 punkti)

**1.** Andrus võitis lotoga 48?000 eurot ja kasutas sellest kaks kolmandikku kinnisvara ostuks. Mitme euro võrra suureneb ostetud kinnisvara väärtus kolme aastaga eeldusel, et kinnisvara väärtus kasvab iga aastaga $2{,}25\%$ võrra?

**2.** Lahendage võrrand $ \log_4(3-x)+\log_4(x+2)=1$.

---

## Lahendused (põhjalikult, iga sammile viide õpikulehelt)

### Ülesanne 1 — väärtuse kasv (täpne samm-sammult lahendus)

**Ülesande tekst kokku:** algsumma €$48\,000$, ostuks kasutatud osa $ \tfrac{2}{3} $, aastane kasv $2{,}25\%$, aeg $3$ aastat.

**Samm 1 — ostuks kasutatud summa leidmine.**  
Kasutame lihtsat korrutamist: ostuks $S_0 = \tfrac{2}{3}\cdot 48000$.
```math
S_0 = \tfrac{2}{3}\cdot 48000 = 32000
```
**(Õpikuleht viide:** *Protsendid ja algväärtuse leidmine; aritmeetika põhitehe.*)

**Samm 2 — protsendi teisendamine kasvufaktoriks.**  
Kui aastane kasv on $p=2{,}25\%$, siis kasvufaktor $q=1+p=1{,}0225$.
```math
q = 1 + 0{,}0225 = 1{,}0225
```
**(Õpikuleht viide:** *Protsentide teisendamine kümnendmurdudeks; geomeetrilise kasvu mõiste.*)

**Samm 3 — kolmeaastane väärtus geomeetrilise kasvu valemi abil.**  
Geomeetrilise kasvu valem: $S_n = S_0\cdot q^n$. Siin $n=3$.
```math
S_3 = S_0\cdot 1{,}0225^3
```
**(Õpikuleht viide:** *Geomeetriline jada / kordne kasv: $g_n=g_1\cdot q^{n-1}$ või ajas kasvuks $S_n=S_0 q^n$.)*

**Samm 4 — kasv eurodes (erinevus).**
```math
\Delta S = S_3 - S_0 = S_0\bigl(1{,}0225^3-1\bigr)
```
Asendame $S_0=32000$:
```math
\Delta S = 32000\bigl(1{,}0225^3-1\bigr)
```
**(Õpikuleht viide:** *Geomeetrilise kasvu rakendamine ja muutuse (diferentsi) leidmine.)*

**Samm 5 — numbriline ligikaudne arvutus.**  
Arvutame $1{,}0225^3$ ligikaudu:
```math
1{,}0225^3 \approx 1{,}0225\cdot1{,}0225\cdot1{,}0225 \approx 1{,}0686
```
Seega
```math
\Delta S \approx 32000\cdot 0{,}0686 \approx 2195{,}20
```
**(Õpikuleht viide:** *Lõplik arvutus; ümardamine rahalistes ühikutes.)*

**Lõplik vastus:** kinnisvara väärtus suureneb umbes **$2195{,}20\ \text{€}$** kolme aastaga.

---

### Ülesanne 2 — logaritmiline võrrand (detailne, iga sammile viide õpikulehelt)

**Ülesande tekst:** $ \log_4(3-x)+\log_4(x+2)=1$.

**Samm 1 — kontrollime defineerimispiire (oluline samm enne lahendamist).**  
Logaritmi argument peab olema positiivne: $3-x>0$ ja $x+2>0$. See annab tingimused:
```math
3-x>0 \Rightarrow x<3
```
```math
x+2>0 \Rightarrow x>-2
```
Seega lubatud $x$ vahemik on $-2<x<3$.  
**(Õpikuleht viide:** *Logaritmide defineerimispiirid; enne lahendamist kontrolli argumentide positiivsust.)*

**Samm 2 — logaritmide liitmise reegel.**  
Kasutame valemit $ \log_a u + \log_a v = \log_a(uv)$. Seega:
```math
\log_4\bigl((3-x)(x+2)\bigr)=1
```
**(Õpikuleht viide:** *Logaritmide omadused: summa ? korrutis.)*

**Samm 3 — teisendus eksponentvõrrandiks.**  
Kui $\log_4(Y)=1$, siis $Y=4^1=4$. Seega:
```math
(3-x)(x+2)=4
```
**(Õpikuleht viide:** *Logaritmi ja eksponenti vastastikune seos: $\log_a Y = b \Leftrightarrow Y = a^b$.)*

**Samm 4 — laiendame ja viime ruutvõrrandi standardkuju.**  
Laiendame:
```math
(3-x)(x+2) = 3x +6 - x^2 -2x = -x^2 + x +6
```
Seame võrdseks 4-ga:
```math
-x^2 + x +6 = 4 \quad\Rightarrow\quad -x^2 + x +2 = 0
```
Korrutame $-1$-ga, et saada standardne kuju:
```math
x^2 - x - 2 = 0
```
**(Õpikuleht viide:** *Ruutvõrrandi teisendamine standardkujule.)*

**Samm 5 — lahendame ruutvõrrandi diskriminandi abil.**  
Diskriminant:
```math
\Delta = b^2 - 4ac = (-1)^2 - 4\cdot1\cdot(-2) = 1 + 8 = 9
```
Juured:
```math
x = \frac{-b \pm \sqrt{\Delta}}{2a} = \frac{1 \pm 3}{2}
```
Seega:
```math
x_1 = \frac{1+3}{2} = 2,\qquad x_2 = \frac{1-3}{2} = -1
```
**(Õpikuleht viide:** *Ruutvõrrandi lahendivalem ja diskriminant.)*

**Samm 6 — kontrollime, kas leitud juured jäävad defineerimisvahemikku.**  
Meie eelnevalt leitud lubatud vahemik oli $-2<x<3$. Mõlemad juured $x=2$ ja $x=-1$ rahuldavad seda. Samuti kontrollime, et logaritmide argumendid ei muutu nulliks ega negatiivseks:
- $x=2$: $3-x=1>0$, $x+2=4>0$ — sobib.
- $x=-1$: $3-(-1)=4>0$, $-1+2=1>0$ — sobib.

**Lõplik vastus:** $x=2$ või $x=-1$.

---

## Õpikuleht: **Logaritmid** (lai ja praktiline kokkuvõte — kõik olulised valemid ja reeglid)

**Mis on logaritm?**  
Logaritm $ \log_a b $ on arv $c$, mis rahuldab $a^c = b$, kus $a>0$, $a\neq1$, ja $b>0$. Seega $ \log_a b = c \Leftrightarrow a^c = b$.

**Põhivalemid ja omadused**
- **Eksponent-logaritmi vastastikkus:**
  ```math
  \log_a b = c \quad\Leftrightarrow\quad a^c = b
  ```
- **Toote reegel:**
  ```math
  \log_a(uv) = \log_a u + \log_a v
  ```
- **Jagatise reegel:**
  ```math
  \log_a\!\left(\frac{u}{v}\right) = \log_a u - \log_a v
  ```
- **Astme reegel:**
  ```math
  \log_a(u^k) = k\log_a u
  ```
- **Muudatuse alus (change of base) valem:**
  ```math
  \log_a b = \frac{\log_c b}{\log_c a}
  ```
  eriti kasulik:
  ```math
  \log_a b = \frac{\ln b}{\ln a} = \frac{\log_{10} b}{\log_{10} a}
  ```
- **Null ja üks:**
  ```math
  \log_a 1 = 0,\qquad \log_a a = 1
  ```
- **Defineerimispiir:** argument peab olema positiivne: $u>0$.

**Logaritmiliste võrrandite lahendamise üldised sammud**
1. **Kontrolli defineerimispiire:** kõik logaritmi argumendid peavad olema $>0$.
2. **Kombineeri logaritmid:** kasuta toote/jaotuse/astme reegleid, et vähendada logaritmide arvu.
3. **Teisenda eksponentvõrrandiks:** kui saad $\log_a(\text{something}) = b$, siis lahenda $\text{something} = a^b$.
4. **Lahenda saadud algebrailine võrrand** (ruutvõrrand, polünoom jms).
5. **Kontrolli leitud lahendite sobivust** defineerimispiiriga (välista argumendi =0 juhtumid).

**Logaritmide võrrandite tüübid ja näpunäited**
- Kui logaritmid on erinevate alustega, kasuta muutmise alusvalemit, et viia samale alusele või kasutada naturaallogaritmi $\ln$.
- Kui võrrandis on logaritmide summa, proovige kombineerida korrutiseks; kui erinevus, siis jagatise reegel.
- Kui logaritm on astmes (nt $\log_a(f(x)) = g(x)$), teisenda eksponentvõrrandiks $f(x) = a^{g(x)}$ ja lahenda.
- Pärast algebrailist lahendamist **kontrolli alati**, et argumendid oleksid positiivsed.

**Logaritmide seosed eksponentidega (kasulik mõistmiseks)**
- Eksponentsed kasvumudelid $y = a^x$ ja logaritmilised mudelid $x = \log_a y$ on üksteise pöördfunktsioonid.
- Kui lahendad võrrandeid, kus muutuja on eksponendis, kasuta logaritmi; kui muutuja on logaritmis, teisenda eksponendiks.

**Näited (kiirülevaade)**
- Lahenda $\log_2(x-1) + \log_2(x+3) = 3$.  
  *Kombineeri:* $\log_2\bigl((x-1)(x+3)\bigr)=3 \Rightarrow (x-1)(x+3)=8$; lahenda polünoom; kontrolli $x$-i, et argumendid oleksid positiivsed.
- Lahenda $\log_3(x) - \log_3(2x-1) = 1$.  
  *Kombineeri:* $\log_3\!\left(\dfrac{x}{2x-1}\right)=1 \Rightarrow \dfrac{x}{2x-1}=3 \Rightarrow x=3(2x-1)$; lahenda ja kontrolli.

**Logaritmide graafik ja käitumine (lühike)**
- Kui alus $a>1$, siis $\log_a x$ on kasvav funktsioon; kui $0<a<1$, siis $\log_a x$ on kahanev.
- $\log_a x$ on defineeritud ainult $x>0$, läheneb $-\infty$ kui $x\to0^+$ ja läheneb $\infty$ kui $x\to\infty$ (kui $a>1$).

**Kasutusvaldkonnad ja miks neid vaja on**
- Logaritme kasutatakse eksponentsiaalse kasvu ja kahanemise modelleerimisel (nt intressid, radioaktiivne lagunemine), skaalade teisendamisel (detsibelid, pH), ning võrrandite lahendamisel, kus muutuja on eksponendis.

---
