# Antràs-Chor Global Value Chains

## Model Family Name
Sequential Production, Incomplete Contracts, and Endogenous Firm Boundaries

## Canonical Economic Question
How should a final-good producer allocate integration and outsourcing across upstream and downstream production stages when supplier investments are noncontractible and technologically sequential?

## Verified References
- Antràs, Pol, and Davin Chor. 2013. “Organizing the Global Value Chain.” *Econometrica* 81(6): 2127-2204. [DOI](https://doi.org/10.3982/ECTA10813).

## When to Use This Model
- Use it when the position of an input along a production chain changes the optimal ownership decision.
- Use it to connect downstreamness, demand elasticity, input substitutability, and intrafirm trade.
- Use it when sequential relationship-specific investment is more important than country-level comparative advantage.

## Typical Primitives
- A final-good firm with productivity (\theta) and a continuum of ordered stages (m\in[0,1]).
- Stage-specific suppliers choosing noncontractible investment (x(m)) at marginal cost (c).
- Production parameter (\alpha\in(0,1)), demand parameter (\rho\in(0,1)), and demand shifter (A).
- Final-firm bargaining shares (\beta_V>\beta_O) under integration and outsourcing.

## Timing
The firm posts an ownership mode for every stage and selects suppliers; production proceeds sequentially; at stage (m), the supplier observes the value completed so far, invests, and bargains over its incremental contribution; final output is sold after the last stage.

## Information Structure
The sequence and current unfinished-product value are observed by the contracting parties. Stage investment is relationship specific and cannot be fully contracted ex ante. Bargaining rules are common knowledge.

## Agent Heterogeneity
Stages differ by position along the chain and may differ in contractibility or cost in extensions. Firms may differ in productivity. Organizational heterogeneity is endogenous: some stages are integrated and others outsourced.

## Choice Variables
- The final firm chooses (\beta(m)\in\{\beta_O,\beta_V\}) through the ownership mode at each stage.
- Each supplier chooses investment (x(m)).
- The cutoff stage between integration and outsourcing is an equilibrium outcome.

## Constraints
- Stages must be completed in technological order.
- Suppliers’ investments are noncontractible and have zero outside value in the baseline.
- Integration raises the final firm’s surplus share but lowers the supplier’s share and investment incentive.
- Organizational choices maximize final-firm profit, not joint surplus.

## Equilibrium Concept or Solution Concept
A subgame-perfect equilibrium solved backward through sequential supplier investment and bargaining. The final firm chooses the piecewise ownership schedule that maximizes its payoff; the solution has a cutoff organizational structure.

## Key Equations
If (r(m)) is revenue secured through stage (m), supplier (m)'s incremental contribution is

\[
r'(m)=\frac{\rho}{\alpha}A^{(1-\rho)\alpha/\rho}
r(m)^{(\rho-\alpha)/\rho}x(m)^{\alpha}.
\]

Supplier investment satisfies

\[
x(m)=\left[\frac{(1-\beta(m))\rho A^{(1-\rho)\alpha/\rho}}{c}\right]^{1/(1-\alpha)}
r(m)^{(\rho-\alpha)/(\rho(1-\alpha))}.
\]

In the relaxed problem, the optimal surplus share is

\[
\beta^*(m)=1-\alpha m^{(\alpha-\rho)/\alpha}.
\]

## Main Mechanism
Ownership trades off rent extraction against supplier investment incentives. When (\rho>\alpha), supplier investments are sequential complements: weak upstream investment depresses all downstream returns, favoring upstream outsourcing and downstream integration. When (\rho<\alpha), investments are sequential substitutes and the ordering reverses.

## Common Propositions
- If (\rho>\alpha), there is a cutoff with upstream stages outsourced and downstream stages integrated.
- If (\rho<\alpha), upstream stages are integrated and downstream stages outsourced.
- Lower (\rho), meaning greater market power, expands the range of integrated stages when both modes coexist.
- The optimal ownership set for a common mode is a connected interval in the benchmark.

## Comparative Statics Usually Available
- A change in demand elasticity relative to input substitutability reverses the relationship between downstreamness and integration.
- A larger gap between (\beta_V) and (\beta_O) changes the cutoff by strengthening both rent extraction and incentive distortions.
- Higher supplier investment cost lowers stage investment; productivity and demand shifters scale the value chain.

## Data Requirements
- Related-party and arm’s-length imports by industry and source.
- Input-output tables to construct upstreamness/downstreamness measures.
- Import-demand elasticities and industry contractibility or relationship-specificity measures.
- Firm or industry controls for productivity and input composition.

## Estimation or Calibration
Test the interaction between downstreamness and demand elasticity in intrafirm import shares. Structural calibration requires (\alpha,\rho,\beta_V,\beta_O,c) and a mapping from observed related-party trade to ownership. Input-output downstreamness must be constructed with a stated orientation.

## Counterfactual Analysis
Change bargaining institutions, demand elasticity, stage costs, or the feasible ownership modes; recompute supplier investments, the ownership cutoff, revenue, and profits. A trade counterfactual requires an added geographic and price-system block.

## Welfare Implications
Private ownership choices balance the final firm’s rent extraction against investment incentives but need not maximize total surplus. Incomplete contracting causes underinvestment, and changing the boundary can shift distortion across stages.

## Welfare Decomposition
Separate supplier investment distortions by stage, final-firm rent capture, organizational costs if added, and consumer surplus. Not applicable as a complete aggregate trade-welfare decomposition in the baseline because country income and trade balance are not closed.

## Common Modeling Pitfalls
- Reversing the stage index or the definition of downstreamness.
- Calling all technological inputs complements; the relevant sequential complement/substitute condition includes the demand curvature (\rho-\alpha).
- Interpreting related-party imports as an error-free measure of integration.
- Using the model for geographic stage location without adding location choices and trade costs.

## How to Extend the Model
- Stage-specific costs, contractibility, bargaining, and supplier asymmetry.
- Multiple countries and endogenous geographic placement of stages.
- Dynamic relationship capital, disruptions, or supplier replacement.

## Example Research Questions This Model Can Support
- Why is intrafirm trade more downstream in some industries but more upstream in others?
- How does demand elasticity change the optimal boundary of a global firm?
- Which stages should integrate after contracting institutions improve?

## Closely Related Model Families
Antràs-Helpman global sourcing; Grossman-Helpman outsourcing; global value-chain geography; relationship-specific investment.

## When This Model Is Not Appropriate
Do not use the baseline to locate production stages across countries, estimate aggregate tariff welfare, or model supplier discovery. Those questions require geographic sourcing, general-equilibrium trade, or search blocks beyond the sequential ownership mechanism.
