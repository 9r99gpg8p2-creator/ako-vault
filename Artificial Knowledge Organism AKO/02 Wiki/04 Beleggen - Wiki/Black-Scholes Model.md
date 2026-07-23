---
id: beleg-black-scholes-model
tags: [beleggen, derivaten, opties, financiële-wiskunde, risico]
discipline: beleggen
type: model
status: uitgewerkt
confidence: 5
sources:
  - "Black, F., & Scholes, M. (1973). The pricing of options and corporate liabilities. Journal of Political Economy, 81(3), 637–654."
  - "Merton, R. C. (1973). Theory of rational option pricing. Bell Journal of Economics, 4(1), 141–183."
  - "Hull, J. C. (2018). Options, Futures, and Other Derivatives (10th ed.). Pearson."
hub: "[[Beleggen]]"
related:
  - "[[Derivaten]]"
  - "[[Capital Asset Pricing Model]]"
  - "[[Risicobeheer]]"
  - "[[Efficiënte Markthypothese]]"
  - "[[Moderne Portefeuille Theorie]]"
  - "[[Gedragseconomie]]"
created: 2026-07-23
updated: 2026-07-23
---

# Black-Scholes Model

## Definitie

Het Black-Scholes model (ook: Black-Scholes-Merton model) is een wiskundig model voor de prijsbepaling van Europese opties op aandelen. Het werd in 1973 gepubliceerd door Fischer Black en Myron Scholes, met fundamentele uitbreidingen door Robert Merton, die in 1997 de Nobelprijs voor Economie ontvingen (Black was in 1995 overleden). Het model levert een gesloten formule voor de theoretische prijs van een calloptie of putoptie op basis van vijf variabelen: de huidige aandelenprijs, de uitoefenprijs, de resterende looptijd, de risicovrije rente en de volatiliteit van het onderliggende aandeel.

## Kernconcepten

- **De Black-Scholes formule:** De prijs van een Europese calloptie is: C = S·N(d₁) − K·e^(−rT)·N(d₂), waarbij d₁ = [ln(S/K) + (r + σ²/2)T] / (σ√T) en d₂ = d₁ − σ√T. N(·) is de cumulatieve standaardnormale verdeling, S de aandelenprijs, K de uitoefenprijs, r de risicovrije rente, T de resterende looptijd en σ de volatiliteit.
- **Aannames van het model:** (1) De aandelenprijs volgt een Geometrische Brownse Beweging (log-normaalverdeling); (2) geen dividenduitkeringen; (3) constante volatiliteit; (4) continue handel mogelijk; (5) geen transactiekosten; (6) risicovrije rente is constant; (7) geen arbitragemogelijkheden.
- **Impliciete volatiliteit:** In de praktijk wordt het model omgekeerd gebruikt: uit de marktprijs van een optie wordt de *impliciete volatiliteit* berekend, een maatstaf voor de door de markt verwachte toekomstige onzekerheid. De VIX-index is gebaseerd op impliciete volatiliteiten.
- **De Greeks:** Partiële afgeleiden van de optieprijs naar de inputvariabelen: Delta (Δ) = gevoeligheid voor aandelenprijs, Gamma (Γ) = verandering in Delta, Theta (Θ) = tijdverval, Vega (ν) = gevoeligheid voor volatiliteit, Rho (ρ) = gevoeligheid voor rente.
- **Delta-hedging:** Een optieportefeuille kan risiconeutraal worden gemaakt door het onderliggend aandeel te kopen of te verkopen in een hoeveelheid gelijk aan de Delta, een techniek die Black-Scholes mogelijk maakt en die de kern vormt van moderne derivatenhandel.
- **Beperkingen:** Het model gaat uit van constante volatiliteit, maar markten laten een *volatility smile* of *skew* zien — lager aandelenprijs gaat gepaard met hogere impliciete volatiliteit. Extreme marktbewegingen (fat tails) worden onderschat. Na de beurskrach van 1987 zijn uitbreidingen zoals stochastische volatiliteitsmodellen (Heston) ontwikkeld.

## Context

In de jaren 1960 en vroeg 1970 bestond geen betrouwbare methode om optieprijzen theoretisch te bepalen. Fischer Black en Myron Scholes publiceerden in 1973 hun baanbrekende artikel in het *Journal of Political Economy*, hetzelfde jaar dat de Chicago Board Options Exchange (CBOE) opende. Het model werd direct door handelaren omarmd en verspreidde zich razendsnel via de calculators van CBOE-handelaren. Robert Merton publiceerde tegelijkertijd een uitbreiding die het model generaliseerde naar een breder scala aan contingent claims en de arbitragevrije prijsvorming wiskundig fundeerde. De Nobelprijs voor Economie in 1997 aan Scholes en Merton (Black posthumously erkend) bevestigde de paradigmatische status van het model. Het Black-Scholes model transformeerde niet alleen de financiële wereld — het legitimeerde kwantitatieve financiën als wetenschappelijke discipline en leidde tot de explosieve groei van de derivatenmarkt, die in omvang de aandelenmarkten verre overtrof.

## Toepassingen

- **Optiehandel:** Marktmakers op optiebeurzen gebruiken Black-Scholes (of varianten) als referentiekader voor biedprijzen en de constructie van hedgeportefeuilles.
- **Risicobeheer:** Delta, Gamma en Vega-hedging stellen financiële instellingen in staat om blootstelling aan marktrisico te kwantificeren en te mitigeren.
- **Bedrijfswaardering:** Reële-optieanalyse past Black-Scholes toe op investeringsbeslissingen met flexibiliteitswaarde (bijv. de waarde van het uitstellen van een investering).
- **Personeelsopties:** Bedrijven gebruiken Black-Scholes voor de verslaggeving van de reële waarde van aandelenopties als personeelsbeloning (IFRS 2, US GAAP ASC 718).
- **Structurele kredietmodellen:** Het Merton-model van obligatiewaardering ziet bedrijfsaandelen als een calloptie op de activa van het bedrijf en gebruikte Black-Scholes om kredietrisico te kwantificeren.
- **Academisch:** Het model is de hoeksteen van het financieel-economisch curriculum en het startpunt voor uitgebreidere stochastische modellen.

## Verbindingen

**Hub:** [[Beleggen]]

**Gerelateerd:**
- [[Derivaten]] — Black-Scholes is het fundamentele prijsmodel voor derivaten, met name opties
- [[Capital Asset Pricing Model]] — beide modellen zijn gebaseerd op no-arbitrage principes en gaan uit van risiconeutraal beleggers in evenwichtsmarkten
- [[Risicobeheer]] — delta-hedging en de Greeks zijn de operationele kern van derivatenrisicobeheer
- [[Efficiënte Markthypothese]] — Black-Scholes veronderstelt informatiefficiente markten; de volatility smile weerlegt gedeeltelijk deze aanname
- [[Moderne Portefeuille Theorie]] — beide modellen zijn pijlers van het klassieke financieel-economische paradigma uit de jaren 1950–1970
- [[Gedragseconomie]] — gedragseconomen bekritiseren de rationaliteitsaannames van Black-Scholes; de volatility skew is empirisch bewijs voor prijsafwijkingen

**Cross-domein:**
- [[Falsifiabilisme]] — de falsificeerbare voorspellingen van Black-Scholes (volatility smile als anomalie) illustreren hoe modellen in de wetenschapsfilosofie worden getest en bijgesteld

## Bronnen

- Black, F., & Scholes, M. (1973). The pricing of options and corporate liabilities. *Journal of Political Economy*, 81(3), 637–654.
- Merton, R. C. (1973). Theory of rational option pricing. *Bell Journal of Economics*, 4(1), 141–183.
- Hull, J. C. (2018). *Options, Futures, and Other Derivatives* (10th ed.). Pearson.
- Taleb, N. N. (1997). *Dynamic Hedging: Managing Vanilla and Exotic Options*. Wiley.
