---
id: beleg-beta-en-volatiliteit
tags: [beleggen, beta, volatiliteit]
discipline: beleggen
type: concept
status: uitgewerkt
confidence: 5
sources:
  - "Sharpe, W.F. (1964). Capital Asset Prices: A Theory of Market Equilibrium Under Conditions of Risk. *Journal of Finance*, 19(3), 425–442."
  - "Markowitz, H. (1952). Portfolio Selection. *Journal of Finance*, 7(1), 77–91."
  - "Damodaran, A. (2012). *Investment Valuation*. Wiley."
hub: "[[Beleggen]]"
related:
  - "[[Capital Asset Pricing Model]]"
  - "[[Risicobeheer]]"
  - "[[Moderne Portefeuille Theorie]]"
  - "[[Diversificatie]]"
created: 2026-07-28
updated: 2026-07-28
---

# Beta en Volatiliteit

## Definitie

Beta (β) is een maatstaf voor de systematische risicogevoeligheid van een effect ten opzichte van de markt als geheel. Volatiliteit is de statistische maatstaf voor de spreiding van rendementen van een effect of index over een bepaalde periode, doorgaans uitgedrukt als standaarddeviatie. Samen vormen beta en volatiliteit de twee pijlers van kwantitatief risicobeheer in moderne portefeuilletheorie.

## Kernconcepten

- **Beta (β):** meet hoe sterk een aandeel meebeweegt met de marktindex. β = 1 betekent exact marktbewegingen volgen; β > 1 verhoogde gevoeligheid; β < 1 gedempt; β < 0 inverse correlatie.
- **Volatiliteit:** standaarddeviatie van rendementen over een periode. Historische volatiliteit is berekend uit gerealiseerde rendementen; impliciete volatiliteit wordt afgeleid uit optieprijzen.
- **Systematisch vs. idiosyncratisch risico:** beta vangt alleen het marktrisico (niet-diversifieerbaar) op. Bedrijfsspecifiek risico kan worden weggediversifieerd.

## Context

Beta werd geformaliseerd door William Sharpe (1964) in het Capital Asset Pricing Model (CAPM), voortbouwend op de portefeuilletheorie van Harry Markowitz (1952). De intuïtie is dat beleggers alleen vergoeding verwachten voor het dragen van systematisch risico — risico dat niet weg te diversifiëren valt.

De VIX-index (Volatility Index), ook wel de 'angstmeter van Wall Street' genannt, meet de impliciete volatiliteit van S&P 500-opties voor de komende 30 dagen en geldt als graadmeter voor marktsentiment en onzekerheid. VIX-waarden boven 30 signaleren doorgaans verhoogde stress in financiële markten.

Beta wordt berekend als: β = Cov(Ri, Rm) / Var(Rm), waarbij Ri het rendement van het effect is en Rm het marktrendement.

## Toepassingen

Beta wordt centraal gebruikt in het CAPM om de vereiste rendementsvoet te bepalen: E(Ri) = Rf + β × (E(Rm) − Rf), waarbij Rf de risicovrije rente is. Een hogere beta leidt tot een hogere vereiste vergoeding. Portefeuillemanagers gebruiken beta bij tactische allocatie: in bullmarkten zoekt men hogere-beta-aandelen (cyclicals, tech); in bearmarkten lagere beta (defensieve sectoren zoals nutsbedrijven, voedingsmiddelen).

Volatiliteit is de grondslag voor optiewaardering (Black-Scholes), Value-at-Risk-berekeningen en stresstests. Risicobeheerders monitoren volatiliteitsclusters — perioden van hoge volatiliteit tendenzen samen te komen (ARCH/GARCH-effect).

## Verbindingen

**Hub:** [[Beleggen]]

**Gerelateerd:**
- [[Capital Asset Pricing Model]] — CAPM is het theoretisch fundament van beta
- [[Risicobeheer]] — volatiliteit en beta zijn primaire risico-inputvariabelen
- [[Moderne Portefeuille Theorie]] — diversificatie minimaliseert idiosyncratisch risico, beta resteert
- [[Diversificatie]] — bèta-neutrale portefeuilles via diversificatie
- [[Opties]] — impliciete volatiliteit bepaalt optiepremies

**Cross-domein:**
- [[Prospect Theory]] — mensen percipiëren volatiliteit asymmetrisch: dalende markten wegen zwaarder (verliesaversie)
- [[Heuristieken]] — beleggers misschatten beta systematisch door recency bias

## Bronnen

- Sharpe, W.F. (1964). Capital Asset Prices: A Theory of Market Equilibrium Under Conditions of Risk. *Journal of Finance*, 19(3), 425–442.
- Markowitz, H. (1952). Portfolio Selection. *Journal of Finance*, 7(1), 77–91.
- Damodaran, A. (2012). *Investment Valuation*. Wiley.
