# Buyer-Supplier Search and Matching

## Model Family Name
Geographic Supplier Search with Heterogeneous Firms and Outsourced Tasks

## Canonical Economic Question
How do firm productivity, geographic search costs, and the distribution of supplier efficiency determine the number and quality of buyer-supplier links and the effect of better connectivity on firm performance?

## Verified References
- Bernard, Andrew B., Andreas Moxnes, and Yukiko U. Saito. 2019. “Production Networks, Geography, and Firm Performance.” *Journal of Political Economy* 127(2): 639-688. [DOI](https://doi.org/10.1086/700764).

## When to Use This Model
- Use it when buyers search across locations for suppliers of outsourced tasks.
- Use it when travel or information costs affect link formation separately from freight costs.
- Use it to connect firm productivity to search radius, number of suppliers, marginal cost, and performance.

## Typical Primitives
- Monopolistically competitive downstream firms with productivity (z) and CES final demand elasticity (\sigma>1).
- A continuum of tasks that can be performed in-house or sourced from upstream firms.
- Potential supplier efficiency with Pareto-type tails governed by (\theta).
- Geographic/communication cost (\tau), distribution (g(\tau,j)), and fixed search cost (f(j)) for market (j).
- Search cutoff (\bar\tau(z,j)), supplier count (n(z,j)), and supplier-efficiency aggregate (\Phi(z,j)).

## Timing
1. A downstream firm observes its productivity and market opportunities.
2. It chooses the set/radius of locations in which to search and pays fixed search costs.
3. Supplier efficiencies are drawn or discovered for tasks.
4. The buyer sources each task from the lowest delivered-cost option or produces it in-house.
5. The firm prices its final variety and produces under monopolistic competition.

## Information Structure
Firms know distributions and search costs before searching but do not know all match efficiencies ex ante. Discovered supplier productivity is observed when sourcing choices are made.

## Agent Heterogeneity
Downstream firms differ in productivity and location. Potential suppliers differ in task efficiency and location. Markets differ in search cost and geographic friction.

## Choice Variables
- Search cutoff/radius (\bar\tau(z,j)) or the set of sourcing markets.
- Supplier choice task by task after search.
- Final price, output, labor, and outsourced input demand.

## Constraints
- Search incurs (wf(j)) per market or search unit.
- A task is outsourced only when the discovered delivered supplier cost beats the in-house option.
- CES demand and constant-markup pricing determine operating profits.
- Search choices must maximize operating profit net of search cost.

## Equilibrium Concept or Solution Concept
A monopolistic-competition equilibrium with optimal costly supplier search. Firms take aggregate wages and price indices as given, choose search cutoffs, form supplier links from discovered matches, and set constant-markup prices. General-equilibrium versions additionally impose free entry and market clearing.

## Key Equations
The efficiency contribution of searched markets and the expected number of suppliers are

\[
\Phi(z,j)=T_0+\int_1^{\bar\tau(z,j)}T\tau^{-\theta}g(\tau,j)d\tau,
\qquad
n(z,j)=\int_1^{\bar\tau(z,j)}g(\tau,j)d\tau.
\]

The optimal search cutoff in the paper’s Appendix A can be written

\[
\bar\tau(z,j)=\kappa_1
\left(\frac{TA}{w^{\sigma}f(j)}\right)^{1/\theta}
\Phi(z,j)^{-k/\theta}z^{(\sigma-1)/\theta},
\]

where (A) is the final-demand shifter and (k) is a composite of demand, production, and supplier-tail parameters. At the margin,

\[
\frac{\theta}{(\sigma-1)(1-\alpha)}\,wf(j)
\]

equals the appropriately scaled gross-profit contribution of the marginal searched market.

## Main Mechanism
More productive downstream firms earn more from any marginal cost reduction, so they search farther and pay to discover more suppliers. A larger supplier set increases the chance of a high-efficiency match, lowers the buyer’s marginal cost, and raises sales and productivity. Lower passenger-travel or information costs expand search even if freight costs are unchanged.

## Common Propositions
- The search cutoff and supplier count rise with downstream productivity.
- Higher search cost lowers the cutoff, supplier count, and sourcing-efficiency index.
- Better geographic connectivity creates links and improves buyer performance, especially in input-intensive sectors.
- More productive buyers can match with more distant or otherwise costly suppliers because their return to search is larger.

## Comparative Statics Usually Available
- (z\uparrow\Rightarrow\bar\tau\uparrow,n\uparrow,\Phi\uparrow).
- (f(j)\uparrow\Rightarrow\bar\tau\downarrow,n\downarrow,\Phi\downarrow).
- A thicker supplier-productivity tail raises the option value of search.
- Greater input intensity raises performance gains from improved supplier access.

## Data Requirements
- Matched buyer-supplier links, firm sales, employment, productivity proxies, industry input intensity, and locations.
- Travel/communication infrastructure and freight-time or shipping-cost measures.
- Link creation/destruction over time and market-level counts of potential suppliers.

## Estimation or Calibration
Estimate link gravity and the productivity/search relationship using firm-link panels. Identify search-cost changes with infrastructure that changes face-to-face access without directly changing freight costs. Calibrate (\sigma,\theta,\alpha), fixed search costs, and the supplier distribution to firm sales and degree moments.

## Counterfactual Analysis
Change travel times, fixed search costs, supplier productivity distributions, or market access; recompute search cutoffs, link sets, marginal costs, and firm performance. General-equilibrium exercises should allow entry, wages, and price indices to adjust.

## Welfare Implications
Lower search frictions improve match quality and lower production costs but consume search resources and may alter entry. Private firms may not internalize how link formation affects suppliers, competing buyers, infrastructure congestion, or aggregate variety.

## Welfare Decomposition
Decompose gains into lower buyer marginal costs from better matches, expanded final-good variety/entry, search-resource costs, and general-equilibrium wage and price-index effects. Not applicable as a single closed-form sufficient statistic in the baseline empirical application.

## Common Modeling Pitfalls
- Treating passenger travel time as an iceberg freight cost rather than a search/information cost.
- Counting observed links without accounting for missing links outside the data universe.
- Confusing greater measured revenue productivity with a pure technical-efficiency gain.
- Holding the supplier set fixed after changing search costs.

## How to Extend the Model
- Cross-border suppliers, tariffs, and customs frictions.
- Dynamic search, relationship capital, switching costs, and incumbent renegotiation.
- Multiproduct buyers and suppliers or capacity constraints.
- Two-sided search effort and matching congestion.

## Example Research Questions This Model Can Support
- Does high-speed passenger transport improve firms by facilitating supplier discovery rather than shipping?
- Why do more productive firms have more suppliers and source from farther away?
- How does digital supplier discovery affect firm productivity and geographic concentration?

## Closely Related Model Families
Arkolakis-Huneeus-Miyauchi two-sided link formation; Grossman-Helpman outsourcing; Chaney trade networks; supplier switching and reconfiguration.

## When This Model Is Not Appropriate
Do not use it when links are assigned administratively, supplier reliability rather than discovery is the main friction, repeated relational enforcement is central, or all relevant suppliers and their prices are already observed costlessly.
