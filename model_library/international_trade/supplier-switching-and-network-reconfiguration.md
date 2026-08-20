# Supplier Switching and Network Reconfiguration

## Model Family Name
Search, Renegotiation, and Supplier Replacement after Trade-Cost Shocks

## Canonical Economic Question
When an unanticipated tariff or supply shock raises the cost of incumbent inputs, when do firms renegotiate, retain, or replace suppliers, and how do sunk search costs shape the transition and welfare incidence?

## Verified References
- Grossman, Gene M., Elhanan Helpman, and Stephen J. Redding. 2024. “When Tariffs Disrupt Global Supply Chains.” *American Economic Review* 114(4): 988-1029. [DOI](https://doi.org/10.1257/aer.20211519).

## When to Use This Model
- Use it for unanticipated policy shocks that hit relationships formed under a different regime.
- Use it when incumbent renegotiation and costly replacement search are distinct adjustment margins.
- Use it when supply-chain transition costs, not only new steady states, matter for welfare.

## Typical Primitives
- Differentiated final-good producers, homogeneous labor good, and a continuum of required intermediate tasks.
- Incumbent domestic or foreign suppliers discovered through sunk search before the shock.
- Match productivity (a), reservation cutoff (\bar a), search effort/cost, fixed entry and operating costs.
- An input tariff (\tau), bargaining weights, final-demand elasticity, and supplier-productivity distribution.
- State variables after the shock: incumbent supplier identities and match productivities.

## Timing
1. Before the shock, firms enter, search, form supply chains, and bargain under anticipated free trade.
2. The government unexpectedly imposes an input tariff.
3. Incumbent buyer-supplier pairs may renegotiate their terms.
4. Buyers decide whether to retain incumbents or incur new search costs for replacements.
5. Entry, pricing, production, and market clearing adjust to the new regime.

## Information Structure
Pre-shock firms know the stationary environment but do not anticipate the tariff. After the tariff is revealed, its rate is common knowledge. Match productivity is observed within an established relationship; potential replacement quality is uncertain before search.

## Agent Heterogeneity
Final producers differ through their match draws and incumbent sourcing patterns. Suppliers differ in location and match productivity. Relationships differ in whether the tariff makes the existing match viable after renegotiation.

## Choice Variables
- Search intensity and reservation productivity for new suppliers.
- Retention, renegotiation, or replacement of each incumbent relationship.
- Intermediate input quantities, final prices and output, and entry/exit.

## Constraints
- A searched match is accepted only when its productivity exceeds the reservation cutoff.
- Sunk search costs cannot be recovered after the shock.
- Bargained input terms must give both parties at least their post-shock outside options.
- Free entry equates expected operating profits with entry and search costs when entry is active.

## Equilibrium Concept or Solution Concept
A pre-shock free-entry monopolistic-competition equilibrium with endogenous search and bilateral bargaining, followed by a post-shock equilibrium conditional on inherited matches. The post-shock solution combines renegotiation of viable incumbents, optimal replacement search, entry, and goods/labor market clearing.

## Key Equations
Let (G(a)) denote the match-productivity distribution and (\bar a) the reservation cutoff. The success probability of a search is

\[
1-G(\bar a),
\]

and optimal search equates its marginal expected match surplus with its marginal cost:

\[
C'(s)=\frac{\partial}{\partial s}
E[\text{post-search relationship surplus}\mid \bar a,\tau].
\]

An incumbent is retained if its joint surplus after the tariff and renegotiation is at least the option value of replacement:

\[
S^{inc}(a,\tau)\geq -C(s)+E[S^{new}(a',\tau)\mathbf 1\{a'\geq\bar a\}].
\]

The free-entry condition has the generic form

\[
E[\pi^{operating}]=f_e+E[\text{sunk search cost}],
\]

with expectations evaluated using equilibrium supplier choices.

## Main Mechanism
Existing matches embody sunk search effort and match-specific surplus. A small tariff may be absorbed through renegotiation without new search. A larger tariff can destroy foreign-match surplus and trigger domestic replacement search, supplier switching, and entry. Consequently, sourcing and welfare responses are nonlinear in the tariff and depend on inherited network state.

## Common Propositions
- There can be an inaction region in which a small tariff changes negotiated payments but not supplier identities.
- Larger tariffs can induce discontinuous replacement search and network reconfiguration.
- The same tariff can have different effects on incumbents and new entrants because only incumbents inherit sunk relationships.
- Welfare losses include search and destroyed relationship capital in addition to conventional tariff and price-index effects.

## Comparative Statics Usually Available
- Higher tariffs weakly reduce the surplus of imported incumbent matches and increase replacement incentives.
- Higher sunk search costs widen the retention/inaction region and slow reconfiguration.
- A thicker upper tail of match productivity raises the option value of new search.
- Stronger incumbent bargaining power changes tariff incidence within retained relationships and may shift replacement thresholds.

## Data Requirements
- Matched importer-supplier panels before and after a tariff or disruption.
- Relationship age, supplier switching, search expenditures or proxies, input prices, quantities, tariffs, and firm entry/exit.
- Initial import shares and empirical sourcing responses for calibration.

## Estimation or Calibration
Calibrate demand and match-productivity elasticities, fixed entry/operating costs, and search costs to initial sourcing shares, firm counts, and link turnover. Identify switching responses using unexpected tariff variation across products and origins. Relationship-level price changes help identify bargaining/pass-through separately from switching.

## Counterfactual Analysis
Condition on the inherited pre-shock network, change the tariff or disruption, and solve renegotiation, replacement search, entry, prices, and welfare. Compare with a counterfactual that incorrectly lets firms choose the entire network afresh to quantify transition/sunk-cost effects.

## Welfare Implications
Tariffs impose conventional consumption and production distortions plus costs from destroyed matches, renewed search, and delayed access to good suppliers. Tariff revenue is a domestic transfer, but search resources and lost match productivity are real losses.

## Welfare Decomposition
Separate: consumer-price effects; tariff revenue; producer and supplier surplus; incumbent renegotiation; supplier-replacement/search costs; entry/variety changes; and the loss of match-specific productivity. The decomposition must distinguish transfers from real resource costs.

## Common Modeling Pitfalls
- Solving only the new steady state and discarding inherited supplier relationships.
- Treating every observed switch as tariff-induced rather than accounting for normal link turnover.
- Confusing renegotiated supplier prices with complete tariff pass-through.
- Assuming switching is frictionless while also claiming supply-chain persistence.

## How to Extend the Model
- Multiple tiers, inventories, capacity constraints, and disruption duration.
- Endogenous ex-ante diversification or resilience investment.
- Relationship capital and incomplete contracts.
- Dynamic learning about supplier quality and repeated policy uncertainty.

## Example Research Questions This Model Can Support
- At what tariff rate do importers replace Chinese suppliers rather than renegotiate?
- How much of a tariff’s welfare cost comes from renewed search and destroyed matches?
- Do sunk relationships delay friend-shoring after a geopolitical shock?

## Closely Related Model Families
Trade-policy uncertainty; buyer-supplier search; relational trade; global sourcing; supply-chain resilience.

## When This Model Is Not Appropriate
Do not use it for fully anticipated permanent policy changes before relationships form, frictionless spot sourcing, or shocks that affect quantities without changing relationship surplus or supplier availability.
