## 23.1 Základní pojmy prostorové geometrie

### Bod, přímka, rovina

|Pojem|Definice|
|---|---|
|**Bod**|základní geometrický objekt (0D)|
|**Přímka**|nekonečná, určena dvěma body (1D)|
|**Rovina**|nekonečná plocha, určena třemi různými body, které neleží na jedné přímce (2D)|
### Určení přímky v prostoru

Přímka je jednoznačně určena:

- **dvěma různými body**
- **bodem a směrovým vektorem**

### Určení roviny v prostoru

Rovina je jednoznačně určena:

- **třemi různými body, které neleží na jedné přímce**
- **přímkou a bodem mimo ni**
- **dvěma různoběžnými přímkami**

---

## 23.2 Vzájemná poloha přímek a rovin

### Dvě přímky v prostoru

|Poloha|Popis|
|---|---|
|**rovnoběžné** (p ∥ q)|neleží v jedné rovině, nemají společný bod|
|**totožné**|jsou stejná přímka|
|**různoběžné**|mají právě jeden společný bod (protínají se)|
|**mimoběžné**|neleží v jedné rovině a nemají společný bod|

> ⚠️ **Mimoběžné přímky** jsou typicky prostorový jev – v rovině neexistují!

### Přímka a rovina

|Poloha|Popis|
|---|---|
|**přímka leží v rovině**|všechny body přímky jsou v rovině|
|**přímka je rovnoběžná s rovinou** (p ∥ α)|nemají žádný společný bod|
|**přímka protíná rovinu**|mají právě jeden společný bod|
|**přímka je kolmá na rovinu** (p ⊥ α)|přímka je kolmá na každou přímku procházející patou kolmice|

### Dvě roviny

|Poloha|Popis|
|---|---|
|**totožné**|jsou stejná rovina|
|**rovnoběžné** (α ∥ β)|nemají žádný společný bod|
|**různoběžné**|protínají se v přímce (osa průniku)|
|**kolmé** (α ⊥ β)|různoběžné a jejich odchylka je 90°|

---

## 23.3 Vzdálenosti v prostoru

### Vzdálenost dvou bodů

$$d(A, B) = \sqrt{(x_B - x_A)^2 + (y_B - y_A)^2 + (z_B - z_A)^2}$$

### Vzdálenost bodu od přímky

Vzdálenost bodu **P** od přímky **p** = délka kolmice spuštěné z P na p.

**Postup:**

1. Najdi patu kolmice (průsečík kolmice z P s přímkou p)
2. Vypočti vzdálenost P od paty kolmice

### Vzdálenost bodu od roviny

Vzdálenost bodu **B** od roviny **ρ** = délka kolmice spuštěné z B na ρ.

**Postup (praktický):**

1. Spusť kolmici z B na rovinu ρ
2. Najdi patu kolmice F (průsečík kolmice s rovinou)
3. d(B, ρ) = |BF|

> 💡 Při úlohách s prostorovou geometrií hledáme nejčastěji vzdálenost pomocí Pythagorovy věty v pomocném pravoúhlém trojúhelníku.

### Vzdálenost dvou mimoběžných přímek

= délka jejich společné kolmice (nejkratší vzdálenost)

---

## 23.4 Odchylky přímek a rovin

### Odchylka dvou přímek

**Různoběžné přímky:** odchylka = velikost svíraného úhlu (bereme ten ostrý nebo pravý, tedy φ ∈ ⟨0°; 90°⟩)

**Mimoběžné přímky:**

- Jednou z přímek (nebo rovnoběžně s ní) provedeme přímku procházející libovolným bodem druhé přímky
- Odchylka mimoběžných přímek = odchylka takto vzniklých různoběžných přímek

> ✏️ **Příklad (z PDF – příklad 7a):** V kvádru ABCDEFGH hledáme odchylku přímek BE a CG. CG je rovnoběžná s BF. Odchylka BE, CG = odchylka BE, BF = úhel EBF.

### Odchylka přímky od roviny

1. Sestrojíme průsečík P přímky p s rovinou α (nebo použijeme rovnoběžný průmět)
2. Z libovolného bodu A na p spustíme kolmici na rovinu α – pata kolmice je bod A'
3. Odchylka = úhel **∠(p, α) = ∠APA'** (úhel mezi přímkou a její průmětnou)

> ✏️ **Příklad (z PDF – příklad 5b):** V čtyřbokém jehlanu ABCDV hledáme odchylku AV od roviny ABC. Průsečík AV s ABC je bod A. Sestrojíme výšku jehlanu VS ⊥ ABC. Odchylka = ∠VAS.

### Odchylka dvou rovin (dvoustěnný úhel)

1. Zvolíme libovolný bod P na hraně průniku rovin (ose)
2. V každé rovině vedeme z P polorovinu kolmou na hranu průniku
3. Odchylka = úhel těchto dvou polorovin

**Praktický postup:**

- Najdeme hranu průniku rovin (přímku α ∩ β)
- Zvolíme bod mimo hranu (nebo na hraně)
- Z tohoto bodu spustíme kolmice na hranu v každé rovině
- Úhel těchto kolmic = odchylka rovin

> ✏️ **Příklad (z PDF – příklad 4a):** V krychli ABCDEFGH odchylka rovin ABC a BDE. Hrana průniku rovin = BD. Z vrcholu A spustíme kolmici na BD → pata M. Z vrcholu E spustíme kolmici na BD → pata M (stejný bod). Odchylka = ∠AME.

---

## 23.5 Obsahy rovinných útvarů

### Přehled vzorců

|Útvar|Vzorec|Popis proměnných|
|---|---|---|
|**Čtverec**|$S = a^2$|a = strana|
|**Obdélník**|$S = a \cdot b$|a, b = strany|
|**Trojúhelník**|$S = \frac{1}{2} \cdot a \cdot h_a$|a = základna, $h_a$ = výška|
|**Trojúhelník** (Heron)|$S = \sqrt{s(s-a)(s-b)(s-c)}$|$s = \frac{a+b+c}{2}$|
|**Rovnoběžník**|$S = a \cdot h_a$|a = základna, $h_a$ = výška|
|**Lichoběžník**|$S = \frac{(a+c) \cdot h}{2}$|a, c = základny, h = výška|
|**Kružnice / kruh**|$S = \pi r^2$|r = poloměr|
|**Kruhová výseč**|$S = \frac{\alpha}{360°} \cdot \pi r^2$|α = středový úhel|
|**Pravidelný n-úhelník**|$S = \frac{n \cdot a \cdot \rho}{2}$|a = strana, ρ = poloměr vepsané kružnice|

### Pravidelný mnohoúhelník – důležité vztahy

Pro pravidelný **n-úhelník** se stranou **a** a poloměrem opsané kružnice **R** a vepsané **ρ**:

$$\rho = R \cdot \cos\left(\frac{180°}{n}\right), \quad a = 2R \cdot \sin\left(\frac{180°}{n}\right)$$

$$S = \frac{1}{2} \cdot n \cdot a \cdot \rho = \frac{n \cdot a^2}{4} \cdot \cot\left(\frac{180°}{n}\right)$$

> ✏️ **Příklad (z PDF – příklad 16):** Pravidelný osmiúhelník s poloměrem vepsané kružnice ρ = 7 cm. $a = 2\rho \cdot \tan(22{,}5°) \approx 5{,}80$ cm; $S = \frac{1}{2} \cdot 8 \cdot 5{,}80 \cdot 7 \approx 162{,}4$ cm²

---

## 23.6 Objemy a povrchy těles

### 🔷 Hranol (obecný)

$$V = S_p \cdot v \quad\quad P = 2S_p + S_{plášť}$$

kde $S_p$ = obsah podstavy, $v$ = výška

---

### 🔷 Krychle (a = hrana)

$$V = a^3 \quad\quad P = 6a^2$$

**Úhlopříčky:**

- Stěnová úhlopříčka: $u_s = a\sqrt{2}$
- Tělesová úhlopříčka: $u = a\sqrt{3}$

> ✏️ Z příkladu 19: $u_s = 8{,}5$ cm → $a = \frac{8{,}5}{\sqrt{2}}$ → $V = a^3$

---

### 🔷 Kvádr (a, b, c = hrany)

$$V = a \cdot b \cdot c \quad\quad P = 2(ab + bc + ac)$$

**Tělesová úhlopříčka:** $u = \sqrt{a^2 + b^2 + c^2}$

> ✏️ Z příkladu 1 (PDF): Kvádr se svírá tělesová úhlopříčka $u = 10$ cm s hranou a pod úhlem 60°, s hranou b pod úhlem 45°. $a = u \cdot \cos(60°) \cdot \ldots$ – řeší se přes složky vektoru úhlopříčky.

---

### 🔷 Jehlan (obecný)

$$V = \frac{1}{3} S_p \cdot v \quad\quad P = S_p + S_{plášť}$$

**Pravidelný n-boký jehlan:** plášť = n trojúhelníků se základnou a a výškou $v_s$ (apotéma):

$$S_{plášť} = \frac{1}{2} \cdot n \cdot a \cdot v_s$$

kde apotéma: $v_s = \sqrt{v^2 + \rho^2}$ (ρ = poloměr vepsané kružnice podstavy)

---

### 🔷 Komolý jehlan

$$V = \frac{v}{3}(S_1 + \sqrt{S_1 S_2} + S_2)$$

$$P = S_1 + S_2 + S_{plášť}$$

kde $S_1$, $S_2$ = obsahy podstav, $v$ = výška

Pro **pravidelný čtyřboký komolý jehlan** se stranami $a_1$, $a_2$ a boční hranou $s$:

$$v = \sqrt{s^2 - \left(\frac{a_1 - a_2}{2}\right)^2 - \left(\frac{a_1 - a_2}{2}\right)^2} = \sqrt{s^2 - \frac{(a_1-a_2)^2}{2}}$$

---

### 🔷 Válec (r = poloměr podstavy, v = výška)

$$V = \pi r^2 v \quad\quad P = 2\pi r^2 + 2\pi r v = 2\pi r(r + v)$$

**Rovnostranný válec:** výška = průměr podstavy, tedy $v = 2r$

---

### 🔷 Kužel (r = poloměr podstavy, v = výška, s = strana/tvořící čára)

$$s = \sqrt{r^2 + v^2}$$

$$V = \frac{1}{3}\pi r^2 v \quad\quad P = \pi r^2 + \pi r s = \pi r(r + s)$$

---

### 🔷 Komolý kužel (r₁, r₂ = poloměry podstav, v = výška, s = tvořící čára)

$$s = \sqrt{v^2 + (r_1 - r_2)^2}$$

$$V = \frac{\pi v}{3}(r_1^2 + r_1 r_2 + r_2^2)$$

$$P = \pi(r_1^2 + r_2^2 + s(r_1 + r_2))$$

---

### 🔷 Koule (r = poloměr)

$$V = \frac{4}{3}\pi r^3 \quad\quad P = 4\pi r^2$$

**Opsaná koule krychli** o hraně a: $r = \frac{a\sqrt{3}}{2}$

---

### 🔷 Kulová úseč (r = poloměr koule, h = výška úseče)

$$V_{úseč} = \frac{\pi h^2}{3}(3r - h) \quad\quad S_{plášť} = 2\pi r h$$

---

### 🔷 Kulová vrstva (r = poloměr koule, h = výška vrstvy)

$$V_{vrstva} = \frac{\pi h}{6}(3\rho_1^2 + 3\rho_2^2 + h^2)$$

kde $\rho_1$, $\rho_2$ jsou poloměry podstav vrstvy.

> ✏️ Z příkladu 24 (PDF): Polokoule o průměru 10 cm → r = 5 cm. Odřízneme kulovou úseč výšky h = 1,5 cm. $V_{vrstva} = V_{polokoule} - V_{úseč}$

---

## 23.7 Postup řešení typických úloh

### Jak určit odchylku boční hrany od roviny podstavy (jehlan/komolý jehlan)

1. Nakresli nárys jehlanu (pohled zboku nebo shora)
2. Boční hrana jde z vrcholu V do rohu podstavy (např. A)
3. Průmět boční hrany do roviny podstavy = úsečka od středu S k rohu A
4. Odchylka φ = $\arctan\left(\frac{v}{SA}\right)$, kde SA = vzdálenost středu podstavy od rohu

### Jak určit odchylku boční stěny od roviny podstavy (jehlan)

1. Apotéma boční stěny = výška trojúhelníkové boční stěny ($v_s$)
2. Průmět apotémy do podstavy = apotéma podstavy (ρ)
3. Odchylka = $\arctan\left(\frac{v}{\rho}\right)$

### Tělová úhlopříčka kvádru – úhel s hranou

Pro kvádr s hranami a, b, c a tělesovou úhlopříčkou $u = \sqrt{a^2+b^2+c^2}$:

$$\cos\alpha = \frac{a}{u}, \quad \cos\beta = \frac{b}{u}, \quad \cos\gamma = \frac{c}{u}$$

kde α, β, γ jsou úhly úhlopříčky s hranami a, b, c.

---

## 23.8 Pravidelný čtyřstěn – speciální vzorce

Pro pravidelný čtyřstěn s hranou **a**:

|Vlastnost|Vzorec|
|---|---|
|Výška stěny (výška rovnostranného trojúhelníku)|$h_s = \frac{a\sqrt{3}}{2}$|
|Vzdálenost vrcholu od protější hrany|$d = \frac{a\sqrt{2}}{2} = \frac{a}{\sqrt{2}}$|
|Výška tělesa|$v = a\sqrt{\frac{2}{3}} = \frac{a\sqrt{6}}{3}$|
|Vzdálenost vrcholu od protější stěny|$= \frac{a\sqrt{6}}{3} \cdot \frac{3}{4} \cdot 4 = \frac{a\sqrt{6}}{3}$ _(celá výška)_|
|Odchylka hrany od protilehlé stěny|$\approx 54°44'$|
|Odchylka dvou stěn|$\approx 70°32'$|

---

## 23.9 Rychlý přehled – vzorce na jednom místě

```
PLOCHY:
  Čtverec:         S = a²
  Obdélník:        S = a·b
  Trojúhelník:     S = ½·a·h
  Lichoběžník:     S = ½·(a+c)·h
  Kruh:            S = π·r²

TĚLESA – OBJEM:
  Hranol:          V = S_p · v
  Jehlan:          V = ⅓ · S_p · v
  Komolý jehlan:   V = v/3 · (S₁ + √(S₁·S₂) + S₂)
  Válec:           V = π·r²·v
  Kužel:           V = ⅓·π·r²·v
  Koule:           V = 4/3·π·r³
  Kulová úseč:     V = π·h²/3·(3r−h)

TĚLESA – POVRCH:
  Krychle:         P = 6·a²
  Kvádr:           P = 2·(ab+bc+ac)
  Válec:           P = 2π·r·(r+v)
  Kužel:           P = π·r·(r+s),   s = √(r²+v²)
  Koule:           P = 4·π·r²

ÚHLOPŘÍČKY (krychle a = hrana):
  Stěnová:         u_s = a·√2
  Tělesová:        u = a·√3
```

---

## 23.10 Časté chyby a na co si dát pozor

> ⚠️ **Odchylka vs. úhel doplňkový:** Odchylka je vždy ostrý nebo pravý úhel (0° až 90°). Pokud vyjde tupý, vezmi doplněk do 180°.

> ⚠️ **Apotéma ≠ výška jehlanu:** Apotéma ($v_s$) je výška boční stěny, výška ($v$) je kolmá vzdálenost vrcholu od podstavy.

> ⚠️ **Povrch = 2 × podstavy + plášť** (u hranolu/válce), ale jen **1 × podstava + plášť** u jehlanu/kužele.

> ⚠️ **Komolý jehlan:** vzorec pro objem je specifický – neplést s hranolem!

> ⚠️ **Pravidelný n-úhelník:** obsah se počítá přes poloměr vepsané kružnice (apotému), ne přes poloměr opsané!
