## 14.1 Pravoúhlý trojúhelník – označení

| Symbol     | Význam                                              |
| ---------- | --------------------------------------------------- |
| $C$        | vrchol s **pravým úhlem**                           |
| $c$        | **přepona** (nejdelší strana, naproti pravému úhlu) |
| $a, b$     | **odvěsny** (kratší strany)                         |
| $\alpha$   | úhel u vrcholu $A$ (naproti straně $a$)             |
| $\beta$    | úhel u vrcholu $B$ (naproti straně $b$)             |
| $v_c$      | výška na přeponu $c$ (z vrcholu $C$)                |
| $c_a, c_b$ | úseky přepony ($c = c_a + c_b$)                     |

---

## 14.2 Pythagorova věta

### Znění:

> V pravoúhlém trojúhelníku platí: **obsah čtverce nad přeponou = součet obsahů čtverců nad odvěsnami.**

$$\boxed{c^2 = a^2 + b^2}$$

### Časté pythagorejské trojice (znát nazpaměť!):

|$a$|$b$|$c$|
|---|---|---|
|3|4|5|
|5|12|13|
|8|15|17|
|7|24|25|
|6|8|10 _(násobek 3-4-5)_|

---

## 14.3 Euklidovy věty

### Odvození ze podobnosti trojúhelníků:

Spustíme výšku $v_c$ z vrcholu $C$ na přeponu $c$. Vzniknou tři podobné trojúhelníky: $$\triangle ABC \sim \triangle ACV_c \sim \triangle CBV_c$$

Z těchto podobností plynou oba Euklidovy vzorce.

---

### 1. Euklidova věta (věta o výšce):

> **Druhá mocnina výšky pravoúhlého trojúhelníku na přeponu se rovná součinu úseků přepony.**

$$\boxed{v_c^2 = c_a \cdot c_b}$$

_Kde $c_a$ je úsek přepony přiléhající k odvěsně $a$, $c_b$ přiléhá k $b$._

---

### 2. Euklidova věta (věta o odvěsně):

> **Druhá mocnina odvěsny se rovná součinu přepony a příslušného úseku přepony.**

$$\boxed{a^2 = c \cdot c_a} \qquad \boxed{b^2 = c \cdot c_b}$$

_Úsek $c_a$ přiléhá k odvěsně $a$ (sdílí s ní vrchol $A$), úsek $c_b$ přiléhá k $b$._

---

### Přehled vztahů v pravoúhlém trojúhelníku:

| Vztah                      | Vzorec                                                |
| -------------------------- | ----------------------------------------------------- |
| Pythagorova věta           | $c^2 = a^2 + b^2$                                     |
| 1. Euklidova (výška)       | $v_c^2 = c_a \cdot c_b$                               |
| 2. Euklidova (odvěsna $a$) | $a^2 = c \cdot c_a$                                   |
| 2. Euklidova (odvěsna $b$) | $b^2 = c \cdot c_b$                                   |
| Délka přepony              | $c = c_a + c_b$                                       |
| Obsah trojúhelníku         | $S = \frac{1}{2} a \cdot b = \frac{1}{2} c \cdot v_c$ |

---

## 14.4 Těžnice pravoúhlého trojúhelníku

Těžnice je úsečka z vrcholu do středu protilehlé strany.

### Klíčová vlastnost:

> **Těžnice na přeponu** ($t_c$) = polovina přepony: $$t_c = \frac{c}{2}$$ _(střed přepony je střed opsané kružnice)_

### Vzorec pro obecnou těžnici:

$$t_a^2 = \frac{2b^2 + 2c^2 - a^2}{4}$$

nebo ekvivalentně: $$t_a = \frac{1}{2}\sqrt{2b^2 + 2c^2 - a^2}$$

Analogicky pro $t_b$ a $t_c$.

### Příklad (úloha 1): $t_a = 5$ cm, $t_b = 2\sqrt{10}$ cm, pravý úhel u $C$

Protože $\angle C = 90°$, platí $t_c = c/2$.
Použijeme vzorce:$$t_a^2 = \frac{2b^2 + 2c^2 - a^2}{4} = 25$$ $$t_b^2 = \frac{2a^2 + 2c^2 - b^2}{4} = 40$$
A Pythagorovu větu: $a^2 + b^2 = c^2$.

Z první rovnice: $2b^2 + 2c^2 - a^2 = 100$ Z druhé rovnice: $2a^2 + 2c^2 - b^2 = 160$

Dosadíme $c^2 = a^2 + b^2$ a řešíme soustavu → $a = 6$, $b = 4$, $c = 2\sqrt{13}$ 

---

## 14.5 Výška na přeponu – úseky přepony

### Jak najít $c_a$ a $c_b$:

Ze 2. Euklidovy věty: $c_a = \frac{a^2}{c}$, $c_b = \frac{b^2}{c}$

### Příklad (úloha 4): $a = 17$ cm, $v_c = 8$ cm, $\angle C = 90°$

Ze 2. Euklidovy věty: $a^2 = c \cdot c_a \implies c_a = \frac{a^2}{c}$

Z 1. Euklidovy věty: $v_c^2 = c_a \cdot c_b = 64$

Víme také: $v_c = \frac{a \cdot b}{c}$ (výška = součin odvěsen / přepona), tedy: $$b = \frac{v_c \cdot c}{a}$$ A z Pythagorovy věty: $a^2 + b^2 = c^2$... → soustava, z níž $c = \frac{a^2}{c_a}$.

Postup: $c_a = \frac{v_c^2 \cdot c}{a^2}$... (viz řešení v PDF: $S = \frac{1156}{15}$ cm²) ✅

---

## 14.6 Aplikace Pythagorovy věty na rovinné obrazce

### Kosočtverec (úloha 6):

Úhlopříčky kosočtverce se navzájem **kolmo půlí**. Strana $a$, úhlopříčky $u_1, u_2$: $$a^2 = \left(\frac{u_1}{2}\right)^2 + \left(\frac{u_2}{2}\right)^2$$

Obsah: $S = \frac{u_1 \cdot u_2}{2}$

**Zadání:** $S = 864$ cm², $u_1 = u_2 + 12$

$$\frac{u_2(u_2+12)}{2} = 864 \implies u_2^2 + 12u_2 - 1728 = 0 \implies u_2 = 36, ; u_1 = 48$$ $$a = \sqrt{18^2 + 24^2} = \sqrt{324 + 576} = \sqrt{900} = 30 \text{ cm}$$

---

### Kosočtverec – obsah přes výšku (úloha 18):

Výška $v = 48$ mm, kratší úhlopříčka $u = 60$ mm.

Z pravého trojúhelníku tvořeného výškou, polovinou kratší úhlopříčky a stranou: $$a^2 = v^2 + \left(\frac{u}{2}\right)^2 = 48^2 + 30^2 = 2304 + 900 = 3204 \implies a \approx 56{,}6 \text{ mm}$$

Obsah: $S = a \cdot v = 56{,}6 \cdot 48 \approx 2400$ mm² ✅ _(nebo $S = \frac{u_1 \cdot u_2}{2}$)_

---

### Rovnoramenný lichoběžník (úloha 17):

Výška lichoběžníku se určí Pythagorovou větou z pravoúhlého trojúhelníku, který vznikne spuštěním výšky.

**Zadání:** základny v poměru 5:3, ramena $r = 5$ m, výška $h = 4{,}8$ m

Ověření: $\left(\frac{a-c}{2}\right)^2 + h^2 = r^2$

Obsah: $S = \frac{(a+c) \cdot h}{2}$

Z poměru $a:c = 5:3$ → nechť $a = 5k$, $c = 3k$. $$\frac{5k - 3k}{2} = k = \sqrt{r^2 - h^2} = \sqrt{25 - 23{,}04} = \sqrt{1{,}96} = 1{,}4 \text{ m}$$ $$a = 7 \text{ m}, ; c = 4{,}2 \text{ m}, ; S = \frac{(7 + 4{,}2) \cdot 4{,}8}{2} = 26{,}88 \text{ m}^2$$

---

### Tětiva v kružnici (úloha 7):

Z Pythagorovy věty pro pravoúhlý trojúhelník: střed kružnice, střed tětivy, krajní bod tětivy. $$r^2 = d^2 + \left(\frac{t}{2}\right)^2$$ kde $d$ = vzdálenost tětivy od středu, $t$ = délka tětivy.

**Zadání:** $d = 8$ cm, $t = r + 13$ (tětiva o 13 cm delší než poloměr)

$$r^2 = 64 + \left(\frac{r+13}{2}\right)^2 = 64 + \frac{r^2 + 26r + 169}{4}$$ $$4r^2 = 256 + r^2 + 26r + 169$$ $$3r^2 - 26r - 425 = 0 \implies r = \frac{26 \pm \sqrt{676 + 5100}}{6} = \frac{26 + 76}{6} = 17 \text{ cm}$$

---

### Dvě rovnoběžné tětivy (úloha 15):

Průměr $2r = 6$ cm → $r = 3$ cm. Tětivy délky $t_1 = 5$ cm a $t_2 = 3$ cm.

Vzdálenosti tětivy od středu: $$d_1 = \sqrt{r^2 - \left(\frac{t_1}{2}\right)^2} = \sqrt{9 - 6{,}25} = \sqrt{2{,}75}$$ $$d_2 = \sqrt{r^2 - \left(\frac{t_2}{2}\right)^2} = \sqrt{9 - 2{,}25} = \sqrt{6{,}75}$$

Vzdálenost tětivy od sebe (jsou-li na **stejné straně** středu nebo **různých stranách**): $$\text{různé strany: } d_1 + d_2 \approx 4{,}26 \text{ cm}$$ $$\text{stejná strana: } |d_1 - d_2| \approx 0{,}94 \text{ cm}$$

---

### Tečna ke kružnici (úloha 13):

Z bodu $A$ vedou tečny ke kružnici $k(S, r)$, body dotyku $T_1, T_2$. Tečna je **kolmá na poloměr** v bodě dotyku.

$$AT^2 = AS^2 - r^2 \quad \text{(Pythagorova věta v trojúhelníku } AST\text{)}$$

**Zadání:** $r = 4$ cm, $AS = 10$ cm → $AT = \sqrt{100-16} = \sqrt{84}$

Vzdálenost bodu $A$ od přímky $T_1T_2$ (tzv. polára): $$d = \frac{r^2}{AS} \cdot \frac{AS}{1} \cdot \frac{1}{AS}... = \frac{r^2}{AS} \cdot \frac{AT^2 + r^2}{AS}$$

Jednodušeji: $A$, střed $T_1T_2$ (označme $M$) a $S$ jsou kolineární. $AM \cdot AS = AT^2$: $$AM = \frac{AT^2}{AS} = \frac{84}{10} = 8{,}4 \text{ cm}$$ 

---

## 14.7 Konstrukční použití Euklidových vět

### Sestrojit úsečku délky $\sqrt{p}$ pomocí 1. Euklidovy věty:

Věta říká: $v^2 = c_a \cdot c_b$, tedy $v = \sqrt{c_a \cdot c_b}$.

**Postup pro $\sqrt{ab}$ (geometrický střed):**

1. Na přímce vyznač úsečku délky $c_a + c_b = a + b$
2. Nad touto úsečkou se sestrojí Thaletova kružnice (průměr = $a+b$)
3. V bodě dělení vztyčíme kolmici – délka od základny k půlkružnici = $\sqrt{a \cdot b}$

**Příklad – sestrojit $\sqrt{10}$ (úloha 9):** $10 = 2 \cdot 5$ → $c_a = 2$, $c_b = 5$ → výška = $\sqrt{10}$ ✅

**Sestrojit $\sqrt{13}$ (úloha 10):** Pythagorovou větou: $\sqrt{13} = \sqrt{4 + 9} = \sqrt{2^2 + 3^2}$ → pravoúhlý trojúhelník se odvěsnami 2 a 3. Euklidovou větou: $13 = 1 \cdot 13$ → $c_a = 1$, $c_b = 13$ → výška = $\sqrt{13}$ ✅

### Sestrojit $\sqrt{S_{obdélníku}}$ – čtverec stejného obsahu (úloha 11):

Obsah obdélníku $3 \times 7 = 21$ cm² → strana čtverce $= \sqrt{21} = \sqrt{3 \cdot 7}$. Pomocí 1. Euklidovy věty: $c_a = 3$, $c_b = 7$ → výška = $\sqrt{21}$ = strana čtverce. 

---

## 14.8 Výpočet stran a úhlů v pravoúhlém trojúhelníku

### Trigonometrické funkce:

$$\sin \alpha = \frac{a}{c} \qquad \cos \alpha = \frac{b}{c} \qquad \tan \alpha = \frac{a}{b}$$

### Příklad (úloha 12): $c_a = 8$ cm, $c_b = 2$ cm

$c = c_a + c_b = 10$ cm

Z 2. Euklidovy věty: $$a^2 = c \cdot c_a = 10 \cdot 8 = 80 \implies a = 4\sqrt{5} \text{ cm}$$ $$b^2 = c \cdot c_b = 10 \cdot 2 = 20 \implies b = 2\sqrt{5} \text{ cm}$$

Ověření: $a^2 + b^2 = 80 + 20 = 100 = c^2$ 

Úhly: $\sin \alpha = \frac{a}{c} = \frac{4\sqrt{5}}{10} \implies \alpha \approx 63°26'$, $\beta = 90° - \alpha \approx 26°34'$ 

### Příklad (úloha 16): $c = 25$ cm, $v_c = 12$ cm

Z obsahu: $S = \frac{1}{2}c \cdot v_c = \frac{1}{2} \cdot 25 \cdot 12 = 150$ cm² = $\frac{1}{2} a \cdot b \implies ab = 300$

Z Pythagorovy věty: $a^2 + b^2 = 625$

$(a+b)^2 = a^2 + 2ab + b^2 = 625 + 600 = 1225 \implies a+b = 35$

$(a-b)^2 = 625 - 600 = 25 \implies a-b = 5$

→ $a = 20$ cm, $b = 15$ cm 

---

## 14.9 Kulový vrchlík – aplikace (úloha 8)

Pozorovatel ve výšce $h = 1$ km nad Zemí (poloměr Země $R \approx 6371$ km).

Vzdálenost k horizontu: $d = \sqrt{h(2R+h)} \approx \sqrt{2Rh}$

Vzdálenost po povrchu (délka oblouku): $s = R \cdot \arccos\frac{R}{R+h}$

Obvod vrchlíku (kruh na horizontu): $o = 2\pi d = 2\pi\sqrt{h(2R+h)} \approx 709{,}55$ km ✅

---

## 14.10 Přehled vzorců

```
PYTHAGOROVA VĚTA:
  a² + b² = c²   (c = přepona, a, b = odvěsny)

EUKLIDOVY VĚTY:
  1. věta (výška):   v² = c_a · c_b
  2. věta (odvěsna): a² = c · c_a
                     b² = c · c_b

ODVOZENÉ VZTAHY:
  c_a = a²/c,  c_b = b²/c
  v_c = a·b/c
  S = ½·a·b = ½·c·v_c

TĚŽNICE:
  t_a = ½·√(2b² + 2c² - a²)
  t_c = c/2  (pro pravoúhlý trojúhelník)

TĚTIVA V KRUŽNICI:
  r² = d² + (t/2)²    (d = vzdálenost od středu)

TEČNA Z VNĚJŠÍHO BODU:
  AT² = AS² - r²      (A = bod, S = střed, r = poloměr)

KONSTRUKČNÍ ÚLOHY:
  √(a·b)  →  1. Euklidova věta: c_a = a, c_b = b, výška = √(a·b)
  √(a²+b²) →  Pythagorova věta: pravoúhlý trojúhelník s odvěsnami a, b
```
