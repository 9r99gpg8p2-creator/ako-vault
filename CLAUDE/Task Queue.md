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
| ✓ | 2026-07-15T consolidatie | Agent 3 | Gap: Intersubjectiviteit | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Intersubjectiviteit.md — confidence 8 (Trevarthen 1974, 1979 + Packer 2021) |
| ✓ | 2026-07-15T consolidatie | Agent 3 | Gap: Activiteitstheorie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Activiteitstheorie.md — confidence 8 (Vygotsky 1978 + Leont'ev 1978 + Engeström 1987 + Packer 2021) |
| ✓ | 2026-07-15T expansie | Agent 3 | Gap: Sociale Ontologie | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Sociale Ontologie.md — confidence 5 (Searle 1995, 2005, 2006) |
| ✓ | 2026-07-15T consolidatie | Agent 3 | Gap: Etnische Identiteit | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Etnische Identiteit.md — confidence 8 (Phinney 1990, 1996, 2001 + Packer 2021) |
| ✓ | 2026-07-15T consolidatie | Agent 3 | Gap: Postkoloniale Psychologie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Postkoloniale Psychologie.md — confidence 5 · 4 relatiepagina's + 1 inzicht |
| ✓ | 2026-07-15T expansie-2 | Agent 3 | Expansie: Utilitarisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Utilitarisme.md — confidence 5 |
| ✓ | 2026-07-15T expansie-2 | Agent 3 | Expansie: De Franse Revolutie | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Franse Revolutie.md — confidence 5 |
| ✓ | 2026-07-15T expansie-2 | Agent 3 | Expansie: Asset Allocatie | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Asset Allocatie.md — confidence 5 |
| ✓ | 2026-07-15T expansie-2 | Agent 3 | Expansie: Klinische Neuropsychologie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Klinische Neuropsychologie.md — confidence 5 |

---

| ✓ | 2026-07-16T consolidatie | Agent 3 | Gap: Rationalisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Rationalisme.md — confidence 5 |
| ✓ | 2026-07-16T consolidatie | Agent 3 | Gap: Immanuel Kant | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Immanuel Kant.md — confidence 5 |
| ✓ | 2026-07-16T consolidatie | Agent 3 | Gap: Intrinsieke Waarde / DCF-modellen | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Intrinsieke Waarde en DCF-modellen.md — confidence 5 |
| ✓ | 2026-07-16T consolidatie | Agent 3 | Gap: Humanisme | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Humanisme.md — confidence 5 |
| ✓ | 2026-07-16T expansie | Agent 3 | Gap: Logisch Positivisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Logisch Positivisme.md — confidence 5 |
| ✓ | 2026-07-16T expansie | Agent 3 | Expansie: Gouden Eeuw | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Gouden Eeuw.md — confidence 5 |
| ✓ | 2026-07-16T expansie | Agent 3 | Expansie: Marktcycli | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Marktcycli.md — confidence 5 |
| ✓ | 2026-07-16T expansie | Agent 3 | Expansie: Cognitieve Gedragstherapie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Cognitieve Gedragstherapie.md — confidence 5 |
| ✓ | 2026-07-16T consolidatie | Agent 3 | Gap: Tulpenmanie | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Tulpenmanie.md — confidence 5 |
| ✓ | 2026-07-16T consolidatie | Agent 3 | Gap: Dialectische Gedragstherapie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Dialectische Gedragstherapie.md — confidence 5 |
| ✓ | 2026-07-16T consolidatie | Agent 3 | Gap: Deontologie verdiepen | Deontologie.md bijgewerkt: Immanuel Kant + Vrije Wil + cross-domein DBT toegevoegd |
| ✓ | 2026-07-16T expansie-2 | Agent 3 | Expansie: Neuroplasticiteit | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Neuroplasticiteit.md — confidence 5 |
| ✓ | 2026-07-16T expansie-2 | Agent 3 | Expansie: Reformatie | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Reformatie.md — confidence 5 |
| ✓ | 2026-07-16T expansie-2 | Agent 3 | Expansie: Stoïcisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Stoïcisme.md — confidence 5 |
| ✓ | 2026-07-16T expansie-2 | Agent 3 | Expansie: Depressie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Depressie.md — confidence 5 |
| ✓ | 2026-07-16T consolidatie-2 | Agent 3 | Gap: Aristoteles | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Aristoteles.md — confidence 5 |
| ✓ | 2026-07-16T consolidatie-2 | Agent 3 | Gap: Angststoornissen | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Angststoornissen.md — confidence 5 |
| ✓ | 2026-07-16T consolidatie-2 | Agent 3 | Gap: Contrareformatie | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Contrareformatie.md — confidence 5 |

| ✓ | 2026-07-17T expansie | Agent 3 | Expansie: Plato | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Plato.md — confidence 5 |
| ✓ | 2026-07-17T expansie | Agent 3 | Expansie: Schizofrenie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Schizofrenie.md — confidence 5 |
| ✓ | 2026-07-17T expansie | Agent 3 | Expansie: Obligaties | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Obligaties.md — confidence 5 |
| ✓ | 2026-07-17T expansie | Agent 3 | Expansie: Het Napoleontische Tijdperk | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Het Napoleontische Tijdperk.md — confidence 5 |
| ✓ | 2026-07-17T expansie-2 | Agent 3 | Gap: Socrates | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Socrates.md — confidence 5 |
| ✓ | 2026-07-17T expansie-2 | Agent 3 | Gap: ADHD | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/ADHD.md — confidence 5 |
| ✓ | 2026-07-17T expansie-2 | Agent 3 | Gap: Dopamine | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Dopamine.md — confidence 5 |
| ✓ | 2026-07-17T expansie-2 | Agent 3 | Expansie: Macroeconomie | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Macroeconomie.md — confidence 5 |
| ✓ | 2026-07-17T consolidatie | Agent 3 | Gap: Verslaving | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Verslaving.md — confidence 5 |
| ✓ | 2026-07-17T consolidatie | Agent 3 | Gap: Monetair Beleid | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Monetair Beleid.md — confidence 5 |
| ✓ | 2026-07-17T expansie | Agent 3 | Expansie: Russische Revolutie | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Russische Revolutie.md — confidence 5 |
| ✓ | 2026-07-17T expansie | Agent 3 | Expansie: Diversificatie | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Diversificatie.md — confidence 5 |
| ✓ | 2026-07-17T expansie | Agent 3 | Expansie: Psychose | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Psychose.md — confidence 5 |
| ✓ | 2026-07-17T expansie | Agent 3 | Expansie: Antiek Griekenland | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Antiek Griekenland.md — confidence 5 |
| ✓ | 2026-07-17T consolidatie | Agent 3 | Gap: Stalinisme | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Stalinisme.md — confidence 5 |
| ✓ | 2026-07-17T consolidatie | Agent 3 | Gap: First Episode Psychosis | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/First Episode Psychosis.md — confidence 5 |
| ✓ | 2026-07-18T expansie | Agent 3 | Expansie: De Middeleeuwen | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Middeleeuwen.md — confidence 5 |
| ✓ | 2026-07-18T expansie | Agent 3 | Expansie: Nietzsche | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Nietzsche.md — confidence 5 |
| ✓ | 2026-07-18T expansie | Agent 3 | Expansie: Inflatie | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Inflatie.md — confidence 5 |
| ✓ | 2026-07-18T expansie | Agent 3 | Expansie: Aandelen | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Aandelen.md — confidence 5 |
| ✓ | 2026-07-18T consolidatie | Agent 3 | Gap: Functionalisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Functionalisme.md — confidence 5 |
| ✓ | 2026-07-18T consolidatie | Agent 3 | Gap: Grote Depressie | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Grote Depressie.md — confidence 5 |
| ✓ | 2026-07-18T consolidatie | Agent 3 | Gap: Weimar Republiek | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Weimar Republiek.md — confidence 5 |

---

| ✓ | 2026-07-18T consolidatie-2 | Agent 3 | Gap: Historisch Materialisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Historisch Materialisme.md — confidence 5 |
| ✓ | 2026-07-18T consolidatie-2 | Agent 3 | Gap: Actief Beleggen | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Actief Beleggen.md — confidence 5 |

---

| ✓ | 2026-07-19T expansie | Agent 3 | Gap: Neuropsychologische Diagnostiek ASS (ADOS-2) | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Neuropsychologische Diagnostiek ASS (ADOS-2).md — confidence 5 |
| ✓ | 2026-07-19T expansie | Agent 3 | Gap: Adorno Autoritaire Persoonlijkheid | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Adorno en de Autoritaire Persoonlijkheid.md — confidence 5 |
| ✓ | 2026-07-19T expansie | Agent 3 | Gap: Acceptatie en Commitment Therapie (ACT) | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Acceptatie en Commitment Therapie.md — confidence 5 |

---

| ✓ | 2026-07-19T consolidatie | Agent 3 | Gap: David Hume | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/David Hume.md — confidence 5 |
| ✓ | 2026-07-19T consolidatie | Agent 3 | Gap: Schematherapie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Schematherapie.md — confidence 5 |
| ✓ | 2026-07-19T consolidatie | Agent 3 | Gap: Kapitalisme | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Kapitalisme.md — confidence 5 |

---

| ✓ | 2026-07-19T expansie-2 | Agent 3 | Expansie: Heuristieken | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Heuristieken.md — confidence 5 |
| ✓ | 2026-07-19T expansie-2 | Agent 3 | Expansie: Persoonlijkheidsstoornissen | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Persoonlijkheidsstoornissen.md — confidence 5 |
| ✓ | 2026-07-19T expansie-2 | Agent 3 | Expansie: Imperialisme | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Imperialisme.md — confidence 5 |
| ✓ | 2026-07-19T expansie-2 | Agent 3 | Expansie: Freud | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Freud.md — confidence 5 |
| ✓ | 2026-07-19T expansie-2 | Agent 3 | Gap: George Berkeley (empirisme-cluster) | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/George Berkeley.md — confidence 5 |
| ✓ | 2026-07-19T expansie-2 | Agent 3 | Gap: Complexe PTSD (C-PTSD) | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Complexe PTSD.md — confidence 5 |
| ✓ | 2026-07-19T expansie-2 | Agent 3 | Gap: Traumatisch Hersenletsel (THL) | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Traumatisch Hersenletsel.md — confidence 5 |
| ✓ | 2026-07-20T expansie | Agent 3 | Expansie: Kapitaalmarkten | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Kapitaalmarkten.md — confidence 5 |
| ✓ | 2026-07-20T expansie | Agent 3 | Expansie: Postmodernisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Postmodernisme.md — confidence 5 |
| ✓ | 2026-07-20T expansie | Agent 3 | Expansie: Het Romeinse Rijk | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Het Romeinse Rijk.md — confidence 5 |
| ✓ | 2026-07-20T expansie | Agent 3 | Expansie: Spinoza | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Spinoza.md — confidence 5 |
| ✓ | 2026-07-20T consolidatie | Agent 3 | Gap: Marxisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Marxisme.md — confidence 5 |
| ✓ | 2026-07-20T consolidatie | Agent 3 | Gap: De Islamitische Gouden Eeuw | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Islamitische Gouden Eeuw.md — confidence 5 |
| ✓ | 2026-07-20T expansie-2 | Agent 3 | Expansie: Financiële Crisis 2008 | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Financiële Crisis 2008.md — confidence 5 |
| ✓ | 2026-07-20T expansie-2 | Agent 3 | Expansie: Factor Investing | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Factor Investing.md — confidence 5 |
| ✓ | 2026-07-20T expansie-2 | Agent 3 | Expansie: Het Byzantijnse Rijk | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Het Byzantijnse Rijk.md — confidence 5 |
| ✓ | 2026-07-20T expansie-2 | Agent 3 | Expansie: Analytische Filosofie | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Analytische Filosofie.md — confidence 5 |
| ✓ | 2026-07-20T consolidatie | Agent 3 | Gap: Taalfilosofie | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Taalfilosofie.md — confidence 5 |
| ✓ | 2026-07-20T consolidatie | Agent 3 | Gap: Private Equity | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Private Equity.md — confidence 5 |
| ✓ | 2026-07-20T expansie-3 | Agent 3 | Expansie: Index Fondsen | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Index Fondsen.md — confidence 5 |
| ✓ | 2026-07-20T expansie-3 | Agent 3 | Expansie: Monetarisme | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Monetarisme.md — confidence 5 |
| ✓ | 2026-07-20T expansie-3 | Agent 3 | Expansie: Mercantilisme | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Mercantilisme.md — confidence 5 |
| ✓ | 2026-07-20T expansie-3 | Agent 3 | Expansie: Kahneman | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Kahneman.md — confidence 5 |
| ✓ | 2026-07-20T consolidatie | Agent 3 | Gap: Amos Tversky | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Amos Tversky.md — confidence 5 |
| ✓ | 2026-07-20T consolidatie | Agent 3 | Gap: Keynesiaanse Economie | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Keynesiaanse Economie.md — confidence 5 |
| ✓ | 2026-07-21T expansie | Agent 3 | Expansie: Risicobeheer | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Risicobeheer.md — confidence 5 |
| ✓ | 2026-07-21T expansie | Agent 3 | Expansie: Filosofie van de Wetenschap | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Filosofie van de Wetenschap.md — confidence 5 |
| ✓ | 2026-07-21T expansie | Agent 3 | Expansie: Maatschappelijk Contract | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Maatschappelijk Contract.md — confidence 5 |
| ✓ | 2026-07-21T expansie | Agent 3 | Expansie: Oude Egypte | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Oude Egypte.md — confidence 5 |
| ✓ | 2026-07-21T consolidatie | Agent 3 | Gap: Falsifiabilisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Falsifiabilisme.md — confidence 5 |
| ✓ | 2026-07-21T consolidatie | Agent 3 | Gap: John Rawls | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/John Rawls.md — confidence 5 |
| ✓ | 2026-07-21T consolidatie | Agent 3 | Gap: Mesopotamië | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Mesopotamië.md — confidence 5 |
| ✓ | 2026-07-21T expansie-2 | Agent 3 | Expansie: Cryptocurrency en Blockchain | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Cryptocurrency en Blockchain.md — confidence 5 |
| ✓ | 2026-07-21T expansie-2 | Agent 3 | Expansie: Benjamin Graham | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Benjamin Graham.md — confidence 5 |
| ✓ | 2026-07-21T expansie-2 | Agent 3 | Expansie: Het Mongoolse Rijk | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Het Mongoolse Rijk.md — confidence 5 |
| ✓ | 2026-07-21T expansie-2 | Agent 3 | Expansie: Jean-Jacques Rousseau | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Jean-Jacques Rousseau.md — confidence 5 |
| ✓ | 2026-07-21T consolidatie | Agent 3 | Gap: Keizerlijk China | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Keizerlijk China.md — confidence 5 |
| ✓ | 2026-07-21T consolidatie | Agent 3 | Gap: Thomas Hobbes | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Thomas Hobbes.md — confidence 5 |
| ✓ | 2026-07-21T consolidatie | Agent 3 | Gap: Stress en de HPA-as | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Stress en de HPA-as.md — confidence 5 |
| ✓ | 2026-07-21T expansie-3 | Agent 3 | Expansie: Groei Investeren | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Groei Investeren.md — confidence 5 |
| ✓ | 2026-07-21T expansie-3 | Agent 3 | Expansie: Warren Buffett | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Warren Buffett.md — confidence 5 |
| ✓ | 2026-07-21T expansie-3 | Agent 3 | Expansie: De Kruistochten | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Kruistochten.md — confidence 5 |
| ✓ | 2026-07-21T expansie-3 | Agent 3 | Expansie: Feodalisme | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Feodalisme.md — confidence 5 |
| ✓ | 2026-07-21T consolidatie | Agent 3 | Gap: De Reconquista | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Reconquista.md — confidence 5 |
| ✓ | 2026-07-21T consolidatie | Agent 3 | Gap: GARP (Growth At a Reasonable Price) | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/GARP.md — confidence 5 |
| ✓ | 2026-07-22T consolidatie | Agent 3 | Gap: Amygdala | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Amygdala.md — confidence 8 |
| ✓ | 2026-07-22T consolidatie | Agent 3 | Gap: Prefrontale Cortex | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Prefrontale Cortex.md — confidence 8 |
| ✓ | 2026-07-22T expansie | Agent 3 | Expansie: Neuroimaging | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Neuroimaging.md — confidence 5 |
| ✓ | 2026-07-22T expansie | Agent 3 | Expansie: Tijdperk van Ontdekkingen | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Tijdperk van Ontdekkingen.md — confidence 5 |
| ✓ | 2026-07-22T expansie | Agent 3 | Expansie: Hermeneutiek | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Hermeneutiek.md — confidence 5 |
| ✓ | 2026-07-22T expansie | Agent 3 | Expansie: Capital Asset Pricing Model | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Capital Asset Pricing Model.md — confidence 5 |
| ✓ | 2026-07-22T expansie | Agent 3 | Duplicaat verwijderd | Moderne Portefeuilletheorie.md (spellingsvariant) samengevallen met bestaande Moderne Portefeuille Theorie.md |
| ✓ | 2026-07-22T consolidatie | Agent 3 | Gap: Insula | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Insula.md — confidence 8 |
| ✓ | 2026-07-22T consolidatie | Agent 3 | Gap: John Stuart Mill | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/John Stuart Mill.md — confidence 5 |
| ✓ | 2026-07-22T consolidatie | Agent 3 | Gap: Structuralisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Structuralisme.md — confidence 5 |
| ✓ | 2026-07-22T expansie | Agent 3 | Gap: Poststructuralisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Poststructuralisme.md — confidence 5 |
| ✓ | 2026-07-22T expansie | Agent 3 | Gap: Libertair Paternalisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Libertair Paternalisme.md — confidence 5 |
| ✓ | 2026-07-22T expansie | Agent 3 | Expansie: Big Five Persoonlijkheidsmodel | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Big Five Persoonlijkheidsmodel.md — confidence 8 |
| ✓ | 2026-07-22T expansie | Agent 3 | Expansie: De Maya-beschaving | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Maya-beschaving.md — confidence 5 |
| ✓ | 2026-07-22T expansie | Agent 3 | Gap: Big Five — klinische validering NEO-PI-R | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/NEO-PI-R.md — confidence 8 |
| ✓ | 2026-07-22T expansie | Agent 3 | Gap: Aztekenbeschaving | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Aztekenbeschaving.md — confidence 5 |
| ✓ | 2026-07-23T expansie | Agent 3 | Expansie: Short Selling | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Short Selling.md — confidence 5 |
| ✓ | 2026-07-23T expansie | Agent 3 | Expansie: De Vikingen | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Vikingen.md — confidence 5 |
| ✓ | 2026-07-23T expansie | Agent 3 | Expansie: Bipolaire Stoornis | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Bipolaire Stoornis.md — confidence 5 |
| ✓ | 2026-07-23T expansie | Agent 3 | Expansie: Merleau-Ponty | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Merleau-Ponty.md — confidence 5 |
| ✓ | 2026-07-23T consolidatie | Agent 3 | Gap: Alzheimer en Dementie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Alzheimer en Dementie.md — confidence 5 |
| ✓ | 2026-07-23T consolidatie | Agent 3 | Gap: Karel de Grote | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Karel de Grote.md — confidence 5 |
| ✓ | 2026-07-23T consolidatie | Agent 3 | Gap: Black-Scholes Model | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Black-Scholes Model.md — confidence 5 |
| ✓ | 2026-07-23T expansie-2 | Agent 3 | Expansie: Hedgefondsen | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Hedgefondsen.md — confidence 5 |
| ✓ | 2026-07-23T expansie-2 | Agent 3 | Expansie: Het Britse Rijk | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Het Britse Rijk.md — confidence 5 |
| ✓ | 2026-07-23T expansie-2 | Agent 3 | Expansie: Michel Foucault | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Michel Foucault.md — confidence 5 |
| ✓ | 2026-07-23T expansie-2 | Agent 3 | Expansie: Afasie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Afasie.md — confidence 5 |
| ✓ | 2026-07-23T consolidatie | Agent 3 | Gap: Dysartrie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Dysartrie.md — confidence 5 |
| ✓ | 2026-07-23T consolidatie | Agent 3 | Gap: Jürgen Habermas | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Jürgen Habermas.md — confidence 5 |
| ✓ | 2026-07-23T consolidatie | Agent 3 | Gap: Vastgoedbeleggen | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Vastgoedbeleggen.md — confidence 5 |
| ✓ | 2026-07-23T expansie-3 | Agent 3 | Expansie: Dividendbeleggen | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Dividendbeleggen.md — confidence 5 |
| ✓ | 2026-07-23T expansie-3 | Agent 3 | Expansie: Alexander de Grote | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Alexander de Grote.md — confidence 5 |
| ✓ | 2026-07-23T expansie-3 | Agent 3 | Expansie: Epilepsie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Epilepsie.md — confidence 5 |
| ✓ | 2026-07-23T expansie-3 | Agent 3 | Expansie: Ziekte van Parkinson | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Ziekte van Parkinson.md — confidence 5 |
| ✓ | 2026-07-23T consolidatie | Agent 3 | Gap: Kritische Theorie (Frankfurter Schule) | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Kritische Theorie.md — confidence 5 |
| ✓ | 2026-07-23T consolidatie | Agent 3 | Gap: Hellenisme | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Hellenisme.md — confidence 5 |
| ✓ | 2026-07-23T consolidatie | Agent 3 | Gap: Ziekte van Huntington | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Ziekte van Huntington.md — confidence 5 |
| ✓ | 2026-07-23T consolidatie | Agent 3 | Gap: Het Perzische Rijk (Achaemenidisch) | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Het Perzische Rijk (Achaemenidisch).md — confidence 5 |
| ✓ | 2026-07-24T expansie | Agent 3 | Expansie: Speculatieve Bubbels | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Speculatieve Bubbels.md — confidence 5 |
| ✓ | 2026-07-24T expansie | Agent 3 | Expansie: Meiji Japan | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Meiji Japan.md — confidence 5 |
| ✓ | 2026-07-24T expansie | Agent 3 | Expansie: Metafysica | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Metafysica.md — confidence 5 |
| ✓ | 2026-07-24T expansie | Agent 3 | Merge: Autismespectrumstoornis | Autisme Spectrum Stoornis.md samengevoegd met Autismespectrumstoornis.md (Wet 14) — confidence 5 |
| ✓ | 2026-07-24T consolidatie | Agent 3 | Gap: Minsky Moment | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Minsky Moment.md — confidence 5 |
| ✓ | 2026-07-24T consolidatie | Agent 3 | Gap: Tokugawa Shogunaat | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Tokugawa Shogunaat.md — confidence 5 |
| ✓ | 2026-07-24T consolidatie | Agent 3 | Gap: Neurodiversiteit | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Neurodiversiteit.md — confidence 5 |
| ✓ | 2026-07-24T expansie | Agent 3 | Expansie: Venture Capital | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Venture Capital.md — confidence 5 |
| ✓ | 2026-07-24T expansie | Agent 3 | Expansie: Nationaal Socialisme | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Nationaal Socialisme.md — confidence 5 |
| ✓ | 2026-07-24T expansie | Agent 3 | Expansie: Deugdethiek | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Deugdethiek.md — confidence 5 |
| ✓ | 2026-07-24T expansie | Agent 3 | Expansie: Kwantitatief Beleggen | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Kwantitatief Beleggen.md — confidence 5 |
| ✓ | 2026-07-24T consolidatie | Agent 3 | Gap: Propaganda | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Propaganda.md — confidence 5 |
| ✓ | 2026-07-24T consolidatie | Agent 3 | Gap: Hannah Arendt | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Hannah Arendt.md — confidence 5 |
| ✓ | 2026-07-24T consolidatie | Agent 3 | Gap: Statistical Arbitrage | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Statistical Arbitrage.md — confidence 5 |
| ✓ | 2026-07-24T expansie-2 | Agent 3 | Expansie: Sociale Psychologie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Sociale Psychologie.md — confidence 5 |
| ✓ | 2026-07-24T expansie-2 | Agent 3 | Expansie: Vietnam Oorlog | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Vietnam Oorlog.md — confidence 5 |
| ✓ | 2026-07-24T expansie-2 | Agent 3 | Expansie: Rentecurve | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Rentecurve.md — confidence 5 |
| ✓ | 2026-07-24T expansie-2 | Agent 3 | Expansie: Heidegger | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Heidegger.md — confidence 5 |
| ✓ | 2026-07-24T consolidatie | Agent 3 | Gap: Groepsdynamica | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Groepsdynamica.md — confidence 5 |
| ✓ | 2026-07-24T consolidatie | Agent 3 | Gap: Koreaoorlog | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Koreaoorlog.md — confidence 5 |
| ✓ | 2026-07-24T consolidatie | Agent 3 | Gap: ETFs | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/ETFs.md — confidence 5 |
| ✓ | 2026-07-24T consolidatie | Agent 3 | Gap: Existentiële Psychiatrie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Existentiële Psychiatrie.md — confidence 5 |
| ✓ | 2026-07-25T consolidatie | Agent 3 | Gap: Syndroom van Korsakov | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Syndroom van Korsakov.md — confidence 8 (Kopelman 1995, Victor et al. 1989) |
| ✓ | 2026-07-25T consolidatie | Agent 3 | Gap: Grondstoffen (Commodities) | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Grondstoffen.md — confidence 5 (Gorton & Rouwenhorst 2006) |
| ✓ | 2026-07-25T consolidatie | Agent 3 | Gap: Cognitieve Reserve | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Cognitieve Reserve.md — confidence 8 (Stern 2002, 2009; Valenzuela & Sachdev 2006) |
| ✓ | 2026-07-25T expansie | Agent 3 | Expansie: Behavioral Finance | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Behavioral Finance.md — confidence 5 (Thaler/Shiller/Kahneman) |
| ✓ | 2026-07-25T expansie | Agent 3 | Expansie: Neuropsychologie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Neuropsychologie.md — confidence 5 (Lezak 2012, Kolb & Whishaw 2015) |
| ✓ | 2026-07-25T expansie | Agent 3 | Merge: René Descartes | Descartes.md samengevoegd met René Descartes.md (Wet 14) — 4 nieuwe gerelateerde links toegevoegd |
| ✓ | 2026-07-25T expansie | Agent 3 | Expansie: ESG Beleggen | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/ESG Beleggen.md — confidence 5 (Eccles 2019, Friede 2015) |
| ✓ | 2026-07-25T expansie | Agent 3 | Gap: John Locke | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/John Locke.md — confidence 5 |
| ✓ | 2026-07-25T expansie | Agent 3 | Gap: Neuropsychologische Testbatterijen | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Neuropsychologische Testbatterijen.md — confidence 5 |
| ✓ | 2026-07-25T expansie-2 | Agent 3 | Expansie: Apraxie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Apraxie.md — confidence 5 |
| ✓ | 2026-07-25T expansie-2 | Agent 3 | Expansie: De Holocaust | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Holocaust.md — confidence 5 |
| ✓ | 2026-07-25T expansie-2 | Agent 3 | Expansie: Leibniz | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Leibniz.md — confidence 5 |
| ✓ | 2026-07-25T expansie-2 | Agent 3 | Expansie: Monte Carlo Simulatie | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Monte Carlo Simulatie.md — confidence 5 |
| ✓ | 2026-07-25T expansie-2 | Agent 3 | Gap: Agnosie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Agnosie.md — confidence 8 (Farah 1990, Humphreys & Riddoch 1987, Lissauer 1890) |
| ✓ | 2026-07-25T expansie-2 | Agent 3 | Gap: Neuropsychologische Revalidatie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Neuropsychologische Revalidatie.md — confidence 8 (Wilson 2003, Prigatano 1999, Cappa 2005) |
| ✓ | 2026-07-26T expansie | Agent 3 | Gap: Episodisch Geheugen | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Episodisch Geheugen.md — confidence 5 |
| ✓ | 2026-07-26T expansie | Agent 3 | Gap: Frontotemporale Dementie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Frontotemporale Dementie.md — confidence 5 |
| ✓ | 2026-07-26T expansie | Agent 3 | Gap: Karl Popper | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Karl Popper.md — confidence 5 |
| ✓ | 2026-07-26T expansie | Agent 3 | Gap: Opties | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Opties.md — confidence 5 |
| ✓ | 2026-07-26T consolidatie | Agent 3 | Gap: Semantisch Geheugen | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Semantisch Geheugen.md — confidence 5 |
| ✓ | 2026-07-26T consolidatie | Agent 3 | Gap: Thomas Kuhn | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Thomas Kuhn.md — confidence 5 |
| ✓ | 2026-07-26T consolidatie | Agent 3 | Gap: Corpus Callosum | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Corpus Callosum.md — confidence 5 |
| ✓ | 2026-07-26T consolidatie | Agent 3 | Gap: Smart Beta | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Smart Beta.md — confidence 5 |
| ✓ | 2026-07-26T expansie | Agent 3 | Expansie: Cognitieve Neurowetenschappen | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Cognitieve Neurowetenschappen.md — confidence 5 |
| ✓ | 2026-07-26T expansie | Agent 3 | Expansie: Limbisch Systeem | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Limbisch Systeem.md — confidence 5 |
| ✓ | 2026-07-26T expansie | Agent 3 | Expansie: Speltheorie | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Speltheorie.md — confidence 5 |
| ✓ | 2026-07-26T expansie | Agent 3 | Expansie: Industrialisatie | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Industrialisatie.md — confidence 5 |
| ✓ | 2026-07-26T consolidatie | Agent 3 | Gap: Thalamus | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Thalamus.md — confidence 5 |
| ✓ | 2026-07-26T consolidatie | Agent 3 | Gap: Basale Ganglia | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Basale Ganglia.md — confidence 5 |
| ✓ | 2026-07-26T consolidatie | Agent 3 | Gap: Hemispatiale Neglect | Reeds aanwezig als Hemispatiale Verwaarlozing.md — geen duplicaat aangemaakt (Wet 2) |
| ✓ | 2026-07-26T consolidatie | Agent 3 | Gap: Lateralisatie van Hersenfuncties | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Lateralisatie van Hersenfuncties.md — confidence 5 |
| ✓ | 2026-07-26T expansie | Agent 3 | Expansie: Cognitieve Flexibiliteit | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Cognitieve Flexibiliteit.md — confidence 5 |
| ✓ | 2026-07-26T expansie | Agent 3 | Expansie: Neuroethiek | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Neuroethiek.md — confidence 5 |
| ✓ | 2026-07-26T expansie | Agent 3 | Expansie: De Dertigjarige Oorlog | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Dertigjarige Oorlog.md — confidence 5 |
| ✓ | 2026-07-26T expansie | Agent 3 | Expansie: Futures en Derivaten | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Futures en Derivaten.md — confidence 5 |
| ✓ | 2026-07-26T consolidatie | Agent 3 | Gap: Aandachtsprocessen | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Aandachtsprocessen.md — confidence 5 |
| ✓ | 2026-07-26T consolidatie | Agent 3 | Gap: Gedragsgenetica | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Gedragsgenetica.md — confidence 5 |
| ✓ | 2026-07-26T consolidatie | Agent 3 | Gap: De Hanzesteden | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Hanzesteden.md — confidence 5 |
| ✓ | 2026-07-26T consolidatie | Agent 3 | Gap: Micro-economie | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Micro-economie.md — confidence 5 |
| ✓ | 2026-07-27T expansie | Agent 3 | Expansie: Prosopagnosie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Prosopagnosie.md — confidence 8 |
| ✓ | 2026-07-27T expansie | Agent 3 | Expansie: Jean-Paul Sartre | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Jean-Paul Sartre.md — confidence 8 |
| ✓ | 2026-07-27T expansie | Agent 3 | Expansie: De Romantiek | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Romantiek.md — confidence 7 |
| ✓ | 2026-07-27T expansie | Agent 3 | Expansie: Samengestelde Interest | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Samengestelde Interest.md — confidence 9 |
| ✓ | 2026-07-27T consolidatie | Agent 3 | Gap: Albert Camus | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Albert Camus.md — confidence 5 |
| ✓ | 2026-07-27T consolidatie | Agent 3 | Gap: Søren Kierkegaard | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Søren Kierkegaard.md — confidence 5 |
| ✓ | 2026-07-27T consolidatie | Agent 3 | Gap: Gyrus Fusiformis | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Gyrus Fusiformis.md — confidence 5 |

---

## Prioriteitsvolgorde

1. Gebruikersverzoek (hoogste prioriteit)
2. Nieuwe Raw gedetecteerd → volledige pipeline
3. Geplande dagelijkse taken
4. Geplande wekelijkse taken
5. Geplande maandelijkse taken
| ✓ | 2026-07-27T expansie-2 | Agent 3 | Expansie: Confabulatie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Confabulatie.md — confidence 5 |
| ✓ | 2026-07-27T expansie-2 | Agent 3 | Expansie: Absurdisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Absurdisme.md — confidence 5 |
| ✓ | 2026-07-27T expansie-2 | Agent 3 | Expansie: De Val van de Sovjet-Unie | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Val van de Sovjet-Unie.md — confidence 5 |
| ✓ | 2026-07-27T expansie-2 | Agent 3 | Expansie: Initial Public Offering | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Initial Public Offering.md — confidence 5 |
| ✓ | 2026-07-27T consolidatie | Agent 3 | Gap: Nihilisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Nihilisme.md — confidence 5 |
| ✓ | 2026-07-27T consolidatie | Agent 3 | Gap: Gorbatsjov | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Gorbatsjov.md — confidence 5 |
| ✓ | 2026-07-27T consolidatie | Agent 3 | Gap: Subarachnoïdale Bloeding | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Subarachnoïdale Bloeding.md — confidence 5 |
| ✓ | 2026-07-27T consolidatie | Agent 3 | Gap: SPAC (Special Purpose Acquisition Company) | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/SPAC.md — confidence 5 |
| ✓ | 2026-07-27T expansie | Agent 3 | Expansie: Prospectief Geheugen | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Prospectief Geheugen.md — confidence 5 |
| ✓ | 2026-07-27T expansie | Agent 3 | Expansie: Balint Syndroom | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Balint Syndroom.md — confidence 5 |
| ✓ | 2026-07-27T expansie | Agent 3 | Expansie: Visuospatiële Functies | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Visuospatiële Functies.md — confidence 5 |
| ✓ | 2026-07-27T expansie | Agent 3 | Expansie: Apartheid | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Apartheid.md — confidence 5 |
| ✓ | 2026-07-27T consolidatie | Agent 3 | Gap: Gerstmann Syndroom | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Gerstmann Syndroom.md — confidence 5 |
| ✓ | 2026-07-27T consolidatie | Agent 3 | Gap: Waarheids- en Verzoeningscommissie | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Waarheids- en Verzoeningscommissie.md — confidence 5 |
| ✓ | 2026-07-27T consolidatie | Agent 3 | Gap: Pariëtaalkwab | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Pariëtaalkwab.md — confidence 5 |
| ✓ | 2026-07-27T consolidatie | Agent 3 | Gap: Restoratieve Justitie | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Restoratieve Justitie.md — confidence 5 |
| ✓ | 2026-07-28T expansie | Agent 3 | Expansie: Temporaalkwab | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Temporaalkwab.md — confidence 5 |
| ✓ | 2026-07-28T expansie | Agent 3 | Expansie: Occipitaalkwab | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Occipitaalkwab.md — confidence 5 |
| ✓ | 2026-07-28T expansie | Agent 3 | Expansie: Cerebellum | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Cerebellum.md — confidence 5 |
| ✓ | 2026-07-28T expansie | Agent 3 | Expansie: Neoliberalisme | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Neoliberalisme.md — confidence 5 |
| ✓ | 2026-07-28T consolidatie | Agent 3 | Gap: Frontaalkwab | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Frontaalkwab.md — confidence 8 |
| ✓ | 2026-07-28T consolidatie | Agent 3 | Gap: Globalisering | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Globalisering.md — confidence 7 |
| ✓ | 2026-07-28T consolidatie | Agent 3 | Gap: Wernicke's Afasie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Wernicke's Afasie.md — confidence 8 |
| ✓ | 2026-07-28T consolidatie | Agent 3 | Gap: Positieve Psychologie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Positieve Psychologie.md — confidence 8 |
| ✓ | 2026-07-28T expansie-2 | Agent 3 | Expansie: Beta en Volatiliteit | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Beta en Volatiliteit.md — confidence 5 |
| ✓ | 2026-07-28T expansie-2 | Agent 3 | Expansie: Liquiditeit | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Liquiditeit.md — confidence 5 |
| ✓ | 2026-07-28T expansie-2 | Agent 3 | Expansie: De Europese Integratie | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Europese Integratie.md — confidence 5 |
| ✓ | 2026-07-28T expansie-2 | Agent 3 | Expansie: Determinisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Determinisme.md — confidence 5 |
| ✓ | 2026-07-28T consolidatie | Agent 3 | Gap: Jean Monnet | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Jean Monnet.md — confidence 5 |
| ✓ | 2026-07-28T consolidatie | Agent 3 | Gap: VIX-index | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/VIX-index.md — confidence 5 |
| ✓ | 2026-07-28T consolidatie | Agent 3 | Gap: Compatibilisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Compatibilisme.md — confidence 5 |
| ✓ | 2026-07-29T expansie | Agent 3 | Expansie: Waardebeleggen | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Waardebeleggen.md — confidence 5 |
| ✓ | 2026-07-29T expansie | Agent 3 | Expansie: Value at Risk | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Value at Risk.md — confidence 5 |
| ✓ | 2026-07-29T expansie | Agent 3 | Expansie: De Arabische Lente | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Arabische Lente.md — confidence 5 |
| ✓ | 2026-07-29T expansie | Agent 3 | Expansie: Postkolonialisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Postkolonialisme.md — confidence 5 |
| ✓ | 2026-07-29T consolidatie | Agent 3 | Gap: Frantz Fanon | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Frantz Fanon.md — confidence 5 |
| ✓ | 2026-07-29T consolidatie | Agent 3 | Gap: Edward Said | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Edward Said.md — confidence 5 |
| ✓ | 2026-07-29T consolidatie | Agent 3 | Gap: Expected Shortfall / CVaR | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Expected Shortfall.md — confidence 5 |
| ✓ | 2026-07-29T expansie | Agent 3 | Gap: Homi Bhabha | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Homi Bhabha.md — confidence 5 |
| ✓ | 2026-07-29T expansie | Agent 3 | Gap: Gayatri Chakravorty Spivak | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Gayatri Chakravorty Spivak.md — confidence 5 |
| ✓ | 2026-07-29T expansie | Agent 3 | Expansie: Momentum Strategie | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Momentum Strategie.md — confidence 5 |
| ✓ | 2026-07-29T expansie | Agent 3 | Expansie: De Chinese Culturele Revolutie | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Chinese Culturele Revolutie.md — confidence 5 |
| ✓ | 2026-07-29T consolidatie | Agent 3 | Gap: Maoïsme | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Maoïsme.md — confidence 5 |
| ✓ | 2026-07-29T consolidatie | Agent 3 | Gap: Subaltern Studies | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Subaltern Studies.md — confidence 5 |
| ✓ | 2026-07-29T expansie | Agent 3 | Gap: Gramsci & Hegemonie | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Gramsci en Hegemonie.md — confidence 5 |
| ✓ | 2026-07-29T expansie | Agent 3 | Gap: Mao Zedong (persoon) | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Mao Zedong.md — confidence 5 |
| ✓ | 2026-07-29T expansie | Agent 3 | Gap: Ranajit Guha | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Ranajit Guha.md — confidence 5 |
| ✓ | 2026-07-29T expansie | Agent 3 | Expansie: Sharpe Ratio | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Sharpe Ratio.md — confidence 5 |
| ✓ | 2026-07-29T consolidatie | Agent 3 | Gap: Tweede Wereldoorlog | Pagina reeds aanwezig (aangemaakt 2026-07-13) — geverifieerd volledig; false gap gesloten |
| ✓ | 2026-07-29T consolidatie | Agent 3 | Merge: Waardebeleggen | Waardebeleggen.md samengevoegd met Waarde Investeren.md (Wet 14); aliases + Greenwald-bron + 3 related-links toegevoegd |
| ✓ | 2026-07-30T expansie | Agent 3 | Expansie: Mild Cognitive Impairment | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Mild Cognitive Impairment.md — confidence 5 |
| ✓ | 2026-07-30T expansie | Agent 3 | Expansie: Edmund Husserl | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Edmund Husserl.md — confidence 5 |
| ✓ | 2026-07-30T expansie | Agent 3 | Expansie: Fama-French Drie-Factor Model | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Fama-French Drie-Factor Model.md — confidence 5 |
| ✓ | 2026-07-30T expansie | Agent 3 | Expansie: De Spaanse Burgeroorlog | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Spaanse Burgeroorlog.md — confidence 5 |
| ✓ | 2026-07-30T consolidatie | Agent 3 | Gap: Psychofarmacologie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Psychofarmacologie.md — confidence 5 |
| ✓ | 2026-07-30T consolidatie | Agent 3 | Gap: Serotonine | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Serotonine.md — confidence 5 |
| ✓ | 2026-07-30T consolidatie | Agent 3 | Gap: Het Inca Rijk | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Het Inca Rijk.md — confidence 5 |
| ✓ | 2026-07-30T consolidatie | Agent 3 | Gap: Intertemporele Keuze | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Intertemporele Keuze.md — confidence 5 |
| ✓ | 2026-07-30T expansie-2 | Agent 3 | Expansie: Zelf-Determinatietheorie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Zelf-Determinatietheorie.md — confidence 5 |
| ✓ | 2026-07-30T expansie-2 | Agent 3 | Expansie: William James | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/William James.md — confidence 5 |
| ✓ | 2026-07-30T expansie-2 | Agent 3 | Expansie: De Honderdjarige Oorlog | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Honderdjarige Oorlog.md — confidence 5 |
| ✓ | 2026-07-30T expansie-2 | Agent 3 | Expansie: Koers-Winstverhouding | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Koers-Winstverhouding.md — confidence 5 |
| ✓ | 2026-07-30T expansie-2 | Agent 3 | Gap: Cognitieve Belastingstheorie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Cognitieve Belastingstheorie.md — confidence 5 |
| ✓ | 2026-07-30T expansie-2 | Agent 3 | Gap: John Dewey | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/John Dewey.md — confidence 5 |
| ✓ | 2026-07-30T expansie-2 | Agent 3 | Gap: De Atlantische Slavenhandel | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Atlantische Slavenhandel.md — confidence 5 |
| ✓ | 2026-07-30T expansie-2 | Agent 3 | Gap: Earnings per Share (EPS) | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Earnings per Share.md — confidence 5 |
| ✓ | 2026-07-30T expansie-3 | Agent 3 | Expansie: Psychometrie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Psychometrie.md — confidence 5 |
| ✓ | 2026-07-30T expansie-3 | Agent 3 | Expansie: Intelligentie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Intelligentie.md — confidence 5 |
| ✓ | 2026-07-30T expansie-3 | Agent 3 | Expansie: Creditrating | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Creditrating.md — confidence 5 |
| ✓ | 2026-07-30T expansie-3 | Agent 3 | Expansie: De Inquisitie | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Inquisitie.md — confidence 5 |
| ✓ | 2026-07-30T consolidatie | Agent 3 | Gap: Return on Equity | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Return on Equity.md — confidence 5 |
| ✓ | 2026-07-30T consolidatie | Agent 3 | Gap: Winstmarge | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Winstmarge.md — confidence 5 |
| ✓ | 2026-07-31T expansie | Agent 3 | Expansie: DuPont Analyse | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/DuPont Analyse.md — confidence 5 |
| ✓ | 2026-07-31T expansie | Agent 3 | Expansie: De Suezcrisis | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Suezcrisis.md — confidence 5 |
| ✓ | 2026-07-31T expansie | Agent 3 | Expansie: Epicurisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Epicurisme.md — confidence 5 |
| ✓ | 2026-07-31T consolidatie | Agent 3 | Gap: Hedonisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Hedonisme.md — confidence 5 |
| ✓ | 2026-07-31T consolidatie | Agent 3 | Gap: EBITDA | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/EBITDA.md — confidence 5 |
| ✓ | 2026-07-31T consolidatie | Agent 3 | Gap: De Algeriaanse Oorlog | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Algeriaanse Oorlog.md — confidence 5 |
| ✓ | 2026-07-31T expansie-2 | Agent 3 | Expansie: De Cubacrisis | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Cubacrisis.md — confidence 5 |
| ✓ | 2026-07-31T expansie-2 | Agent 3 | Expansie: De Zijderoute | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Zijderoute.md — confidence 5 |
| ✓ | 2026-07-31T expansie-2 | Agent 3 | Expansie: Conjunctuurcycli | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Conjunctuurcycli.md — confidence 5 |
| ✓ | 2026-07-31T expansie-2 | Agent 3 | Expansie: Duits Idealisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Duits Idealisme.md — confidence 5 |
| ✓ | 2026-07-31T consolidatie | Agent 3 | Gap: Sectorrotatie | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Sectorrotatie.md — confidence 5 |
| ✓ | 2026-07-31T consolidatie | Agent 3 | Gap: Friedrich Schelling | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Friedrich Schelling.md — confidence 5 |
| ✓ | 2026-07-31T consolidatie | Agent 3 | Gap: Bounded Rationality | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Bounded Rationality.md — confidence 5 |
| ✓ | 2026-07-31T expansie | Agent 3 | Expansie: Neuropsychologische Screening | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Neuropsychologische Screening.md — confidence 5 |
| ✓ | 2026-07-31T expansie | Agent 3 | Expansie: Vrije Kasstroom | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Vrije Kasstroom.md — confidence 5 |
| ✓ | 2026-07-31T expansie | Agent 3 | Expansie: Magna Carta | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Magna Carta.md — confidence 5 |
| ✓ | 2026-07-31T expansie | Agent 3 | Expansie: Neoplatonisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Neoplatonisme.md — confidence 5 |
| ✓ | 2026-07-31T consolidatie | Agent 3 | Gap: Neuropsychologische Screening uitbreiden | RBANS, FAB, CANTAB toegevoegd als specifieke instrumenten — confidence 5 |
| ✓ | 2026-07-31T consolidatie | Agent 3 | Gap: Vrije Kasstroom verdiepen | Owner earnings (Buffett-methode), FCFF/FCFE formules toegevoegd — confidence 5 |
| ✓ | 2026-07-31T consolidatie | Agent 3 | Gap: Habeas Corpus Act (1679) | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Habeas Corpus Act (1679).md — confidence 5 |
| ✓ | 2026-07-31T consolidatie | Agent 3 | Gap: Neoplatonisme uitbreiden | Iamblichus, Proclus, islamitische transmissie uitgebreid — confidence 5 |
| ✓ | 2026-07-31T | Agent 3 | Gap: Bill of Rights (1689) | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Bill of Rights (1689).md — confidence 5 |
| ✓ | 2026-08-01T consolidatie | Agent 3 | Gap: De Glorious Revolution (1688) | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Glorious Revolution (1688).md — confidence 5 |
| ✓ | 2026-08-01T consolidatie | Agent 3 | Gap: Ibn Khaldun | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Ibn Khaldun.md — confidence 5 |
| ✓ | 2026-08-01T consolidatie | Agent 3 | Gap: Geneeskunde van de Geest (Psychiatriegeschiedenis) | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Geneeskunde van de Geest (Psychiatriegeschiedenis).md — confidence 5 |
| ✓ | 2026-08-01T expansie | Agent 3 | Expansie: Eetstoornissen | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Eetstoornissen.md — confidence 5 |
| ✓ | 2026-08-01T expansie | Agent 3 | Expansie: Liberalisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Liberalisme.md — confidence 5 |
| ✓ | 2026-08-01T expansie | Agent 3 | Expansie: Het Congres van Wenen | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Het Congres van Wenen.md — confidence 5 |
| ✓ | 2026-08-01T expansie | Agent 3 | Expansie: Emerging Markets | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Emerging Markets.md — confidence 5 |
| ✓ | 2026-08-01T consolidatie | Agent 3 | Gap: OCD — Obsessief-Compulsieve Stoornis | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Obsessief-Compulsieve Stoornis.md — confidence 5 |
| ✓ | 2026-08-01T consolidatie | Agent 3 | Gap: Nationalisme | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Nationalisme.md — confidence 5 |
| ✓ | 2026-08-01T consolidatie | Agent 3 | Gap: Frontier Markets | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Frontier Markets.md — confidence 5 |
| ✓ | 2026-08-01T consolidatie | Agent 3 | Gap: Democratie | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Democratie.md — confidence 5 |
| ✓ | 2026-08-01T expansie | Agent 3 | Gap: Stroop Test | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Stroop Test.md — confidence 5 |
| ✓ | 2026-08-01T expansie | Agent 3 | Gap: Procedureel Geheugen | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Procedureel Geheugen.md — confidence 5 |
| ✓ | 2026-08-01T expansie | Agent 3 | Gap: De Wetenschappelijke Revolutie | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/De Wetenschappelijke Revolutie.md — confidence 5 |
| ✓ | 2026-08-01T expansie | Agent 3 | Gap: Dollar Cost Averaging | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Dollar Cost Averaging.md — confidence 5 |
| ✓ | 2026-08-01T consolidatie | Agent 3 | Gap: Trail Making Test | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Trail Making Test.md — confidence 8 (Reitan 1958, Lezak 2012) |
| ✓ | 2026-08-01T consolidatie | Agent 3 | Gap: Wisconsin Card Sorting Test (WCST) | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Wisconsin Card Sorting Test.md — confidence 8 (Berg 1948, Milner 1963, Heaton 1993) |
| ✓ | 2026-08-01T consolidatie | Agent 3 | Gap: WAIS (Wechsler Adult Intelligence Scale) | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/WAIS.md — confidence 8 (Wechsler 1955/2008, Lezak 2012) |
| ✓ | 2026-08-02T consolidatie | Agent 3 | Gap: RAVLT (Rey Auditory Verbal Learning Test) | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/RAVLT.md — confidence 8 (Rey 1958, Schmidt 1996, Lezak 2012) |
| ✓ | 2026-08-02T consolidatie | Agent 3 | Gap: Cognitieve Architectuur | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Cognitieve Architectuur.md — confidence 7 (Anderson 1983, Baddeley 2000, Evans 2008) |
| ✓ | 2026-08-02T consolidatie | Agent 3 | Gap: Deep Brain Stimulation (DBS) | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Deep Brain Stimulation.md — confidence 8 (Benabid 1987, Mayberg 2005, Lozano 2013) |
| ✓ | 2026-08-02T expansie | Agent 3 | Gap: Confucianisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Confucianisme.md — confidence 5 |
| ✓ | 2026-08-02T expansie | Agent 3 | Gap: Boeddhisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Boeddhisme.md — confidence 5 |
| ✓ | 2026-08-02T expansie | Agent 3 | Gap: Mental Accounting | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Mental Accounting.md — confidence 5 (Thaler 1980, 1999) |
| ✓ | 2026-08-02T expansie | Agent 3 | Gap: Forensische Neuropsychologie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Forensische Neuropsychologie.md — confidence 5 |
| ✓ | 2026-08-02T consolidatie | Agent 3 | Gap: Taoisme | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Taoisme.md — confidence 5 |
| ✓ | 2026-08-02T consolidatie | Agent 3 | Gap: Anchoring (Ankereffect) | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Anchoring.md — confidence 5 (Kahneman & Tversky 1974) |
| ✓ | 2026-08-02T consolidatie | Agent 3 | Gap: Slaapstoornissen | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Slaapstoornissen.md — confidence 5 (DSM-5-TR, Walker 2017) |
| ✓ | 2026-08-02T expansie | Agent 3 | Gap: Borderline Persoonlijkheidsstoornis | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Borderline Persoonlijkheidsstoornis.md — confidence 5 (DSM-5-TR, Linehan 1993, Bateman & Fonagy 2004) |
| ✓ | 2026-08-02T expansie | Agent 3 | Gap: Cognitieve Herstructurering | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Cognitieve Herstructurering.md — confidence 5 (Beck 1979, Burns 1980) |
| ✓ | 2026-08-02T expansie | Agent 3 | Gap: Economische Ongelijkheid | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Economische Ongelijkheid.md — confidence 5 (Piketty 2014, Milanovic 2016) |
| ✓ | 2026-08-02T expansie | Agent 3 | Expansie: Absolutisme | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Absolutisme.md — confidence 5 |
| ✓ | 2026-08-02T expansie | Agent 3 | Expansie: Motivatie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Motivatie.md — confidence 5 |
| ✓ | 2026-08-02T expansie | Agent 3 | Expansie: Wilhelm Wundt | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Wilhelm Wundt.md — confidence 5 |
| ✓ | 2026-08-02T expansie | Agent 3 | Expansie: Sociale Klasse | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Sociale Klasse.md — confidence 5 |
| ✓ | 2026-08-02T consolidatie | Agent 3 | Gap: Mentaliseren | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Mentaliseren.md — confidence 5 (Fonagy & Bateman 2002/2004) |
| ✓ | 2026-08-02T consolidatie | Agent 3 | Gap: Cognitieve Triade (Beck) | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Cognitieve Triade (Beck).md — confidence 5 (Beck 1967/1979) |
| ✓ | 2026-08-03T expansie | Agent 3 | Gap: Mindfulness (MBSR) | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Mindfulness (MBSR).md — confidence 5 |
| ✓ | 2026-08-03T expansie | Agent 3 | Gap: Flow (Csikszentmihalyi) | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Flow (Csikszentmihalyi).md — confidence 5 |
| ✓ | 2026-08-03T expansie | Agent 3 | Gap: Eudaimonia | Aangemaakt: 02 Wiki/02 Filosofie - Wiki/Eudaimonia.md — confidence 5 |
| ✓ | 2026-08-03T expansie | Agent 3 | Gap: Tweede Wereldoorlog — Militaire Operaties | Aangemaakt: 02 Wiki/03 Geschiedenis - Wiki/Tweede Wereldoorlog — Militaire Operaties.md — confidence 5 |
| ✓ | 2026-08-03T expansie-2 | Agent 3 | Expansie: Alexithymie | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Alexithymie.md — confidence 8 (Sifneos 1972, Taylor et al. 1997) |
| ✓ | 2026-08-03T expansie-2 | Agent 3 | Expansie: Functionele Neurologische Stoornis | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Functionele Neurologische Stoornis.md — confidence 8 (Stone et al., DSM-5-TR) |
| ✓ | 2026-08-03T expansie-2 | Agent 3 | Expansie: Phineas Gage | Aangemaakt: 02 Wiki/01 Psychologie - Wiki/Phineas Gage.md — confidence 8 (Harlow 1868, Damasio 1994, Macmillan 2000) |
| ✓ | 2026-08-03T expansie-2 | Agent 3 | Expansie: Overconfidence Bias | Aangemaakt: 02 Wiki/04 Beleggen - Wiki/Overconfidence Bias.md — confidence 8 (Fischhoff 1977, Moore & Healy 2008, Barber & Odean 2001) |
| ↓ | 2026-08-03T expansie-2 | Agent 3 | Gap: Somatische Markerhypothese (Damasio) | Directe koppeling Phineas Gage + Vrije Wil; cross-domein psychologie ↔ filosofie |
| ↓ | 2026-08-03T expansie-2 | Agent 3 | Gap: Dissociatieve Identiteitsstoornis | Raakvlak FNS en PTSD; relevant MSc Klinische Neuropsychologie |
