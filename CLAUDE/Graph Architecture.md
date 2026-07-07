---
tags: [systeem, architectuur]
type: architectuur
---

# Graph Architecture — AKO

> Permanente architectuurregels voor de Obsidian graph.
> Wordt gelezen door de Orchestrator in STAP 1 en gehandhaafd in STAP 8.
> Nooit afwijken van deze structuur.

**Systeemkoppelingen:** [[AKO]] · [[AKO v1.6]] · [[Wiki Template]] · [[Link Protocol]]

---

## Centrale node

**`CLAUDE/AKO.md`** — de centrale intelligentienode van AKO.

Alle vier domein-hubs verbinden direct naar `[[AKO]]`.
Geen enkel concept verbindt direct naar AKO, tenzij het een systeemconcept is.

Kleur in graph: rgb(255, 127, 80) — integer `16744272` — `path:"CLAUDE"`

---

## Primaire domeinen

| Domein | Map | Tag | Kleur RGB | Integer |
|---|---|---|---|---|
| Psychologie | `02 Wiki/01 Psychologie - Wiki/` | `tag:psychologie` | 26, 188, 156 | 1752220 |
| Filosofie | `02 Wiki/02 Filosofie - Wiki/` | `tag:filosofie` | 155, 89, 182 | 10181046 |
| Geschiedenis | `02 Wiki/03 Geschiedenis - Wiki/` | `tag:geschiedenis` | 231, 76, 60 | 15158332 |
| Beleggen | `02 Wiki/04 Beleggen - Wiki/` | `tag:beleggen` | 227, 179, 65 | 14922561 |

---

## Wiel-architectuur

```
                       [[AKO]]
                          ●  (CLAUDE map — oranje)
           ┌──────────────┼──────────────┐──────────────┐
           │              │              │              │
    [[Psychologie]]  [[Filosofie]]  [[Geschiedenis]]  [[Beleggen]]
          ●               ●               ●               ●
          ↓               ↓               ↓               ↓
     [concepten]      [concepten]     [concepten]     [concepten]
          ↕               ↕               ↕               ↕
              cross-domein bridges (03 conceptual graph/)
```

---

## Node placement rules

Bij elke nieuwe Wiki-pagina die Agent 3 aanmaakt:

1. Bepaal het primaire domein op basis van het bestandspad
2. Zet `hub: "[[Discipline]]"` in frontmatter
3. Voeg `**Hub:** [[Discipline]]` toe in `## Verbindingen`
4. Controleer of het concept cross-domein is (bijv. Behavioral Finance → Psychologie + Beleggen)
5. Zo ja: voeg cross-domein links toe in `## Verbindingen` → `**Cross-domein:**`

---

## Cross-domein bridges — prioritaire verbindingen

| Van | Naar | Voorbeeldconcepten |
|---|---|---|
| Psychologie | Beleggen | Behavioral Finance, Verliesaversie, Prospect Theory, Cognitieve Bias |
| Filosofie | Psychologie | Bewustzijn, Vrije Wil, Epistemologie, Dualisme |
| Geschiedenis | Filosofie | Wetenschappelijke Revolutie, Verlichting, Positivisme |
| Geschiedenis | Psychologie | Wetenschapsgeschiedenis, Biografie van pioniers |
| Filosofie | Beleggen | Beslissingsethiek, Rationaliteit |

Doel: minimaal 1 cross-domein brug per 5 Wiki-pagina's.

---

## Buitenste kennisring — minimum connectivity

Elke conceptpagina moet verbinden met:
- Minimaal **1** primair domein (via hub-link in `## Verbindingen`)
- Minimaal **2** andere conceptpagina's (via related links)

Geïsoleerde nodes (0 outbound links) zijn niet toegestaan.

---

## Hub pagina's — actuele concept-index

Elke hub pagina (`Psychologie.md`, `Filosofie.md`, `Geschiedenis.md`, `Beleggen.md`) bevat:
- Link naar `[[AKO]]` (verbinding met centrale intelligentie)
- Links naar alle conceptpagina's in dat domein (sectie `## Concepten`)
- Links naar alle drie andere hubs (sectie `## Cross-domein`)

Agent 8 (Graph Architect) houdt de hub pagina's actueel na elke pipeline-run.

---

## Graph Health drempelwaarden

| Metric | Kritisch | Gezond | Uitstekend |
|---|---|---|---|
| Isolated nodes | > 5 | 0 | 0 |
| Hub connectivity | < 70% | ≥ 85% | ≥ 95% |
| Cross-domain ratio | < 1:10 | ≥ 1:5 | ≥ 1:3 |
| Hub pagina's up-to-date | Nee | Ja | Ja |

---

## Succes criteria

De graph is gezond wanneer:
- `[[AKO]]` zichtbaar centraal staat (meeste verbindingen)
- De vier domain-hubs duidelijk zichtbaar zijn als tweede ring
- Concepten zich groeperen rondom hun domein-hub
- Cross-domein bridges verbinden de vier clusters
- Geen geïsoleerde nodes
- De graph lijkt op een wiel, niet op losse clusters
