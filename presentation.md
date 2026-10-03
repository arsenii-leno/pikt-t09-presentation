---
marp: true
theme: uncover
paginate: true
header: 'PIKT 2026 | T09: Kybernetický incident a zodpovednosť'
footer: 'FIIT STU v Bratislave'
style: |
  section {
    font-family: 'Inter', system-ui, sans-serif;
    text-align: left;
    background-color: #0d1117;
    color: #c9d1d9;
    padding: 40px 60px;
  }
  h1, h2, h3 {
    color: #58a6ff;
  }
  strong {
    color: #f0f6fc;
  }
  table {
    font-size: 0.72em;
    width: 100%;
    border-collapse: collapse;
    margin-top: 15px;
  }
  th {
    background-color: #161b22;
    color: #58a6ff;
    border-bottom: 2px solid #30363d;
    padding: 10px;
    text-align: left;
  }
  td {
    border-bottom: 1px solid #21262d;
    padding: 9px 10px;
  }
  .role-box {
    background-color: #161b22;
    border-left: 4px solid #58a6ff;
    padding: 12px;
    border-radius: 4px;
    margin-top: 10px;
  }
---

# Keď hacker zaútočí
## Kto nesie právnu zodpovednosť za kybernetický incident?

**Téma T09** | Predmet: PIKT 2026  
**Inštitúcia:** FIIT STU v Bratislave  
**Tím:** 4-členná študentská skupina  

---

### Rozdelenie úloh v tíme (Kto čo robí)

| Člen tímu | Modul & Otázky zo zadania | Rozsah a zameranie |
| :--- | :--- | :--- |
| **Študent 1** | **Časť 1:** Pojem incidentu a prevencia (Otázky 1 a 2) | Zákon o KB, NIS 2, tech./org. opatrenia |
| **Študent 2** | **Časť 2:** Notifikačné povinnosti (Otázka 3) | Lehoty NBÚ, CSIRT, ÚOOÚ, GDPR čl. 33/34 |
| **Arsenii Leno** | **Časť 3:** Formy právnej zodpovednosti (Otázka 4) | Trestná (TZ), správna a osobná zodpovednosť štatutára |
| **Študent 4** | **Časť 4:** Prípadová štúdia reálneho útoku (Otázka 5) | Ransomware útok, analýza zlyhaní, dopady |

---

<!-- _class: invert -->
# ČASŤ 1
### Pojem kybernetického incidentu a prevencia
**Zodpovedný:** Študent 1

---

### Čo je kybernetický incident? (Otázka 1)

* **Právna definícia:**
  * Zákon č. 69/2018 Z. z. o kybernetickej bezpečnosti a smernica NIS 2.
  * Udalosť s nepriaznivým vplyvom na dostupnosť, pravosť, integritu alebo dôvernosť uchovávaných alebo prenášaných údajov.
* **Rozlíšenie pojmov:**
  * **Zraniteľnosť:** slabina v kóde alebo infraštruktúre.
  * **Hrozba:** potenciálny aktér alebo vektor útoku.
  * **Incident:** reálne narušenie bezpečnosti s dopadom na aktíva.

---

### Bezpečnostné povinnosti organizácie (Otázka 2)

* **Kategorizácia subjektov:**
  * Prevádzkovateľ základnej služby vs. poskytovateľ digitálnej služby (podľa NIS 2: kľúčové vs. dôležité subjekty).
* **Minimálne bezpečnostné štandardy:**
  * Riadenie prístupov a identít (MFA, Zero Trust).
  * Bezpečnosť dodávateľského reťazca (*supply chain security*).
  * Pravidelné zálohovanie offline a plány kontinuity činností (BCP/DRP).
  * Pravidelné vzdelávanie personálu a penetračné testovanie.

---

<!-- _class: invert -->
# ČASŤ 2
### Notifikačné povinnosti organizácie
**Zodpovedný:** Študent 2

---

### Kedy a komu hlásiť incident? (Otázka 3)

1. **Hlásenie na NBÚ / SK-CERT:**
   * Povinné pri **závažnom kybernetickom incidente**.
   * Dvojstupňový systém lehôt podľa NIS 2:
     * **Do 24 hodín:** včasné varovanie (*early warning*).
     * **Do 72 hodín:** podrobná notifikácia incidentu s prvotným vyhodnotením.
     * **Do 1 mesiaca:** záverečná správa.
2. **Hlásenie na Úrad na ochranu osobných údajov SR (ÚOOÚ):**
   * Povinné pri úniku osobných údajov (*data breach*) podľa čl. 33 GDPR do **72 hodín**.

---

### Oznámenie dotknutým osobám a zatajenie

* **Notifikácia používateľov (čl. 34 GDPR):**
  * Ak incident predstavuje **vysoké riziko** pre práva a slobody fyzických osôb (napr. heslá, platobné údaje, rodné čísla).
  * Musí sa vykonať bez zbytočného odkladu.
* **Dôsledky zatajenia incidentu:**
  * Zatajenie je samostatným závažným správnym deliktom.
  * Priťažujúca okolnosť pri ukladaní pokút zo strany regulátora.

---

<!-- _class: invert -->
# ČASŤ 3
### Formy právnej zodpovednosti
**Zodpovedný:** Arsenii Leno

---

### Trestnoprávna zodpovednosť útočníka (Otázka 4)

* Trestný zákon SR (zákon č. 300/2005 Z. z.):
  * **§ 247:** Neoprávnený prístup do počítačového systému.
  * **§ 247a:** Neoprávnený zásah do počítačového systému alebo údajov (DDoS, zničenie/pozmenenie dát).
  * **§ 247b:** Výroba, držba a šírenie prístupového zariadenia, hesliel alebo exploitu.
* Súbeh s majetkovou kriminalitou:
  * Vydieranie (§ 189 TZ) a hrubý nátlak pri **ransomware** útokoch.

---

### Správna zodpovednosť organizácie

* **Sankcie od NBÚ (Zákon o KB a smernica NIS 2):**
  * Pokuty až do výšky **10 000 000 EUR** alebo **2 % celosvetového obratu** za zanedbanie bezpečnostných opatrení.
* **Sankcie od ÚOOÚ (GDPR):**
  * Pokuty až do **20 000 000 EUR** alebo **4 % celosvetového ročného obratu** za nedostatočné zabezpečenie dát (čl. 32 GDPR).
* **Reputačné a administratívne opatrenia:**
  * Povinné zverejnenie porušenia, auditné nápravné príkazy.

---

### Občianskoprávna zodpovednosť a štatutári

* **Zodpovednosť voči poškodeným:**
  * Náhrada skutočnej škody a ušlého zisku obchodným partnerom.
  * Nemajetková ujma dotknutých osôb za neoprávnený únik ich súkromia.
* **Osobná zodpovednosť vedenia (C-level / konatelia):**
  * Obchodný zákonník: porušenie **povinnosti konať s odbornou starostlivosťou** (*duty of care*).
  * NIS 2: možnosť priameho postihu manažmentu vrátane dočasného zákazu výkonu funkcie za ignorovanie kybernetickej bezpečnosti.

---

<!-- _class: invert -->
# ČASŤ 4
### Prípadová štúdia reálneho kybernetického útoku
**Zodpovedný:** Študent 4

---

### Prípad: Ransomware útok na zdravotnícke zariadenie (Otázka 5)

* **Vektor útoku a priebeh:**
  * Phishingový email zamestnancovi $\rightarrow$ infikovanie stanice $\rightarrow$ laterálny pohyb v sieti.
  * Exfiltrácia dát pacientov na darknet a zašifrovanie produkčných databáz.
  * Požiadavka na výkupné v kryptomene za dešifrovací kľúč.
* **Zistené zlyhania prevencie:**
  * Neaktualizovaný systém, neexistujúce segmentovanie siete, absencia offline záloh a MFA.

---

### Právne posúdenie modelového prípadu

* **Voči útočníkovi:**
  * Trestné stíhanie za neoprávnený prístup (§ 247 TZ) a vydieranie (§ 189 TZ).
* **Voči nemocnici (prevádzkovateľovi):**
  * Porušenie povinností podľa Zákona o KB (zlyhanie riadenia rizík).
  * Masívne porušenie GDPR – kompromitácia osobitnej kategórie osobných údajov o zdravotnom stave (čl. 9 GDPR).
* **Dopad:** žaloby pacientov na náhradu nemajetkovej ujmy a strata dôvery verejnosti.

---

### Záver

* Bezpečnosť v IT nie je technická voľba, ale **zákonom vymáhateľný štandard**.
* Zodpovednosť za incident sa rozpadá medzi **útočníka, organizáciu a jej vedenie**.
* Správna reakcia a včasná notifikácia (24 h / 72 h) dokážu predísť fatálnym pokutám a sankciám.

---

# Ďakujeme za pozornosť!
### Otázky a diskusia
