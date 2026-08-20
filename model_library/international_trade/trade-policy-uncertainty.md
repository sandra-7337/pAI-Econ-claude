# Trade-Policy Uncertainty

## Model Family Name
Irreversible Export Entry under Stochastic Trade Policy

## Canonical Economic Question
How does uncertainty about future tariff regimes affect irreversible export entry, prices, trade, and welfare even when the currently applied tariff does not change?

## Verified References
- Handley, Kyle, and Nuno Limão. 2017. “Policy Uncertainty, Trade, and Welfare: Theory and Evidence for China and the United States.” *American Economic Review* 107(9): 2731-2783. [DOI](https://doi.org/10.1257/aer.20141419).

## When to Use This Model
- Use it when firms pay sunk costs to enter an export market and future market access is uncertain.
- Use it when trade agreements reduce the probability or duration of a high-tariff regime.
- Use it to separate the effect of lower uncertainty from the effect of lower applied tariffs.

## Typical Primitives
- Heterogeneous foreign firms with productivity (a), CES import demand, and sunk export-entry cost (K).
- Current tariff (\tau_t) following a Markov process (\Lambda(\tau'\mid\tau)).
- Low/normal and high/threat tariff regimes, discount factor (\beta), death/exit probability, and fixed operating costs.
- Entry status is a state variable because the sunk cost is irreversible.

## Timing
1. The current tariff state is observed.
2. An inactive firm chooses whether to pay (K) and enter.
3. Active firms price and sell; profits are realized.
4. Firms may exit exogenously; the tariff transitions according to (\Lambda).
5. The sequence repeats.

## Information Structure
Firms know the tariff transition matrix but not future realizations. The agreement changes beliefs/transition probabilities. Productivity is known to the firm; aggregate price indices are rationally anticipated.

## Agent Heterogeneity
Firms differ in productivity and entry status. Products/sectors differ in the gap between the threat tariff and the applied tariff, creating heterogeneous uncertainty exposure.

## Choice Variables
- Inactive firms choose entry or waiting.
- Active firms choose export price and quantity under CES demand.
- In extensions, firms choose exit, product scope, or capacity.

## Constraints
- Entry requires the sunk cost (K).
- Operating profits depend on productivity, the tariff-inclusive price, and the importer price index.
- The value function must respect tariff transitions and firm death/exit.
- Free entry or a productivity cutoff aggregates firm decisions into import varieties and values.

## Equilibrium Concept or Solution Concept
A stationary recursive general equilibrium with firm entry cutoffs for each tariff state. Firm values solve Bellman equations; entry occurs when the value net of the sunk cost is nonnegative; import price indices and expenditure are consistent with the mass of active exporters.

## Key Equations
For an inactive firm of productivity (a), the option value satisfies

\[
V^0(a,\tau)=\max\left\{0,
-K+\pi(a,\tau)+\beta E_{\tau'\mid\tau}[V^1(a,\tau')]
\right\}.
\]

An active exporter satisfies

\[
V^1(a,\tau)=\pi(a,\tau)+\beta E_{\tau'\mid\tau}
[(1-\delta)V^1(a,\tau')],
\]

with modifications when exit is endogenous. The state-specific entry cutoff (a^*(\tau)) solves

\[
-K+\pi(a^*(\tau),\tau)+\beta E[V^1(a^*(\tau),\tau')]=0.
\]

Reducing the probability or expected duration of a high-tariff state raises the continuation value and lowers the productivity threshold required for entry.

## Main Mechanism
The sunk cost creates an option value of waiting. Even under a low current tariff, a credible future tariff threat reduces the expected payoff to entry. A trade agreement that binds the high tariff makes entry more attractive, expands imported varieties, lowers the import price index, and raises real income without requiring an immediate applied-tariff cut.

## Common Propositions
- Greater policy uncertainty or a more persistent high-tariff threat delays entry and reduces import variety.
- The effect is larger for products with a larger threat-versus-applied tariff gap.
- Reducing uncertainty lowers prices through entry and variety, not only through the intensive margin of incumbent firms.
- A deterministic permanent-tariff equivalent can summarize welfare gains only conditional on the model’s entry and demand structure.

## Comparative Statics Usually Available
- (K\uparrow) increases the option value of waiting and raises the entry cutoff.
- A higher probability or duration of the high-tariff state raises the cutoff.
- More patient firms respond more strongly to persistent future policy risk.
- A larger threat tariff increases uncertainty exposure and the entry response to a binding agreement.

## Data Requirements
- Applied and legally possible/threat tariffs by product over time.
- Export entry/exit, product-country trade values and unit values, firm productivity or size, and policy transition dates.
- Import expenditure and price indices for general-equilibrium estimation.

## Estimation or Calibration
Use cross-product variation in the threat gap and a policy event that changes its credibility. Estimate demand elasticity and the nonlinear export response jointly or import them from verified sources. Identify policy-state duration/transition parameters from institutional rules and historical regime persistence.

## Counterfactual Analysis
Change transition probabilities while holding current tariffs fixed; compare with an applied-tariff change. Simulate removal of bindings, temporary suspensions, or renewed threats. Report entry, import variety, prices, trade values, and welfare.

## Welfare Implications
Credible bindings can raise welfare by inducing entry and reducing the import price index. The benefit depends on sunk costs and persistence, and may differ from a tariff-cut welfare calculation because the current statutory rate can remain unchanged.

## Welfare Decomposition
Separate incumbent intensive-margin trade, new exporter/variety entry, option value, sunk entry resources, price-index effects, tariff revenue, and general-equilibrium expenditure/wage effects.

## Common Modeling Pitfalls
- Measuring uncertainty only by observed tariff volatility when the relevant object is the distribution of future regimes.
- Treating a tariff binding as an applied tariff cut.
- Ignoring selection because only sufficiently productive firms enter.
- Using a static gravity regression that cannot represent the option value of waiting.

## How to Extend the Model
- Multimarket and multiproduct entry.
- Supplier relationships, dynamic sourcing, and switching costs.
- Endogenous government credibility or political transitions.
- Learning about policy-state probabilities.

## Example Research Questions This Model Can Support
- How much export growth after accession reflects reduced tariff uncertainty rather than applied tariff cuts?
- Do temporary tariff exemptions stimulate entry if firms expect them to expire?
- How does uncertainty about trade-agreement renewal affect exporter participation?

## Closely Related Model Families
Dynamic export market entry; trade-policy shocks; supplier switching; heterogeneous firms and trade.

## When This Model Is Not Appropriate
Do not use it when entry is reversible and costless, future policy is known with certainty, or only contemporaneous intensive-margin pass-through is of interest.
