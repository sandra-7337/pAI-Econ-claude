# Trade-Policy Shocks in Quantitative General Equilibrium

## Model Family Name
Structural Tariff and Retaliation Counterfactual Framework

## Canonical Economic Question
What are the aggregate, sectoral, regional, and distributional consequences of an observed or hypothetical tariff shock once import demand, domestic production, retaliation, tariff revenue, and general-equilibrium prices adjust?

## Verified References
- Fajgelbaum, Pablo D., Pinelopi K. Goldberg, Patrick J. Kennedy, and Amit K. Khandelwal. 2020. “The Return to Protectionism.” *Quarterly Journal of Economics* 135(1): 1-55. [DOI](https://doi.org/10.1093/qje/qjz036).
- Caliendo, Lorenzo, and Fernando Parro. 2015. “Estimates of the Trade and Welfare Effects of NAFTA.” *Review of Economic Studies* 82(1): 1-44. [DOI](https://doi.org/10.1093/restud/rdu035).

## When to Use This Model
- Use it to quantify unilateral tariffs, retaliation, trade agreements, or product-country exclusions.
- Use it when reduced-form price and quantity elasticities must be embedded in general equilibrium.
- Use it when sectoral or regional incidence matters in addition to national aggregate welfare.

## Typical Primitives
- Regions/countries (i,n), sectors/products (g), workers or factors, domestic and imported varieties.
- Import and export demand elasticities, domestic supply elasticities, bilateral tariffs (t_{ing}), and trade costs.
- Baseline imports, exports, domestic sales, production, expenditure, factor income, and tariff revenue.
- Short-run implementations may hold factor allocation or sectoral employment relatively fixed; long-run implementations allow reallocation.

## Timing
1. A baseline equilibrium is observed.
2. Import tariffs and possibly retaliatory tariffs change.
3. Border and duty-inclusive prices, import demand, exports, and domestic production respond.
4. Factor prices, expenditures, production, and government revenue clear in general equilibrium.

## Information Structure
The realized policy shock is common knowledge. Anticipation is excluded from the baseline event-study/counterfactual framework; use the trade-policy-uncertainty card if policy probabilities affect entry before implementation.

## Agent Heterogeneity
Sectors differ in elasticities, tariff exposure, and input use. Regions/workers differ in local industry composition and consumption baskets. Countries differ in retaliatory exposure and market power.

## Choice Variables
- Consumers and firms choose domestic versus imported varieties.
- Producers choose output and factor demand.
- Workers/factors reallocate according to the chosen horizon.
- Government tariff choices are exogenous in an impact analysis and endogenous only in an optimal-policy extension.

## Constraints
- Import demand and domestic supply must be consistent with price changes.
- Goods and factor markets clear.
- Tariff revenue is rebated or spent according to an explicit closure.
- Bilateral retaliation must be included on exports as well as imports.

## Equilibrium Concept or Solution Concept
A comparative general equilibrium calibrated to an observed baseline. Estimated import/export elasticities discipline bilateral responses; equilibrium price indices, factor returns, output, and expenditure jointly satisfy market clearing. The exact structure may be Armington, EK, or multisector Ricardian, but must be declared.

## Key Equations
For a CES/Armington import demand block,

\[
\frac{X_{ing}}{X_{nhg}}=
\left(\frac{p_{ig}(1+t_{ing})}{p_{hg}(1+t_{nhg})}\right)^{-\epsilon_g}
\times\frac{a_{ing}}{a_{nhg}}.
\]

A local reduced-form import response is

\[
d\log M_{ing}=-\epsilon_g\,d\log[p_{ig}(1+t_{ing})]+d\log E_{ng}+\text{substitution terms}.
\]

National welfare accounting can be organized as

\[
\Delta W=Delta CS+\Delta PS+\Delta TR+\Delta ToT-\Delta RC,
\]

where (TR) is tariff revenue and (RC) collects real adjustment/search/resource costs. Transfers must not be counted as resource destruction.

## Main Mechanism
Tariffs raise relative import prices, contract targeted imports, protect some domestic producers, expose exporters to retaliation, and reallocate expenditure and factors. General-equilibrium wage and price changes redistribute effects across regions. Aggregate consumer/importer losses can be much larger than net real-income losses because tariff revenue and producer gains are transfers within the country.

## Common Propositions
- Import and retaliatory tariffs reduce targeted trade volumes when demand elasticities are positive.
- Complete border-price pass-through places the statutory tariff initially on domestic import buyers.
- Net national welfare subtracts tariff revenue and producer gains from gross buyer losses before measuring deadweight loss.
- Regional incidence depends jointly on production exposure, retaliation, and consumption exposure.

## Comparative Statics Usually Available
- Larger trade elasticities generate larger quantity responses and deadweight loss for a given tariff.
- Greater foreign export-supply elasticity shifts incidence toward domestic buyers.
- Stronger input-output links spread tariffs beyond directly targeted industries.
- Slower factor mobility increases short-run regional dispersion.

## Data Requirements
- Product-country tariff schedules and timing, customs values/quantities, and duty payments.
- Domestic production, employment, wages, input-output use, exports, and regional industry shares.
- Price indices at the border and downstream, plus retaliation schedules.

## Estimation or Calibration
Estimate import and export responses from differential tariff changes with product and origin-time controls. Map elasticities and baseline shares into a structural GE model. Use pre-policy data for calibration and separate anticipation from realized treatment.

## Counterfactual Analysis
Remove, escalate, reallocate, or reciprocate tariffs; solve the equilibrium and report import/export volumes, production, wages, prices, revenue, and welfare. Include no-retaliation, fixed-network, and alternative factor-mobility cases.

## Welfare Implications
Protection can redistribute toward protected producers but usually creates consumption and production distortions. Terms-of-trade gains are possible for a large country; retaliation and input tariffs can overturn them. Distributional losses can be concentrated even when aggregate effects are small.

## Welfare Decomposition
Report consumer/importer losses, domestic producer gains, tariff revenue, terms-of-trade changes, retaliation losses, input-cost propagation, variety changes, and real adjustment costs. State whether the welfare object is national, global, or household-specific.

## Common Modeling Pitfalls
- Equating gross import-buyer losses with aggregate deadweight loss.
- Ignoring foreign retaliation or input tariffs.
- Mixing short-run estimated elasticities with a long-run frictionless factor model.
- Treating politically targeted tariffs as random without an identification strategy.

## How to Extend the Model
- Endogenous policy choice and trade wars.
- Firm-to-firm sourcing and switching.
- Heterogeneous households and regional labor markets.
- Policy uncertainty before tariffs are realized.

## Example Research Questions This Model Can Support
- What fraction of a tariff war’s welfare cost comes from retaliation rather than own tariffs?
- Which regions lose after accounting for both protected production and export retaliation?
- How would eliminating input tariffs differ from eliminating final-good tariffs?

## Closely Related Model Families
Caliendo-Parro; tariff pass-through; trade-policy uncertainty; network welfare; trade-labor dynamics.

## When This Model Is Not Appropriate
Do not use a static realized-shock framework when anticipation drives investment, when supplier relationships are inherited and costly to replace, or when the policy is too small for a full GE model to add value over transparent reduced-form incidence accounting.
