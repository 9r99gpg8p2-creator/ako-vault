---
tags: [systeem, protocol]
type: systeem
---

# Link Protocol — AKO v1.1

> Harde regels voor het aanmaken en beheren van verbindingen.
> Agent 4 volgt dit protocol exact.

**Systeemkoppelingen:** [[AKO v1.0]] · [[AKO v1.1]] · [[AKO v1.2]] · [[AKO v1.3]] · [[AKO v1.4]] · [[AKO v1.5]] · [[AKO v1.6]] · [[Wiki Template]] · [[Naming Convention]] · [[Shared Memory]]

---

## Principe

Een link bestaat alleen als er een betekenisvolle intellectuele relatie is.

Elke link heeft een type. Een link zonder type is verboden.

---

## Minimumnormen per pagina

| Type pagina | Minimum links | Maximum links |
|---|---|---|
| Wiki-concept | 3 | 12 |
| Hub | 5 | onbeperkt |
| Graph relatiepagina | 2 | 6 |
| Graph inzichtpagina | 3 | 10 |

Pagina's onder het minimum worden door Agent 7 gemarkeerd als incompleet.

---

## Verplichte linktypen per Wiki-pagina

### 1. Hub-link en sub-hub-link (verplicht)

Elke Wiki-pagina linkt naar precies één sub-hub (indien aanwezig) of direct naar de domein-hub.

```markdown
**Hub:** [[Psychologie]]
**Subcategorie:** [[Cognitieve Psychologie]]
```

### 2. Gerelateerde concepten (minimaal 2) met verbindingssterkte

Altijd met expliciet type én sterktescore (★1–10):

```markdown
**Gerelateerd:**
- [[Werkgeheugen]] ★7 — onderdeel van: executieve functies
- [[Prefrontale Cortex]] ★8 — neurale basis van dit concept
- [[ADHD]] ★6 — klinische casus van gebrekkige inhibitie
```

**Verbindingssterkte ★ — schaal:**

| Score | Betekenis |
|---|---|
| 9–10 | Fundamentele relatie — kernverbinding in het netwerk |
| 7–8 | Sterke relatie — breed onderbouwd, meerdere bronnen |
| 5–6 | Matige relatie — plausibel, beperkt bewijs |
| 3–4 | Zwakke relatie — suggestief, hypothetisch |
| 1–2 | Speculatief — voor verder onderzoek |

Agent 4 kent de sterkte toe en herberekent deze wanneer nieuwe literatuur beschikbaar komt.

### 3. Cross-domein links (optioneel, max 20% van alle links)

Alleen na inhoudelijke verificatie. Altijd met reden:

```markdown
**Cross-domein:**
- [[Efficiënte Markthypothese]] — gedeeld principe: gebrekkige remming ondermijnt rationeel systeem
```

---

## Toegestane relatietypen

| Type | Gebruik wanneer |
|---|---|
| `oorzaak` | A veroorzaakt B |
| `gevolg` | A is het gevolg van B |
| `onderdeel van` | A is een subcomponent van B |
| `overkoepelt` | A is de bredere categorie van B |
| `tegenstelling` | A en B staan conceptueel tegenover elkaar |
| `aanvulling` | A en B versterken elkaars verklaring |
| `historische parallel` | A vertoont hetzelfde patroon als B in andere context |
| `psychologisch mechanisme` | A verklaart het gedrag beschreven in B |
| `gedeeld mentaal model` | A en B beschrijven hetzelfde principe vanuit ander domein |
| `neurale basis` | A is de neurologische onderbouwing van B |
| `klinische casus` | A is een concreet geval van het abstracte principe B |

---

## Waar links staan

Links staan op **twee plaatsen** in elke pagina:

1. **Frontmatter** — voor machines en Agent 7:
```yaml
related:
  - "[[Werkgeheugen]]"
  - "[[Prefrontale Cortex]]"
```

2. **Body (sectie Verbindingen)** — voor leesbaarheid, altijd met relatietype:
```markdown
## Verbindingen
- [[Werkgeheugen]] — onderdeel van: executieve functies
```

Beide moeten gesynchroniseerd zijn. Agent 4 controleert dit.

---

## Graph-noten (03 conceptual graph/)

### Relatiepagina's — Agent 4

Wanneer een relatie tussen twee concepten complex genoeg is voor een eigen pagina:

```markdown
---
type: relatie
concepts:
  - "[[Concept A]]"
  - "[[Concept B]]"
relatietype: gedeeld mentaal model
discipline: [beide disciplines]
created: YYYY-MM-DD
---

# Concept A — Concept B

[Beschrijving van de relatie. Waarom zijn deze concepten verbonden? Wat leren we van de vergelijking?]

## Bewijs
[Onderbouwing van de relatie]

## Implicaties
[Wat volgt hieruit voor beide domeinen?]
```

### Inzichtpagina's — Agent 5

```markdown
---
type: inzicht
disciplines: [minimaal 2]
hypothese: [ja | nee]
confidence: [1–10]
created: YYYY-MM-DD
---

# [Naam van het inzicht of patroon]

## Patroon
[Beschrijving van het terugkerende principe]

## Bewijs per discipline
### Psychologie
### Filosofie
### Geschiedenis
### Beleggen

## Hypothese
[Wat voorspelt dit patroon? Wat zou het weerleggen?]

## Verbonden concepten
- [[Concept A]]
- [[Concept B]]
```

---

## Verboden

- Nooit een link zonder relatietype in de body.
- Nooit meer dan 20% cross-domein links per pagina.
- Nooit linken naar een pagina die niet bestaat (unresolved links = fout van Agent 4).
- Nooit een link verwijderen zonder te controleren of de relatie écht zwak is.
