---
id: beleg-value-at-risk
tags: [beleggen, risicobeheer]
discipline: beleggen
type: concept
status: uitgewerkt
confidence: 5
sources:
  - "Jorion, P. (2006). Value at Risk: The New Benchmark for Managing Financial Risk. McGraw-Hill."
  - "Riskmetrics Group (1996). RiskMetrics Technical Document. J.P. Morgan."
hub: "[[Beleggen]]"
related:
  - "[[Risicobeheer]]"
  - "[[Beta en Volatiliteit]]"
  - "[[Monte Carlo Simulatie]]"
  - "[[Financiële Crisis 2008]]"
  - "[[Black-Scholes Model]]"
created: 2026-07-29
updated: 2026-07-29
---

# Value at Risk

## Definitie

Value at Risk (VaR) is een statistische risicomaatstaf die aangeeft welk maximaal verlies een portefeuille of positie kan oplopen over een bepaalde tijdshorizon bij een gegeven betrouwbaarheidsniveau. Een VaR van €1 miljoen bij een betrouwbaarheidsniveau van 95% over één dag betekent dat de portefeuille op meer dan 95% van de handelsdagen minder dan €1 miljoen verliest — maar op 5% van de dagen kan het verlies dit bedrag overschrijden.

## Kernconcepten

- **Betrouwbaarheidsniveau**: doorgaans 95% of 99%; hogere niveaus geven grotere VaR-schattingen
- **Tijdshorizon**: VaR wordt berekend voor een dag, een week of een maand; banken gebruiken standaard een 10-daagse VaR voor wettelijk kapitaal
- **Drie berekeningsmodellen**:
  - *Historische simulatie*: VaR berekend op basis van historische rendementen van de portefeuille
  - *Parametrische methode (variantie-covariantie)*: veronderstelt dat rendementen normaal verdeeld zijn
  - *Monte Carlo simulatie*: genereert duizenden scenario's via kansmodellen
- **Beperking — staartrisico**: VaR zegt niets over de omvang van verliezen voorbij het betrouwbaarheidsniveau (*Expected Shortfall* of CVaR doet dit wel)

## Context

VaR werd in de jaren negentig populair nadat J.P. Morgan zijn RiskMetrics-systeem introduceerde en in 1996 open publiceerde. Het Basel-akkoord maakte VaR vervolgens verplicht voor banken als onderdeel van marktrisicobeheer.

De Financiële Crisis van 2008 legde grote zwakheden bloot in VaR-modellen: historische data weerspiegelden geen extreme marktbewegingen (zwarte zwanen), correlaties braken bij stress samen, en modellen gaven een vals gevoel van zekerheid. Critici zoals Nassim Taleb wezen erop dat VaR het staartrisico systematisch onderschat.

Na 2008 zijn regulators overgeschakeld naar aanvullende maatstaven zoals *Expected Shortfall* (ES of CVaR), die ook de gemiddelde omvang van verliezen in het staartgebied meten.

## Toepassingen

- **Bankenregulering**: Basel II en III vereisen VaR-berekeningen voor het bepalen van minimaal vereist kapitaal bij marktrisico
- **Portefeuillebeheer**: vermogensbeheerders gebruiken VaR om risicoplafonds te bewaken
- **Stress testing**: VaR wordt aangevuld met stressscenario's om te testen wat er bij extreme marktbewegingen gebeurt
- **Handelslimietbeheer**: handelsbureaus stellen dagelijkse VaR-limieten per handelaar of afdeling

## Verbindingen

**Hub:** [[Beleggen]]

**Gerelateerd:**
- [[Risicobeheer]] — VaR is het centrale instrument in financieel risicobeheer
- [[Beta en Volatiliteit]] — inputvariabelen voor de parametrische VaR-methode
- [[Monte Carlo Simulatie]] — één van de drie standaardmethoden voor VaR-berekening
- [[Financiële Crisis 2008]] — toonde de beperkingen van VaR-modellen bloot
- [[Black-Scholes Model]] — deelt veronderstellingen over normaalverdeling en volatiliteit

**Cross-domein:**
- [[Cognitieve Biases]] — VaR-modellen negeren psychologische biases die werkelijk marktgedrag bepalen

## Bronnen

- Jorion, P. (2006). *Value at Risk: The New Benchmark for Managing Financial Risk*. McGraw-Hill.
- Riskmetrics Group (1996). *RiskMetrics Technical Document*. J.P. Morgan.
- Basel Committee on Banking Supervision (1996). *Amendment to the Capital Accord to Incorporate Market Risks*. BIS.
