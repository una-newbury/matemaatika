Siin on ülesannete tekstid, nende samm-sammulised lahendused ja eksamiks vajalik lühike teooriaosa koos valemitega. Kõik matemaatilised väljendid on vormistatud Markdowni ja LaTeX-i abil, mis sobib otse GitHubi README faili jaoks.

---

## Ülesanne 8 (10 punkti)

On antud funktsioon $f(x) = -x^2 - 2x + 3$.

1. Arvutage funktsiooni $f(x)$ nullkohad ja graafiku haripunkti koordinaadid.
2. Joonestage funktsiooni $f(x)$ graafik.
3. Viirutage kujund, mis on piiratud $x$-telje ja funktsiooni $f(x) = -x^2 - 2x + 3$ graafikuga. Arvutage selle kujundi täpne pindala.

### Lahendus

#### 1. Nullkohad ja haripunkt

**Nullkohad:**
Nullkohtade leidmiseks paneme funktsiooni võrduma nulliga:


$$-x^2 - 2x + 3 = 0$$

Korrutame kogu võrrandit $-1$-ga, et lihtsustada lahendamist:


$$x^2 + 2x - 3 = 0$$

Kasutame ruutvõrrandi lahendivalemit (või Viète'i teoreemi):


$$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$

$$x = \frac{-2 \pm \sqrt{2^2 - 4 \cdot 1 \cdot (-3)}}{2 \cdot 1} = \frac{-2 \pm \sqrt{4 + 12}}{2} = \frac{-2 \pm \sqrt{16}}{2} = \frac{-2 \pm 4}{2}$$

$$x_1 = \frac{-2 + 4}{2} = 1$$

$$x_2 = \frac{-2 - 4}{2} = -3$$

Funktsiooni nullkohad on $X_0 = \{-3; 1\}$.

**Haripunkti koordinaadid $H(x_h; y_h)$:**
Haripunkti $x$-koordinaat:


$$x_h = \frac{-b}{2a} = \frac{-(-2)}{2 \cdot (-1)} = \frac{2}{-2} = -1$$

Haripunkti $y$-koordinaat (asendame $x_h$ algsesse funktsiooni):


$$y_h = -(-1)^2 - 2 \cdot (-1) + 3 = -1 + 2 + 3 = 4$$

Graafiku haripunkt on $H(-1; 4)$.

#### 2. Graafiku joonestamine

Kuna ruutliikme kordaja $a = -1$ (negatiivne), avanevad parabooli harud **allapoole**.
Sümmeetriatelg on sirge $x = -1$. Graafiku joonestamiseks on meil olemas:

* Haripunkt: $(-1; 4)$
* Nullkohad (lõikepunktid $x$-teljega): $(-3; 0)$ ja $(1; 0)$
* Lõikepunkt $y$-teljega (kus $x=0$): $(0; 3)$

#### 3. Kujundi pindala arvutamine

Kujund on piiratud parabooli ja $x$-teljega vahemikus $x = -3$ kuni $x = 1$. Kuna selles vahemikus on funktsioon graafiku kohal ($y > 0$), arvutame pindala määratud integraali abil:

$$S = \int_{-3}^{1} (-x^2 - 2x + 3) \, dx$$

Leiame algfunktsiooni:


$$F(x) = \left[ -\frac{x^3}{3} - x^2 + 3x \right]_{-3}^{1}$$

Rakendame Newton-Leibnizi valemit $F(1) - F(-3)$:


$$F(1) = -\frac{1^3}{3} - 1^2 + 3 \cdot 1 = -\frac{1}{3} - 1 + 3 = 2 - \frac{1}{3} = \frac{5}{3}$$

$$F(-3) = -\frac{(-3)^3}{3} - (-3)^2 + 3 \cdot (-3) = -\frac{-27}{3} - 9 - 9 = 9 - 9 - 9 = -9$$

Arvutame vahe:


$$S = F(1) - F(-3) = \frac{5}{3} - (-9) = 9 + \frac{5}{3} = 9 + 1\frac{2}{3} = 10\frac{2}{3}$$

Kujundi täpne pindala on $10\frac{2}{3}$ (või $\frac{32}{3}$) pindalaühikut.

---

## Ülesanne 6 (10 punkti)

Joonisel on funktsiooni $f(x) = x^3 - 6x^2 + 9x - 1$ graafik ja kolm selle graafiku puutujat, mille tõusud on $-1$, $1,5$ ja $3$.

1. Märkige iga puutuja juurde selle tõus. *(Märkus: Kuna joonist ennast tekstis pole, kirjeldame põhimõtet lahenduses).*
2. Leidke funktsiooni $f(x)$
1. tuletis;
2. kasvamis- ja kahanemisvahemikud.


3. Koostage funktsiooni $f(x)$ graafiku puutuja võrrand kohal $x_0 = 4$.

### Lahendus

#### 1. Puutujate tõusude määramine jooniselt

Kuna sirge tõus $k$ näitab sirge suunda:

* Kui sirge **tõuseb** (vasakult paremale liikudes), on tõus positiivne ($1,5$ ja $3$). Mida järsem on tõus, seda suurem on arv (tõus $3$ on järsem kui $1,5$).
* Kui sirge **langeb**, on tõus negatiivne (tõus $-1$).

#### 2. Tuletis ning kasvamis- ja kahanemisvahemikud

**1) Tuletis:**
Leiame funktsiooni $f(x) = x^3 - 6x^2 + 9x - 1$ tuletise, kasutades astmefunktsiooni tuletisreegleid:


$$f'(x) = 3x^2 - 12x + 9$$

**2) Kasvamis- ja kahanemisvahemikud:**
Funktsioon on kasvav seal, kus $f'(x) > 0$, ja kahanev seal, kus $f'(x) < 0$.
Leiame esmalt ekstreemumkohad ehk punktid, kus tuletis on $0$:


$$3x^2 - 12x + 9 = 0$$

Jagame kogu võrrandi $3$-ga:


$$x^2 - 4x + 3 = 0$$

Viète'i teoreemi järgi (või lahendivalemiga):


$$x_1 = 1, \quad x_2 = 3$$

Tuletisliige $f'(x) = 3x^2 - 12x + 9$ on parabool, mis avaneb ülespoole. See tähendab, et:

* Vahemikus $(-\infty; 1)$ on tuletis positiivne ($+$)
* Vahemikus $(1; 3)$ on tuletis negatiivne ($-$)
* Vahemikus $(3; \infty)$ on tuletis positiivne ($+$)

**Vastus:**

* Kasvamisvahemikud: $X \uparrow_1 = (-\infty; 1)$ ja $X \uparrow_2 = (3; \infty)$
* Kahanemisvahemik: $X \downarrow = (1; 3)$

#### 3. Puutuja võrrand kohal $x_0 = 4$

Puutuja võrrandi üldkuju on:


$$y - y_0 = k(x - x_0)$$

Kus:

1. $x_0 = 4$
2. $y_0 = f(x_0) = f(4)$
3. $k = f'(x_0) = f'(4)$

**Arvutame $y_0$:**


$$y_0 = 4^3 - 6 \cdot 4^2 + 9 \cdot 4 - 1 = 64 - 6 \cdot 16 + 36 - 1 = 64 - 96 + 36 - 1 = 3$$

**Arvutame tõusu $k$:**


$$k = f'(4) = 3 \cdot 4^2 - 12 \cdot 4 + 9 = 3 \cdot 16 - 48 + 9 = 48 - 48 + 9 = 9$$

**Koostame võrrandi:**


$$y - 3 = 9(x - 4)$$

$$y - 3 = 9x - 36$$

$$y = 9x - 33$$

Puutuja võrrand on $y = 9x - 33$.

---

## ?? Õpiku lehekülg: Teooria ja Valemid

See osa on mõeldud kordamiseks. Kui põhitõed on ununenud, alusta siit!

### 1. Ruutfunktsioon ja selle graafik

Ruutfunktsiooni üldkuju on:

```math
f(x) = ax^2 + bx + c,\quad a \neq 0

```

* **Graafikuks** on parabool. Kui $a > 0$, avanevad harud üles; kui $a < 0$, avanevad harud alla.
* **Nullkohad ($f(x) = 0$)** leitakse ruutvõrrandi lahendivalemiga:

$$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$


* **Haripunkti $H(x_h; y_h)$** koordinaadid:

$$x_h = \frac{-b}{2a}, \quad y_h = f(x_h)$$



### 2. Tuletis ja funktsiooni uurimine

Tuletis näitab funktsiooni muutumise kiirust (graafiku puutuja tõusu) igas punktis.

**Põhilised tuletisvalemid:**

* $(c)' = 0$ (konstandi tuletis on null)
* $(x)' = 1$
* $(x^n)' = n \cdot x^{n-1}$ (näiteks $(x^3)' = 3x^2$ ja $(x^2)' = 2x$)
* $(c \cdot f(x))' = c \cdot f'(x)$

**Seos graafikuga:**

* Kui vahemikus $f'(x) > 0$, siis funktsioon **kasvab** ($X \uparrow$).
* Kui vahemikus $f'(x) < 0$, siis funktsioon **kahaneb** ($X \downarrow$).
* Punktid, kus $f'(x) = 0$, on **ekstreemumkohad** (seal asuvad graafiku kohalikud tipud ja põhjad).

### 3. Graafiku puutuja sirge võrrand

Funktsiooni graafiku puutuja punktis $(x_0; y_0)$ on sirge, mille võrrand on:

```math
y - y_0 = f'(x_0) \cdot (x - x_0)

```

Kus:

* $x_0$ on antud puutepunkti $x$-koordinaat.
* $y_0 = f(x_0)$ on funktsiooni väärtus selles punktis.
* $k = f'(x_0)$ on funktsiooni tuletise väärtus ehk sirge **tõus**.

### 4. Integraal ja pindala

Määratud integraali abil saab arvutada graafiku ja $x$-telje vahele jääva kujundi pindala.

Kui funktsioon $f(x)$ on vahemikus $[a; b]$ positiivne ($y \ge 0$), siis pindala arvutatakse:

```math
S = \int_{a}^{b} f(x) \, dx = F(b) - F(a)

```

Kus $F(x)$ on algfunktsioon (tuletise vastandtehe).

**Algfunktsiooni leidmise reegel (integreerimine):**


$$\int x^n \, dx = \frac{x^{n+1}}{n+1} + C$$

* Näiteks: $\int x^2 \, dx = \frac{x^3}{3}$ ja $\int x \, dx = \frac{x^2}{2}$
* Arvu (konstandi) integreerimine: $\int c \, dx = cx$
