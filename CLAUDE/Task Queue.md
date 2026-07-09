---
tags: [systeem, queue]
type: operationeel
---

# Task Queue — AKO

> Persistente taakwachtrij. Wordt beheerd door de Orchestrator.
> Alleen de Orchestrator schrijft naar dit bestand (Wet 10).
> Agents signaleren taken aan de Orchestrator — nooit rechtstreeks hier.

**Systeemkoppelingen:** [[AKO]]

---

## Statusmarkeringen

| Status | Betekenis |
|---|---|
| `↓` | Wacht in queue |
| `⏳` | Wordt uitgevoerd |
| `✓` | Succesvol afgerond |
| `✗` | Mislukt — zie System Log |
| `⏭` | Overgeslagen na 3 retries |

---

## Queue

| Status | Tijdstip | Agent | Taak | Detail |
|---|---|---|---|---|
| ✓ | 2026-07-07T06:07Z | Agent 2 | Wikipedia API onbeschikbaar | Opgelost: Orchestrator gebruikt nu User-Agent headers + MediaWiki fallback + nl.wikipedia. Intern kennismodel als laatste redmiddel. |
| ✓ | 2026-07-08T00:00Z | Agent 3 | Gap: Werkgeheugen | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Werkgeheugen.md — confidence 9 |
| ✓ | 2026-07-08T00:00Z | Agent 3 | Gap: Executieve Functies | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Executieve Functies.md — confidence 9 |
| ✓ | 2026-07-08T00:00Z | Agent 3 | Gap: Anosognosie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Anosognosie.md — confidence 8 |
| ✓ | 2026-07-08T00:00Z | Agent 3 | Gap: Verliesaversie | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Verliesaversie.md — confidence 9 |
| ✓ | 2026-07-08T00:00Z | Agent 3 | Gap: Gedragseconomie | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Gedragseconomie.md — confidence 9 |
| ✓ | 2026-07-08T00:00Z | Agent 3 | Gap: Paradigmawisseling | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Paradigmawisseling.md — confidence 9 |
| ✓ | 2026-07-08T00:00Z | Agent 3 | Gap: Bewustzijn | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Bewustzijn.md — confidence 7 |
| ✓ | 2026-07-08T06:01Z | Agent 3 | Gap: Geheugenconsolidatie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Geheugenconsolidatie.md — confidence 5 |
| ✓ | 2026-07-08T06:01Z | Agent 3 | Gap: Vrije Wil | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Vrije Wil.md — confidence 5 |
| ✓ | 2026-07-08T06:01Z | Agent 3 | Gap: Cognitieve Biases (overzicht) | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Cognitieve Biases.md — confidence 5 |
| ✓ | 2026-07-08T06:01Z | Agent 3 | Gap: Reconsolidatie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Reconsolidatie.md — confidence 5 |
| ✓ | 2026-07-08T06:01Z | Agent 3 | Gap: Morele Verantwoordelijkheid | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Morele Verantwoordelijkheid.md — confidence 5 |
| ✓ | 2026-07-08T06:01Z | Agent 3 | Gap: Herding | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Herding.md — confidence 5 |
| ✓ | 2026-07-09T00:03Z | Agent 3 | Gap: PTSD | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/PTSD.md — confidence 5 |
| ✓ | 2026-07-09T00:03Z | Agent 3 | Gap: Efficiënte Markthypothese | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Efficiënte Markthypothese.md — confidence 5 |
| ✓ | 2026-07-09T consolidatie | Agent 3 | Gap: Embodied Cognition | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Embodied Cognition.md — confidence 5 |
| ✓ | 2026-07-09T consolidatie | Agent 3 | Gap: Psychoanalyse | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Psychoanalyse.md — confidence 5 |
| ✓ | 2026-07-09T consolidatie | Agent 3 | Gap: EMDR | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/EMDR.md — confidence 5 |

---

| ↓ | 2026-07-09T expansie | Agent 3 | Gap: Slaap en Geheugenconsolidatie | Psychologie — neurobiologie van slaap als consolidatieproces; direct relevant MSc CNP |
| ↓ | 2026-07-09T expansie | Agent 3 | Gap: Ethiek | Filosofie — normatieve ethiek (deontologie, consequentialisme, deugdethiek); fundament klinische dilemma's |
| ↓ | 2026-07-09T expansie | Agent 3 | Gap: Eerste Wereldoorlog | Geschiedenis — voedingsbodem voor totalitarisme en fascisme; ontbrekende twintigste-eeuwse context |

---

## Prioriteitsvolgorde

1. Gebruikersverzoek (hoogste prioriteit)
2. Nieuwe Raw gedetecteerd → volledige pipeline
3. Geplande dagelijkse taken
4. Geplande wekelijkse taken
5. Geplande maandelijkse taken
