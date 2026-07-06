---
tags: [systeem, conventie]
type: systeem
---

# Naming Convention — AKO v1.1

> Harde regels voor bestandsnamen in de hele vault.
> Consistente naamgeving voorkomt kapotte links en dubbele pagina's.

**Systeemkoppelingen:** [[AKO v1.0]] · [[AKO v1.1]] · [[AKO v1.2]] · [[AKO v1.3]] · [[AKO v1.4]] · [[AKO v1.5]] · [[AKO v1.6]] · [[Wiki Template]] · [[Link Protocol]] · [[Shared Memory]]

---

## Algemene regels

1. **Taal:** Nederlands. Uitzondering: wetenschappelijke termen zonder gangbare Nederlandse vertaling blijven Engels (bijv. `Prospect Theory`, `Default Mode Network`).
2. **Spaties toegestaan.** Obsidian ondersteunt spaties in bestandsnamen. Gebruik ze voor leesbaarheid.
3. **Title Case.** Elk hoofdwoord begint met een hoofdletter: `Cognitieve Dissonantie`, `Efficiënte Markthypothese`.
4. **Geen prefixen of suffixen.** Geen `01_`, geen `(C)`, geen `[KG]`. De map bepaalt het type.
5. **Geen speciale tekens** behalve koppelteken (–) en ampersand (&) waar inhoudelijk nodig.

---

## Per maptype

### 02 Wiki — conceptpagina's

| Correct | Fout |
|---|---|
| `Prospect Theory.md` | `01_Prospect_Theory.md` |
| `Cognitieve Dissonantie.md` | `cognitieve-dissonantie.md` |
| `Werkgeheugen.md` | `(C) Werkgeheugen.md` |
| `Efficiënte Markthypothese.md` | `EMH.md` |

- Gebruik de volledige naam, geen afkortingen als paginanaam.
- Aliassen mogen wel in de frontmatter staan: `aliases: ["EMH"]`

### 02 Wiki — hubpagina's

Enkelvoudig, één woord, geen suffix:

`Psychologie.md` · `Filosofie.md` · `Geschiedenis.md` · `Beleggen.md`

### 03 conceptual graph — relatiepagina's (Agent 4)

Beschrijf de relatie met een koppelteken tussen de twee concepten:

`Verliesaversie — Prospect Theory.md`
`Inhibitie — Rationeel Handelen.md`

### 03 conceptual graph — inzichtpagina's (Agent 5)

Beschrijf het patroon of het inzicht direct:

`Rede als Correctiemechanisme.md`
`Kritische Perioden in Systemen.md`

### 04 Daily summeries

`YYYY-MM-DD Dagrapport.md`

Voorbeeld: `2026-07-03 Dagrapport.md`

### 05 Daily quizzes

Quiz: `YYYY-MM-DD Quiz.md`

Leerpad: `YYYY-MM-DD Leerpad [Onderwerp].md`

Voorbeelden:
- `2026-07-03 Quiz.md`
- `2026-07-03 Leerpad Prospect Theory.md`

### 07 Reflection

`YYYY-WW Reflectie.md`

`WW` = weeknummer (01–53), altijd twee cijfers.

Voorbeeld: `2026-27 Reflectie.md`

---

## Conflictoplossing

Wanneer twee pagina's dezelfde naam zouden krijgen:

1. Controleer eerst of het écht hetzelfde concept is → samenvoegen (Agent 3).
2. Zo niet: voeg een verduidelijking toe tussen haakjes: `Aandacht (Cognitief).md` vs. `Aandacht (Klinisch).md`

---

## Verboden

- Nooit een pagina hernoemen zonder alle links naar die pagina bij te werken.
- Nooit afkortingen als primaire paginanaam.
- Nooit datums in Wiki-paginanamen.
