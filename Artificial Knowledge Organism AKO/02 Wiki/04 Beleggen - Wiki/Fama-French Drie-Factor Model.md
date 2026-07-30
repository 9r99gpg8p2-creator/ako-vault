---
id: beleg-fama-french-drie-factor
tags: [beleggen, model]
discipline: beleggen
type: model
status: uitgewerkt
confidence: 5
sources:
  - "Fama, E.F. & French, K.R. (1992). The Cross-Section of Expected Stock Returns. Journal of Finance, 47(2), 427–465."
  - "Fama, E.F. & French, K.R. (1993). Common risk factors in the returns on stocks and bonds. Journal of Financial Economics, 33(1), 3–56."
hub: "[[Beleggen]]"
related:
  - "[[Capital Asset Pricing Model]]"
  - "[[Factor Investing]]"
  - "[[Moderne Portefeuille Theorie]]"
created: 2026-07-30
updated: 2026-07-30
---

# Fama-French Drie-Factor Model

## Definitie

Het Fama-French Drie-Factor Model is een vermogensprijsmodel ontwikkeld door Eugene Fama en Kenneth French (1992, 1993) dat het verwachte aandelenrendement verklaart via drie systematische risicofactoren: marktrisico (β), het kleine-minus-grote-marktkapitalisatie effect (SMB) en het hoge-minus-lage boekwaarde/marktwaarde effect (HML). Het model breidt het CAPM uit, dat uitsluitend op marktrisico stoelt, en verklaart een groter deel van de cross-sectionele rendementsvariantie.

## Kernconcepten

- **Marktfactor (MKT-Rf):** Het excess rendement van de marktportefeuille boven de risicovrije rente. Identiek aan de bètafactor uit het CAPM.
- **SMB (Small Minus Big):** Het rendementsverschil tussen een portefeuille van kleine en grote aandelen op basis van marktkapitalisatie. Kleinere aandelen presteren gemiddeld beter (*size premium*).
- **HML (High Minus Low):** Het rendementsverschil tussen aandelen met een hoge boekwaarde-marktwaarde-ratio (waarde-aandelen) en aandelen met een lage ratio (groei-aandelen). Waarde-aandelen presteren gemiddeld beter (*value premium*).
- **Factormodel:** Verwacht rendement = Rf + β₁·(MKT−Rf) + β₂·SMB + β₃·HML
- **Alpha (α):** Restrendement dat niet door de drie factoren verklaard wordt; een positieve alfa impliceert overperformance na risico-correctie.

## Context

Het CAPM (Sharpe, 1964; Lintner, 1965) voorspelde dat de bèta ten opzichte van de marktportefeuille het volledige verwachte rendement verklaart. Empirisch bleek deze voorspelling echter gebrekkig: small-cap aandelen en waarde-aandelen leverden structureel hogere rendementen dan het CAPM op basis van hun bèta voorspelde.

Fama en French identificeerden in hun 1992- en 1993-papers twee extra factoren die deze anomalieën systematisch vangen. Interpretatiedebat: sommigen zien SMB en HML als compensatie voor extra risico (risico-based verklaring); anderen zien ze als bewijs van marktinefficiëntie en gedragseconomische mispricing (behavioral verklaring, zie ook Behavioral Finance en Prospect Theory).

In 2015 breidde Fama-French het model uit naar een *vijf-factor model* door profitability (RMW — Robust Minus Weak) en investment (CMA — Conservative Minus Aggressive) toe te voegen, waarna het HML-factor deels zijn verklarende kracht verloor.

## Toepassingen

**Vermogensbeheer:** Fondsbeheerders gebruiken het model om alpha te meten — winstgevend beleggen echt risico-gecorrigeerde outperformance of slechts blootstelling aan bekende factoren? Factorblootstelling wordt bewust nagebootst door factor-ETF's en Smart Beta-strategieën.

**Academisch onderzoek:** Het Fama-French model is de standaardbenchmark voor prestatie-attributie in empirisch financieel onderzoek. Publicaties die aandelenportefeuillestudies bevatten, meten doorgaans alpha ten opzichte van het FF3-model.

**Portefeuilleconstructie:** Beleggers met een *value tilt* of *small-cap tilt* exploiteren bewust de HML- en SMB-premies; dit is de basis van Factor Investing en Smart Beta-producten.

**Risicobeheer:** De factorblootstellingen bieden inzicht in de bronnen van portefeuillerisico. Een portefeuille met hoge HML-lading is gevoeliger voor rotaties in de markt van waarde naar groei.

## Verbindingen

**Hub:** [[Beleggen]]

**Gerelateerd:**
- [[Capital Asset Pricing Model]] — Fama-French breidt het CAPM uit met twee extra factoren om zijn empirische tekortkomingen te adresseren
- [[Factor Investing]] — het FF-model is de theoretische basis voor systematisch factorgebaseerd beleggen
- [[Moderne Portefeuille Theorie]] — MPT levert het risicodiversificatieframework; FF3 verfijnt de rendementsverwachting
- [[Efficiënte Markthypothese]] — Fama is de grondlegger van de EMH; het bestaan van factorpremies zet spanning op zijn eigen efficiëntiehypothese
- [[Smart Beta]] — Smart Beta-producten implementeren FF3-factoren in indexvorm
- [[Behavioral Finance]] — gedragseconomische interpretatie van de factorpremies als mispricing door cognitieve biases

**Cross-domein:**
- [[Prospect Theory]] — verliesaversie en de waardepremie vertonen overlap: beleggers mijden waarde-aandelen door verliesangst (psychologie × beleggen)

## Bronnen

- Fama, E.F. & French, K.R. (1992). The Cross-Section of Expected Stock Returns. *Journal of Finance*, 47(2), 427–465.
- Fama, E.F. & French, K.R. (1993). Common risk factors in the returns on stocks and bonds. *Journal of Financial Economics*, 33(1), 3–56.
- Fama, E.F. & French, K.R. (2015). A five-factor asset pricing model. *Journal of Financial Economics*, 116(1), 1–22.
