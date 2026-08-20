# Armington Structural Gravity

## Model Family Name
CES Trade by National Origin with Multilateral Resistance

## Canonical Economic Question
How do bilateral trade costs and relative expenditure capacity determine trade between origin-differentiated national varieties once general-equilibrium resistance to all partners is respected?

## Verified References
- Armington, Paul S. 1969. “A Theory of Demand for Products Distinguished by Place of Production.” *IMF Staff Papers* 16(1): 159-178. [IMF publication page](https://www.elibrary.imf.org/view/journals/024/1969/001/article-A007-en.xml).
- Anderson, James E., and Eric van Wincoop. 2003. “Gravity with Gravitas: A Solution to the Border Puzzle.” *American Economic Review* 93(1): 170-192. [DOI](https://doi.org/10.1257/000282803321455214).

## When to Use This Model
- Use it when products are differentiated by country or region of origin and firm selection is unnecessary.
- Use structural gravity to estimate trade-cost effects or evaluate bilateral barriers while respecting multilateral resistance.
- Use it as a transparent benchmark for tariffs, border effects, or regional integration.

## Typical Primitives
- Origins (i), destinations (j), origin output (Y_i), destination expenditure (E_j), and world income (Y).
- CES elasticity (\sigma>1), origin taste or quality weights, and bilateral iceberg costs (t_{ij}\geq1).
- One aggregate variety per origin in the canonical aggregate formulation.
- Outward multilateral resistance (\Pi_i) and inward multilateral resistance (P_j) as equilibrium price-index terms.

## Timing
Static. Outputs, expenditures, and bilateral costs are given or jointly determined; consumers allocate expenditure across origins; multilateral-resistance terms and trade flows solve simultaneously.

## Information Structure
Complete information about preferences, delivered prices, expenditures, and trade costs. There is no firm-level private information or idiosyncratic productivity draw.

## Agent Heterogeneity
Origins differ in output and variety attributes; destinations differ in expenditure and access to all suppliers. Within a destination, consumers are represented by a CES aggregator.

## Choice Variables
- Consumers choose quantities from each origin.
- Competitive suppliers choose output conditional on technology in the general-equilibrium closure.
- Bilateral trade flows and multilateral-resistance indices are equilibrium outcomes.

## Constraints
- CES expenditure exhausts destination income.
- Delivered prices equal factory-gate prices times bilateral trade costs.
- Bilateral shipments sum to origin output and destination purchases sum to expenditure.
- Trade-cost counterfactuals must update both inward and outward multilateral resistance.

## Equilibrium Concept or Solution Concept
A competitive structural-gravity equilibrium. Given output, expenditure, and bilateral costs, the nonlinear multilateral-resistance system determines bilateral trade; a full general-equilibrium version also solves production, income, and market clearing.

## Key Equations
An Armington CES aggregate can be written as

\[
Q_j=\left[\sum_i \beta_{ij}^{1/\sigma}q_{ij}^{(\sigma-1)/\sigma}\right]^{\sigma/(\sigma-1)}.
\]

Structural gravity is

\[
X_{ij}=\frac{Y_iE_j}{Y}
\left(\frac{t_{ij}}{\Pi_iP_j}\right)^{1-\sigma},
\]

with multilateral resistance satisfying

\[
\Pi_i^{1-\sigma}=\sum_j\frac{E_j}{Y}
\left(\frac{t_{ij}}{P_j}\right)^{1-\sigma},
\qquad
P_j^{1-\sigma}=\sum_i\frac{Y_i}{Y}
\left(\frac{t_{ij}}{\Pi_i}\right)^{1-\sigma}.
\]

## Main Mechanism
A bilateral barrier matters relative to each partner’s access to the rest of the world. Inward resistance summarizes the destination’s overall remoteness from suppliers; outward resistance summarizes the origin’s overall remoteness from markets. Ignoring either term misattributes multilateral forces to the bilateral barrier.

## Common Propositions
- Bilateral trade is increasing in origin output and destination expenditure and decreasing in bilateral costs relative to multilateral resistance.
- The trade elasticity is (1-\sigma) with respect to iceberg costs in the baseline.
- A uniform proportional increase in all bilateral costs may leave relative trade shares unchanged under suitable normalization.
- Border effects inferred from naive gravity can be biased when multilateral resistance is omitted.

## Comparative Statics Usually Available
- Lower (t_{ij}) increases (X_{ij}) directly and changes every (\Pi) and (P) indirectly.
- More remote destinations trade more with a given partner, other bilateral costs equal.
- A larger (\sigma) makes expenditure shares more responsive to relative delivered prices.

## Data Requirements
- Bilateral trade including domestic flows, output, expenditure, and consistent geographic units.
- Tariffs, freight costs, distance, borders, language, or policy variables used to parameterize trade costs.
- Panel identifiers and exporter-time/importer-time fixed effects for empirical structural gravity.

## Estimation or Calibration
Estimate multiplicative gravity with PPML and exporter-time and importer-time fixed effects to absorb multilateral resistance; include domestic trade when possible. Mapping policy coefficients into trade-cost changes requires an independently justified (\sigma) or trade elasticity.

## Counterfactual Analysis
Change bilateral costs, solve the multilateral-resistance system, and update trade flows. In a conditional-GE exercise hold outputs and expenditures fixed; in a full-GE exercise update incomes, production, and expenditure until markets clear.

## Welfare Implications
In a one-sector CES endowment version, real income depends on the CES price index and income. Welfare results are sensitive to whether output is fixed, trade is balanced, tariff revenue is rebated, and production responds; a conditional-gravity counterfactual alone is not a complete welfare calculation.

## Welfare Decomposition
Separate changes in nominal income, inward multilateral resistance/consumer prices, outward market access, tariff revenue, and any terms-of-trade response. Not applicable as a unique decomposition in the demand-only Armington system because production and income closure are unspecified.

## Common Modeling Pitfalls
- Estimating log-linear gravity after dropping zeros and ignoring heteroskedasticity.
- Omitting domestic trade or multilateral-resistance controls.
- Treating a border coefficient as a welfare effect without solving the equilibrium.
- Confusing the substitution elasticity with a separately estimated reduced-form policy coefficient.

## How to Extend the Model
- Multiple sectors, input-output linkages, tariffs, and nonhomothetic demand.
- Endogenous production and factor-market clearing.
- Heterogeneous firms or Ricardian technology when origin varieties are too coarse.

## Example Research Questions This Model Can Support
- How does a free-trade agreement reallocate bilateral trade after multilateral resistance adjusts?
- How large is a national border effect once domestic trade is included?
- Which destinations are insulated from a bilateral tariff by access to alternative suppliers?

## Closely Related Model Families
Eaton-Kortum Ricardian gravity; ACR welfare sufficient statistics; Caliendo-Parro; quantitative trade counterfactuals.

## When This Model Is Not Appropriate
Do not use a one-variety-per-origin Armington model when firm selection, extensive margins, granular supplier networks, product quality, or endogenous comparative advantage is the object of study. Conditional structural gravity is also insufficient for welfare unless an income and production closure is added.
