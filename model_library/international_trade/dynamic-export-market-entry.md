# Dynamic Export Market Entry

## Model Family Name
Dynamic Heterogeneous Exporters with Sunk Market-Entry Costs

## Canonical Economic Question
How do sunk entry costs, prior export status, heterogeneous profits, and expectations about future exchange rates or demand generate persistent export participation and delayed responses to trade shocks?

## Verified References
- Das, Sanghamitra, Mark J. Roberts, and James R. Tybout. 2007. “Market Entry Costs, Producer Heterogeneity, and Export Dynamics.” *Econometrica* 75(3): 837-873. [DOI](https://doi.org/10.1111/j.1468-0262.2007.00769.x).

## When to Use This Model
- Use it when export status is persistent because entering is more costly than continuing.
- Use it for policies or exchange-rate processes whose effects depend on expectations and prior exporting experience.
- Use it when plant-level export quantities and participation must be modeled jointly.

## Typical Primitives
- Plants (i), time (t), export status (e_{i,t-1}), productivity or cost heterogeneity, and export-demand shifters.
- Exchange rate, foreign demand, domestic production costs, and stochastic transition laws.
- Sunk entry cost for nonexporters, continuation or fixed exporting cost for incumbents, and discount factor (β).
- Static export-profit function conditional on export quantity.

## Timing
At the start of a period, a plant observes its state and current shocks; it decides whether to export and, conditional on exporting, how much; profits are realized; aggregate shocks and plant states evolve.

## Information Structure
Plants observe current state variables and know their transition processes but not future realizations. Plant heterogeneity may contain persistent observed and unobserved components.

## Agent Heterogeneity
Plants differ in export profitability, production cost, demand, and export history. Industries may differ in sunk costs and profit functions. Aggregate exchange-rate and foreign-demand shocks are common.

## Choice Variables
- Binary export participation (e_{it}).
- Export quantity or revenue conditional on participation.
- In extensions, destination entry, exit, investment, or learning.

## Constraints
- New exporters pay the sunk entry cost; incumbents do not repay it unless the model specifies re-entry depreciation.
- Export quantities satisfy the plant’s static profit maximization.
- State transitions and expectations must be consistent with the estimated stochastic process.
- The dynamic value function must respect the observed initial-condition treatment.

## Equilibrium Concept or Solution Concept
A dynamic discrete-continuous decision problem for each plant, usually estimated in partial equilibrium. The value function determines export participation; the conditional profit problem determines export supply. Aggregate exports integrate choices over the plant distribution.

## Key Equations
Let (s_{it}) collect current profitability states and let (F_E) be the sunk cost. A reduced-form Bellman equation is

\[
V(s_{it},e_{i,t-1})=
\max_{e_{it}\in\{0,1\},\,q^x_{it}\geq0}
\left\{\pi^d_{it}
+e_{it}\left[\pi^x(q^x_{it};s_{it})
-F_E(1-e_{i,t-1})\right]
+\beta E_tV(s_{i,t+1},e_{it})\right\}.
\]

The export decision is

\[
e_{it}=1
\quad\Longleftrightarrow\quad
V^X(s_{it},e_{i,t-1})\geq V^D(s_{it},e_{i,t-1}).
\]

## Main Mechanism
Entry is an irreversible or partially irreversible investment. A temporary favorable shock can induce entry and affect exports after the shock disappears; an incumbent may remain despite low current profit because exit would sacrifice its entry investment. Expectations therefore change both timing and magnitude.

## Common Propositions
- Export participation exhibits true state dependence when sunk entry costs are positive.
- Entry and exit thresholds differ, generating hysteresis.
- Aggregate export supply depends on the full distribution of plants and histories, not only the current exchange rate.
- Revenue subsidies and entry subsidies can have different effects because they target intensive and extensive margins differently.

## Comparative Statics Usually Available
- Higher sunk costs widen the inaction region and reduce entry.
- More persistent favorable foreign demand raises the option value of entry.
- Greater uncertainty can delay entry when investment is irreversible, although the sign depends on profit curvature and exit options.
- Export revenue subsidies affect incumbents and entrants, while entry subsidies directly target only the transition into exporting.

## Data Requirements
- Plant-level panel data with export status, export revenue or quantity, sales, and production costs.
- Exchange rates, foreign demand, domestic costs, and policy variables over time.
- Enough entry and exit transitions to separate state dependence from persistent heterogeneity.

## Estimation or Calibration
Estimate the static export-profit function and dynamic parameters jointly or sequentially. The canonical application uses Bayesian Markov chain Monte Carlo. Identification of sunk costs comes from participation transitions conditional on persistent heterogeneity and aggregate state variables.

## Counterfactual Analysis
Simulate plant decisions under alternative exchange-rate processes, export-revenue subsidies, or entry-cost subsidies. Initialize with the observed plant distribution and propagate states long enough to distinguish transition from long-run effects.

## Welfare Implications
The canonical plant problem quantifies export responses, not a complete national-welfare equilibrium. Welfare requires consumer surplus, fiscal cost, domestic factor-market effects, and any terms-of-trade response to be added.

## Welfare Decomposition
Not applicable in the baseline partial-equilibrium estimation. In an extended welfare model, separate current operating profit, sunk resource costs, consumer price effects, fiscal transfers, and general-equilibrium wages or terms of trade.

## Common Modeling Pitfalls
- Interpreting serial correlation in export status as sunk costs without controlling for persistent heterogeneity.
- Treating sunk entry payments as recurring fixed costs.
- Solving a static participation model for a policy that changes expectations.
- Comparing counterfactual steady states while ignoring the transition path.

## How to Extend the Model
- Multiple destinations, learning about demand, customer accumulation, or product entry.
- Endogenous productivity investment and financing constraints.
- General-equilibrium wages, exchange rates, and trade-policy uncertainty.

## Example Research Questions This Model Can Support
- Why does export participation respond slowly to a temporary depreciation?
- Are export-revenue subsidies more effective than entry-cost subsidies?
- How much export persistence reflects sunk costs rather than plant heterogeneity?

## Closely Related Model Families
Melitz firm heterogeneity; multiproduct trade; trade-policy uncertainty; dynamic supplier switching.

## When This Model Is Not Appropriate
Do not use the partial-equilibrium baseline to evaluate aggregate welfare, worker adjustment, or production-network propagation. A static Melitz model is sufficient when export history and expectations are empirically irrelevant.
