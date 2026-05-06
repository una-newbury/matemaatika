### Ülesanne 11. (10 punkti)

**1.** Andrus võitis lotoga 48?000 eurot ja kasutas sellest kaks kolmandikku kinnisvara ostuks. Mitme euro võrra suureneb ostetud kinnisvara väärtus kolme aastaga eeldusel, et kinnisvara väärtus kasvab iga aastaga 2,25% võrra?

**2.** Lahendage võrrand $\log_4(3-x)+\log_4(x+2)=1$.

---

## Lahendused

### Ülesanne 1 — väärtuse kasv (sammud)
Ostetud summa on kaks kolmandikku summast $48\,000$.
```math
S_0 = \tfrac{2}{3}\cdot 48000 = 32000
```
Aastane kasvumäär on $2{,}25\%$, st kasvufaktor iga aasta kohta on $1+0{,}0225=1{,}0225$. Kolme aasta järel on väärtus
```math
S_3 = S_0\cdot 1{,}0225^3
```
Arvutame kasvu eurodes:
```math
\Delta S = S_3 - S_0 = S_0\bigl(1{,}0225^3-1\bigr)
```
Asendades $S_0=32000$:
```math
\Delta S = 32000\bigl(1{,}0225^3-1\bigr)
```
Arvutame ligikaudu:
```math
1{,}0225^3 \approx 1{,}0225\cdot1{,}0225\cdot1{,}0225 \approx 1{,}0686
```
Seega
```math
\Delta S \approx 32000\cdot 0{,}0686 \approx 2195{,}2
```
**Vastus:** ostetud kinnisvara väärtus suureneb umbes **2195,20 eurot** kolme aastaga.

*(Märkus: täpsema arvu saab kalkulaatoriga; valem ja sammud on ülal.)*   [GeeksForGeeks](https://www.geeksforgeeks.org/maths/geometric-sequence-formulas/)

---

### Ülesanne 2 — logaritmiline võrrand
Võrrand on
```math
\log_4(3-x)+\log_4(x+2)=1.
```
Kasutame logaritmi omadust: $\log_a u+\log_a v=\log_a(uv)$. Seega
```math
\log_4\bigl((3-x)(x+2)\bigr)=1.
```
See tähendab
```math
(3-x)(x+2)=4^1=4.
```
Lahendame ruutvõrrandi:
```math
(3-x)(x+2)=3x+6 - x^2 -2x = -x^2 + x +6 =4
```
Seega
```math
-x^2 + x +6 =4 \quad\Rightarrow\quad -x^2 + x +2 =0
```
Korrutame -1-ga:
```math
x^2 - x -2 =0
```
Lahendame diskriminandi abil:
```math
\Delta = (-1)^2 -4\cdot1\cdot(-2)=1+8=9
```
Seega juured
```math
x = \frac{1\pm\sqrt{9}}{2} = \frac{1\pm3}{2}
```
Saame $x=2$ või $x=-1$. Kontrollime logaritmide defineerimispiire: argumendid peavad olema positiivsed:
- Kui $x=2$: $3-x=1>0$, $x+2=4>0$ — sobib.
- Kui $x=-1$: $3-(-1)=4>0$, $-1+2=1>0$ — sobib.

**Vastus:** $x=2$ või $x=-1$.   [Mathematics Stack Exchange](https://math.stackexchange.com/questions/1136935/properties-of-geometric-series)

---

## Õpikulehed: jada ja seeriad (vajalikud valemid)

#### Aritmeetiline jada
- $a_n = a_1 + (n-1)d$.
- Summa $S_n = \dfrac{n}{2}(a_1+a_n)=\dfrac{n}{2}\bigl(2a_1+(n-1)d\bigr)$.   [Math Portal](https://www.mathportal.org/formulas/series_formulas.pdf)

#### Geomeetriline jada
- $g_n = g_1\cdot q^{\,n-1}$.
- Lõpliku summa $S_n = g_1\cdot\dfrac{1-q^n}{1-q}$ kui $q\neq1$.
- Lõpmatu summa (kui $|q|<1$): $S_\infty=\dfrac{g_1}{1-q}$.   [Wikipedia](https://en.wikipedia.org/wiki/Geometric_series)  [GeeksForGeeks](https://www.geeksforgeeks.org/maths/geometric-sequence-formulas/)

#### Muud kasulikud valemid
- Geomeetrilise jada suhe kahe järjestikuse liikme vahel: $q=\dfrac{g_{n+1}}{g_n}$.
- Logaritmide põhivõrrandid: $\log_a u+\log_a v=\log_a(uv)$, $\log_a u-\log_a v=\log_a(u/v)$, $\log_a u^k = k\log_a u$.   [Studying of mathematics online](https://onlinemschool.com/math/formula/geometric_sequence/)  [Mathematics Stack Exchange](https://math.stackexchange.com/questions/1136935/properties-of-geometric-series)
