---
id: beleg-monte-carlo-simulatie
tags: [beleggen, risicobeheer, kwantitatief, statistiek]
discipline: beleggen
type: model
status: uitgewerkt
confidence: 5
sources:
  - "Glasserman, P. (2003). Monte Carlo Methods in Financial Engineering. Springer."
  - "Bodie, Z., Kane, A., & Marcus, A.J. (2018). Investments (11th ed.). McGraw-Hill."
hub: "[[Beleggen]]"
related:
  - "[[Risicobeheer]]"
  - "[[Kwantitatief Beleggen]]"
  - "[[Black-Scholes Model]]"
  - "[[Statistical Arbitrage]]"
  - "[[Behavioral Finance]]"
created: 2026-07-25
updated: 2026-07-25
---

# Monte Carlo Simulatie

## Definitie

Monte Carlo simulatie is een kwantitatieve rekentechniek waarbij duizenden tot miljoenen willekeurige scenario's worden gegenereerd om de kansverdelingen van onzekere uitkomsten te schatten. In de financiële wereld wordt de methode gebruikt voor portefeuille-analyse, optiewaardering, risicobeheer (Value at Risk) en pensioenplanning. De naam verwijst naar het casino van Monte Carlo als symbool voor kansprocessen.

## Kernconcepten

- **Stochastisch proces**: Monte Carlo modelleert variabelen (aandelenkoersen, rentes, volatiliteit) als stochastische processen — doorgaans geometrische Brownse beweging — en simuleert duizenden mogelijke toekomstpaden
- **Value at Risk (VaR)**: Monte Carlo-VaR berekent het maximale verlies dat met een gegeven zekerheid (bijv. 99%) over een bepaalde periode niet zal worden overschreden, door de volledige kansverdeling te simuleren
- **Optiewaardering**: Complexe opties (Aziatische opties, barrieropties) die geen analytische oplossing hebben in het Black-Scholes-kader worden gewaardeerd via Monte Carlo door het uitbetaalprofiel over alle gesimuleerde paden te middelen
- **Correlatiematrix**: Simulaties van meerdere activa vereisen een realistische modellering van onderlinge correlaties; de Cholesky-decompositie wordt gebruikt om gecorreleerde steekproeven te genereren
- **Variance reduction techniques**: Methoden zoals antithetic variables, control variates en importance sampling verminderen de rekentijd en verbeteren de nauwkeurigheid van Monte Carlo-schattingen

## Context

De Monte Carlo-methode werd in de jaren 1940 ontwikkeld door Stanislaw Ulam en John von Neumann in het kader van het Manhattan Project, waarbij het werd gebruikt om neutronen-diffusie te simuleren. De naam werd door Nicholas Metropolis bedacht. In de jaren 1970–1980 vond de methode zijn weg naar de financiële economie, met name via de optiewaardering (Black-Scholes, 1973) en later het portefeuillerisicobeheer.

In de bankenwereld werd Monte Carlo-VaR na de financiële crisis van 2008 (Basel III) steeds vaker geëist door toezichthouders als aanvulling op historische en parametrische VaR-methoden. De methode werd populair in pensioenfondsplanning door scenarioanalyse van rendementsverdelingen over lange horizons.

## Toepassingen

- **Portefeuillesimulatie**: Simuleer 10.000 scenario's voor een gemengde portefeuille over 20 jaar om de kansverdeling van eindvermogen te berekenen — basis voor pensioenadvies
- **Optiewaardering**: Monte Carlo is de standaardmethode voor exotische opties die geen gesloten analytische oplossing kennen
- **Stress testing**: Banken en vermogensbeheerders gebruiken Monte Carlo-scenario's om de impact van extreme marktgebeurtenissen (tail risk) op portefeuilles te kwantificeren
- **Kredietrisico**: Credit VaR en verwachte verliesberekeningen voor kredietportefeuilles via Monte Carlo-simulatie van wanbetalingscorrelaties
- **ALM (Asset Liability Management)**: Pensioenfondsen simuleren toekomstige verplichtingen versus beleggingsopbrengsten over meerdere economische scenario's

## Verbindingen

**Hub:** [[Beleggen]]

**Gerelateerd:**
- [[Risicobeheer]] — Monte Carlo is een van de drie primaire VaR-methoden naast historische simulatie en parametrische methoden
- [[Kwantitatief Beleggen]] — Monte Carlo als kern van kwantitatieve portefeuille-analyse
- [[Black-Scholes Model]] — Monte Carlo als alternatief voor analytische optiewaardering bij complexe derivaten
- [[Statistical Arbitrage]] — Monte Carlo-simulaties worden gebruikt om strategieën te backtesten en risico te kwantificeren
- [[Diversificatie]] — Monte Carlo toont hoe correlaties en diversificatie de kansverdeling van portefeuillerendementen vormen

**Cross-domein:**
- [[Falsifiabilisme]] — Monte Carlo-modellen zijn afhankelijk van modelaannames; wanneer de aannames falen (bijv. normale verdeling vs. fat tails), falen ook de uitkomsten — epistemologisch relevant voor modelrisico

## Bronnen

- Glasserman, P. (2003). *Monte Carlo Methods in Financial Engineering*. Springer.
- Bodie, Z., Kane, A., & Marcus, A.J. (2018). *Investments* (11th ed.). McGraw-Hill.
- Metropolis, N., & Ulam, S. (1949). The Monte Carlo Method. *Journal of the American Statistical Association*, 44(247), 335–341.
