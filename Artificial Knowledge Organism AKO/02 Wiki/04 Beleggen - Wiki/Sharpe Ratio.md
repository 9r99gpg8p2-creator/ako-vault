---
id: beleg-sharpe-ratio
tags: [beleggen, risicobeheer, portefeuilletheorie, prestatiemeting]
discipline: beleggen
type: model
status: uitgewerkt
confidence: 5
sources:
  - "Sharpe, W.F. (1966). 'Mutual Fund Performance.' Journal of Business, 39(1), 119–138."
  - "Sharpe, W.F. (1994). 'The Sharpe Ratio.' Journal of Portfolio Management, 21(1), 49–58."
hub: "[[Beleggen]]"
related:
  - "[[Risicobeheer]]"
  - "[[Moderne Portefeuille Theorie]]"
  - "[[Capital Asset Pricing Model]]"
  - "[[Beta en Volatiliteit]]"
  - "[[Factor Investing]]"
created: 2026-07-29
updated: 2026-07-29
---

# Sharpe Ratio

## Definitie

De **Sharpe Ratio** is een maatstaf voor het voor risico gecorrigeerde rendement van een beleggingsportefeuille of activum, ontwikkeld door econoom William F. Sharpe (1966, herzien 1994). De ratio berekent hoeveel extra rendement (boven de risicovrije rente) een belegger ontvangt per eenheid totaal risico (gemeten als standaarddeviatie van het rendement). Een hogere Sharpe Ratio betekent een beter voor risico gecorrigeerd rendement. Sharpe ontving in 1990 de Nobelprijs voor Economie mede voor dit werk.

## Kernconcepten

- **Formule**: Sharpe Ratio = (R_p - R_f) / σ_p, waarbij R_p = gemiddeld portefeuillerendement, R_f = risicovrije rente, σ_p = standaarddeviatie van het portefeuillerendement.
- **Risicopremie**: De teller (R_p - R_f) is de *excess return* — het rendement boven de risicovrije rente (doorgaans staatsobligaties). Dit is de vergoeding voor het nemen van risico.
- **Standaarddeviatie als risico**: De noemer meet de totale volatiliteit van rendementen (zowel opwaartse als neerwaartse). Dit omvat zowel systematisch als idiosyncratisch risico.
- **Benchmarkvergelijking**: Fondsen worden vergeleken op basis van hun Sharpe Ratio — een fonds met 10% rendement en Sharpe 0,5 presteert risico-gewogen slechter dan een fonds met 8% rendement en Sharpe 1,0.
- **Varianten**: De *Treynor Ratio* gebruikt bèta in de noemer (alleen systematisch risico); de *Sortino Ratio* gebruikt alleen neerwaartse volatiliteit; de *Information Ratio* vergelijkt actief beheer met een benchmark.

## Context

William F. Sharpe ontwikkelde de ratio als uitbreiding van het *Capital Asset Pricing Model* (CAPM). In zijn oorspronkelijke artikel (1966) gebruikte hij de term "reward-to-variability ratio"; de naam "Sharpe Ratio" werd later door de industrie geadopteerd. In zijn herziene artikel (1994) verfijnde Sharpe de definitie voor gebruik met ex-post (historische) rendementen.

De ratio is een directe toepassing van de moderne portefeuilletheorie van Harry Markowitz: de efficiënte grenslijn identificeert portefeuilles die het hoogste rendement bieden bij een gegeven risiconiveau. De Sharpe Ratio kwantificeert de hellingshoek van de kapitaalmarktlijn — hoe steil de lijn, hoe beter de verhouding rendement/risico.

## Toepassingen

- **Fondsvergelijking**: Institutionele en particuliere beleggers gebruiken de Sharpe Ratio om actief beheerde fondsen, ETFs en hedgefondsen te vergelijken op risico-gecorrigeerde prestaties.
- **Portefeuilleoptimalisatie**: In kwantitatieve beleggingsstrategieën wordt de portefeuille geoptimaliseerd om de Sharpe Ratio te maximaliseren.
- **Prestatiebeoordeling**: Vermogensbeheerders rapporteren hun Sharpe Ratio als standaard KPI naast absoluut rendement.
- **Beperkingen**: De ratio gaat uit van normaal verdeelde rendementen (wat bij beleggingen niet altijd opgaat), negeert het onderscheid tussen opwaartse en neerwaartse volatiliteit, en kan worden gemanipuleerd via optiestrategieën.

## Verbindingen

**Hub:** [[Beleggen]]

**Gerelateerd:**
- [[Risicobeheer]] — de Sharpe Ratio is een kernmaatstaf voor risicobeheer
- [[Moderne Portefeuille Theorie]] — de theoretische basis van de ratio
- [[Capital Asset Pricing Model]] — Sharpe ontwikkelde zowel CAPM als de ratio
- [[Beta en Volatiliteit]] — de verwante maatstaven voor systematisch risico
- [[Factor Investing]] — factorportefeuilles worden beoordeeld op Sharpe Ratio

**Cross-domein:**
- [[Prospect Theory]] — de psychologie van risicoperceptie staat haaks op de rationele risicomaatstaf van de Sharpe Ratio
- [[Cognitieve Biases]] — beleggers misinterpreteren Sharpe Ratio door recency bias en framing

## Bronnen

- Sharpe, W.F. (1966). "Mutual Fund Performance." *Journal of Business*, 39(1), 119–138.
- Sharpe, W.F. (1994). "The Sharpe Ratio." *Journal of Portfolio Management*, 21(1), 49–58.
- Bacon, C.R. (2008). *Practical Portfolio Performance Measurement and Attribution*. Wiley.
