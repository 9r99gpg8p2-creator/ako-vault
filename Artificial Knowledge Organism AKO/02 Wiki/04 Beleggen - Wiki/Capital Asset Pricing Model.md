---
id: beleg-capm
tags: [beleggen, concept]
discipline: beleggen
type: model
status: uitgewerkt
confidence: 5
sources:
  - "Sharpe, W. F. (1964). Capital asset prices: A theory of market equilibrium under conditions of risk. Journal of Finance, 19(3), 425–442."
  - "Lintner, J. (1965). The valuation of risk assets and the selection of risky investments in stock portfolios and capital budgets. Review of Economics and Statistics, 47(1), 13–37."
hub: "[[Beleggen]]"
related:
  - "[[Moderne Portefeuille Theorie]]"
  - "[[Efficiënte Markthypothese]]"
  - "[[Risicobeheer]]"
  - "[[Factor Investing]]"
  - "[[Gedragseconomie]]"
created: 2026-07-22
updated: 2026-07-22
---

# Capital Asset Pricing Model

## Definitie

Het Capital Asset Pricing Model (CAPM) is een financieel model dat het verwachte rendement van een belegging beschrijft als functie van het systematische risico (bèta) ten opzichte van de markt. Het CAPM stelt dat het vereiste rendement van een actief gelijk is aan de risicovrije rente plus een risicopremie die proportioneel is aan de marktgevoeligheid (bèta) van dat actief. Het model is de meest gebruikte theorie voor de prijsstelling van risicovol kapitaal en de berekening van vermogenskosten.

## Kernconcepten

- **Bèta (β)** — maatstaf voor systematisch risico: bèta = 1 betekent dat de belegging even volatiel is als de markt; β > 1 is actiefvolatiel, β < 1 is defensief; β < 0 is negatief gecorreleerd met de markt
- **Risicovrije rente (Rf)** — het rendement op een risicoloze belegging (doorgaans staatsobligaties met korte looptijd), de minimumdrempel waaronder geen rationele belegger zou investeren
- **Marktrisicopremie (ERP)** — het surplus rendement dat beleggers eisen boven de risicovrije rente om marktrisico te compenseren (historisch 4–6% per jaar voor aandelen vs. obligaties)
- **Security Market Line (SML)** — grafische weergave van het CAPM: alle beleggingen die op de SML liggen, zijn correct gewaardeerd; boven de SML = ondergewaardeerd, eronder = overgewaardeerd
- **Formule:** E(Ri) = Rf + βi × (E(Rm) − Rf), waarbij E(Rm) het verwachte marktrendement is

## Context

Het CAPM werd onafhankelijk ontwikkeld door William Sharpe (1964), John Lintner (1965) en Jan Mossin (1966), voortbouwend op de Moderne Portefeuilletheorie van Harry Markowitz. Sharpe ontving in 1990 de Nobelprijs, samen met Markowitz en Merton Miller.

Het model formaliseert de intuïtie dat beleggers alleen beloond worden voor het nemen van niet-diversifieerbaar risico (systematisch of marktrisico). Idiosyncratisch risico (bedrijfsspecifiek) kan immers worden weggediversifieerd. De formule verschaft een kwantitatieve basis voor:
- het berekenen van de gewogen gemiddelde kapitaalkosten (WACC) in corporate finance
- het evalueren van beleggingsprestaties (Sharpe ratio, Jensen's alpha)
- het bepalen van een fair rendement bij acquisities en investerings beslissingen

Empirisch bleek het CAPM echter tekort te schieten: Fama en French (1992, 1993) toonden aan dat ook omvang (small-cap premium) en boekwaarde-marktwaardeverhouding (value premium) extra rendementen verklaren die bèta alleen niet kan verklaren. Dit leidde tot het driefactorenmodel van Fama-French en later uitbreidingen (Carhart vier-factor, Fama-French vijf-factor). Desalniettemin blijft het CAPM het standaardmodel in onderwijs en praktijk.

## Toepassingen

- **Corporate finance** — berekening van het vereiste aandelenrendement als component van de WACC bij investeringsbeslissingen en bedrijfswaarderingen
- **Portefeuilleperformancemeting** — Jensen's alpha (werkelijk rendement minus CAPM-rendement) toetst of een fondsbeheerder outperformance leverde
- **Aandelenwaardering** — als inputvariabele in DCF-modellen (disconteringsvoet)
- **Risicoanalyse** — bèta als maatstaf voor marktgevoeligheid van een positie
- **Regulatoire kapitaaleisen** — financiële instellingen gebruiken CAPM-afgeleide modellen voor risicowaardering

## Verbindingen

**Hub:** [[Beleggen]]

**Gerelateerd:**
- [[Moderne Portefeuille Theorie]] — het CAPM is de directe uitbreiding van MPT, waarbij de evenwichtsprijsstelling van activa wordt bepaald
- [[Efficiënte Markthypothese]] — CAPM veronderstelt efficiënte markten; informatievoorsprong kan de SML niet duurzaam verslaan
- [[Risicobeheer]] — bèta is een kernmaatstaf in portefeuillerisicobeheer
- [[Factor Investing]] — factormodellen (Fama-French) zijn reacties op de tekortkomingen van het eenfactor-CAPM
- [[Gedragseconomie]] — gedragseconomen betwisten de rationele agenten-aanname waarop het CAPM berust

**Cross-domein:**
- [[Prospect Theory]] — Kahneman & Tversky tonen dat beleggers niet de nutsmaximalisatie volgen die het CAPM veronderstelt
- [[Risicoperceptie]] — psychologisch onderzoek toont dat risicobeleving van beleggers afwijkt van de statistische bèta

## Bronnen

- Sharpe, W. F. (1964). Capital asset prices: A theory of market equilibrium under conditions of risk. *Journal of Finance*, 19(3), 425–442.
- Lintner, J. (1965). The valuation of risk assets and the selection of risky investments in stock portfolios and capital budgets. *Review of Economics and Statistics*, 47(1), 13–37.
- Fama, E. F., & French, K. R. (1992). The cross-section of expected stock returns. *Journal of Finance*, 47(2), 427–465.
