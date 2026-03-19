## 17.1 Základní trigonometrické funkce v pravoúhlém trojúhelníku

Pro pravoúhlý trojúhelník s pravým úhlem u $C$, přeponou $c$ a odvěsnami $a$, $b$:

$$\sin \alpha = \frac{a}{c} \qquad \cos \alpha = \frac{b}{c} \qquad \tan \alpha = \frac{a}{b} \qquad \cot \alpha = \frac{b}{a}$$

### Výškový a hloubkový úhel:

```
        objekt
       /|
      / |
     /  | výška
    /α  |
   /    |
pozorovatel -------- bod pod objektem
```

- **Výškový úhel** $\alpha$ – díváme se **nahoru** od horizontály
- **Hloubkový úhel** $\beta$ – díváme se **dolů** od horizontály

---

## 17.2 Sinová věta

### Znění:

> V každém trojúhelníku platí: poměr délky strany k sinu protilehlého úhlu je pro všechny strany stejný (= průměr opsané kružnice).

$$\boxed{\frac{a}{\sin \alpha} = \frac{b}{\sin \beta} = \frac{c}{\sin \gamma} = 2R}$$

kde $R$ je poloměr kružnice opsané trojúhelníku.

### Kdy použít sinovou větu:

|Zadání|Použij|
|---|---|
|1 strana + 2 úhly (USU, SSU, SUU)|Sinová věta ✅|
|2 strany + protilehlý úhel (SSÚ)|Sinová věta ✅ (pozor na 2 řešení!)|
|3 strany (SSS)|Kosinová věta|
|2 strany + sevřený úhel (SÚS)|Kosinová věta|

### Postup řešení (2 strany + protilehlý úhel – SSÚ):

⚠️ **Ambiguitní případ** – může existovat 0, 1 nebo 2 řešení!

Pokud je dáno $a$, $b$, $\alpha$:

1. Vypočti $\sin \beta = \frac{b \sin \alpha}{a}$
2. Pokud $\sin \beta > 1$ → **žádné řešení**
3. Pokud $\sin \beta \leq 1$:
    - $\beta_1 = \arcsin(\sin \beta)$
    - $\beta_2 = 180° - \beta_1$ (zkontroluj, zda $\alpha + \beta_2 < 180°$)
    - Pro každé přípustné $\beta$ dopočítej $\gamma$ a $c$

**Příklad (úloha 3):** $a = 65$ cm, $b = 46$ cm, $\alpha = 42°35'$

$$\sin \beta = \frac{46 \cdot \sin 42°35'}{65} = \frac{46 \cdot 0{,}6756}{65} \approx 0{,}4778 \implies \beta \approx 28°33'$$

$\beta_2 = 180° - 28°33' = 151°27'$: $\alpha + \beta_2 = 42°35' + 151°27' > 180°$ → **nevyhovuje**

→ Jen jedno řešení: $\gamma = 180° - 42°35' - 28°37' = 108°48'$

Ze sinové věty: $c = \frac{a \sin \gamma}{\sin \alpha} = \frac{65 \cdot \sin 108°48'}{\sin 42°35'} \approx 90{,}9$ cm ✅

---

## 17.3 Kosinová věta

### Znění:

> Čtverec libovolné strany trojúhelníku se rovná součtu čtverců zbývajících dvou stran, zmenšenému o dvojnásobek jejich součinu vynásobeného kosinem sevřeného úhlu.

$$\boxed{a^2 = b^2 + c^2 - 2bc \cos \alpha}$$ $$b^2 = a^2 + c^2 - 2ac \cos \beta$$ $$c^2 = a^2 + b^2 - 2ab \cos \gamma$$

### Odvozený tvar (pro výpočet úhlu ze tří stran):

$$\cos \alpha = \frac{b^2 + c^2 - a^2}{2bc}$$

### Kdy použít kosinovou větu:

|Zadání|Co počítám|
|---|---|
|3 strany (SSS)|Všechny úhly|
|2 strany + sevřený úhel (SÚS)|Třetí stranu, pak úhly|

### Příklad (úloha 1): $a = 32{,}5$, $b = 58{,}4$, $c = 72{,}6$ cm

$$\cos \alpha = \frac{58{,}4^2 + 72{,}6^2 - 32{,}5^2}{2 \cdot 58{,}4 \cdot 72{,}6} = \frac{3410 + 5271 - 1056}{8481} \approx 0{,}8987 \implies \alpha \approx 25°57'$$

Analogicky $\beta \approx 51°49'$, $\gamma = 180° - \alpha - \beta \approx 102°14'$ ✅

### Příklad (úloha 12): $b = a+2$, $c = a+3$, $\beta = 60°$

Ze sinové věty: $$\cos 60° = \frac{a^2 + (a+3)^2 - (a+2)^2}{2a(a+3)} = \frac{1}{2}$$

$$a^2 + a^2 + 6a + 9 - a^2 - 4a - 4 = a(a+3)$$ $$a^2 + 2a + 5 = a^2 + 3a \implies a = 5 \text{ cm}$$

---

## 17.4 Vlastnosti trojúhelníku – přehled vzorců

### Základní vztahy:

$$\alpha + \beta + \gamma = 180°$$

### Obsah trojúhelníku – různé vzorce:

| Vzorec                                        | Kdy použít                           |
| --------------------------------------------- | ------------------------------------ |
| $S = \frac{1}{2} a \cdot h_a$                 | znám stranu a výšku                  |
| $S = \frac{1}{2} ab \sin \gamma$              | znám 2 strany a sevřený úhel         |
| $S = \frac{abc}{4R}$                          | znám 3 strany a opsanou kružnici     |
| Heronův vzorec: $S = \sqrt{s(s-a)(s-b)(s-c)}$ | znám 3 strany; $s = \frac{a+b+c}{2}$ |

### Poloměry kružnic:

$$R = \frac{a}{2\sin\alpha} = \frac{abc}{4S} \quad \text{(opsaná)}$$ $$r = \frac{S}{s} \quad \text{(vepsaná)}, ; s = \frac{a+b+c}{2}$$

---

## 17.5 Řešení obecného trojúhelníku – postup

### Krok 1: Rozpoznej typ zadání

```
SSS  → kosinová věta → všechny úhly
SÚS  → kosinová věta → 3. strana → sinová → zbývající úhly
USU  → sinová věta → zbývající strany
SUU  → sinová věta (γ = 180°-α-β) → zbývající strany
SSÚ  → sinová věta → POZOR na 2 řešení!
```

### Krok 2: Výpočet

### Krok 3: Ověření

- Součet úhlů = 180°
- Největší strana leží naproti největšímu úhlu
- Trojúhelníková nerovnost: každá strana < součet zbývajících dvou

---

## 17.6 Lichoběžník a rovnoběžník – výpočty trigonometrií

### Lichoběžník (úloha 11): $a = 30$, $b = 13$, $c = 16$, $d = 15$ cm

**Postup:** Spustíme výšku(y), vzniknou pravoúhlé trojúhelníky. Nebo pomocí kosinové věty po rozdělení na trojúhelník + obdélník.

Pro rovnoramenný lichoběžník: $b = d$, výška $h = \sqrt{b^2 - \left(\frac{a-c}{2}\right)^2}$

Pro obecný lichoběžník: Prodlužme stranu $c$ na délku $a$. Přebytek $= a - c$ rozdělíme podle výšek bočních stran. Označme $x$ a $a - c - x$: $$x^2 + h^2 = d^2, \quad (a-c-x)^2 + h^2 = b^2$$

### Rovnoběžník (úloha 9): $a = 58$ cm, $u = 89$ cm, $v = 52$ cm

Úhlopříčky rovnoběžníku se navzájem půlí → polovina každé úhlopříčky: $p = 44{,}5$ cm, $q = 26$ cm.

Z kosinové věty v trojúhelníku tvořeném stranami $a$, $p$, $q$: $$\cos \varphi = \frac{a^2 + q^2 - p^2}{2aq}$$

Obsah rovnoběžníku: $S = ab \sin \alpha$ nebo $S = \frac{u \cdot v \cdot \sin \varphi}{2} \cdot 2 = uv\sin\varphi/2 \cdot 2$

Přesněji: $S = \frac{1}{2} u \cdot v \cdot \sin \varphi$ kde $\varphi$ je úhel mezi úhlopříčkami:

Z kosinovy věty: $a^2 = \left(\frac{u}{2}\right)^2 + \left(\frac{v}{2}\right)^2 - 2\cdot\frac{u}{2}\cdot\frac{v}{2}\cos\varphi$ $$58^2 = 44{,}5^2 + 26^2 - 2\cdot44{,}5\cdot26\cdot\cos\varphi$$ $$\cos\varphi = \frac{1980{,}25 + 676 - 3364}{2313} \approx -0{,}2974 \implies \varphi \approx 107°17'$$

$S = \frac{1}{2}\cdot89\cdot52\cdot\sin(107°17') \approx 2203$ cm² 

---

## 17.7 Praktické aplikace – typy úloh

### Typ 1: Výška budovy / mraku (výškový úhel)

```
          X (objekt)
         /|
        / |
       /  | h
      /α  |
     /    |
    P------B
       d
```

$\tan \alpha = \frac{h}{d} \implies h = d \cdot \tan \alpha$

**Příklad (úloha 14) – výška mraku:**

Pozorovatelna $P$ ve výšce $115$ m nad jezerem. Výškový úhel k mraku $\alpha = 20°57'$, hloubkový úhel k obrazu mraku v jezeře $\beta = 24°12'$.

Označme výšku mraku nad hladinou $H$, vodorovnou vzdálenost $d$: $$\tan \alpha = \frac{H - 115}{d}, \quad \tan \beta = \frac{H + 115}{d}$$

Vydělíme: $\frac{\tan \beta}{\tan \alpha} = \frac{H + 115}{H - 115}$

$H(\tan\beta - \tan\alpha) = 115(\tan\beta + \tan\alpha) \implies H = 115 \cdot \frac{\tan\beta + \tan\alpha}{\tan\beta - \tan\alpha} \approx 1438$ m 

---

### Typ 2: Letadlo – dvě polohy (úloha 15)

Výška letadla $h = 3500$ m (konstantní). Úhly $\alpha_1 = 25°$, $\alpha_2 = 48°$.

Vzdálenosti pozorovatelny od bodu pod letadlem: $$d_1 = \frac{h}{\tan \alpha_1}, \quad d_2 = \frac{h}{\tan \alpha_2}$$

Uletěná vzdálenost: $\Delta d = d_1 - d_2 = h\left(\frac{1}{\tan\alpha_1} - \frac{1}{\tan\alpha_2}\right)$

$$= 3500\left(\frac{1}{\tan 25°} - \frac{1}{\tan 48°}\right) = 3500(2{,}145 - 0{,}900) \approx 4354 \text{ m}$$ 

---

### Typ 3: Zorný úhel (úloha 8)

Pozorovatel P, předmět délky $a = 12$ m, vzdálenosti $PA = 15$ m, $PB = 24$ m.

Z kosinové věty v trojúhelníku PAB: $$\cos \varphi = \frac{PA^2 + PB^2 - AB^2}{2 \cdot PA \cdot PB} = \frac{225 + 576 - 144}{720} = \frac{657}{720} \approx 0{,}9125 \implies \varphi \approx 24°9'$$

---

### Typ 4: Skládání a rozkládání sil (úlohy 5, 6)

**Výslednice dvou sil** $F_1$, $F_2$ svírajících úhel $\alpha$:

V trojúhelníku sil: strany $F_1$, $F_2$, výslednice $F$. Úhel mezi $F_1$ a $F_2$ je $\alpha$, takže vnitřní úhel trojúhelníku je $180° - \alpha$.

$$F^2 = F_1^2 + F_2^2 - 2F_1 F_2 \cos(180° - \alpha) = F_1^2 + F_2^2 + 2F_1 F_2 \cos\alpha$$

**Příklad (úloha 5):** $F_1 = 84{,}5$ N, $F_2 = 47{,}8$ N, $\alpha = 56°40'$

$$F = \sqrt{84{,}5^2 + 47{,}8^2 + 2\cdot84{,}5\cdot47{,}8\cdot\cos56°40'} \approx 117{,}75 \text{ N}$$ 

**Rozklad síly** $F$ na dvě složky $F_1$, $F_2$ svírající s ní úhly $\alpha$ a $\beta$:

Ze sinové věty v trojúhelníku sil (úhel u $F$ = $180° - \alpha - \beta$): $$\frac{F}{\sin(180°-\alpha-\beta)} = \frac{F_1}{\sin\beta} = \frac{F_2}{\sin\alpha}$$ $$F_1 = \frac{F\sin\beta}{\sin(\alpha+\beta)}, \quad F_2 = \frac{F\sin\alpha}{\sin(\alpha+\beta)}$$

**Příklad (úloha 6):** $F = 2217{,}6$ N, $\alpha = 46°32'$, $\beta = 54°12'$

$$F_1 = \frac{2217{,}6\cdot\sin54°12'}{\sin(100°44')} \approx 1830{,}6 \text{ N}$$ 

---

### Typ 5: Šířka příkopu / řeky (úloha 4)

**Příkop s profilem rovnoramenného lichoběžníku:** dno $d = 2{,}75$ m, ramena $r = 3{,}5$ m, úhel $\alpha = 28°$

Výška: $h = r\sin\alpha = 3{,}5\cdot\sin28° \approx 1{,}64$ m Přesah ramene: $x = r\cos\alpha = 3{,}5\cdot\cos28° \approx 3{,}09$ m Šířka nahoře: $s = d + 2x = 2{,}75 + 6{,}18 \approx 8{,}93$ m 

**Šířka řeky (úloha 10):**

Pozorovatelna výška $v = 15$ m, vodorovná vzdálenost od břehu $l = 30$ m. Zorný úhel $\varphi = 15°$.

Vzdálenost k bližšímu břehu řeky: $\tan\alpha_1 = \frac{v}{l} \implies \alpha_1 = \arctan\frac{15}{30}$ Vzdálenost k vzdálenějšímu: tangens se liší o úhel $\varphi$.

Označme $\alpha_1$ úhel hloubkový k bližšímu břehu, $\alpha_2 = \alpha_1 - \varphi$ k vzdálenějšímu: $$\text{šířka} = v\left(\frac{1}{\tan\alpha_2} - \frac{1}{\tan\alpha_1}\right) - l + l = v(\cot\alpha_2 - \cot\alpha_1)$$

Numericky: $\alpha_1 = \arctan(15/30) = 26{,}57°$, $\alpha_2 = 26{,}57° - 15° = 11{,}57°$ $$\text{šířka} = 15(\cot11{,}57° - \cot26{,}57°) \approx 15(4{,}89 - 2) \approx 43{,}3 \text{ m}$$

---

## 17.8 Pravoúhlý trojúhelník – řešení ze součtu stran (úloha 13)

**Zadání:** $a + b = 9{,}6$ m, $\alpha = 37°30'$

Z definice: $\tan\alpha = \frac{a}{b} \implies a = b\tan\alpha$

Dosadíme: $b\tan\alpha + b = 9{,}6 \implies b = \frac{9{,}6}{1 + \tan37°30'} = \frac{9{,}6}{1 + 0{,}7673} \approx 4{,}17$ m

$a = 9{,}6 - 4{,}17 = 5{,}43$ m, $c = \frac{a}{\sin\alpha} = \frac{5{,}43}{\sin37°30'} \approx 6{,}85$ m 

---

## 17.9 Pravidelný $n$-úhelník

Pro pravidelný $n$-úhelník se stranou $a$ a poloměrem opsané kružnice $R$:

$$a = 2R\sin\frac{\pi}{n} = 2R\sin\frac{180°}{n}$$

Poloměr vepsané kružnice (apotéma): $$r = R\cos\frac{\pi}{n}$$

Obsah: $$S = \frac{1}{2} n a r = \frac{n a^2}{4}\cot\frac{\pi}{n} = n R^2\sin\frac{\pi}{n}\cos\frac{\pi}{n} = \frac{n R^2}{2}\sin\frac{2\pi}{n}$$

Vnitřní úhel: $$\varphi = \frac{(n-2)\cdot 180°}{n}$$

---

## 17.10 Přehled vzorců na jednom místě

```
SINOVÁ VĚTA:
  a/sin α = b/sin β = c/sin γ = 2R
  → použij pro: USU, SUU, SSÚ (pozor: 2 řešení!)

KOSINOVÁ VĚTA:
  a² = b² + c² - 2bc·cos α
  cos α = (b² + c² - a²) / (2bc)
  → použij pro: SSS, SÚS

OBSAH TROJÚHELNÍKU:
  S = ½·a·hₐ = ½·ab·sin γ
  S = √[s(s-a)(s-b)(s-c)],  s = (a+b+c)/2  [Heron]

PRAKTICKÉ VZORCE:
  výška z úhlu:     h = d·tan α
  skládání sil:     F² = F₁² + F₂² + 2F₁F₂·cos α
  rozkládání sil:   F₁ = F·sin β / sin(α+β)
  pravidelný n-úhel: a = 2R·sin(180°/n)

ŘEŠENÍ TROJÚHELNÍKU:
  SSS  → kosinová věta → úhly
  SÚS  → kosinová věta → 3. strana → sinová → úhly
  USU/SUU → sinová věta → strany
  SSÚ  → sinová věta → OVĚŘIT 2 řešení
```

