---
discipline: geschiedenis
type: template
status: template
---

# Inbox — Geschiedenis

Plaats jouw aantekeningen in deze map. De pipeline verwerkt ze automatisch bij de volgende run.

---

## Formaat: Collegeaantekening

```markdown
---
discipline: geschiedenis
type: collegeaantekening
bron: Hoorcollege [Vaknaam] — Universiteit Utrecht
datum: 2026-07-09
status: nieuw
---

# [Titel college]

[Jouw aantekeningen in eigen woorden]

## Concepten
- Concept A — [korte omschrijving]
- Concept B — [korte omschrijving]

## Bronnen die de docent noemde
- Auteur (jaar). Titel.
```

---

## Formaat: Artikel / Paper

```markdown
---
discipline: geschiedenis
type: artikel-resumé
bron: Auteur, A. (jaar). Titel artikel. Journal, vol(nr), pp–pp.
datum: 2026-07-09
status: nieuw
---

# Resumé: [Artikeltitel]

[Eigen samenvatting]

## Kernbevindingen
1. ...
2. ...

## Verband met wat ik al weet
- Lijkt op [[Paradigmawisseling]] omdat...
```

---

> **Regels:**
> - Zet `status: nieuw` om verwerking te activeren
> - Bestanden met `status: verwerkt` worden niet opnieuw verwerkt
> - Dit templatebestand (status: template) wordt nooit aangeraakt door de pipeline
