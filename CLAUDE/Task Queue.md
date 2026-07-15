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

| ✓ | 2026-07-09T expansie | Agent 3 | Gap: Slaap en Geheugenconsolidatie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Slaap en Geheugenconsolidatie.md — confidence 5 |
| ✓ | 2026-07-09T expansie | Agent 3 | Gap: Ethiek | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Ethiek.md — confidence 5 |
| ✓ | 2026-07-09T expansie | Agent 3 | Gap: Eerste Wereldoorlog | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Eerste Wereldoorlog.md — confidence 5 |

---

| ✓ | 2026-07-13T expansie | Agent 3 | Gap: Piaget | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Piaget.md — confidence 8 (Packer 2021) |
| ✓ | 2026-07-13T expansie | Agent 3 | Gap: Vygotsky | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Vygotsky.md — confidence 8 (Packer 2021) |
| ✓ | 2026-07-12T consolidatie | Agent 3 | Gap: Klassieke Conditionering | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Klassieke Conditionering.md — confidence 9 |
| ✓ | 2026-07-12T consolidatie | Agent 3 | Gap: Sociale Leertheorie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Sociale Leertheorie.md — confidence 9 |
| ✓ | 2026-07-13T expansie | Agent 3 | Gap: Niche Constructie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Niche Constructie.md — confidence 8 (Packer 2021) |
| ✓ | 2026-07-13T expansie | Agent 3 | Gap: Behaviorisme | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Behaviorisme.md — confidence 9 |
| ✓ | 2026-07-13T expansie | Agent 3 | Gap: Koude Oorlog | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Koude Oorlog.md — confidence 5 |
| ✓ | 2026-07-13T expansie | Agent 1 | Inbox verwerkt | deel04 verwerkt — 5 kandidaten gedetecteerd; 3 wiki-pagina's aangemaakt (Emotieregulatie, Synaptogenese, Culturele Ontwikkelingspaden) |
| ✓ | 2026-07-13T consolidatie | Agent 3 | Gap: Interactieve Specialisatie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Interactieve Specialisatie.md — confidence 8 (Johnson 2001 + Packer 2021) |
| ✓ | 2026-07-13T consolidatie | Agent 3 | Gap: Precursor Emoties | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Precursor Emoties.md — confidence 8 (Izard/Camras 1992 + Packer 2021) |
| ✓ | 2026-07-13T consolidatie | Agent 1 | Inbox verwerkt | deel05 verwerkt — Hechtingstheorie UPDATE (4 hypothesen) + 3 wiki-pagina's (Interactieve Specialisatie, Precursor Emoties, Geleid Participeren) |
| ✓ | 2026-07-13T expansie | Agent 3 | Gap: Affordances | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Affordances.md — confidence 7 (Gibson 1966 + Packer 2021) |
| ✓ | 2026-07-13T consolidatie | Agent 3 | Gap: Intern Werkmodel | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Intern Werkmodel.md — confidence 8 (Bowlby 1973, 1980) |
| ✓ | 2026-07-14T expansie | Agent 3 | Gap: Collectieve Intentionaliteit | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Collectieve Intentionaliteit.md — confidence 8 (Packer deel06 + Tomasello 2019) |
| ✓ | 2026-07-14T consolidatie | Agent 3 | Gap: Spiegelzelfherkenning | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Spiegelzelfherkenning.md — confidence 8 (Amsterdam 1972 + Tomasello 2019 + Packer 2021) |
| ✓ | 2026-07-14T consolidatie | Agent 3 | Gap: Familimodellen | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Familimodellen.md — confidence 8 (Kağıtçıbaşı 2005 + Packer 2021) |
| ✓ | 2026-07-14T consolidatie | Agent 3 | Gap: Preoperationeel Denken | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Preoperationeel Denken.md — confidence 8 (Piaget & Inhelder 1969 + Bruner 1964 + Packer 2021) |
| ✓ | 2026-07-14T consolidatie | Agent 3 | Gap: Zone of Proximal Development | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Zone of Proximal Development.md — confidence 8 (Vygotsky 1978 + Packer deel09) |
| ✓ | 2026-07-14T consolidatie | Agent 3 | Gap: Hogere Psychologische Functies | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Hogere Psychologische Functies.md — confidence 8 (Vygotsky 1997a + Packer deel09) |
| ✓ | 2026-07-14T expansie | Agent 3 | Gap: Meta-emotie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Meta-emotie.md — confidence 8 (Gottman et al. 1997 + Packer 2021) |
| ✓ | 2026-07-14T expansie | Agent 3 | Gap: Intent Participatie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Intent Participatie.md — confidence 8 (Rogoff et al. 2003 + Packer 2021) |
| ✓ | 2026-07-14T consolidatie | Agent 3 | Gap: Epistemologisch Relativisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Epistemologisch Relativisme.md — confidence 8 (Perry 1970 + Kuhn 1991 + Chandler 1987 + Packer 2021) |
| ✓ | 2026-07-14T consolidatie | Agent 3 | Gap: Ethiek van Zorg | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Ethiek van Zorg.md — confidence 8 (Gilligan 1982 + Noddings 1984 + Packer 2021) |
| ✓ | 2026-07-14T consolidatie | Agent 1 | Inbox verwerkt | deel11 verwerkt — 5 kandidaten gedetecteerd; Theory of Mind UPDATE (teleologische stance, representationele theorie); 4 gaps naar queue |
| ✓ | 2026-07-14T expansie | Agent 3 | Gap: Kohlberg | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Kohlberg.md — confidence 8 (Kohlberg 1963/2008, Packer deel12) |
| ✓ | 2026-07-14T expansie | Agent 3 | Gap: Fuzzy Trace Theory | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Fuzzy Trace Theory.md — confidence 8 (Reyna & Brainerd 1995, Packer deel11/12) |
| ✓ | 2026-07-14T expansie | Agent 3 | Gap: Dual Process Theorie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Dual Process Theorie.md — confidence 8 (Evans 2008, Kahneman 2011, Packer deel12) |
| ✓ | 2026-07-14T expansie | Agent 3 | Gap: Erikson | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Erikson.md — confidence 8 (Erikson 1950, 1994a/b, Packer deel12) |
| ✓ | 2026-07-14T expansie | Agent 1 | Inbox verwerkt | deel12 verwerkt (bibliografie C–L) — 4 wiki-pagina's aangemaakt; 2 nieuwe gaps geïdentificeerd |
| ✓ | 2026-07-14T consolidatie | Agent 3 | Gap: Situated Learning | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Situated Learning.md — confidence 8 (Lave & Wenger 1991) |
| ✓ | 2026-07-14T consolidatie | Agent 3 | Gap: Adolescent Peergroepen | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Adolescent Peergroepen.md — confidence 8 (Packer 2021 + Rubin 1983 + Way 2006) |
| ✓ | 2026-07-14T consolidatie | Agent 1 | Inbox verwerkt | deel13 verwerkt (bibliografie M–W + index) — 5 nieuwe gaps geïdentificeerd |
| ✓ | 2026-07-15T expansie | Agent 3 | Gap: Scaffolding | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Scaffolding.md — confidence 8 (Wood/Bruner/Ross 1976 + Packer 2021) |
| ↓ | 2026-07-14T consolidatie | Agent 3 | Gap: Intersubjectiviteit | Psych — Trevarthen (1974, 1979): primaire intersubjectiviteit als vroegste vorm van sociaal bewustzijn; voorloper van Theory of Mind |
| ↓ | 2026-07-14T consolidatie | Agent 3 | Gap: Activiteitstheorie | Psych — Vygotsky/Leont'ev: activiteit als eenheid van analyse voor psychologisch onderzoek; context voor situated learning |
| ✓ | 2026-07-15T expansie | Agent 3 | Gap: Sociale Ontologie | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Sociale Ontologie.md — confidence 5 (Searle 1995, 2005, 2006) |
| ↓ | 2026-07-14T consolidatie | Agent 3 | Gap: Etnische Identiteit | Psych — Phinney (1990, 1996, 2001): etnische identiteitsontwikkeling bij adolescenten; kruispunt van Adolescentie en Culturele Psychologie |
| ↓ | 2026-07-15T expansie | Agent 3 | Gap: Intersubjectiviteit | Psych — Trevarthen (1974, 1979): primaire intersubjectiviteit als vroegste vorm van sociaal bewustzijn; voorloper van Theory of Mind |
| ↓ | 2026-07-15T expansie | Agent 3 | Gap: Activiteitstheorie | Psych — Vygotsky/Leont'ev: activiteit als eenheid van analyse; context voor situated learning en ZPD |
| ↓ | 2026-07-15T expansie | Agent 3 | Gap: Etnische Identiteit | Psych — Phinney (1990, 1996, 2001): etnische identiteitsontwikkeling bij adolescenten; MSc KNP-relevant |

---

## Prioriteitsvolgorde

1. Gebruikersverzoek (hoogste prioriteit)
2. Nieuwe Raw gedetecteerd → volledige pipeline
3. Geplande dagelijkse taken
4. Geplande wekelijkse taken
5. Geplande maandelijkse taken
