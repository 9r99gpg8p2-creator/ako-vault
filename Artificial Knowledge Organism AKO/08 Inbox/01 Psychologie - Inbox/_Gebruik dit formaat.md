---
status: template
---

# Inbox — Psychologie

Drop hier elk `.md` bestand met psychologie-inhoud. **Geen frontmatter vereist.**

Het systeem detecteert automatisch de discipline, extraheert wiki-kandidaten en verwerkt ze.

---

## Minimaal voorbeeld (werkt direct)

```markdown
# Hoorcollege Cognitieve Neuropsychologie — 9 juli 2026

Werkgeheugen is het systeem dat informatie tijdelijk actief houdt.
Baddeley (1974) onderscheidt: fonologische lus, visuospatieel kladblok,
centrale executieve en episodische buffer.

Reconsolidatie: herinneringen worden bij ophaling labil en kunnen worden
overschreven. Window: ~6 uur. Relevant voor EMDR bij PTSD.

Cognitieve belasting: de hoeveelheid werkgeheugen die een taak vereist.
Hoge belasting verstoort leren. Sweller (1988).
```

Agent 1 haalt hieruit automatisch: Werkgeheugen, Reconsolidatie, EMDR, PTSD, Cognitieve belasting.

---

## Optioneel: frontmatter voor meer controle

```markdown
---
discipline: psychologie
type: collegeaantekening | boek-samenvatting | artikel-resumé | opdracht
bron: Titel — Auteur (jaar)
datum: 2026-07-09
---
```

Zonder frontmatter werkt het ook. Met frontmatter heb je meer controle over de bron-attributie.

---

> Bestanden met `status: verwerkt` worden niet opnieuw verwerkt.
> Bestanden die beginnen met `_` worden altijd overgeslagen (dit bestand dus ook).
