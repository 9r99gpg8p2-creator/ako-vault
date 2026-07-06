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
| — | — | — | — | — |

---

## Prioriteitsvolgorde

1. Gebruikersverzoek (hoogste prioriteit)
2. Nieuwe Raw gedetecteerd → volledige pipeline
3. Geplande dagelijkse taken
4. Geplande wekelijkse taken
5. Geplande maandelijkse taken
