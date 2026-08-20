# Quantitative Trade Counterfactuals

## Model Family Name
Structural Gravity and Exact-Hat Algebra

## Canonical Economic Question
How can observed trade shares and a small set of structural elasticities be used to compute equilibrium trade and welfare changes without separately estimating all technology and bilateral trade-cost levels?

## Verified References
- Dekle, Robert, Jonathan Eaton, and Samuel Kortum. 2008. “Global Rebalancing with Gravity: Measuring the Burden of Adjustment.” *IMF Staff Papers* 55(3): 511-540. [DOI](https://doi.org/10.1057/imfsp.2008.17).
- Costinot, Arnaud, and Andrés Rodríguez-Clare. 2014. “Trade Theory with Numbers: Quantifying the Consequences of Globalization.” In *Handbook of International Economics*, vol. 4, 197-261. [DOI](https://doi.org/10.1016/B978-0-444-54314-1.00004-5).

## When to Use This Model
- Use it to solve counterfactual changes around an observed trade equilibrium.
- Use it when baseline bilateral shares are reliable but technology and iceberg-cost levels are not separately identified.
- Use it as a computational method attached to a clearly specified Armington, Ricardian, or heterogeneous-firm gravity model.

## Typical Primitives
- Baseline bilateral expenditure shares (λ_{ij}), domestic shares, incomes/expenditures, deficits or transfers, and factor endowments.
- Counterfactual changes in iceberg costs, tariffs, technology, endowments, or transfers.
- A positive trade elasticity (ε) and any sectoral substitution, input-output, or factor-supply parameters required by the chosen model.
- A closure for trade balances, tariff revenue, labor mobility, and nontraded sectors.

## Timing
Static comparison of two equilibria. The method solves exact proportional changes and does not describe adjustment between them.

## Information Structure
Not applicable as an independent information structure. Exact-hat algebra inherits the information assumptions of the underlying structural model and uses observed equilibrium shares as sufficient baseline statistics.

## Agent Heterogeneity
Inherited from the underlying model: countries, sectors, factors, or firms may differ. Only heterogeneity that aggregates into the chosen equilibrium equations and baseline shares is retained.

## Choice Variables
Not applicable as a standalone behavioral model. The underlying model supplies consumer, producer, and entry choices; the hat system solves changes in wages, prices, expenditures, trade shares, and welfare.

## Constraints
- Every hatted equation must be derived by dividing the counterfactual equilibrium condition by its baseline counterpart.
- Baseline accounting identities and market clearing must hold.
- The counterfactual must specify deficit/transfer and tariff-revenue closure.
- Structural elasticities must be invariant over the counterfactual unless the model explicitly allows them to change.

## Equilibrium Concept or Solution Concept
An exact-change representation of a competitive or monopolistically competitive gravity equilibrium. A nonlinear fixed point in relative wages, prices, expenditures, and shares is solved subject to counterfactual market clearing.

## Key Equations
For a one-sector constant-elasticity gravity model with unit-cost change (\widehat c_i) and trade-cost change (\widehat\tau_{ij}),

\[
\widehat P_j
=\left[\sum_i\lambda_{ij}
(\widehat c_i\widehat\tau_{ij})^{-\varepsilon}\right]^{-1/\varepsilon},
\]

\[
\lambda'_{ij}
=\frac{\lambda_{ij}
(\widehat c_i\widehat\tau_{ij})^{-\varepsilon}}
{\sum_k\lambda_{kj}
(\widehat c_k\widehat\tau_{kj})^{-\varepsilon}}.
\]

Income changes then satisfy the model-specific goods-market and balance equations. Under the ACR restrictions,

\[
\widehat W_j=\widehat\lambda_{jj}^{-1/\varepsilon}.
\]

## Main Mechanism
Baseline trade shares absorb unknown technology, taste, and trade-cost levels. Counterfactual changes reweight those shares according to changes in delivered costs; general-equilibrium income and price feedback then closes the system.

## Common Propositions
- Exact hats can compute counterfactual changes without recovering all structural levels.
- The method is exact only for the equations of the maintained model; it is not a generic approximation.
- Domestic trade shares and trade elasticities often dominate aggregate welfare results in one-sector gravity models.
- Multiple sectors and intermediates require sectoral shares, elasticities, and input-output linkages.

## Comparative Statics Usually Available
- A larger trade elasticity yields stronger trade-share substitution for a given delivered-cost change.
- Stronger input-output linkages transmit sectoral shocks more broadly.
- Alternative deficit closure can materially change wage and absorption responses.
- Fixed versus mobile factors change how the burden of adjustment is distributed.

## Data Requirements
- Balanced bilateral trade matrices including domestic sales.
- Output, expenditure, value added, final demand, tariffs, and transfers/deficits.
- Sectoral input-output tables and factor payments for richer models.
- Model-consistent elasticities with uncertainty ranges.

## Estimation or Calibration
Construct baseline shares from a balanced social accounting matrix and estimate or import structural elasticities from credible variation. Exact-hat algebra does not identify elasticities; it conditions on them. Validate by reproducing the baseline identities before running shocks.

## Counterfactual Analysis
Specify the shock and closure; initialize hats at one; iterate wages, prices, expenditures, and shares until all market-clearing residuals are small. Report convergence tolerances, numeraire, baseline reproduction, and sensitivity to elasticities and closure.

## Welfare Implications
Welfare is model dependent. The domestic-share formula applies only under ACR restrictions; tariff revenue, intermediates, multiple factors, nontraded goods, scale economies, and imbalances require their own exact welfare equations.

## Welfare Decomposition
Decompose changes into price indices, nominal income/terms of trade, tariff revenue, transfers, sectoral linkages, and factor reallocation. Nonlinear decomposition is path dependent unless a stated Shapley or line-integral method is used.

## Common Modeling Pitfalls
- Treating exact-hat algebra as an economic model rather than a solution method.
- Omitting domestic trade or starting from an unbalanced input-output table.
- Leaving trade-deficit and tariff-revenue closure implicit.
- Reporting a fixed point without checking every equilibrium residual.

## How to Extend the Model
- Multisector input-output trade, heterogeneous firms, multiple factors, migration, or dynamic capital.
- Endogenous production networks and supplier relationships.
- Parameter uncertainty, Bayesian counterfactual intervals, or model comparison.

## Example Research Questions This Model Can Support
- What are the trade and welfare effects of a bilateral tariff change?
- How does eliminating current-account imbalances alter relative wages and absorption?
- How sensitive is a policy counterfactual to the trade elasticity and deficit closure?

## Closely Related Model Families
Armington structural gravity; Eaton-Kortum; ACR sufficient statistics; Caliendo-Parro; network general-equilibrium welfare.

## When This Model Is Not Appropriate
Do not use exact hats to identify causal parameters, model transition dynamics, or answer questions whose central state variables are absent from the maintained structural model. It cannot rescue a misspecified equilibrium system.
