---
id: bel-opties
tags: [beleggen, concept]
discipline: beleggen
type: concept
status: uitgewerkt
confidence: 5
sources:
  - "Black, F., & Scholes, M. (1973). The Pricing of Options and Corporate Liabilities. Journal of Political Economy, 81(3), 637–654."
  - "Hull, J. C. (2018). Options, Futures, and Other Derivatives (10th ed.). Pearson."
  - "Cox, J. C., Ross, S. A., & Rubinstein, M. (1979). Option pricing: A simplified approach. Journal of Financial Economics, 7(3), 229–263."
hub: "[[Beleggen]]"
related:
  - "[[Derivaten]]"
  - "[[Black-Scholes Model]]"
  - "[[Risicobeheer]]"
  - "[[Verliesaversie]]"
created: 2026-07-26
updated: 2026-07-26
---

# Opties

## Definitie

Een optie is een financieel derivaat dat de koper het recht geeft — maar niet de plicht — om een onderliggend actief (aandeel, index, grondstof, valuta) te kopen of te verkopen tegen een vooraf bepaalde prijs (de **uitoefenprijs** of *strike price*) op of vóór een bepaalde datum (de **vervaldatum**). De verkoper van de optie (*writer*) is wél verplicht de transactie uit te voeren als de koper dat verlangt. De koper betaalt voor dit recht een **premie** aan de verkoper.

## Kernconcepten

- **Call-optie:** Het recht om het onderliggende actief te kopen. Winst voor de koper wanneer de marktprijs de uitoefenprijs overstijgt.
- **Put-optie:** Het recht om het onderliggende actief te verkopen. Winst voor de koper wanneer de marktprijs daalt onder de uitoefenprijs.
- **Intrinsieke waarde vs. tijdswaarde:** De premie van een optie bestaat uit twee componenten. Intrinsieke waarde = het voordeel bij directe uitoefening (max. 0 of positief). Tijdswaarde = de verwachte kans dat de optie nog dieper *in-the-money* raakt vóór expiratie — neemt af naarmate de vervaldatum nadert (*theta*).
- **Griekse letters (Greeks):** Maatstaven voor de gevoeligheid van de optiepremie: *delta* (koerswijziging onderliggende), *gamma* (verandering van delta), *theta* (tijdsverval), *vega* (impliciete volatiliteit), *rho* (rente).
- **Europese vs. Amerikaanse opties:** Europese opties mogen alleen op de vervaldatum worden uitgeoefend; Amerikaanse opties op elk moment daarvóór.
- **Impliciete volatiliteit:** De marktimpliciet verwachte toekomstige volatiliteit van het onderliggende actief, afgeleid uit de optiepremie via het Black-Scholes model. Hoge impliciete volatiliteit leidt tot hogere premies.

## Context

Opties bestaan al eeuwen: in het zeventiende-eeuwse Amsterdam werden futures en opties verhandeld op de tulpenmarkt — de beroemde Tulpenmanie. De moderne theorie van optieprijsbepaling werd geformaliseerd door Fischer Black en Myron Scholes in 1973, met de publicatie van het Black-Scholes model — een revolutionaire doorbraak waarvoor Robert Merton en Scholes in 1997 de Nobelprijs voor Economie ontvingen (Black was inmiddels overleden). De Chicago Board Options Exchange (CBOE) opende in 1973 als de eerste gestandaardiseerde optiebeurs. Sindsdien is de markt exponentieel gegroeid; in 2020 overtrof het dagelijks volume van opties op Amerikaanse aandelen het volume van de aandelen zelf. Naast de theorie van Black-Scholes zijn het binomiale model (Cox-Ross-Rubinstein, 1979) en Monte Carlo-simulaties gangbare methoden voor optieprijzing van complexere contracten.

## Toepassingen

- **Hedging:** Beleggers gebruiken put-opties om portefeuilles te beschermen tegen koersdalingen (*protective put*). Bedrijven gebruiken opties om valuta- en grondstofprijsrisico's af te dekken.
- **Inkomensstrategieën:** Het schrijven van *covered calls* (verkopen van calls op posities die je bezit) genereert premie-inkomsten ten koste van opwaartse deelname boven de uitoefenprijs.
- **Speculatie met hefboom:** Een kleine premiebetaling geeft exposure aan een groot onderliggend bedrag. Verlies is beperkt tot de premie; de winst is theoretisch onbeperkt (voor call-kopers).
- **Impliciete volatiliteit als marktsignaal:** De VIX-index (*Volatility Index*) is gebaseerd op de impliciete volatiliteit van S&P 500-opties en wordt gebruikt als maatstaf voor marktangst. Een hoge VIX duidt op grote onzekerheid in de markt.
- **Gedragseconomisch aspect:** Onderzoek toont aan dat beleggers opties niet rationeel prijzen — zij overschatten de kans op extreme uitkomsten (*fat tails*), wat leidt tot systematische mis-pricing die traders kunnen benutten.

## Verbindingen

**Hub:** [[Beleggen]]

**Gerelateerd:**
- [[Derivaten]] — onderdeel van: opties zijn de meest verhandelde categorie van derivaten
- [[Black-Scholes Model]] — oorzaak/gevolg: het Black-Scholes model is het fundament van moderne optieprijsbepaling
- [[Risicobeheer]] — toepassing: opties zijn het meest gebruikte instrument voor portefeuille-hedging
- [[Verliesaversie]] — cross-domein: verliesaversie verklaart waarom beleggers bereid zijn een hoge premie te betalen voor bescherming (puts), ook als de kans op verlies klein is
- [[Volatiliteit]] — aanvulling: impliciete volatiliteit is de centrale variabele in optieprijsbepaling

**Cross-domein:**
- [[Verliesaversie]] — de bereidheid hoge premies te betalen voor neerwaartse bescherming weerspiegelt de psychologische asymmetrie in het wegen van verliezen versus winsten (Kahneman & Tversky)

## Bronnen

- Black, F., & Scholes, M. (1973). The Pricing of Options and Corporate Liabilities. *Journal of Political Economy, 81*(3), 637–654.
- Hull, J. C. (2018). *Options, Futures, and Other Derivatives* (10th ed.). Pearson.
- Cox, J. C., Ross, S. A., & Rubinstein, M. (1979). Option pricing: A simplified approach. *Journal of Financial Economics, 7*(3), 229–263.
