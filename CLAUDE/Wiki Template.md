---
tags: [systeem, template]
type: systeem
---

# Wiki Template — AKO v1.1

> Dit is het verplichte sjabloon voor elke Wiki-pagina.
> Agent 3 kopieert dit sjabloon en vult de placeholders in.
> Nooit afwijken van deze structuur.

**Systeemkoppelingen:** [[AKO v1.0]] · [[AKO v1.1]] · [[AKO v1.2]] · [[AKO v1.3]] · [[AKO v1.4]] · [[AKO v1.5]] · [[AKO v1.6]] · [[Naming Convention]] · [[Link Protocol]] · [[Shared Memory]]

---

## Sjabloon (kopieer dit)

```markdown
---
id: [uniek-id: discipline-concept, bijv. psych-prospect-theory]
discipline: [psychologie | filosofie | geschiedenis | beleggen]
type: [concept | theorie | gebeurtenis | model | persoon]
status: [concept | uitgewerkt | definitief]
confidence: [1–10]
sources:
  - "[Auteur (jaar). Titel. Uitgever.]"
hub: "[[Psychologie]]"
related:
  - "[[Concept A]]"
  - "[[Concept B]]"
created: [YYYY-MM-DD]
updated: [YYYY-MM-DD]
---

# [Conceptnaam]

## Definitie

[Wat is dit concept? Één alinea. Feitelijk en precies.]

## Kernconcepten

- [Kernidee 1]
- [Kernidee 2]
- [Kernidee 3]

## Context

[Historische, theoretische of wetenschappelijke context. Wanneer ontstond dit concept? Wie ontwikkelde het?]

## Toepassingen

[Hoe wordt dit concept gebruikt in de praktijk of wetenschap?]

## Verbindingen

**Hub:** [[Discipline]]

**Gerelateerd:**
- [[Concept A]] — [type relatie: oorzaak / gevolg / tegenstelling / aanvulling / onderdeel van]
- [[Concept B]] — [type relatie]
- [[Concept C]] — [type relatie]

**Cross-domein:**
- [[Concept uit ander domein]] — [reden van verbinding]

## Bronnen

- [Auteur (jaar). *Titel*. Uitgever.]
- [URL of DOI indien online]
```

---

## Confidence schaal

| Score | Betekenis |
|---|---|
| 9–10 | Wetenschappelijke consensus. Peer-reviewed, breed gerepliceerd. |
| 7–8 | Peer-reviewed. Enig debat, maar solide onderbouwing. |
| 5–6 | Geloofwaardige bronnen. Beperkt empirisch bewijs. |
| 3–4 | Plausibel. Enkelvoudige bron of expertopinie. |
| 1–2 | Speculatief. Hypothese. Niet empirisch getoetst. |

## Regels

- Elk veld in de frontmatter is verplicht.
- `related` bevat minimaal 2 en maximaal 8 items.
- `sources` bevat altijd minimaal één bron. Geen bron = confidence maximaal 4.
- `hub` is altijd één van de vier hubs: `[[Psychologie]]` · `[[Filosofie]]` · `[[Geschiedenis]]` · `[[Beleggen]]`
- Status `definitief` alleen wanneer confidence ≥ 7 én minimaal 2 bronnen aanwezig.
