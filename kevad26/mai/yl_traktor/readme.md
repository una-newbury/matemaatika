### Ülesanne (ekstrakt pildilt)

Uus aitraktor maksab 30 000 eurot. Selle traktori hind väheneb iga aastaga ühe ja sama protsendi võrra ning kahe aasta pärast maksab aitraktor 26 508 eurot.

1. Mitme protsendi võrra väheneb igal aastal aitraktori hind?
2. Mis on selle aitraktori hind 5 aasta pärast? Vastus ümardage täpsusega 10 eurot.
3. Mis aasta lõpuks on aitraktori hind vähemalt poole võrra väiksem alg­hinnast?

---

### Lahendus (parandatud ja kontrollitud)

#### Üldine valem

```math
L = A\left(1 - \frac{p}{100}\right)^n,
```

kus  
$L$ – lõpphind,  
$A$ – alg­hind,  
$p$ – iga-aastane vähenemisprotsent,  
$n$ – aastate arv.

---

#### 1) Iga-aastane vähenemisprotsent

Antud:  
$A = 30000$,  
$L = 26508$,  
$n = 2$.

```math
26508 = 30000\left(1 - \frac{p}{100}\right)^2
```

```math
\left(1 - \frac{p}{100}\right)^2 = \frac{26508}{30000}
```

```math
1 - \frac{p}{100} = \sqrt{\frac{26508}{30000}}
```

Arvutame:

```math
\frac{26508}{30000} \approx 0.8836
```

```math
\sqrt{0.8836} \approx 0.9406
```

```math
1 - \frac{p}{100} \approx 0.9406
```

```math
\frac{p}{100} \approx 1 - 0.9406 = 0.0594
```

```math
p \approx 5.94\%
```

Ümardades: iga-aastane hinnalangus on umbes $6\%$.

**Kontroll:**  
Kui $p \approx 5.94\%$, siis tegur on $1 - \frac{p}{100} \approx 0.9406$,  
$30000 \cdot 0.9406^2 \approx 26508$ – sobib.

---

#### 2) Traktori hind 5 aasta pärast

Kasutame sama iga-aastast vähenemist. Võime kasutada kas täpsemat tegurit $0.9406$ või ümardatud $0.94$. Ülesandes on kasutatud $0.94$, vaatame, kas vastus on mõistlik.

```math
L = 30000 \cdot 0.94^5
```

Arvutame ligikaudu:

```math
0.94^2 \approx 0.8836
```

```math
0.94^3 \approx 0.8836 \cdot 0.94 \approx 0.8306
```

```math
0.94^4 \approx 0.8306 \cdot 0.94 \approx 0.7807
```

```math
0.94^5 \approx 0.7807 \cdot 0.94 \approx 0.7339
```

```math
L \approx 30000 \cdot 0.7339 \approx 22017
```

Ümardades 10 euro täpsuseni:

```math
L \approx 22020\ \text{eurot}
```

See langeb kokku pildil oleva vastusega, seega lahendus on sisuliselt korrektne.

---

#### 3) Millise aasta lõpuks on hind vähemalt poole võrra väiksem?

Tõlgendame küsimust nii: leida väikseim täisarvuline $n$, mille korral

```math
L \leq \frac{1}{2}A.
```

Meil on $A = 30000$, seega $\frac{1}{2}A = 15000$.

```math
15000 = 30000 \left(1 - \frac{p}{100}\right)^n
```

Kuna eelnevalt kasutati tegurit $0.94$, jätkame sellega:

```math
15000 = 30000 \cdot 0.94^n
```

```math
0.5 = 0.94^n
```

Võtame logaritmid:

```math
\log 0.5 = \log 0.94^n = n \log 0.94
```

```math
n = \frac{\log 0.5}{\log 0.94}
```

Arvutame ligikaudu:

```math
\log 0.5 \approx -0.3010,\quad \log 0.94 \approx -0.0269
```

```math
n \approx \frac{-0.3010}{-0.0269} \approx 11.2
```

See tähendab, et pärast umbes $11.2$ aastat on hind pooleks langenud. Aastate arvu peab võtma täisarvuna ülespoole, sest alles 12. aasta lõpus on hind **kindlasti** alla poole algväärtusest.

Seega:

```math
n = 12
```

**Vastus:** 12. aasta lõpuks on traktori hind alla poole esialgsest väärtusest.

---

### Vigade ja märkuste kokkuvõte

- **1. küsimus:** arvutus $p \approx 6\%$ on sisuliselt õige (täpsemalt umbes $5.94\%$).
- **2. küsimus:** $L \approx 22020\ €$ (10 euro täpsuseni) on korrektne.
- **3. küsimus:** väide, et küsimus on ebakorrektne, ei ole põhjendatud – küsimus on täiesti üheselt mõistetav, kui tõlgendada seda nii, et otsitakse esimest aastat, mille lõpuks hind on **vähemalt** poole võrra väiksem (st $\leq 15000$). Lahendus logaritmidega ja järeldus „12. aasta lõpus” on korrektne; kommentaar aastani 2100 on eksitav ja mittevajalik.

---

## “Õpiku lehekülg” – vajalik teooria eksamiks

### Eksponentsiaalne kasvamine ja kahanemine

#### Üldine kuju

Kui mingi suurus muutub iga ajaperioodi järel sama protsendi võrra, siis on tegu eksponentsiaalse muutumisega.

```math
L = A\left(1 + \frac{p}{100}\right)^n
```

- kasvamisel ($p > 0$)
- kahanemisel ($p < 0$) või kirjutame eraldi:

```math
L = A\left(1 - \frac{q}{100}\right)^n,
```

kus $q > 0$ on kahanemisprotsent.

**Mõisted:**

- $A$ – algväärtus (alg­hind, algkogus jne)
- $L$ – lõppväärtus pärast $n$ perioodi
- $p$ või $q$ – protsent perioodi kohta
- $n$ – perioodide arv (aastad, kuud jne)

---

### Protsent ja tegur

Kui suurus **väheneb** iga aasta $q\%$ võrra, siis iga aasta korrutame:

```math
\text{tegur} = 1 - \frac{q}{100}.
```

Kui suurus **kasvab** iga aasta $p\%$ võrra, siis iga aasta korrutame:

```math
\text{tegur} = 1 + \frac{p}{100}.
```

Näited:

- $10\%$ kasv: tegur $1.10$
- $6\%$ kahanemine: tegur $0.94$

---

### Kuidas leida protsent, kui alg- ja lõppväärtus on teada?

Kui on teada $A$, $L$ ja $n$, ning eeldame eksponentsiaalset muutumist:

```math
L = A\left(1 + \frac{p}{100}\right)^n
```

1. Jagame mõlemad pooled $A$-ga:

```math
\frac{L}{A} = \left(1 + \frac{p}{100}\right)^n
```

2. Võtame juure (nt kui $n = 2$, siis ruutjuure):

```math
1 + \frac{p}{100} = \sqrt[n]{\frac{L}{A}}
```

3. Lahutame 1 ja korrutame 100-ga:

```math
\frac{p}{100} = \sqrt[n]{\frac{L}{A}} - 1
```

```math
p = 100\left(\sqrt[n]{\frac{L}{A}} - 1\right).
```

Kahanemise korral on $p$ negatiivne või kasutame eraldi $q$:

```math
1 - \frac{q}{100} = \sqrt[n]{\frac{L}{A}}.
```

---

### Kuidas leida aastate arv $n$ logaritmide abil?

Kui on teada $A$, $L$ ja protsent (st tegur $k$), siis:

```math
L = A \cdot k^n
```

```math
\frac{L}{A} = k^n
```

Võtame logaritmi (võib olla kümnendlogaritm või naturaallogaritm – oluline on, et mõlemal pool sama):

```math
\log \frac{L}{A} = \log k^n = n \log k
```

```math
n = \frac{\log \frac{L}{A}}{\log k}.
```

**Oluline:**
- Kui $0 < k < 1$ (kahanemine), siis $\log k$ on negatiivne.
- Kui $L < A$, siis $\frac{L}{A} < 1$ ja $\log \frac{L}{A}$ on samuti negatiivne.
- Negatiivne jagatud negatiivsega annab positiivse $n$.

---

### Tüüpilised eksamistiilis sammud

1. **Kirjuta valem õigesti:**

   - Kasuta alati kuju $L = A \cdot k^n$, kus $k$ on kasvamis- või kahanemistegur.
   - Seosta $k$ protsendiga: $k = 1 \pm \frac{p}{100}$.

2. **Asenda andmed valemisse:**

   - Pane $A$, $L$, $n$ või $p$ õigesse kohta.
   - Ära jäta ühikuid (eurod, aastad) lõplikus vastuses mainimata.

3. **Lahenda samm-sammult:**

   - Kui otsid $p$, kasuta juurt (nt ruutjuur, kuupjuur) või logaritme.
   - Kui otsid $n$, kasuta logaritme.

4. **Ümarda alles lõpus:**

   - Hoia vahepeal rohkem kohti (nt 4–5 kohta pärast koma).
   - Ümarda vastus vastavalt ülesande nõudele (nt 10 euro täpsuseni, ühe kümnendkohani jne).

5. **Kontrolli vastuse mõistlikkust:**

   - Kui on kahanemine, peab $k$ olema väiksem kui 1.
   - Kui $L$ on väiksem kui $A$, peab $n$ olema positiivne.
   - Kui räägitakse “poole võrra väiksem”, kontrolli, kas kasutad $\frac{1}{2}A$ või midagi muud.

---
