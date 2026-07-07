---
tags: [systeem, geheugen]
type: systeem
---

# Shared Memory Protocol — AKO v1.2

> Protocol voor gedeelde sessiecontext. Alle agents lezen dit als richtlijn.
> Shared Memory is geen databestand — het is de actieve werkcontext die Claude Code opbouwt en bijhoudt gedurende een sessie.

**Systeemkoppelingen:** [[AKO]] · [[AKO v1.6]] · [[AKO v1.5]] · [[AKO v1.4]] · [[AKO v1.3]] · [[AKO v1.2]] · [[AKO v1.1]] · [[AKO v1.0]] · [[Wiki Template]] · [[Naming Convention]] · [[Link Protocol]] · [[Task Queue]] · [[System Log]]

---

## Wat is Shared Memory?

Shared Memory is de gedeelde werksessiecontext die alle agents informeert. Het bestaat niet als een apart databestand — het is de kennis over de gebruiker en de vault-staat die Claude Code tijdens een sessie actief bijhoudt en doorgeeft aan elke volgende agent.

Elke agent ontvangt dezelfde context. Geen agent begint blind.

---

## Wat wordt bijgehouden?

### 1. Gebruikersinteresses

Onderwerpen die de gebruiker actief wil verdiepen of benadrukken. Wordt bepaald door de gebruiker zelf — Agent 6 vraagt hier dagelijks naar.

**Voorbeeld:**
> Gebruiker wil vandaag focussen op evolutionaire psychologie en de relatie met speltheorie.

### 2. Leespatronen

Auteurs, theorieën en concepten die frequent voorkomen in nieuwe Raw-bestanden. Agent 1 signaleert dit aan de Orchestrator.

**Voorbeeld:**
> Kahneman verschijnt in 4 van de laatste 5 Raw-bestanden. Taleb in 3. Signaal: behavioral economics is actief thema.

### 3. Stijgende interesses

Thema's die in frequentie toenemen over meerdere sessies heen. De Orchestrator traceert dit over tijd.

**Voorbeeld:**
> Evolutionaire psychologie werd 2 sessies geleden voor het eerst gesignaleerd. Frequentie stijgt. Mogelijk waardevolle uitbreiding van het Psychologie-domein.

### 4. Actieve kennishiaten

Gaps gesignaleerd door Agent 3 via de Gap Engine. Worden doorgegeven aan Agent 2 als zoekprioriteit.

**Voorbeeld:**
> Gap gesignaleerd: Speltheorie ontbreekt terwijl Behavioral Finance al goed gedekt is. Agent 2 zoekt hierop.

### 5. Benadrukte kennis vandaag

Directe input van de gebruiker via Agent 6. Heeft de hoogste prioriteit voor die sessie.

**Voorbeeld:**
> Gebruiker vraagt: "Focus vandaag op de Romeinse Republiek en parallellen met moderne democratie."

---

## Hoe Shared Memory werkt per agent

| Agent | Leest | Schrijft |
|---|---|---|
| Orchestrator | Alles | Leespatronen, stijgende interesses |
| Agent 1 | Benadrukte kennis | Frequentiesignalen (via Orchestrator) |
| Agent 2 | Interesses + gaps | — |
| Agent 3 | Interesses + gaps | Nieuwe gaps (via Orchestrator) |
| Agent 4 | Interesses + stijgende thema's | — |
| Agent 5 | Interesses + stijgende thema's | — |
| Agent 6 | Alles | Benadrukte kennis vandaag (na check-in) |
| Agent 7 | — | — |

Alleen de Orchestrator en Agent 6 schrijven naar Shared Memory. Alle andere agents lezen alleen.

---

## Workflow

```
Sessie start
↓
Orchestrator laadt Shared Memory in werkcontext
↓
Agent 6: check-in → gebruiker benoemt prioriteit → opslaan in context
↓
Alle agents draaien met dezelfde gedeelde context
↓
Einde sessie: Orchestrator actualiseert Shared Memory op basis van wat is gevonden
```

---

## Regels

- Shared Memory is sessiegebonden. Het bestaat als actieve context, niet als extern bestand.
- Verouderde informatie wordt verwijderd door de Orchestrator. Wat niet meer relevant is, verdwijnt.
- Gebruikersinteresses worden nooit door agents zelf bepaald. Altijd door de gebruiker via Agent 6.
- Gaps worden alleen toegevoegd als Agent 3 een inhoudelijke reden heeft. Geen willekeurige uitbreidingen.
