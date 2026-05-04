### Sisukord

- [Ülesanne 2 — Kommipakis (lahendatud)](#ülesanne-2)
- [Ülesanne 5 — Vanuseülesanne (täielik lahendus)](#ülesanne-5)
- [Valemid ja meelespea (selle tüübi ülesannetele)](#valemid-ja-meelespea)

---

### Ülesanne 2 — Kommipakis (5 punkti)

**Ülesande tekst (väljavõte dokumendist):** „Kommipakis on 50 kommi, neist 15 on sinised, 11 oranžid, 8 pruunid ja 9 kollased. Kõik ülejäänud kommid on rohelised. 1. Mitu protsenti pakis olevatest kommidest on rohelised? 2. Mari valib kommipakist juhuslikult kaks kommi. Arvutage tõenäosus, et mõlemad kommid on sinised.“

**Lahendus samm-sammult (selgelt ja lihtsasti loetav):**

1. **Roheliste arv ja protsent.**  
   Arvutame roheliste arvu:
```math
\text{rohelised} = 50 - (15 + 11 + 8 + 9) = 50 - 43 = 7
```
   Protsent:
```math
\text{protsent} = \frac{7}{50}\cdot 100\% = 14\%
```

2. **Tõenäosus, et mõlemad valitud kommid on sinised (ilma asendamiseta).**  
   Esimese valiku tõenäosus on $15/50$. Kui esimene on sinine, jääb siniseid $14$ ja kokku $49$ kommi. Seega:
```math
P(\text{mõlemad sinised}) = \frac{15}{50}\cdot\frac{14}{49} = \frac{210}{2450} = \frac{3}{35}
```
   Või protsendina:
```math
\frac{3}{35}\approx 0{,}085714\quad\text{ehk}\quad 8{,}5714\%
```

**Vastus kokku:** rohelisi on **7** tk ehk **14%**; mõlema sinise tõenäosus on **$\dfrac{3}{35}$** (umbes **8,57%**).

---


### Ülesanne 5 — Vanuseülesanne (10 punkti)

**Ülesande tekst (väljavõte dokumendist):**  
„Isa ja lapse vanuste summa on praegu 41 aastat. Nelja aasta pärast on isa lapsest 6 korda vanem. 1. Kui vanad on isa ja laps praegu? 2. Kui vana on ema praegu, kui aasta tagasi oli ema, isa ja lapse vanuste summa 70 aastat? 3. Ema ja isa kohtusid esimest korda siis, kui nende vanuste summa oli 44 aastat. Mitu aastat tagasi see toimus?“

**Lahendus samm-sammult:**

1. **Määrame muutujad ja võrrandid.**  
   Olgu $f$ isa praegune vanus ja $c$ lapse praegune vanus. Antud on:
```math
f + c = 41
```
   ning nelja aasta pärast:
```math
f + 4 = 6\cdot (c + 4)
```

2. **Lahendame süsteemi.**  
   Teisest võrrandist:
```math
f + 4 = 6c + 24 \Rightarrow f = 6c + 20
```
   Asendame esimesse:
```math
6c + 20 + c = 41 \Rightarrow 7c + 20 = 41 \Rightarrow 7c = 21 \Rightarrow c = 3
```
   Siis:
```math
f = 41 - c = 41 - 3 = 38
```

   **Seega:** laps on praegu **3** aastat ja isa **38** aastat vana.

3. **Ema vanus (osa 2).**  
   Aasta tagasi oli kolme inimese vanuste summa 70:
```math
(m - 1) + (f - 1) + (c - 1) = 70
```
   Kus $m$ on ema praegune vanus. Lihtsustame:
```math
m + f + c - 3 = 70 \Rightarrow m = 73 - (f + c)
```
   Kuna $f + c = 41$:
```math
m = 73 - 41 = 32
```
   **Ema on praegu 32 aastat vana.**

4. **Millal kohtusid (osa 3).**  
   Ema ja isa praegused vanused on $m=32$ ja $f=38$, summa $m+f=70$. Otsime $t$ aastat tagasi, kui nende vanuste summa oli 44:
```math
(f - t) + (m - t) = 44 \Rightarrow f + m - 2t = 44
```
   Asendame $f+m=70$:
```math
70 - 2t = 44 \Rightarrow 2t = 26 \Rightarrow t = 13
```
   **Nad kohtusid 13 aastat tagasi.**

**Vastus kokku:** isa 38 a, laps 3 a; ema praegu 32 a; nad kohtusid **13** aastat tagasi.

---

## Valemid ja meelespea (selle tüübi ülesannetele)

Allpool on lühike, selge ja praktiline valemite- ja meetodite kogumik, mis aitab neid tüüpi riigieksami ülesandeid lahendada. Pane see meelde ja kasuta lahendamisel samme — see aitab eksamil aega kokku hoida ja vigu vältida.

---

#### Protsendid ja osakaalud
- **Protsendi leidmine:** kui osa on $a$ ja kogu $A$, siis protsent on
```math
\text{protsent} = \frac{a}{A}\cdot 100\%
```
- **Osa leidmine protsendi järgi:** kui protsent on $p\%$ ja kogu $A$, siis osa on
```math
a = \frac{p}{100}\cdot A
```

---

#### Tõenäosus (ilma asendamiseta)
- Kui valime järjest kaks eset ilma tagasi panemata, siis tõenäosus, et esimene on sündmus $E_1$ ja teine $E_2$:
```math
P(E_1\ \text{ja}\ E_2) = P(E_1)\cdot P(E_2\mid E_1)
```
- Näide: $k$ soodsat esimest valikut ja $n$ kokku:
```math
P_1 = \frac{k}{n},\quad P_2 = \frac{k-1}{n-1}
```

---

#### Lineaarsed võrrandid ja süsteemid (vanuseülesanded)
- Kui on kaks inimest ja antud on summa ning mingi suhe tulevikus või minevikus, kasuta muutujad ja lahenda lineaarne süsteem:
```math
\begin{cases}
x + y = S\\
x + a = r\cdot (y + a)
\end{cases}
```
  Lahenda teisest $x$ või $y$ väljendades ja asenda esimesse.

---

#### Võrrandid, murdvõrrandid ja määramispiirid
- Kui võrrandis on murd, kontrolli, et nimetaja ei oleks null. Märgi ära keelatud väärtused enne lahendamist.
- Kui lahendad murdvõrrandit, korda mõlemad pooled nimetajate ühise nimetajaga (kui see ei tekita valeid lahendeid), või teisenda samm-sammult ja kontrolli lõpus.

---

#### Ruutfunktsioonid ja faktoreerimine
- Kui tekib ruutvõrrand $ax^2+bx+c=0$, kasuta diskriminandi ja ruutvõrrandi valemit:
```math
D = b^2 - 4ac,\quad x = \frac{-b\pm\sqrt{D}}{2a}
```
- Faktoreerimine: otsi kaks arvu, mille korrutis on $ac$ ja summa $b$.

---

#### Ebavõrdsused (võrratused)
- Kui korrutad või jagad ebavõrdsust negatiivse arvuga, **muuda ebavõrdsuse suunda**.
- Kontrolli lahendite kuulumist määramispiirkonda (nt jagamine nulliga keelatud).

---

#### Kuidas kirjutada lahendust eksamil (näpunäited)
- **Alusta muutujate selge määratlusega.** Näiteks: „Olgu $x$ isa praegune vanus ja $y$ lapse praegune vanus.“
- **Kirjuta iga samm loogiliselt ja lühidalt.** Hindajad ei loe ebaselget mustandit.
- **Kontrolli piirväärtusi ja keelatud väärtusi** (nt nimetaja ei tohi olla 0).
- **Lõpus esita vastus selgelt**: „Vastus: isa 38 a, laps 3 a.“

---
