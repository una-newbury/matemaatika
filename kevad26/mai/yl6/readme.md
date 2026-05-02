Ülesanne 6. (10 punkti)

On antud funktsioon $f(x) = x^3 + 3x^2 - 9x - 2$

1. Leidke funktsiooni $f(x)$ graafiku maksimum- ja miinimumpunkti koordinaadid.
2. Sirge $s$ läbib funktsiooni $f(x)$ graafiku ekstreemumpunkte. Koostage sirge $s$ võrrand.
3. Kas sirge s on tõusev või langev? Põhjendage oma vastust.

---

Lahendame samm-sammult.

### 1. Maksimum- ja miinimumpunktid

Antud on funktsioon

```math
f(x) = x^3 + 3x^2 - 9x - 2
```

Leidmiseks võtame tuletise:

```math
f'(x) = 3x^2 + 6x - 9
```

Leiame kriitilised punktid, lahendades võrrandi $f'(x) = 0$:

```math
3x^2 + 6x - 9 = 0
```

Jagame 3-ga:

```math
x^2 + 2x - 3 = 0
```

Lahendame ruutvõrrandi:

```math
x^2 + 2x - 3 = (x - 1)(x + 3) = 0
```

Seega

```math
x_1 = 1,\quad x_2 = -3
```

Nüüd leiame vastavad funktsiooni väärtused.

```math
f(1) = 1^3 + 3\cdot 1^2 - 9\cdot 1 - 2 = 1 + 3 - 9 - 2 = -7
```

```math
f(-3) = (-3)^3 + 3\cdot(-3)^2 - 9\cdot(-3) - 2 = -27 + 27 + 27 - 2 = 25
```

Et teha kindlaks, kumb on maksimum ja kumb miinimum, kasutame teist tuletist:

```math
f''(x) = 6x + 6
```

```math
f''(1) = 6\cdot 1 + 6 = 12 > 0
```

Seega $x = 1$ juures on **miinimumpunkt**.

```math
f''(-3) = 6\cdot (-3) + 6 = -18 + 6 = -12 < 0
```

Seega $x = -3$ juures on **maksimumpunkt**.

**Vastus 1:**  
Maksimum: $(-3,\ 25)$  
Miinimum: $(1,\ -7)$

![img.png](img.png)
---

### 2. Sirge $s$ võrrand, mis läbib ekstreemumpunkte

Ekstreemumpunktid on $(-3, 25)$ ja $(1, -7)$. Koostame sirge, mis läbib neid kahte punkti.

Leidame tõusukordaja $k$:

```math
k = \frac{y_2 - y_1}{x_2 - x_1} = \frac{-7 - 25}{1 - (-3)} = \frac{-32}{4} = -8
```

Kasutame punkt-kaldenurga kuju, näiteks punktiga $(-3, 25)$:

```math
y - 25 = -8(x + 3)
```

Avaldame $y$:

```math
y - 25 = -8x - 24
y = -8x + 1
```

**Vastus 2:**  
Sirge $s$ võrrand on

```math
y = -8x + 1
```

---

### 3. Kas sirge $s$ on tõusev või langev?

Sirge üldkujul $y = kx + b$ on:

- **tõusev**, kui $k > 0$
- **langev**, kui $k < 0$

Meie sirgel

```math
y = -8x + 1
```

on tõusukordaja

```math
k = -8 < 0
```

Seega sirge on **langev**.

**Vastus 3:**  
Sirge $s$ on langev, sest tema tõusukordaja on negatiivne ($k = -8$).
