## 24.1 Co je komplexní číslo

Komplexní číslo vzniklo jako rozšíření reálných čísel tak, aby šlo řešit rovnice jako $x^2 + 1 = 0$.

Zavedeme imaginární jednotku: $$\boxed{i^2 = -1, \quad i = \sqrt{-1}}$$

**Algebraický (základní) tvar:** $$z = a + bi, \quad a, b \in \mathbb{R}$$

|Symbol|Název|Popis|
|---|---|---|
|$a = \text{Re}(z)$|reálná část|„klasická" složka|
|$b = \text{Im}(z)$|imaginární část|koeficient u $i$|
|$\bar{z} = a - bi$|číslo sdružené|změníme znaménko imaginární části|
|$\|z\| = \sqrt{a^2 + b^2}$|absolutní hodnota (modul)|vzdálenost od počátku v Gaussově rovině|

### Speciální případy

|Podmínka|Typ čísla|
|---|---|
|$b = 0$|reálné číslo ($z \in \mathbb{R}$)|
|$a = 0, b \neq 0$|**ryze imaginární** číslo|
|$a = 0, b = 0$|nula|

> ✏️ **Příklad (z PDF – příklad 2):** Kdy je $z = 8 - 6x - xi$ ryze imaginární? Reálná část = 0: $8 - 6x = 0 \Rightarrow x = \frac{4}{3}$

---

## 24.2 Gaussova rovina (komplexní rovina)

Komplexní číslo $z = a + bi$ zobrazíme jako bod $(a, b)$ nebo jako vektor $\vec{oz}$.

```
Im
 ↑
 |        • z = a + bi
 b|       /
 |      / |z| = √(a²+b²)
 |    /  φ
 |  /φ
 |/______→ Re
       a
```

- **Vodorovná osa** = reálná osa (Re)
- **Svislá osa** = imaginární osa (Im)
- **Číslo sdružené** $\bar{z}$ = odraz přes reálnou osu

### Geometrická interpretace operací

- **Součet** $z_1 + z_2$ = vektorové skládání (jako součet vektorů)
- **Rozdíl** $z_1 - z_2$ = vektorový rozdíl
- **Sdružené číslo** $\bar{z}$ = souměrnost podle reálné osy

---

## 24.3 Mocniny imaginární jednotky i

Mocniny $i$ se opakují s periodou 4:

|Exponent|Výsledek|
|---|---|
|$i^0 = 1$||
|$i^1 = i$||
|$i^2 = -1$||
|$i^3 = -i$||
|$i^4 = 1$|(cyklus se opakuje)|

**Jak vypočítat $i^n$ pro velké $n$:** $$i^n = i^{n \mod 4}$$

Vydělíme $n$ čtyřmi a podíváme se na zbytek.

> ✏️ **Příklad (z PDF – příklad 9a):** $i^{-31}$ $-31 = -32 + 1$, tedy $i^{-31} = i^1 = i$ Nebo: $i^{-31} = \frac{1}{i^{31}} = \frac{1}{i^3} = \frac{1}{-i} = \frac{i}{1} = i$

---

## 24.4 Početní operace – algebraický tvar

### Sčítání a odčítání

$$(a + bi) \pm (c + di) = (a \pm c) + (b \pm d)i$$

Sčítáme/odčítáme reálné a imaginární části zvlášť.

### Násobení

$$(a + bi)(c + di) = ac + adi + bci + bdi^2 = (ac - bd) + (ad + bc)i$$

> Vzpomeneme $i^2 = -1$ a upravíme.

### Dělení

$$\frac{a + bi}{c + di} = \frac{(a + bi)(c - di)}{(c + di)(c - di)} = \frac{(ac + bd) + (bc - ad)i}{c^2 + d^2}$$

**Postup:** Rozšíříme zlomek číslem sdruženým ke jmenovateli – jmenovatel se stane reálným číslem.

> ✏️ **Příklad (z PDF – příklad 6):** $z = \frac{-i}{2(1-i)}$ $= \frac{-i(1+i)}{2(1-i)(1+i)} = \frac{-i - i^2}{2(1+1)} = \frac{-i + 1}{4} = \frac{1}{4} - \frac{1}{4}i$

### Rovnost komplexních čísel

Dvě komplexní čísla jsou si rovna, právě když se rovnají jejich reálné i imaginární části: $$a + bi = c + di \iff a = c \text{ a } b = d$$

> ✏️ **Příklad (z PDF – příklad 3):** Řeš $x(1+i) + yi = \frac{1}{2} + 2i$ Levá strana: $(x) + (x+y)i$ Rovnost: $x = \frac{1}{2}$ a $x + y = 2 \Rightarrow y = \frac{3}{2}$

---

## 24.5 Goniometrický tvar komplexního čísla

$$\boxed{z = r(\cos\varphi + i\sin\varphi)}$$

kde:

- $r = |z| = \sqrt{a^2 + b^2}$ ... **modul** (absolutní hodnota)
- $\varphi = \arg(z)$ ... **argument** (úhel s kladnou reálnou osou)

### Převod z algebraického do goniometrického tvaru

1. Vypočítej modul: $r = \sqrt{a^2 + b^2}$
2. Zjisti argument: $\varphi = \arctan\left(\frac{b}{a}\right)$ – **pozor na kvadrant!**

|Kvadrant|$a$|$b$|Úprava argumentu|
|---|---|---|---|
|I.|$+$|$+$|$\varphi = \arctan(b/a)$|
|II.|$-$|$+$|$\varphi = 180° - \arctan(\|b/a\|)$|
|III.|$-$|$-$|$\varphi = 180° + \arctan(\|b/a\|)$|
|IV.|$+$|$-$|$\varphi = 360° - \arctan(\|b/a\|)$|

> ✏️ **Příklad (z PDF – příklad 4):** $z = \frac{-1+2i}{1+3i}$ Nejprve zjednodušíme (dělení): $z = \frac{(-1+2i)(1-3i)}{(1+3i)(1-3i)} = \frac{-1+3i+2i-6i^2}{1+9} = \frac{5+5i}{10} = \frac{1}{2} + \frac{1}{2}i$ $r = \sqrt{(1/2)^2 + (1/2)^2} = \frac{\sqrt{2}}{2}$; $\varphi = 45°$ $z = \frac{\sqrt{2}}{2}(\cos 45° + i\sin 45°)$

---

## 24.6 Exponenciální tvar komplexního čísla

$$\boxed{z = r \cdot e^{i\varphi}}$$

Vychází z **Eulerova vzorce:** $$e^{i\varphi} = \cos\varphi + i\sin\varphi$$

Převod je přímý z goniometrického tvaru – místo $(\cos\varphi + i\sin\varphi)$ napíšeme $e^{i\varphi}$.

### Přehled všech tvarů

|Tvar|Zápis|
|---|---|
|Algebraický|$z = a + bi$|
|Goniometrický|$z = r(\cos\varphi + i\sin\varphi)$|
|Exponenciální|$z = r \cdot e^{i\varphi}$|

---

## 24.7 Operace v goniometrickém tvaru

Nechť $z_1 = r_1(\cos\varphi_1 + i\sin\varphi_1)$ a $z_2 = r_2(\cos\varphi_2 + i\sin\varphi_2)$.

### Násobení

$$z_1 \cdot z_2 = r_1 r_2 \bigl(\cos(\varphi_1+\varphi_2) + i\sin(\varphi_1+\varphi_2)\bigr)$$

> Moduly se **násobí**, argumenty se **sčítají**.

### Dělení

$$\frac{z_1}{z_2} = \frac{r_1}{r_2} \bigl(\cos(\varphi_1-\varphi_2) + i\sin(\varphi_1-\varphi_2)\bigr)$$

> Moduly se **dělí**, argumenty se **odčítají**.

---

## 24.8 Moivreova věta – mocnění

$$\boxed{z^n = r^n(\cos(n\varphi) + i\sin(n\varphi))}$$

**Postup mocnění:**

1. Převeď $z$ do goniometrického tvaru
2. Modul umocni: $r^n$
3. Argument vynásob: $n\varphi$
4. Výsledek převeď zpět do algebraického tvaru (pokud je to potřeba)

> ✏️ **Příklad (z PDF – příklad 8):** $z = -\frac{\sqrt{2}}{2} - i\frac{\sqrt{2}}{2}$, vypočti $z^8$ $r = 1$, $\varphi = 225° = \frac{5\pi}{4}$ $z^8 = 1^8(\cos(8 \cdot 225°) + i\sin(8 \cdot 225°)) = \cos(1800°) + i\sin(1800°) = \cos(0°) + i\sin(0°) = 1$

> ✏️ **Příklad (z PDF – příklad 9c):** $(1+i)^6$ $r = \sqrt{2}$, $\varphi = 45°$ $(1+i)^6 = (\sqrt{2})^6(\cos(6 \cdot 45°) + i\sin(270°)) = 8(0 + i(-1)) = -8i$

---

## 24.9 Odmocňování – n-té kořeny komplexního čísla

$$\boxed{\sqrt[n]{z} = \sqrt[n]{r} \left(\cos\frac{\varphi + 2k\pi}{n} + i\sin\frac{\varphi + 2k\pi}{n}\right), \quad k = 0, 1, 2, \ldots, n-1}$$

Rovnice $w^n = z$ má vždy **přesně n řešení** v oboru $\mathbb{C}$.

**Postup:**

1. Převeď pravou stranu do goniometrického tvaru: $z = r(\cos\varphi + i\sin\varphi)$
2. Modul odmocni: $\sqrt[n]{r}$
3. Argument vyděl a přidej otočení o $\frac{360°}{n}$ pro každé $k$
4. Zapiš všechna řešení pro $k = 0, 1, \ldots, n-1$

> 💡 Kořeny leží v Gaussově rovině rovnoměrně na kružnici o poloměru $\sqrt[n]{r}$ – jsou od sebe vzdáleny o úhel $\frac{360°}{n}$.

> ✏️ **Příklad (z PDF – příklad 14a):** $z^6 - 1 = 0$, tedy $z^6 = 1$ $r = 1$, $\varphi = 0°$ $z_k = \cos\frac{0° + 360°k}{6} + i\sin\frac{360°k}{6} = \cos(60°k) + i\sin(60°k)$, $k = 0, 1, 2, 3, 4, 5$ Výsledek: 6 čísel rovnoměrně rozmístěných na jednotkové kružnici.

---

## 24.10 Binomická rovnice

Rovnice tvaru $z^n = c$, kde $c \in \mathbb{C}$.

**Postup:**

1. Převeď $c$ do goniometrického tvaru: $c = r(\cos\varphi + i\sin\varphi)$
2. Řeš jako n-tou odmocninu: $z_k = \sqrt[n]{r}\left(\cos\frac{\varphi + 360°k}{n} + i\sin\frac{\varphi + 360°k}{n}\right)$
3. Zapiš pro $k = 0, 1, \ldots, n-1$

> ✏️ **Příklad (z PDF – příklad 14b):** $x^3 - 8 = 0 \Rightarrow x^3 = 8$ $r = 8$, $\varphi = 0°$; $\sqrt[3]{8} = 2$ $x_k = 2\left(\cos\frac{360°k}{3} + i\sin\frac{360°k}{3}\right)$ $x_0 = 2$; $x_1 = 2(\cos 120° + i\sin 120°) = -1 + \sqrt{3}i$; $x_2 = -1 - \sqrt{3}i$

---

## 24.11 Kvadratická rovnice v oboru ℂ

### Diskriminant a kořeny

$$ax^2 + bx + c = 0 \implies x_{1,2} = \frac{-b \pm \sqrt{D}}{2a}, \quad D = b^2 - 4ac$$

|$D$|Kořeny|
|---|---|
|$D > 0$|dva různé reálné kořeny|
|$D = 0$|dvojnásobný reálný kořen|
|$D < 0$|dva komplexně sdružené kořeny $x_{1,2} = \frac{-b \pm i\sqrt{|

> ⚠️ V oboru $\mathbb{C}$ má každá kvadratická rovnice vždy **právě 2 kořeny** (počítáme i dvojnásobné).

### Vièteovy vzorce (vztah kořenů a koeficientů)

Pro $x^2 + px + q = 0$ (normovaný tvar): $$x_1 + x_2 = -p \quad \text{(součet kořenů)}$$ $$x_1 \cdot x_2 = q \quad \text{(součin kořenů)}$$

**Sestavení rovnice ze zadaných kořenů:** $$x^2 - (x_1 + x_2)x + x_1 \cdot x_2 = 0$$

> ✏️ **Příklad (z PDF – příklad 21):** $x_1 = \frac{\sqrt{2}}{2}(1-i)$, $x_2 = -\frac{\sqrt{2}}{2}(1-i)$ $x_1 + x_2 = 0$; $x_1 \cdot x_2 = -\frac{1}{2}(1-i)^2 = -\frac{1}{2}(1 - 2i - 1) = -\frac{1}{2}(-2i) = i$ Rovnice: $x^2 + i = 0$

### Koeficienty jsou komplexní

Pokud jsou koeficienty komplexní, kořeny obecně **nejsou sdružené**. Řešíme standardním vzorcem, ale $\sqrt{D}$ musíme vypočítat jako odmocninu komplexního čísla.

> ✏️ **Příklad (z PDF – příklad 25):** Rovnice $ax^2 + bx + c = 0$ s reálnými koef., $c = 1$, $x_1 = -2 - i$ Koeficienty jsou reálné → $x_2 = \overline{x_1} = -2 + i$ (sdružený kořen) Součet: $x_1 + x_2 = -4$; Součin: $x_1 x_2 = (-2)^2 + 1^2 = 5$ $x^2 + 4x + 5 = 0$, vydělíme $a$ tak aby $c = 1$: $\frac{1}{5}x^2 + \frac{4}{5}x + 1 = 0$

---

## 24.12 Sdružené kořeny – důležité pravidlo

> 💡 **Pravidlo:** Má-li rovnice s **reálnými koeficienty** komplexní kořen $z = a + bi$, pak i $\bar{z} = a - bi$ je kořenem.

Komplexní kořeny reálné kvadratické rovnice přicházejí vždy v párech sdružených čísel.

---

## 24.13 Rozklad kvadratického trojčlenu v ℂ

Každý kvadratický trojčlen lze v $\mathbb{C}$ rozložit na součin dvou lineárních činitelů:

$$ax^2 + bx + c = a(x - x_1)(x - x_2)$$

kde $x_1, x_2$ jsou kořeny rovnice $ax^2 + bx + c = 0$.

> ✏️ **Příklad (z PDF – příklad 28a):** $x^2 + x + 1$ $D = 1 - 4 = -3 < 0$; $x_{1,2} = \frac{-1 \pm i\sqrt{3}}{2}$ Rozklad: $\left(x + \frac{1}{2} - \frac{\sqrt{3}}{2}i\right)\left(x + \frac{1}{2} + \frac{\sqrt{3}}{2}i\right)$

---

## 24.14 Množiny komplexních čísel v Gaussově rovině

Podmínky na modul $|z - z_0|$ popisují **kružnice** nebo **kruhy** se středem $z_0$:

|Podmínka|Geometrický útvar|
|---|---|
|$\|z - z_0\| = r$|kružnice se středem $z_0$ a poloměrem $r$|
|$\|z - z_0\| < r$|otevřený kruh (bez hranice)|
|$\|z - z_0\| \leq r$|uzavřený kruh (s hranicí)|
|$\|z - z_0\| > r$|vnějšek kružnice|
|$r_1 \leq \|z - z_0\| < r_2$|mezikruží (prstenec)|

**Kde je střed?** Střed kružnice $|z - z_0| = r$ je bod $z_0 = a + bi$, tedy souřadnice $(a, b)$ v Gaussově rovině.

> ✏️ **Příklad (z PDF – příklad 18a):** $M_1 = {z \in \mathbb{C}; 2 \leq |z + 2i| < 4}$ $|z - (0 - 2i)| \Rightarrow$ střed je bod $(0, -2)$ Mezikruží od poloměru 2 (včetně) do poloměru 4 (bez hranice)

**Podmínka $|z - z_1| \leq |z - z_2|$** = množina bodů bližších (nebo stejně vzdálených) k $z_1$ než k $z_2$ = polorovinu (přímka je osa úsečky $z_1 z_2$).

---

## 24.15 Rychlý přehled – vzorce na jednom místě

```
ALGEBRAICKÝ TVAR:       z = a + bi
MODUL:                  |z| = √(a² + b²)
SDRUŽENÉ ČÍSLO:         z̄ = a - bi
ARGUMENT:               φ = arctan(b/a)  [pozor na kvadrant!]

GONIOMETRICKÝ TVAR:     z = r(cos φ + i·sin φ)
EXPONENCIÁLNÍ TVAR:     z = r·e^(iφ)

NÁSOBENÍ (gon.):        r₁r₂ · (cos(φ₁+φ₂) + i·sin(φ₁+φ₂))
DĚLENÍ (gon.):          (r₁/r₂) · (cos(φ₁-φ₂) + i·sin(φ₁-φ₂))

MOIVREOVA VĚTA:         zⁿ = rⁿ(cos(nφ) + i·sin(nφ))

N-TÉ KOŘENY:            z_k = ⁿ√r · (cos((φ+360°k)/n) + i·sin((φ+360°k)/n))
                        k = 0, 1, ..., n−1

KVADRATICKÁ:            D = b² - 4ac
  D < 0 → x₁,₂ = (−b ± i√|D|) / (2a)

VIÈTEOVY VZORCE (x²+px+q=0):
  x₁ + x₂ = −p
  x₁ · x₂ = q

MOCNINY i:
  i⁰=1, i¹=i, i²=−1, i³=−i, i⁴=1  (perioda 4)
```

---

## 24.16 Časté chyby a na co si dát pozor

> ⚠️ **Kvadrant při výpočtu argumentu:** $\arctan$ vrací hodnoty jen v $(-90°, 90°)$. Pokud $a < 0$, přidej 180° (nebo 360° pro IV. kvadrant). Vždy překontroluj, ve kterém kvadrantu číslo leží!

> ⚠️ **Dělení – rozšiřujeme sdruženým ke jmenovateli**, ne k čitateli.

> ⚠️ **Binomická rovnice:** Nezapomeň, že $z^n = c$ má **n řešení**, ne jedno! Hodnota $k$ jde od 0 do $n-1$.

> ⚠️ **Sdružené kořeny platí jen pro reálné koeficienty.** Pokud má rovnice koeficienty komplexní, kořeny sdružené být nemusí.

> ⚠️ **Moivreova věta:** Platí pro celá $n$, i záporná. Pro záporné $n$: $z^{-n} = \frac{1}{z^n}$.

> ⚠️ **Absolutní hodnota součinu:** $|z_1 \cdot z_2| = |z_1| \cdot |z_2|$ – lze využít k rychlému výpočtu.
