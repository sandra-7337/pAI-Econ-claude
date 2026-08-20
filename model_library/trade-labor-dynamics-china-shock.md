# Trade and Labor Market Dynamics — China Trade Shock

## Model Family Name
Dynamic Multisector Spatial Trade with Labor Mobility and Input-Output Linkages

## Canonical Economic Question
What are the aggregate and local employment and welfare effects of a trade shock when workers reallocate gradually across regions and sectors connected by trade and production linkages?

## Verified References
- Caliendo, Lorenzo, Maximiliano Dvorkin, and Fernando Parro. 2019. “Trade and Labor Market Dynamics: General Equilibrium Analysis of the China Trade Shock.” *Econometrica* 87(3): 741-835. [DOI](https://doi.org/10.3982/ECTA13758).

## When to Use This Model
- Use it for dynamic general-equilibrium incidence across regional-sector labor markets.
- Use it when labor mobility, goods mobility, geography, and input-output linkages jointly matter.
- Use dynamic hat algebra when observed allocations and fundamental changes are available but fundamental levels are difficult to identify.

## Typical Primitives
- Countries, U.S. states or regions, sectors, and regional-sector labor markets.
- Workers with log utility, current employment location, migration costs, and extreme-value preference shocks.
- Sectoral Fréchet productivity, labor and structures, input-output shares, iceberg trade costs, and trade elasticities.
- Home production/nonemployment and a closure for rental income and trade imbalances.

## Timing
Each period, workers earn current income and consume; idiosyncratic mobility shocks arrive; workers choose next-period region-sector status based on continuation values; labor stocks update; the next static trade-production equilibrium clears.

## Information Structure
The baseline transition uses perfect foresight over fundamental paths. Counterfactual shocks can be learned after an anticipated baseline has been formed. Idiosyncratic mobility shocks are private.

## Agent Heterogeneity
Workers differ by current labor market and idiosyncratic tastes. Markets differ in sector, region, trade exposure, productivity, structures, and input-output position. Workers are otherwise homogeneous in the baseline.

## Choice Variables
- Workers choose next-period region, sector, or nonemployment.
- Competitive firms choose labor, structures, and intermediate inputs.
- Wages, rents, trade shares, expenditures, migration shares, and labor allocations are equilibrium outcomes.

## Constraints
- Labor evolves from gross migration flows.
- Structures are locally fixed in the baseline.
- Sectoral goods and input-output expenditure clear.
- Trade shares are consistent with delivered costs and Fréchet productivity.
- Worker values and migration probabilities must be mutually consistent.

## Equilibrium Concept or Solution Concept
A sequential competitive equilibrium built from a static multicountry-multisector trade equilibrium at each date and a forward-looking dynamic discrete-choice migration block. Dynamic and counterfactual hat algebra solve changes without recovering all fundamental levels.

## Key Equations
Sectoral trade shares have Eaton-Kortum form

\[
\pi_{ni,t}^j
=\frac{T_{i,t}^j(c_{i,t}^j\kappa_{ni,t}^j)^{-\theta_j}}
{\sum_hT_{h,t}^j(c_{h,t}^j\kappa_{nh,t}^j)^{-\theta_j}}.
\]

For origin labor market (a) and destination market (b), migration shares are

\[
\mu_{ab,t}
=\frac{\exp[(\beta V_{b,t+1}-\tau_{ab})/\nu]}
{\sum_c\exp[(\beta V_{c,t+1}-\tau_{ac})/\nu]}.
\]

Labor stocks evolve as

\[
L_{b,t+1}=\sum_a\mu_{ab,t}L_{a,t}.
\]

Sectoral unit costs combine wages, structure rents, and intermediate price indices according to observed cost shares.

## Main Mechanism
A foreign productivity or trade-cost shock changes import competition and intermediate-input prices. Regional-sector exposure differs because baseline trade and production structures differ. Forward-looking workers respond gradually because moving is costly, spreading adjustment and welfare effects over time and across connected markets.

## Common Propositions
- Dynamic hat algebra identifies equilibrium changes from initial trade, expenditure, migration, and employment allocations plus changes in fundamentals and elasticities.
- Input-output linkages transmit foreign shocks beyond directly exposed manufacturing sectors.
- Mobility frictions generate persistent and heterogeneous local employment and welfare responses.
- The published China-shock application attributes about 0.55 million U.S. manufacturing job losses during 2000-2007 to the shock while finding aggregate U.S. gains.

## Comparative Statics Usually Available
- Greater migration elasticity speeds reallocation and narrows persistent local welfare differences.
- Larger trade elasticity strengthens sourcing responses to productivity or cost changes.
- Larger intermediate-input shares amplify cross-sector transmission.
- Higher moving costs or stronger local fixed-factor exposure increase local persistence.

## Data Requirements
- Bilateral country-sector trade including domestic flows and sectoral input-output tables.
- Regional-sector employment, wages, structures or rents, and gross migration flows.
- Productivity or trade-cost changes used to construct the shock.
- Initial expenditure, trade shares, and nonemployment flows.

## Estimation or Calibration
Calibrate cost and expenditure shares from input-output data, trade elasticities from sectoral trade variation, and mobility elasticity from gross flows or external estimates. Construct the shock from model-consistent productivity/trade changes rather than mechanically treating import growth as exogenous.

## Counterfactual Analysis
Specify baseline and counterfactual fundamental paths; solve continuation values backward and employment, trade, and production forward; iterate until the terminal condition and all temporary equilibria are consistent. Report impact, transition, and long-run outcomes.

## Welfare Implications
Aggregate gains from cheaper goods and inputs can coexist with losses in exposed labor markets. Welfare includes the transition path and option value of future mobility; long-run real wages alone understate adjustment costs.

## Welfare Decomposition
Decompose welfare into consumption-price effects, wage and rent changes, migration costs, nonemployment/home production, input-output propagation, and terminal continuation value. Separate aggregate level effects from differential local exposure.

## Common Modeling Pitfalls
- Treating an observed import shock as exogenous productivity without an identification strategy.
- Omitting input-output linkages or nonemployment.
- Inferring aggregate employment or welfare from reduced-form cross-market differences.
- Comparing steady states and ignoring transition welfare.

## How to Extend the Model
- Social insurance, wage insurance, or disability programs.
- International migration, heterogeneous skills, labor supply, or firm dynamics.
- Endogenous supplier networks, capital accumulation, and policy uncertainty.

## Example Research Questions This Model Can Support
- How do tariff or productivity shocks affect employment across state-sector labor markets?
- How much do intermediate inputs offset direct import competition?
- Which mobility policies reduce transition losses without erasing aggregate gains?

## Closely Related Model Families
Caliendo-Parro; dynamic spatial general equilibrium; trade shocks; input-output production networks.

## When This Model Is Not Appropriate
Do not use it when only a reduced-form differential effect is required, firm-level sourcing is central, international worker mobility dominates, or the available data cannot identify gross migration and sectoral trade linkages.
