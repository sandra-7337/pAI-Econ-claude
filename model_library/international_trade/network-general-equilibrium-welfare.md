# Network General Equilibrium and Welfare Decomposition

## Model Family Name
Nonlinear Multisector General Equilibrium with Production Networks and Wedges

## Canonical Economic Question
How can aggregate output and welfare responses to productivity, trade-cost, and wedge shocks be expressed using microeconomic shares, substitution elasticities, and network statistics beyond first-order Hulten accounting?

## Verified References
- Baqaee, David Rezza, and Emmanuel Farhi. 2019. “The Macroeconomic Impact of Microeconomic Shocks: Beyond Hulten’s Theorem.” *Econometrica* 87(4): 1155-1203. [DOI](https://doi.org/10.3982/ECTA15202).
- Baqaee, David Rezza, and Emmanuel Farhi. 2024. “Networks, Barriers, and Trade.” *Econometrica* 92(2): 505-541. [DOI](https://doi.org/10.3982/ECTA17513).

## When to Use This Model
- Use it for large or nonlinear shocks in disaggregated production/trade networks.
- Use it when markups, tariffs, taxes, nominal rigidities, or other wedges break first-best aggregation.
- Use it to decompose welfare and GDP changes using observed shares plus substitution elasticities.

## Typical Primitives
- Producers, factors, households, and possibly countries connected by an input-output network.
- General constant-returns production functions and homothetic household demand.
- Productivity (A_i), wedges (\mu_i), input expenditure shares (\Omega_{ij}), Domar weights (\lambda_i), and factor-income shares.
- Structural substitution elasticities and returns to scale.
- In trade applications, iceberg costs/tariffs and country-sector bilateral expenditure shares.

## Timing
Static comparative equilibrium. Shocks to productivity, wedges, or trade barriers occur; firms and households reoptimize; prices, shares, factor allocation, trade, output, and welfare clear jointly.

## Information Structure
Complete information and price taking in the baseline. Wedges are primitives or policy variables rather than private information.

## Agent Heterogeneity
Producers differ in network position, Domar weight, technology, markups/wedges, and substitution patterns. Factors and households may be heterogeneous in extensions, but the canonical formulas require explicit welfare weights.

## Choice Variables
- Firms choose factor and intermediate demands.
- Households choose consumption and factor supply where relevant.
- Governments may choose tariffs or taxes in policy exercises.
- Prices, trade shares, Domar weights, and the input-output matrix are endogenous outside Cobb-Douglas special cases.

## Constraints
- Producer cost minimization and zero-profit or markup pricing conditions.
- Household budgets and market clearing for all goods and factors.
- Trade balance or specified transfers/deficits.
- Wedge accounting must distinguish real resource costs from tax or tariff transfers.

## Equilibrium Concept or Solution Concept
A competitive or wedge-distorted general equilibrium. Local responses are characterized by implicit differentiation around an observed equilibrium; exact counterfactuals solve the full nonlinear equilibrium in changes. The approximation order must be stated explicitly.

## Key Equations
The input-output matrix and Leontief inverse are

\[
\Omega_{ij}=\frac{p_jx_{ij}}{p_i y_i},
\qquad
\Psi=(I-\Omega)^{-1},
\qquad
\lambda_i=\frac{p_i y_i}{GDP}.
\]

At an efficient point, Hulten’s first-order formula is

\[
d\log Y=\sum_i\lambda_i\,d\log A_i.
\]

For finite shocks, a second-order approximation takes the form

\[
\Delta\log Y
\approx
\boldsymbol\lambda^\top\Delta\log\mathbf A
+\frac12(\Delta\log\mathbf A)^\top
\mathcal H_Y
(\Delta\log\mathbf A),
\]

where (\mathcal H_Y) is constructed from network exposures, structural substitution elasticities, factor reallocation, and returns to scale. With wedges, welfare generally differs from real GDP:

\[
d\log W=d\log Y-\text{wedge-weighted reallocation and transfer terms}.
\]

## Main Mechanism
The first-order effect of a micro productivity shock is its Domar weight. For large shocks, prices and expenditure shares move; whether inputs are general-equilibrium complements or substitutes determines amplification and asymmetry. Initial wedges create first-order welfare effects from reallocations, so GDP, TFP, and welfare need not move together.

## Common Propositions
- Hulten’s theorem is the exact first derivative at an efficient benchmark, not a complete large-shock formula.
- Network nonlinearities can amplify negative shocks and attenuate positive shocks under complementarity.
- Structural micro elasticities map into reduced-form general-equilibrium elasticities through the network.
- In distorted trade networks, the same micro sufficient statistics characterize local welfare losses and can support approximate or exact counterfactuals.
- Disaggregation matters most when wedges, substitution patterns, and network centrality are heterogeneous.

## Comparative Statics Usually Available
- Lower substitution elasticities strengthen bottleneck/complementarity amplification.
- Larger Domar weights increase first-order macro influence.
- More severe initial wedges increase first-order welfare consequences of reallocation.
- Greater factor immobility can amplify adverse shocks by limiting substitution and reallocation.

## Data Requirements
- Detailed input-output or world input-output tables; gross output, value added, factor payments, and final demand.
- Producer/country-sector productivity and wedge measures.
- Structural substitution elasticities, returns to scale, trade elasticities, tariffs, and bilateral trade shares.
- A social-welfare specification and transfer treatment when households are heterogeneous.

## Estimation or Calibration
Calibrate shares directly from a benchmark social accounting matrix. Estimate substitution elasticities from relative price and expenditure-share responses or import-demand variation. Recover wedges from markups, taxes, tariffs, or first-order conditions. Validate local derivatives against finite counterfactual solutions.

## Counterfactual Analysis
For small shocks, use first- or second-order formulas and report approximation order. For large shocks, solve the nonlinear equilibrium in exact changes and compare it with linear and quadratic approximations. Decompose results by shocked node, propagation path, substitution, factor reallocation, and wedge interaction.

## Welfare Implications
Real GDP is not generally welfare in the presence of tariffs, markups, transfers, or heterogeneous households. Removing a barrier can raise measured productivity while causing adverse terms-of-trade or distributional effects. Network detail can materially change losses from trade barriers.

## Welfare Decomposition
At minimum report: direct technology/endowment effects; terms of trade; tariff/tax revenue transfers; markup or wedge reallocation; network propagation; nonlinear substitution; factor reallocation; and, where relevant, household distribution. State the numeraire and welfare weights.

## Common Modeling Pitfalls
- Calling a first-order Hulten calculation a large-shock counterfactual.
- Using final expenditure shares where Domar sales weights are required.
- Treating tariff revenue as destroyed resources.
- Comparing GDP and welfare without specifying transfers, ownership, and terms of trade.
- Feeding a noisy or inconsistent social accounting matrix into a nonlinear solver without balancing it.

## How to Extend the Model
- Heterogeneous households and distributional welfare.
- Endogenous network formation, firm entry, markups, or capacity constraints.
- Dynamic adjustment, inventories, and capital accumulation.
- Optimal trade or industrial policy using sufficient-statistics derivatives.

## Example Research Questions This Model Can Support
- How much does a semiconductor shock reduce welfare once nonlinear substitution and bottlenecks are included?
- Which tariff reductions yield the largest welfare gain in a distorted global production network?
- When does sectoral aggregation conceal important welfare losses from trade barriers?

## Closely Related Model Families
Fixed input-output production networks; ACR welfare statistics; Caliendo-Parro trade; quantitative exact-hat counterfactuals; endogenous network formation.

## When This Model Is Not Appropriate
Do not use this toolbox without the micro shares and elasticities needed to discipline it. A simpler ACR or fixed-network formula is preferable when the maintained assumptions make higher-order reallocation and wedges quantitatively irrelevant.
