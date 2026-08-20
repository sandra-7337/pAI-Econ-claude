# Tariff Pass-Through and Incidence

## Model Family Name
Border-Price Transmission and Welfare Incidence of Tariffs

## Canonical Economic Question
How much of a tariff is absorbed by foreign exporters versus passed into duty-inclusive import and downstream prices, and how are the resulting consumer, importer, producer, government, and efficiency effects distributed?

## Verified References
- Amiti, Mary, Stephen J. Redding, and David E. Weinstein. 2019. “The Impact of the 2018 Tariffs on Prices and Welfare.” *Journal of Economic Perspectives* 33(4): 187-210. [DOI](https://doi.org/10.1257/jep.33.4.187).
- Fajgelbaum, Pablo D., Pinelopi K. Goldberg, Patrick J. Kennedy, and Amit K. Khandelwal. 2020. “The Return to Protectionism.” *Quarterly Journal of Economics* 135(1): 1-55. [DOI](https://doi.org/10.1093/qje/qjz036).

## When to Use This Model
- Use it when the outcome is a border, wholesale, producer, or consumer price response to tariffs.
- Use it to distinguish statutory incidence from economic incidence.
- Use it to translate estimated pass-through and trade elasticities into welfare accounting.

## Typical Primitives
- Import demand (D(p^c)), foreign export supply (S^*(p^b)), pre-duty border price (p^b), and duty-inclusive price (p^c).
- Ad valorem tariff (t), domestic substitutes, importer/distributor markups, and downstream input shares.
- Demand elasticity (\epsilon_D), foreign export-supply elasticity (\epsilon_S^*), and domestic supply response.
- Baseline imports, tariffs, consumer expenditure, domestic production, and tariff revenue.

## Timing
The tariff is imposed; foreign exporters may change border prices; importers pay duties and choose prices/markups; buyers substitute across origins and domestic goods; domestic producers respond; government rebates or spends revenue.

## Information Structure
The realized tariff is observed. Pricing may be competitive or imperfectly competitive but that choice must be explicit. Anticipatory entry belongs in the policy-uncertainty model.

## Agent Heterogeneity
Products/origins differ in demand and export-supply elasticities, market power, invoicing, contract duration, and downstream input intensity. Households and firms differ in exposure through consumption and input use.

## Choice Variables
- Foreign exporters choose (p^b) if they have market power.
- Importers/distributors choose duty-inclusive prices and markups.
- Buyers choose quantities and substitute across sources.
- Domestic producers choose output and prices.

## Constraints
- Price wedge: (p^c=(1+t)p^b), before domestic distribution margins and taxes.
- Import demand equals foreign export supply at the traded quantity.
- Tariff revenue is (TR=t p^b M) under an ad valorem tariff.
- Goods-market and budget constraints close the incidence calculation.

## Equilibrium Concept or Solution Concept
A partial-equilibrium import-market equilibrium for immediate pass-through, optionally embedded in a quantitative general equilibrium for domestic producer, wage, input-output, and welfare effects.

## Key Equations
Define border-price absorption

\[
\rho_b=\frac{d\log p^b}{d\log(1+t)}.
\]

Then duty-inclusive pass-through is

\[
\rho_c=\frac{d\log p^c}{d\log(1+t)}=1+\rho_b.
\]

Under competitive import demand and export supply, the incidence split is governed by elasticities; in a log-linear benchmark,

\[
\rho_c=\frac{\epsilon_S^*}{\epsilon_S^*+\epsilon_D},
\qquad
-\rho_b=\frac{\epsilon_D}{\epsilon_S^*+\epsilon_D},
\]

with both elasticities expressed as positive magnitudes. Perfectly elastic foreign export supply implies (\rho_b=0) and full pass-through to domestic import buyers.

## Main Mechanism
The side of the market with the less elastic response bears more of the tariff. A foreign exporter with a highly elastic outside market does not cut its pre-duty price, leaving domestic importers to pay the duty. Domestic markups, distribution costs, input-output use, and substitution then determine how much reaches producer and consumer prices.

## Common Propositions
- Statutory payment at customs does not identify economic incidence.
- If pre-duty border prices do not fall, the tariff is fully passed to duty-inclusive import prices.
- Gross importer/consumer losses exceed deadweight loss because tariff revenue is a domestic transfer.
- Input tariffs can raise downstream domestic producer prices even for firms that do not import directly.

## Comparative Statics Usually Available
- More elastic foreign export supply increases domestic pass-through.
- More elastic import demand increases foreign absorption and quantity adjustment.
- Higher domestic input shares amplify downstream producer-price effects.
- Greater importer market power can generate variable-markup absorption or amplification.

## Data Requirements
- Transaction-level customs values, quantities, duties, origin, product, and importer.
- Border unit values or price indices before duties, duty-inclusive prices, and downstream producer/consumer prices.
- Domestic output, import shares, input-output exposure, and tariff revenue.

## Estimation or Calibration
Exploit product-origin-time tariff changes with granular fixed effects and pretrend checks. Estimate border-price and duty-inclusive-price responses separately. Use quantities to recover trade elasticities and domestic price data to trace downstream transmission.

## Counterfactual Analysis
Change tariffs and evaluate border-price absorption, import substitution, domestic prices, revenue, and deadweight loss. Embed the estimates in GE when wages, domestic production, retaliation, or input-output spillovers are material.

## Welfare Implications
Domestic buyers bear a tariff when foreign border prices do not adjust. National welfare must add tariff revenue and domestic producer surplus and subtract production/consumption distortions; global welfare additionally treats terms-of-trade transfers between countries symmetrically.

## Welfare Decomposition
Report foreign exporter surplus, domestic importer/distributor surplus, consumer loss, domestic producer gain, tariff revenue, terms-of-trade transfer, and deadweight loss. For input tariffs, add downstream cost and markup effects.

## Common Modeling Pitfalls
- Estimating only duty-inclusive prices and calling the coefficient foreign incidence.
- Using unit values without addressing quality or product-composition changes.
- Counting tariff revenue as a resource loss.
- Assuming full pass-through at the border implies identical retail-price pass-through.

## How to Extend the Model
- Variable markups and strategic exporter pricing.
- Sticky contracts, exchange-rate invoicing, and dynamic adjustment.
- Firm-to-firm bargaining and supplier switching.
- Heterogeneous-household and regional incidence.

## Example Research Questions This Model Can Support
- Did foreign exporters cut border prices after a tariff, or did domestic importers bear it?
- How much of an input tariff appears in downstream producer prices?
- How do market power and supplier relationships alter tariff incidence?

## Closely Related Model Families
Trade-policy shocks; supplier switching; Armington/EK import demand; network welfare.

## When This Model Is Not Appropriate
Do not use a static pass-through model when policy uncertainty drives entry, when supplier identities change discontinuously and are the main outcome, or when observed unit values cannot be separated from quality/composition.
