---
tags: [systeem, queue]
type: operationeel
---

# Task Queue — AKO

> Persistente taakwachtrij. Wordt beheerd door de Orchestrator.
> Alleen de Orchestrator schrijft naar dit bestand (Wet 10).
> Agents signaleren taken aan de Orchestrator — nooit rechtstreeks hier.

**Systeemkoppelingen:** [[AKO v1.3]] · [[AKO v1.6]] · [[System Log]] · [[Shared Memory]]

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
| ↓ | 2026-07-07T06:07Z | Agent 3 | Gap: Werkgeheugen | Concept genoemd in Neuropsychologische Rehabilitatie — geen eigen pagina. Discipline: Psychologie. |
| ↓ | 2026-07-07T06:07Z | Agent 3 | Gap: Executieve Functies | Concept genoemd in Neuropsychologische Rehabilitatie — geen eigen pagina. Discipline: Psychologie. |
| ↓ | 2026-07-07T06:07Z | Agent 3 | Gap: Anosognosie | Concept beschreven in meerdere pagina's — geen eigen pagina. Discipline: Psychologie. |
| ↓ | 2026-07-07T06:07Z | Agent 3 | Gap: Verliesaversie | Concept in related-veld Prospect Theory — geen eigen pagina. Discipline: Beleggen. |
| ↓ | 2026-07-07T06:07Z | Agent 3 | Gap: Gedragseconomie | Concept in related-veld Prospect Theory — geen eigen pagina. Discipline: Beleggen. |
| ↓ | 2026-07-07T06:07Z | Agent 3 | Gap: Paradigmawisseling | Concept in related-veld Wetenschappelijke Revolutie — geen eigen pagina. Discipline: Geschiedenis. |
| ↓ | 2026-07-07T06:07Z | Agent 3 | Gap: Bewustzijn | Concept in related-veld Filosofie van de Geest — geen eigen pagina. Discipline: Filosofie. |

---

## Prioriteitsvolgorde

1. Gebruikersverzoek (hoogste prioriteit)
2. Nieuwe Raw gedetecteerd → volledige pipeline
3. Geplande dagelijkse taken
4. Geplande wekelijkse taken
5. Geplande maandelijkse taken
