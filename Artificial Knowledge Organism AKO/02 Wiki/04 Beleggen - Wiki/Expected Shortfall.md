---
id: beleg-expected-shortfall
tags: [beleggen, concept]
discipline: beleggen
type: model
status: uitgewerkt
confidence: 5
sources:
  - "Artzner, P., Delbaen, F., Eber, J.M., & Heath, D. (1999). Coherent measures of risk. *Mathematical Finance*, 9(3), 203–228."
  - "Rockafellar, R.T., & Uryasev, S. (2000). Optimization of conditional value-at-risk. *Journal of Risk*, 2(3), 21–41."
  - "McNeil, A.J., Frey, R., & Embrechts, P. (2015). *Quantitative Risk Management*. Princeton University Press."
hub: "[[Beleggen]]"
related:
  - "[[Value at Risk]]"
  - "[[Risicobeheer]]"
  - "[[Financiële Crisis 2008]]"
  - "[[Black-Scholes Model]]"
created: 2026-07-29
updated: 2026-07-29
---

# Expected Shortfall

## Definitie

Expected Shortfall (ES), ook wel Conditional Value-at-Risk (CVaR) of Average Value-at-Risk (AVaR) genoemd, is een risicomaatstaf die aangeeft wat het verwachte verlies is in de ergste gevallen — namelijk in de gevallen die voorbij de Value-at-Risk (VaR) grens vallen. Concreet: als VaR op 95%-niveau aangeeft dat het maximale verlies op 1 dag €1 miljoen is, dan geeft ES (95%) aan wat het *gemiddelde* verlies is in de slechtste 5% van de gevallen. ES is een coherente risicomaatstaf en geldt als de opvolger van VaR in de internationale regelgeving na de Financiële Crisis van 2008.

## Kernconcepten

- **Definitie formeel:** ES(α) = E[X | X ≤ VaR(α)] — het verwachte verlies gegeven dat het verlies de VaR-drempel overschrijdt.
- **Coherente risicomaatstaf:** ES voldoet aan de vier axioma's van Artzner et al. (1999): translatie-invariantie, subadditiviteit, positieve homogeniteit en monotoniciteit. VaR voldoet níet aan subadditiviteit, wat ES superieur maakt voor portefeuille-risicometing.
- **Staartrisico (tail risk):** ES capteert het risico in de staart van de verdelingscurve — de zeldzame maar catastrofale verliezen die VaR negeert door enkel een kwantiel te rapporteren.
- **Basel III/IV en FRTB:** Na de Financiële Crisis van 2008 schreef het Bazels Comité voor Bankentoezicht in de Fundamental Review of the Trading Book (FRTB) voor dat banken ES moeten gebruiken in plaats van VaR voor de berekening van marktrisico-kapitaaleisen.
- **CVaR-optimalisatie:** Rockafellar & Uryasev (2000) toonden aan dat CVaR-minimalisatie als convex optimalisatieprobleem kan worden geformuleerd, wat efficiënte berekening mogelijk maakt — ook voor grote portefeuilles.

## Context

Value-at-Risk (VaR) werd in de jaren 1990 geïntroduceerd door JP Morgan als standaard risicomaatstaf en werd vervolgens opgenomen in de Basel II-regelgeving. Een fundamenteel bezwaar tegen VaR is dat het geen informatie geeft over de ernst van verliezen die de VaR-drempel overschrijden — het zegt enkel dat met kans α geen groter verlies optreedt, maar zwijgt over hoe groot het verlies kán zijn als het wél misgaat. Dit probleem werd pijnlijk zichtbaar tijdens de Financiële Crisis van 2008, toen staartrisico's zich materialiseerden op een schaal die VaR-modellen niet hadden voorzien. Het Bazels Comité migreerde in de FRTB (gepubliceerd 2016, geïmplementeerd 2023) naar ES als primaire risicomaatstaf. Expected Shortfall is uitgebreid bestudeerd door wiskundigen en financieel economen; het mathematische fundament werd gelegd door Artzner et al. (1999) in hun klassieke artikel over coherente risicomaatstaven.

## Toepassingen

- **Bankkapitaalvereisten (FRTB):** Grote banken berekenen dagelijks ES op 97.5%-niveau voor hun handelsboek als basis voor de minimale kapitaaleisen onder Basel IV.
- **Portefeuille-optimalisatie:** Vermogensbeheerders gebruiken CVaR-minimalisatie als objectieffunctie bij de samenstelling van portefeuilles die robuust zijn tegen staartrisico's.
- **Stresstesting:** ES complementeert stresstests door niet alleen extreme scenario's te definiëren maar ook de verwachte ernst van verliezen in die scenario's te kwantificeren.
- **Risicomanagement bij verzekeraars:** Solvency II en vergelijkbare regelgevingskaders voor verzekeraars gebruiken ES-achtige maatstaven (TVaR) voor de berekening van solvabiliteitsvereisten.

## Verbindingen

**Hub:** [[Beleggen]]

**Gerelateerd:**
- [[Value at Risk]] — ES is de directe opvolger van VaR; corrigeert het fundamentele subadditiviteitsgebrek van VaR
- [[Risicobeheer]] — ES is de meest gehanteerde staartrisico-maatstaf in professioneel risicobeheer
- [[Financiële Crisis 2008]] — de crisis toonde de tekortkomingen van VaR aan en leidde tot de adoptie van ES
- [[Black-Scholes Model]] — beide modellen veronderstellen kansverdelingen; ES is explicieter over de verdeling van staartverliezen

**Cross-domein:**
- [[Prospect Theory]] — verliesaversie en de asymmetrische waardering van verliezen verklaren waarom staartrisico psychologisch zwaar weegt
- [[Falsifiabilisme]] — de overstap van VaR naar ES is een voorbeeld van hoe wetenschappelijke en regulatoire modellen worden herzien na empirisch falen

## Bronnen

- Artzner, P., Delbaen, F., Eber, J.M., & Heath, D. (1999). Coherent measures of risk. *Mathematical Finance*, 9(3), 203–228.
- Rockafellar, R.T., & Uryasev, S. (2000). Optimization of conditional value-at-risk. *Journal of Risk*, 2(3), 21–41.
- McNeil, A.J., Frey, R., & Embrechts, P. (2015). *Quantitative Risk Management*. Princeton University Press.
