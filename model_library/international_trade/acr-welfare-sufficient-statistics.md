# ACR Welfare Formula and Sufficient Statistics

## Model Family Name
Sufficient-Statistics Welfare Analysis for CES Trade Models

## Canonical Economic Question
Under what restrictions can the welfare effect of a trade-cost change be recovered from only the change in the domestic expenditure share and the trade elasticity?

## Verified References
- Arkolakis, Costas, Arnaud Costinot, and Andrés Rodríguez-Clare. 2012. “New Trade Models, Same Old Gains?” *American Economic Review* 102(1): 94-130. [DOI](https://doi.org/10.1257/aer.102.1.94).

## When to Use This Model
- Use it for a disciplined welfare calculation when the target model satisfies the ACR macro restrictions.
- Use it to compare the aggregate gains from trade across Armington, Ricardian, and heterogeneous-firm models that share the same domestic trade share and trade elasticity.
- Use it as a benchmark, not as a substitute for a richer model when additional margins matter for the policy question.

## Typical Primitives
- Country income and expenditure, domestic expenditure share (\lambda_{nn}), and a positive absolute trade elasticity (\varepsilon>0).
- CES demand/import system, one factor of production, and constant elasticity of trade flows with respect to variable trade costs.
- The equilibrium restrictions of balanced trade and aggregate profits that are constant shares of revenue in the canonical class.

## Timing
Static comparison between an initial and counterfactual equilibrium. The formula does not model a transition path.

## Information Structure
Not applicable as an independent informational environment: ACR is a cross-model welfare result. Information assumptions are inherited from the underlying Armington, Ricardian, or monopolistic-competition model.

## Agent Heterogeneity
Countries may differ, and the underlying model may contain technologies, varieties, or heterogeneous firms. For the aggregate welfare result, that micro heterogeneity must aggregate into the domestic share and a common trade elasticity under the stated restrictions.

## Choice Variables
Not applicable as a standalone decision problem. The underlying trade model determines sourcing, entry, production, and prices; ACR maps two equilibrium statistics into aggregate welfare.

## Constraints
- CES import demand with a constant trade elasticity.
- One factor and balanced trade in the canonical theorem.
- The domestic expenditure share must be measured consistently, including domestic sales.
- Changes in profits, entry, and variety must satisfy the aggregation conditions of the theorem.

## Equilibrium Concept or Solution Concept
Two equilibria of any model inside the ACR class are compared using an exact sufficient-statistics mapping. One must first verify that the underlying equilibrium belongs to that class.

## Key Equations
Let (\widehat x=x'/x), let (\lambda_{nn}) be the share of country (n)'s expenditure on domestic goods, and let (\varepsilon>0) be the absolute trade elasticity. Then

\[
\widehat W_n=\widehat\lambda_{nn}^{-1/\varepsilon}.
\]

For a move from autarky, where the counterfactual domestic share equals one, to an observed trade equilibrium,

\[
\frac{W_n^{trade}}{W_n^{autarky}}
=\lambda_{nn}^{-1/\varepsilon}.
\]

## Main Mechanism
Opening to trade lowers the domestic expenditure share. Conditional on the trade elasticity, this share change summarizes the endogenous price-index response and all model-specific extensive and intensive margins that satisfy the ACR restrictions.

## Common Propositions
- Models with different microfoundations can imply the same aggregate gains from trade when they share (\lambda_{nn}) and (\varepsilon).
- Lower domestic expenditure and a smaller absolute trade elasticity imply larger measured gains from trade.
- Micro-level adjustment margins affect welfare through their effect on the two sufficient statistics, not as separate add-ons, within the theorem’s domain.

## Comparative Statics Usually Available
- (\partial\log W_n/\partial\log\lambda_{nn}=-1/\varepsilon).
- For a given fall in the domestic share, a larger (\varepsilon) implies smaller welfare gains because sourcing substitutes more easily.
- Comparative statics outside the theorem’s restrictions require the full structural model.

## Data Requirements
- Domestic absorption and expenditure on domestic goods for each equilibrium or scenario.
- A credible estimate of the aggregate trade elasticity using the same cost concept and model aggregation.
- Consistent national accounts and trade data; gross and value-added shares must not be mixed.

## Estimation or Calibration
Estimate (\varepsilon) from trade-flow responses to exogenous changes in variable trade costs, or use a model-consistent external estimate. Compute (\lambda_{nn}) as domestic expenditure divided by total absorption. Report sensitivity to plausible elasticities and measurement of domestic trade.

## Counterfactual Analysis
Obtain the counterfactual domestic share from data or a structural trade model, then apply the formula. The formula alone does not predict (\widehat\lambda_{nn}); it evaluates welfare conditional on that equilibrium response.

## Welfare Implications
The result is exact for the specified class, not a universal approximation. It can fail with multiple factors and distributional objectives, non-CES demand, variable markups, external economies, input-output linkages not covered by the aggregation, trade imbalances, or transitional dynamics.

## Welfare Decomposition
Not applicable as a unique mechanism decomposition. The result deliberately compresses admissible mechanisms into (\lambda_{nn}) and (\varepsilon); decomposing entry, variety, productivity, or terms of trade requires returning to the underlying model and avoiding double counting.

## Common Modeling Pitfalls
- Treating the formula as universally valid because a model has CES demand.
- Using the elasticity coefficient with the wrong sign or failing to state that (\varepsilon) is an absolute value.
- Applying an autarky formula to a bilateral policy change without computing the new domestic share.
- Claiming that the formula identifies adjustment mechanisms; it identifies aggregate welfare under restrictions.

## How to Extend the Model
- Use multisector or input-output sufficient-statistics results with sectoral shares and elasticities.
- Add distributional welfare by solving factor or household heterogeneity explicitly.
- Embed the formula as a diagnostic benchmark beside a richer quantitative model.

## Example Research Questions This Model Can Support
- What aggregate gains from trade are implied by a country’s domestic expenditure share?
- How sensitive are welfare conclusions to alternative credible trade elasticities?
- Does a richer model deliver welfare gains beyond the ACR benchmark, and which violated restriction explains the difference?

## Closely Related Model Families
Armington structural gravity; Eaton-Kortum; Melitz; quantitative exact-hat analysis; network general-equilibrium welfare.

## When This Model Is Not Appropriate
Do not use it as the main model when the research question concerns sectoral incidence, labor reallocation, supplier relationships, uncertainty, dynamics, market power, or a mechanism excluded by the sufficient-statistics theorem.
