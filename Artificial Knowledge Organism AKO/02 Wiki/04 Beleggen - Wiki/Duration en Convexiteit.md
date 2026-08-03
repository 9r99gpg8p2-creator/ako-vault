---
id: beleg-duration-convexiteit
tags: [beleggen, obligaties, rentegevoeligheid, duration, convexiteit]
discipline: beleggen
type: concept
status: uitgewerkt
confidence: 5
sources:
  - "Fabozzi, F. J. (2016). Bond Markets, Analysis, and Strategies (9th ed.). Pearson."
  - "Tuckman, B., & Serrat, A. (2011). Fixed Income Securities: Tools for Today's Markets (3rd ed.). Wiley."
hub: "[[Beleggen]]"
related:
  - "[[Obligaties]]"
  - "[[Obligatiemarkt]]"
  - "[[Rentecurve]]"
  - "[[Risicobeheer]]"
  - "[[Value at Risk]]"
created: 2026-08-03
updated: 2026-08-03
---

# Duration en Convexiteit

## Definitie

Duration en convexiteit zijn twee samenhangende maatstaven voor de rentegevoeligheid van een obligatie of obligatieportefeuille. Duration meet de lineaire (eerste-orde) gevoeligheid van de obligatieprijs voor een renteverandering; convexiteit corrigeert voor de niet-lineaire (tweede-orde) afwijking die optreedt bij grotere rentebewegingen. Samen geven zij een nauwkeurige schatting van hoeveel een obligatieportefeuille in waarde verandert bij een verschuiving van de rentecurve.

## Kernconcepten

- **Macaulay Duration:** het gewogen gemiddelde van de tijdstippen waarop de kasstromen van een obligatie worden ontvangen, gewogen naar de contante waarde van elke kasstroom. Uitgedrukt in jaren. Een obligatie met een Macaulay Duration van 7 jaar heeft zijn economisch zwaartepunt op jaar 7.
- **Modified Duration:** de procentuele prijsverandering van een obligatie bij een renteverandering van 1 basispunt (0,01%). Berekend als Macaulay Duration gedeeld door (1 + yield/m), waarbij m het aantal couponbetalingen per jaar is.
  - Formule: ΔP/P ≈ −ModDuration × Δy
- **Dollar Duration (DV01):** de absolute prijsverandering in euro's (of dollars) bij een renteverandering van 1 basispunt. Essentieel instrument voor risicohedging.
- **Convexiteit:** de tweede afgeleide van de prijsrente-relatie. Obligaties hebben van nature positieve convexiteit: de prijsstijging bij een rentedaling is groter dan de prijsdaling bij een vergelijkbare rentestijging. Dit is een voordeel voor de obligatiehouder.
  - Gecombineerde benadering: ΔP/P ≈ −ModDuration × Δy + ½ × Convexiteit × (Δy)²
- **Negatieve convexiteit:** callable bonds (obligaties met een terugkoopoptie voor de emittent) vertonen negatieve convexiteit in het relevante rentebereik — de emittent koopt terug bij dalende rentes, wat de prijsstijging begrenst.
- **Portfolio Duration:** de gewogen gemiddelde duration van alle obligaties in een portefeuille. Gebruikt voor het meten en managen van het totale renterisico.
- **Key Rate Duration:** de gevoeligheid van een obligatie voor veranderingen in rentes op specifieke looptijdpunten van de curve (bijv. 2 jaar, 10 jaar, 30 jaar), in tegenstelling tot parallelle verschuivingen.

## Context

De concepten duration en convexiteit zijn ontwikkeld in de context van het portefeuillebeheer van obligaties in de twintigste eeuw. Frederick Macaulay introduceerde de Macaulay Duration in 1938 als een maatstaf voor de gemiddelde looptijd van een obligatie. In de jaren 1970 en 1980, toen rentevolatiliteit sterk toenam door de oliecrises en de Volcker-schok in de VS (de renteophoging om inflatie te bestrijden), werd duration het centrale risicobeheerstool voor obligatiebeleggers.

Met de opkomst van gesofisticeerde rentederivaten (swaps, swaptions, caps/floors) in de jaren 1990 werd convexiteit een kritische factor in het meten van de niet-lineaire risico's van complexe obligatiestructuren. Hedgefondsen en zakenbanken gebruiken DV01 en convexiteit dagelijks voor het afdekken van grote renteboekhouding.

## Toepassingen

- **Risicohedging:** Een obligatiebeheerder die de duration van de portefeuille wil verlengen zonder obligaties te kopen, kan renteswaps (receive fixed, pay floating) gebruiken om synthetisch duration toe te voegen.
- **Asset-Liability Management (ALM):** Pensioenfondsen en verzekeraars matchen de duration van hun obligatieportefeuille met de duration van hun verplichtingen om renterisico te elimineren (immunisatiestrategie).
- **Bullet vs. Barbell:** Een bullet-strategie concentreert kasstromen rond één looptijdpunt; een barbell-strategie verdeelt ze tussen korte en lange looptijden. Beide kunnen dezelfde duration hebben maar verschillen in convexiteit — de barbell heeft meer convexiteit.
- **Sensitiviteitsanalyse:** Bij waardering van obligatieportefeuilles onder stressscenario's (renteschok van +200bp) wordt convexiteit onmisbaar voor nauwkeurige schade-inschatting.
- **ETF en indexbeheer:** Duration is de primaire risicofactor die passieve obligatie-ETFs proberen te repliceren ten opzichte van hun benchmark.

## Verbindingen

**Hub:** [[Beleggen]]

**Gerelateerd:**
- [[Obligaties]] — duration en convexiteit zijn fundamentele kenmerken van elke individuele obligatie
- [[Obligatiemarkt]] — het brede marktrisico wordt in duration-termen uitgedrukt en beheerd
- [[Rentecurve]] — key rate duration meet gevoeligheid voor veranderingen in specifieke delen van de curve
- [[Risicobeheer]] — duration en DV01 zijn de primaire tools voor het meten en hedgen van renterisico
- [[Value at Risk]] — obligatie-VaR-modellen zijn grotendeels gebaseerd op duration-gebaseerde sensitiviteit

**Cross-domein:**
- [[Prospect Theory]] — beleggers reageren asymmetrisch op convexiteitsvoordelen: de vrees voor verlies (rentestijging) weegt zwaarder dan de verwachte convexiteitswinst bij rentedalingen

## Bronnen

- Fabozzi, F. J. (2016). *Bond Markets, Analysis, and Strategies* (9th ed.). Pearson.
- Tuckman, B., & Serrat, A. (2011). *Fixed Income Securities: Tools for Today's Markets* (3rd ed.). Wiley.
