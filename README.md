# 🐶 Dog Breeds Analysis Dashboard

---

## 📌 O projektu

Tento projekt vznikl jako závěrečný projekt v rámci kurzu **Power BI v Engeto Academy**.

Cílem bylo vytvořit interaktivní report pro analýzu dat o psích plemenech. Report umožňuje porovnávat fyzické a behaviorální charakteristiky jednotlivých plemen, sledovat rozdíly mezi skupinami a zobrazit detailní profil konkrétního plemene.

---

## 📊 Použitá data

Dataset obsahuje informace o **391 psích plemenech**.

Mezi analyzované oblasti patří:

- skupina plemene,
- velikost plemene,
- průměrná výška,
- průměrná hmotnost,
- průměrná délka života,
- inteligence,
- cvičitelnost,
- energetická úroveň,
- celkový zdravotní stav,
- potřeba pohybu,
- vztah k rodině, dětem, cizím lidem a ostatním psům,
- odkaz na detailní informace o plemeni.

---

## 🧭 Struktura reportu

Report obsahuje čtyři interaktivní stránky.

### 1. Executive Dashboard

Úvodní stránka poskytuje základní přehled o datasetu.

Obsahuje:

- celkový počet plemen,
- průměrnou výšku,
- průměrnou hmotnost,
- průměrnou délku života,
- rozdělení plemen podle skupin,
- rozdělení plemen podle velikosti.

### 2. Physical Characteristics

Stránka zaměřená na fyzické vlastnosti plemen.

Obsahuje:

- tabulku s detaily jednotlivých plemen,
- scatter plot výšky a hmotnosti,
- průměrnou délku života podle skupin plemen,
- dynamický panel **Did You Know?**

### 3. Behavior & Lifestyle

Stránka porovnává behaviorální charakteristiky mezi skupinami plemen.

Obsahuje:

- matici jednotlivých behaviorálních atributů,
- porovnání ukazatelů **Social Friendliness**, **Learning Ability** a **Activity Needs**,
- dynamický textový panel **Behavior Insight**.

### 4. Breed Profile

Detailní profil vybraného plemene.

Obsahuje:

- výběr podle skupiny, velikosti a názvu plemene,
- základní fyzické charakteristiky,
- hvězdičkové behaviorální hodnocení,
- slovní kategorii společenskosti,
- dynamický odkaz na podrobný popis plemene,
- tlačítko pro vymazání všech průřezů.

---

## 🗂️ Datový model

Datový model je vytvořen jako jednoduché hvězdicové schéma.

Použité tabulky:

- `Dogs`
- `Breed Groups`
- `Dog Sizes`
- `Measure Table`

Tabulky `Breed Groups` a `Dog Sizes` jsou propojeny s tabulkou `Dogs` relacemi typu **1:N**.

# 🧮 DAX

Projekt obsahuje vlastní:

- Measures
- Kalkulované sloupce
- Kalkulovanou tabulku

## Příklady vytvořených measures

- Total Breeds
- Average Height (cm)
- Average Weight (kg)
- Average Lifespan (years)
- Average Social Friendliness
- Average Learning Ability
- Average Activity Needs
- Behavior Insight
- Fun Fact
- Selected Breed
- Selected Height
- Selected Weight
- Selected Lifespan

## Kalkulovaný sloupec

Projekt využívá kalkulovaný sloupec:

`Family Friendliness Category`

který na základě kombinace atributů:

- Kid-Friendly
- Affectionate With Family
- Dog Friendly
- Friendly Toward Strangers

vytváří slovní kategorii společenskosti:

- Highly Social
- Moderately Social
- Less Social

---

# ⚙️ Použité technologie

- Microsoft Power BI Desktop
- Power Query
- DAX

---

# 🎨 Použité prvky Power BI

V projektu byly využity:

- KPI Cards
- Table
- Matrix
- Clustered Column Chart
- Donut Chart
- Scatter Plot
- Slicery
- Navigace mezi stránkami
- Dynamické textové prvky
- Dynamický Web URL
- Reset Filters
- Cross-filtering mezi vizuály

---

# ✨ Hlavní funkce reportu

| Funkce | Popis |
|--------|-------|
| 📌 Interaktivní slicery | Filtrování podle skupiny, velikosti a plemene |
| 🧭 Navigace | Přepínání mezi stránkami reportu |
| 💡 Dynamické texty | Did You Know? a Behavior Insight |
| ⭐ Behaviorální hodnocení | Hvězdičkové hodnocení vlastností |
| 🐕 Breed Profile | Detailní informace o vybraném plemeni |
| 🌐 Learn More | Přímý odkaz na detailní popis plemene |
| 🔄 Reset Filters | Vymazání všech filtrů na stránce |

---

# 📁 Struktura projektu

```text
Dog-Breeds-Analysis/
│
├── Dog_Breeds_Analysis.pbix
├── dogs_cleaned.csv
├── README.md
└── images/
    └── dashboard-preview.png
```

---
