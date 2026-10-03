# PIKT 2026 – T09: Právna zodpovednosť za kybernetický incident[cite: 1]

Prezentácia a tímové podklady k ročníkovej práci z predmetu Právo informačných a komunikačných technológií (PIKT 2026) na FIIT STU[cite: 1].

---

## 👥 Rozdelenie úloh v tíme[cite: 1]

* **Časť 1:** Pojem incidentu a prevencia (Otázky 1 a 2 zo zadania – Zákon o KB č. 69/2018 Z. z., smernica NIS 2, technické a organizačné opatrenia)[cite: 1].
* **Časť 2:** Notifikačné povinnosti (Otázka 3 zo zadania – hlásenie na NBÚ, SK-CERT a Úrad na ochranu osobných údajov, lehoty 24 h / 72 h podľa NIS 2 a GDPR)[cite: 1].
* **Časť 3 (Arsenii Leno):** Formy právnej zodpovednosti (Otázka 4 zo zadania – trestná zodpovednosť útočníka podľa § 247 TZ, správne pokuty a osobná zodpovednosť manažmentu)[cite: 1].
* **Časť 4:** Prípadová štúdia reálneho kybernetického útoku (Otázka 5 zo zadania – rozbor konkrétneho incidentu a aplikácia právnych noriem)[cite: 1].

---

## 📋 Formálne požiadavky na prácu[cite: 1]

* **Celkový rozsah práce:** 2 000 – 4 000 slov pre 4-člennú skupinu[cite: 1].
* **Minimálny rozsah na člena:** Každý autor musí vypracovať najmenej 500 slov[cite: 1].
* **Evidencia autorstva:** V texte práce musí byť jednoznačne uvedené meno autora konkrétnej časti a jej presný rozsah v slovách[cite: 1].
* **Právny základ:** Text nesmie zostať len v rovine technického opisu a musí obsahovať aspoň jeden konkrétny prípad alebo judikatúru[cite: 1].

---

## 🚀 Vibe-coding návod (Marp prezentácia)

Prezentácia sa vytvára priamo z Markdown súboru `presentation.md` prostredníctvom nástroja **Marp**.

### 1. Inštalácia závislostí
Pred prvým spustením si nainštalujte balíky:
```bash
npm install

```

### 2. Spustenie živého náhľadu (Live Reload)

Pre interaktívnu úpravu slajdov v reálnom čase spustite:

```bash
npm run dev

```

*Prehliadač sa automaticky obnoví pri každom uložení súboru `presentation.md`.*

### 3. Export prezentácie

* **Generovanie HTML prezentácie:**
```bash
npm run build:html

```


* **Generovanie PDF verzie:**
```bash
npm run build:pdf

```



---

## ✍️ Štruktúra zápisu slajdov

* **Nový slajd:** Oddeľuje sa tromi pomlčkami:
```markdown
---

```


* **Titulný slajd sekcie:** Použite direktívu inverzie farieb:
```markdown
<!-- _class: invert -->
# ČASŤ X
### Názov sekcie

```


* **Formátovanie textu:** Používajte stručné body, odrážky a tučné zvýraznenie dôležitých právnych pojmov.

---

## 🔄 Git workflow pre spoluprácu

1. Pred začiatkom práce si vždy stiahnite aktuálny stav z GitHubu:
```bash
git pull origin main

```


2. Upravte svoju časť v súbore `presentation.md`.
3. Skontrolujte zmeny a odošlite ich:
```bash
git add presentation.md
git commit -m "feat(sekcia-X): aktualizácia obsahu"
git push origin main

```

Dokumentet strukturerar projektets formella ramar med ett totalt ordkrav på 2 000–4 000 ord och minst 500 ord per person[cite: 1], fördelar ansvarsområdena för tema T09[cite: 1] samt förklarar de tekniska kommandona för Marp och versionshanteringen i Git.

```
