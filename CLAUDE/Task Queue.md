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

---

## Prioriteitsvolgorde

1. Gebruikersverzoek (hoogste prioriteit)
2. Nieuwe Raw gedetecteerd → volledige pipeline
3. Geplande dagelijkse taken
4. Geplande wekelijkse taken
5. Geplande maandelijkse taken
