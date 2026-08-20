# Dynamic Spatial General Equilibrium (Kleinman-Liu-Redding)

## Model Family Name
Forward-Looking Capital Accumulation with Dynamic Migration and Spatial Trade

## Canonical Economic Question
How do gradual capital accumulation and costly forward-looking migration interact to determine regional transition paths, convergence speeds, and welfare after local shocks?

## Verified References
- Kleinman, Benny, Ernest Liu, and Stephen J. Redding. 2023. “Dynamic Spatial General Equilibrium.” *Econometrica* 91(2): 385-424. [DOI](https://doi.org/10.3982/ECTA20273).

## When to Use This Model
- Use it when regional capital and labor adjust jointly and gradually.
- Use it for transition paths after productivity, amenity, trade-cost, or migration-cost shocks.
- Use it when different spatial eigenmodes imply heterogeneous speeds or nonmonotonic convergence.

## Typical Primitives
- Locations (i), mobile workers, immobile landlords, local capital (k_{it}), and population (l_{it}).
- Local productivity (z_{it}), amenities (b_{it}), trade costs (τ_{ni,t}), and migration costs (κ_{in,t}).
- Cobb-Douglas production with labor share (μ), CES/Armington trade elasticity, depreciation (δ), and discounting.
- Idiosyncratic extreme-value location preferences in the migration block.

## Timing
Each period, fundamentals are realized; firms produce and goods trade; workers consume wages and choose next-period locations; landlords consume and invest in next-period local capital; population and capital states update.

## Information Structure
The deterministic baseline uses perfect foresight over the counterfactual path. Workers receive idiosyncratic location shocks; stochastic fundamentals can be added under rational expectations.

## Agent Heterogeneity
Locations differ in fundamentals and states. Workers differ by current location and idiosyncratic mobility tastes. Landlords are immobile and own location-specific capital.

## Choice Variables
- Workers choose next-period location.
- Landlords choose consumption and investment.
- Firms choose static labor and capital demand.
- Wages, rental rates, trade shares, migration shares, population, and capital are equilibrium outcomes.

## Constraints
- Location-specific capital evolves through investment and depreciation.
- Population flows follow migration choices and aggregate labor is fixed.
- Goods, labor, and capital markets clear in every period.
- Intertemporal choices satisfy value-function and Euler conditions plus terminal or transversality conditions.

## Equilibrium Concept or Solution Concept
A sequential competitive equilibrium and associated steady state. Nonlinear dynamic exact-hat algebra solves perfect-foresight transitions; linearization around steady state permits spectral characterization of adjustment modes.

## Key Equations
Production in location (i) is

\[
y_{it}=z_{it}
\left(\frac{l_{it}}{\mu}\right)^\mu
\left(\frac{k_{it}}{1-\mu}\right)^{1-\mu}.
\]

With unit cost (c_{it}), Armington trade shares take the form

\[
\pi_{ni,t}
=\frac{(c_{it}\tau_{ni,t})^{1-\sigma}}
{\sum_j(c_{jt}\tau_{nj,t})^{1-\sigma}}.
\]

Migration shares under extreme-value tastes have logit form

\[
m_{in,t}
=\frac{\exp[(\beta V_{n,t+1}-\kappa_{in,t})/\nu]}
{\sum_j\exp[(\beta V_{j,t+1}-\kappa_{ij,t})/\nu]}.
\]

State laws include

\[
l_{n,t+1}=\sum_i m_{in,t}l_{it},
\qquad
k_{i,t+1}=(1-\delta)k_{it}+I_{it}.
\]

## Main Mechanism
Workers and capital are complementary, but both adjust slowly for different reasons. Migration responds to expected future real wages and amenities; investment responds to expected returns. Their interaction produces multiple spatial adjustment modes with different speeds and can generate persistent or nonmonotonic regional responses.

## Common Propositions
- A steady-state spatial equilibrium can be characterized under constant fundamentals.
- Dynamic exact hats incorporate investment without recovering all fundamental levels.
- Linearized transition dynamics decompose into eigencomponents with heterogeneous convergence rates.
- A shock’s persistence depends on its projection onto slow and fast spatial modes, not on one universal convergence coefficient.

## Comparative Statics Usually Available
- Higher migration costs slow labor reallocation.
- Lower depreciation or stronger capital persistence slows capital adjustment.
- Stronger trade integration changes the spatial transmission of local shocks.
- Capital-labor complementarity can amplify persistence and produce overshooting.

## Data Requirements
- Regional capital stocks, population, wages/income, and output over time.
- Bilateral trade and migration flows.
- Investment, depreciation, trade costs, amenities, and productivity shifters or their changes.

## Estimation or Calibration
Use trade shares to discipline trade elasticity and migration flows to discipline mobility elasticity and costs; match capital and population dynamics. The published application uses U.S. state data from 1965-2015. Exact hats reduce the need to identify fundamental levels but not elasticities or initial states.

## Counterfactual Analysis
Specify paths for productivity, amenities, trade, or migration costs; impose a terminal steady state or long horizon; solve backward-looking values and forward state laws; verify goods and factor clearing at every date. Compare nonlinear and linearized solutions for large shocks.

## Welfare Implications
Welfare depends on the full discounted transition, not only the destination steady state. Mobile workers and immobile landlords can experience different welfare effects, and slow adjustment can make a favorable long-run shock costly for some cohorts or locations.

## Welfare Decomposition
Decompose discounted welfare into wage/rental income, price indices, amenities, moving costs, investment/consumption timing, and terminal value. A steady-state welfare comparison omits transition costs.

## Common Modeling Pitfalls
- Treating capital or labor as adjusting instantaneously.
- Summarizing convergence with one scalar rate.
- Omitting terminal conditions or failing to test horizon sensitivity.
- Using static exact hats for a transition-path question.

## How to Extend the Model
- Agglomeration, housing, multiple sectors, and input-output linkages.
- Cross-location capital ownership or financial frictions.
- Stochastic fundamentals, heterogeneous workers, and labor-force participation.

## Example Research Questions This Model Can Support
- Why do regional productivity shocks have persistent and heterogeneous effects?
- How does infrastructure affect the joint transition of capital and population?
- Which spatial eigenmodes account for slower income convergence?

## Closely Related Model Families
Static spatial trade; trade-labor dynamics; quantitative trade counterfactuals; dynamic migration.

## When This Model Is Not Appropriate
Do not use it when capital is fully mobile, migration is irrelevant, firm-level decisions dominate, or only a static long-run comparison is needed.
