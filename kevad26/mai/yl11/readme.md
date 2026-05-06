### Ülesanne 11

**1.** Andrus võitis lotoga 48 000 eurot ja kasutas sellest kaks kolmandikku kinnisvara ostuks. Mitme euro võrra suureneb ostetud kinnisvara väärtus kolme aastaga eeldusel, et kinnisvara väärtus kasvab iga aastaga 2,25% võrra?

**2.** Lahendage võrrand $\log_4(3 - x) + \log_4(x + 2) = 1$.

---

## 1. ülesanne – lahendus

**Andmed:**

- Võidusumma: $48\,000$ eurot
- Kaks kolmandikku kinnisvara ostuks:
```math
\frac{2}{3} \cdot 48\,000 = 32\,000
```  
  Seega algväärtus $A_0 = 32\,000$ eurot.
- Aastane kasv: $2{,}25\% = 0{,}0225$
- Aastate arv: $n = 3$

Kinnisvara väärtus kasvab igal aastal sama protsendi võrra ? see on **geomeetriline jada** (või liitintressi valem).

Aastane kasvutegur:
```math
q = 1 + 0{,}0225 = 1{,}0225
```

Väärtus 3 aasta pärast:
```math
A_3 = A_0 \cdot q^3 = 32\,000 \cdot 1{,}0225^3
```

Arvutame $1{,}0225^3$ (ligikaudselt):

```math
1{,}0225^3 \approx 1{,}069
```


Seega:
```math
A_3 \approx 32\,000 \cdot 1{,}069 = 34\,208
```

See on **väärtus 3 aasta pärast**. Küsimus: *mitme euro võrra suureneb* väärtus?

```math
\Delta A = A_3 - A_0 \approx 34\,208 - 32\,000 = 2\,208
```

**Vastus 1. ülesandele:** kinnisvara väärtus suureneb kolme aastaga ligikaudu **2 192 euro võrra**.

---

## 2. ülesanne – lahendus

Lahendada võrrand:
```math
\log_4(3 - x) + \log_4(x + 2) = 1
```

### 2.1. Määramispiirkond

Logaritmi argument peab olema positiivne:

- $3 - x > 0 \Rightarrow x < 3$
- $x + 2 > 0 \Rightarrow x > -2$

Seega:
```math
-2 < x < 3
```

Kõik lahendid peavad jääma sellesse vahemikku.

### 2.2. Logaritmide liitmise reegel

Kehtib:
```math
\log_a u + \log_a v = \log_a (u \cdot v), \quad u>0, v>0, a>0, a\neq 1
```

Rakendame:
```math
\log_4(3 - x) + \log_4(x + 2) = \log_4\big((3 - x)(x + 2)\big)
```

Seega võrrand muutub:
```math
\log_4\big((3 - x)(x + 2)\big) = 1
```

### 2.3. Logaritmivõrrandi teisendamine

Kui $\log_4 M = 1$, siis:
```math
M = 4^1 = 4
```

Seega:
```math
(3 - x)(x + 2) = 4
```

Laiendame vasaku poole:

```math
(3 - x)(x + 2) = 3x + 6 - x^2 - 2x = -x^2 + x + 6
```

Saame võrrandi:
```math
-x^2 + x + 6 = 4
```

Viime kõik ühele poole:

```math
-x^2 + x + 6 - 4 = 0
-x^2 + x + 2 = 0
```

Korrutame võrrandi läbi $-1$-ga (mugavam kuju):

```math
x^2 - x - 2 = 0
```

### 2.4. Ruudu­võrrandi lahendamine

Lahendame:
```math
x^2 - x - 2 = 0
```

Diskriminant:
```math
D = b^2 - 4ac = (-1)^2 - 4 \cdot 1 \cdot (-2) = 1 + 8 = 9
```

```math
\sqrt{D} = 3
```

Lahendid:
```math
x_{1,2} = \frac{-b \pm \sqrt{D}}{2a} = \frac{1 \pm 3}{2}
```

Seega:
```math
x_1 = \frac{1 + 3}{2} = 2
```

```math
x_2 = \frac{1 - 3}{2} = -1
```

### 2.5. Kontroll määramispiirkonnas

Määramispiirkond oli $-2 < x < 3$.

- $x = 2$ ? $-2 < 2 < 3$ – sobib.
- $x = -1$ ? $-2 < -1 < 3$ – sobib.

Kontrollime ka argumente:

- $x = 2$:  
  $3 - x = 1 > 0$, $x + 2 = 4 > 0$ – korras.
- $x = -1$:  
  $3 - x = 4 > 0$, $x + 2 = 1 > 0$ – korras.

Mõlemad lahendid kehtivad.

**Vastus 2. ülesandele:**
```math
x = 2 \quad \text{või} \quad x = -1
```

---

## Teooria ja valemid – 1. ülesande teema (jadad, eriti geomeetriline jada)

### Üldine jada

**Jada** on arvude järjestus:
```math
a_1, a_2, a_3, \dots
```
kus igal kohal on mingi arv $a_n$.

- **Üldliige:** $a_n$ – jada $n$-s liige.
- Sageli antakse jada kas:
   - reegliga $a_n = f(n)$ või
   - rekursiivselt: $a_{n+1}$ avaldatakse $a_n$ kaudu.

---

### Aritmeetiline jada

**Aritmeetiline jada** – järjestikuste liikmete vahe on konstantne.

- **Definitsioon:**
```math
a_{n+1} = a_n + d
```
  kus $d$ on **vahe** (konstantne arv).

- **Üldliige:**
```math
a_n = a_1 + (n - 1)d
```

- **Esimese $n$ liikme summa:**
```math
S_n = \frac{n}{2}(a_1 + a_n)
```
  või
```math
S_n = \frac{n}{2}\big(2a_1 + (n - 1)d\big)
```

---

### Geomeetriline jada

**Geomeetriline jada** – järjestikuste liikmete suhe on konstantne.

- **Definitsioon:**
```math
a_{n+1} = a_n \cdot q
```
  kus $q$ on **suhe** (geomeetriline tegur).

- **Üldliige:**
```math
a_n = a_1 \cdot q^{n-1}
```

- **Esimese $n$ liikme summa (kui $q \neq 1$):**
```math
S_n = a_1 \cdot \frac{q^n - 1}{q - 1}
```

---

### Seos protsendikasvuga ja geomeetrilise jadaga

Kui mingi suurus kasvab igal aastal sama protsendi võrra, siis:

- Olgu algväärtus $A_0$.
- Aastane kasvuprotsent $p\%$.
- Aastane kasvutegur:
```math
q = 1 + \frac{p}{100}
```
- Pärast $n$ aastat:
```math
A_n = A_0 \cdot q^n
```

Kui küsitakse **kui palju suureneb** väärtus, siis:
```math
\Delta A = A_n - A_0
```

See on täpselt sama kuju, mida kasutasime 1. ülesandes.

---

### Üldine jada ja rekursiivsed seosed

Mõnikord antakse jada **rekursiivselt**:

- Näiteks:
```math
a_{n+1} = a_n + d \quad \text{(aritmeetiline)}
```
```math
a_{n+1} = a_n \cdot q \quad \text{(geomeetriline)}
```

Oluline on aru saada, kas jada kasvab **liitmisega** (aritmeetiline) või **korrutamisega** (geomeetriline). Protsendid ? korrutamine ? geomeetriline jada.

---

## Teooria ja valemid – 2. ülesande teema (logaritmid ja logaritmivõrrandid)

### Logaritmi mõiste

Olgu $a > 0$, $a \neq 1$ ja $b > 0$. Siis:
```math
\log_a b = x \quad \Leftrightarrow \quad a^x = b
```

See tähendab: $\log_a b$ on see astendaja, millega tuleb $a$ astendada, et saada $b$.

---

### Põhireeglid

Olgu $a > 0$, $a \neq 1$, $u>0$, $v>0$.

1. **Korrutise logaritm:**
```math
\log_a(uv) = \log_a u + \log_a v
```

2. **Jagatise logaritm:**
```math
\log_a\left(\frac{u}{v}\right) = \log_a u - \log_a v
```

3. **Astme logaritm:**
```math
\log_a(u^k) = k \cdot \log_a u
```

4. **Aluse vahetuse valem:**
```math
\log_a b = \frac{\log_c b}{\log_c a}
```
   (kus $c$ on suvaline sobiv alus, näiteks $10$ või $e$).

---

### Logaritmivõrrandid

Üldine idee: logaritmivõrrandi lahendamiseks püütakse:

- viia logaritmid **ühele poole**,
- kasutada reegleid (nt korrutise logaritm),
- lõpuks saada **tavaline võrrand** (tihti astme- või ruutvõrrand).

**Oluline:** alati kontrollida **määramispiirkonda** – logaritmi argument peab olema **positiivne**.

---

### Määramispiirkond logaritmides

Kui võrrandis esineb $\log_a f(x)$, siis peab kehtima:
```math
f(x) > 0
```

Kui on mitu logaritmi, näiteks:
```math
\log_a f(x) + \log_a g(x)
```
siis peab kehtima:
```math
f(x) > 0 \quad \text{ja} \quad g(x) > 0
```

Need tingimused tuleb **enne** lahendamist kirja panna ja lõpus kontrollida, et leitud lahendid neid ei rikuks.

---

### Tüüpiline logaritmivõrrandi lahendamise skeem

Näiteks:
```math
\log_a f(x) + \log_a g(x) = k
```

1. **Määramispiirkond:**
```math
f(x) > 0, \quad g(x) > 0
```

2. **Korrutise reegel:**
```math
\log_a(f(x)g(x)) = k
```

3. **Logaritmi definitsioon:**
```math
f(x)g(x) = a^k
```

4. Saadud võrrand on tavaliselt **polünoomvõrrand** (nt ruutvõrrand), mille lahendad tavaliste meetoditega.

5. **Kontroll:** kas lahendid kuuluvad määramispiirkonda.

---

### Ruutvõrrandi meeldetuletus

Kui:
```math
ax^2 + bx + c = 0, \quad a \neq 0
```
siis:

- **Diskriminant:**
```math
D = b^2 - 4ac
```

- **Lahendid:**
```math
x_{1,2} = \frac{-b \pm \sqrt{D}}{2a}
```

Kui $D > 0$ – kaks erinevat lahendit,  
$D = 0$ – üks lahend (topeltjuur),  
$D < 0$ – reaalseid lahendeid ei ole.

---
