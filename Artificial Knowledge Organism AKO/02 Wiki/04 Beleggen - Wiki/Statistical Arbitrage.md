---
id: beleg-statistical-arbitrage
tags: [beleggen, concept]
discipline: beleggen
type: concept
status: uitgewerkt
confidence: 5
sources:
  - "Gatev, E., Goetzmann, W.N. & Rouwenhorst, K.G. (2006). Pairs Trading: Performance of a Relative-Value Arbitrage Rule. Review of Financial Studies, 19(3), 797–827."
  - "Pole, A. (2007). Statistical Arbitrage: Algorithmic Trading Insights and Techniques. Wiley."
  - "Zuckerman, G. (2019). The Man Who Solved the Market. Portfolio/Penguin."
hub: "[[Beleggen]]"
related:
  - "[[Kwantitatief Beleggen]]"
  - "[[Efficiënte Markthypothese]]"
  - "[[Risicobeheer]]"
  - "[[Hedgefondsen]]"
  - "[[Factor Investing]]"
created: 2026-07-24
updated: 2026-07-24
---

# Statistical Arbitrage

## Definitie

Statistical arbitrage (stat arb) is een kwantitatieve beleggingsstrategie die gebruikmaakt van statistische en wiskundige modellen om tijdelijke prijsafwijkingen tussen gerelateerde financiële instrumenten te identificeren en te exploiteren. De strategie berust op de veronderstelling dat historische prijsrelaties — gedreven door fundamentele economische krachten — op termijn herstellen naar een gemiddelde (mean reversion). Stat arb is typisch marktneutraal: long- en shortposities worden gecombineerd zodat het nettoblootstelling aan brede marktbewegingen minimaal is.

## Kernconcepten

- **Mean reversion**: De centrale aanname van stat arb: wanneer twee gerelateerde instrumenten tijdelijk uit hun historische prijsverhouding lopen, zal die verhouding herstellen. De strategie koopt het "goedkope" instrument en short het "dure" — en wacht op convergentie.
- **Pairs trading**: De eenvoudigste vorm van stat arb. Twee instrumenten met historisch hoge correlatie (bijv. Coca-Cola en PepsiCo) worden gemonitord. Als de spread tussen hun koersen buiten een statistische drempel beweegt, wordt de onderpresteerder gekocht en de uitpresteerder geshort.
- **Spread en z-score**: De spread is het prijs- of rendemenverschil tussen twee instrumenten. De z-score meet hoeveel standaarddeviaties de huidige spread van het historisch gemiddelde afwijkt. Een z-score boven +2 of onder −2 signaleert een handelskans.
- **Coïntegratie**: Een krachtigere statistische basis dan correlatie. Twee tijdreeksen zijn coïntegreerd als een lineaire combinatie van beide stationair is — hun prijzen divergeren op korte termijn maar hebben een langetermijnevenwicht (Engle & Granger 1987).
- **Portfolio stat arb**: In plaats van paren worden mandjes van aandelen ingezet. Factormodellen (zoals Barra) verklaren het rendement via markt-, sector- en stijlfactoren. Het residu (het onverklaarde deel) is de bron van alpha.
- **Holding period**: Stat arb-strategieën variëren van microseconden (HFT) tot weken. Langer houdende strategieën zijn minder gevoelig voor transactiekosten maar blootgesteld aan macro-schokken.

## Context

Statistical arbitrage werd gepionierd door de quantitative equities-divisie van Morgan Stanley in de jaren tachtig, onder leiding van Nunzio Tartaglia. Het team ontdekte dat aandelenparen met historisch hoge correlaties tijdelijke divergenties vertoonden die winstgevend exploiteerbaar waren. Na de ontmanteling van het team verspreidde de kennis zich naar hedgefondsen.

Jim Simons' Renaissance Technologies gebruikte vergelijkbare mean-reversion-principes als basis voor het Medallion Fund — hoewel het exacte model een streng bewaard geheim is. DE Shaw, Two Sigma en Citadel bouwden later grote stat arb-divisies. In academische kringen werd de strategie formeel beschreven door Gatev, Goetzmann & Rouwenhorst (2006), die aantoonden dat pairs trading over de periode 1962–2002 significant positieve rendementen opleverde — hoewel de alpha na publicatie gedeeltelijk verdween, wat de efficiënte markthypothese gedeeltelijk ondersteunt.

Een fundamenteel risico van stat arb is *model risk*: de aanname dat historische relaties in de toekomst standhouden. Bij LTCM (Long-Term Capital Management) werd een vergelijkbare strategie in 1998 fataal toen de Russische staatsobligatiemarkt ineenstortte en alle correlaties gelijktijdig braken — de zogenaamde "flight to quality". De strategie verloor zijn effectiviteit precies op het moment dat de posities het grootst waren.

## Toepassingen

- **Equity marktneutraal**: Long/short aandelenparen binnen dezelfde sector om sectorrisico te neutraliseren en puur van relatieve mispricing te profiteren.
- **ETF arbitrage**: Exploiteren van tijdelijke afwijkingen tussen ETF-koersen en de nettovermogenswaarde (NAV) van de onderliggende portefeuille.
- **Crypto stat arb**: Prijsverschillen van dezelfde cryptocurrency op verschillende exchanges (cross-exchange arbitrage) — bijzonder lucratief in vroege marktfasen.
- **Fixed income stat arb**: Exploiteren van afwijkingen in de rentecurve of tussen gerelateerde obligaties — een kernstrategie van LTCM.

## Verbindingen

**Hub:** [[Beleggen]]

**Gerelateerd:**
- [[Kwantitatief Beleggen]] — aanvulling: stat arb is de meest bekende toepassing van kwantitatief beleggen
- [[Efficiënte Markthypothese]] — tegenstelling: stat arb impliceert dat markten tijdelijk inefficiënt zijn — de strategie existeert bij gratie van marktimperfecties
- [[Risicobeheer]] — aanvulling: stat arb vereist strikte risicocontrole (stop-loss op spread-divergentie, kapitaalallocatie)
- [[Hedgefondsen]] — context: stat arb is een primaire strategie van marktneutrale hedgefondsen
- [[Factor Investing]] — verwant: beide verklaren rendementen via systematische factoren; stat arb focust op residuele alpha na factorcorrectie

**Cross-domein:**
- [[Werkgeheugen]] — cross-domein: algoritmische handelssystemen zijn een extern werkgeheugen dat mensen bevrijdt van de cognitieve last van real-time monitoring van honderden instrumenten
- [[Dual Process Theorie]] — cross-domein: stat arb elimineert System 1 (emotioneel, heuristisch) volledig en vervangen het door zuiver System 2-gebaseerde regeltoepassing

## Bronnen

- Gatev, E., Goetzmann, W.N. & Rouwenhorst, K.G. (2006). Pairs Trading: Performance of a Relative-Value Arbitrage Rule. *Review of Financial Studies*, 19(3), 797–827.
- Pole, A. (2007). *Statistical Arbitrage: Algorithmic Trading Insights and Techniques*. Wiley.
- Zuckerman, G. (2019). *The Man Who Solved the Market*. Portfolio/Penguin.
- Engle, R.F. & Granger, C.W.J. (1987). Co-Integration and Error Correction: Representation, Estimation, and Testing. *Econometrica*, 55(2), 251–276.
