# Melitz Model — Firm Heterogeneity and Trade

## Model Family Name
Monopolistic Competition with Heterogeneous Firms and Export Selection

## Canonical Economic Question
Why do only the more productive firms export, and how does trade exposure reallocate market shares and resources across firms within an industry?

## Verified References
- Melitz, Marc J. 2003. “The Impact of Trade on Intra-Industry Reallocations and Aggregate Industry Productivity.” *Econometrica* 71(6): 1695-1725. [DOI](https://doi.org/10.1111/1468-0262.00467).

## When to Use This Model
- Use it when firm productivity and export participation are central.
- Use it for entry, exit, selection, and within-industry reallocation after trade liberalization.
- Use it when symmetric-firm Krugman trade cannot explain exporter premia.

## Typical Primitives
- CES demand with elasticity (σ>1) and monopolistic competition.
- Potential entrants pay sunk cost (f_e) and draw productivity (φ) from distribution (G).
- Active firms pay fixed production cost (f), destination fixed export cost (f_x), and iceberg cost (τ).
- Exogenous firm death probability and free entry in the steady-state baseline.

## Timing
Potential firms pay the sunk entry cost and draw productivity; low-productivity draws exit; active firms produce and decide whether to export; exogenous death and new entry keep the industry in steady state.

## Information Structure
Productivity is unknown before entry and observed after the sunk cost is paid. Conditional on the draw, firms know aggregate prices and costs and take the price index as given.

## Agent Heterogeneity
Firms differ in productivity. Equilibrium separates exiters, domestic-only firms, and exporters by productivity cutoffs. Consumers are representative in the baseline.

## Choice Variables
- Potential firms choose entry.
- Active firms choose price, output, and export participation.
- Entry mass, domestic and export cutoffs, price indices, wages, and trade shares are equilibrium outcomes.

## Constraints
- Variable profit must cover fixed production and destination costs.
- CES demand implies constant markups.
- Free entry equates expected post-entry value to the sunk entry cost.
- Labor and goods markets clear; the mass of entrants replaces exogenous deaths in steady state.

## Equilibrium Concept or Solution Concept
A stationary monopolistic-competition equilibrium with free entry and endogenous productivity cutoffs. Domestic zero profit, export zero profit, free entry, price aggregation, and labor clearing jointly determine the allocation.

## Key Equations
For a firm from country (i),

\[
p_i(\varphi)=\frac{\sigma}{\sigma-1}\frac{w_i}{\varphi}.
\]

Domestic revenue and profit can be written as

\[
r_i(\varphi)=E_i\left(\frac{p_i(\varphi)}{P_i}\right)^{1-\sigma},
\qquad
\pi_i^d(\varphi)=\frac{r_i(\varphi)}{\sigma}-w_if_i.
\]

Export profit to (j) is

\[
\pi_{ij}^x(\varphi)
=\frac{E_j}{\sigma}
\left(\frac{\tau_{ij}p_i(\varphi)}{P_j}\right)^{1-\sigma}
-w_if_{ij}^x.
\]

Cutoffs satisfy (\pi_i^d(\varphi_i^*)=0) and (\pi_{ij}^x(\varphi_{ij}^{x*})=0).

## Main Mechanism
Fixed market-access costs make exporting profitable only for firms with enough productivity and variable profit. Trade exposure raises competition and reallocates expenditure toward productive domestic and foreign firms; marginal domestic firms exit and high-productivity firms expand.

## Common Propositions
- Exporters are selected from the upper tail of productivity.
- Exporters have higher sales and employment than domestic-only firms under common demand.
- Greater trade exposure reallocates market shares toward more productive firms and raises aggregate industry productivity.
- Firm productivity is exogenous in the baseline; exporter premia reflect self-selection, not learning by exporting.

## Comparative Statics Usually Available
- Lower variable trade costs raise export profitability and trade at intensive and extensive margins.
- Lower fixed export costs mainly expand export participation.
- Tougher import competition raises the domestic survival cutoff in the canonical symmetric liberalization.
- Greater productivity dispersion concentrates exports more heavily in top firms.

## Data Requirements
- Firm or plant panel data with sales, employment, entry/exit, export status, and destinations.
- Trade costs, tariffs, destination expenditure, wages, and price indices.
- Productivity or cost measures, recognizing that revenue productivity embeds demand and markups.

## Estimation or Calibration
Discipline (G), fixed costs, and trade costs with firm-size distributions, entry/exit, exporter shares, and destination participation. Identification of sunk versus recurring export costs requires panel transitions; cross-sectional exporter premia do not distinguish selection from learning.

## Counterfactual Analysis
Change variable or fixed trade costs; recompute entry, survival and export cutoffs, firm masses, prices, wages, trade, and aggregate productivity. Report exit, entry, intensive, and extensive margins separately.

## Welfare Implications
Trade changes variety, selection, prices, and nominal income. Aggregate gains do not imply that workers tied to exiting firms avoid transition losses. Under Pareto and the ACR restrictions, domestic trade share and trade elasticity summarize aggregate welfare; otherwise solve the full model.

## Welfare Decomposition
Decompose price-index change into imported variety, domestic variety, and reallocation/selection components, plus wage or terms-of-trade effects. Decompositions must avoid counting measured productivity reallocation as an additional gain when it already lowers prices.

## Common Modeling Pitfalls
- Confusing Melitz selection with Krugman’s symmetric firms.
- Treating exporter premia as proof of causality from productivity to exporting.
- Omitting the productivity distribution while claiming closed-form aggregation.
- Applying ACR welfare outside its restrictions.

## How to Extend the Model
- Multiproduct and multidestination firms.
- Dynamic export entry, learning, innovation, or financing.
- Variable markups, comparative-advantage sectors, or buyer-supplier search.

## Example Research Questions This Model Can Support
- How does tariff liberalization affect firm exit and export participation?
- Which firm margins account for aggregate productivity changes after trade opening?
- How do fixed destination costs shape the concentration of exports?

## Closely Related Model Families
Krugman new trade theory; multiproduct firms; dynamic export entry; ACR welfare.

## When This Model Is Not Appropriate
Do not use the baseline when firms are symmetric, strategic oligopoly matters, productivity is an endogenous state, or persistent buyer-supplier relationships are the central mechanism.
