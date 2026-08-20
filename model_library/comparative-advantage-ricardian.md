# Comparative Advantage — Ricardian Model

## Model Family Name
Classical and Continuum-Goods Ricardian Trade

## Canonical Economic Question
How do cross-country differences in relative labor productivity determine specialization, trade, relative wages, and gains from trade?

## Verified References
- Ricardo, David. 1817. *On the Principles of Political Economy and Taxation*, Chapter 7, “On Foreign Trade.” [Library of Economics and Liberty edition](https://www.econlib.org/library/Ricardo/ricP.html).
- Dornbusch, Rudiger, Stanley Fischer, and Paul A. Samuelson. 1977. “Comparative Advantage, Trade, and Payments in a Ricardian Model with a Continuum of Goods.” *American Economic Review* 67(5): 823-839. [Author-hosted article PDF](https://economics.mit.edu/sites/default/files/2023-05/fischer_comp_advantage.pdf).

## When to Use This Model
- Use it when technology differences are the source of comparative advantage.
- Use it for specialization, relative-wage, and terms-of-trade questions with one factor.
- Use the continuum-goods version when marginal rather than complete specialization is needed.

## Typical Primitives
- Two countries (H,F), labor endowments (L_H,L_F), and one homogeneous factor, labor.
- Goods (g) or a continuum (z∈[0,1]), unit labor requirements (a_H(z),a_F(z)), and homothetic preferences.
- Competitive production and, in extensions, iceberg trade costs.
- State variables: not applicable in the static baseline; technologies and endowments are parameters.

## Timing
Static. Firms compare unit labor costs; consumers demand goods; the relative wage and specialization cutoff adjust until goods, labor, and trade balance clear.

## Information Structure
Complete information about technologies, prices, and preferences. Firms and households are price takers.

## Agent Heterogeneity
Countries differ in technology and labor supply. Workers within a country are homogeneous. Goods differ in relative unit labor requirements.

## Choice Variables
- Firms choose which goods to produce and labor inputs.
- Consumers choose goods consumption.
- The relative wage and specialization pattern are equilibrium objects.

## Constraints
- Unit cost is (w_i a_i(z)).
- Each good is supplied by the lowest-cost country, with ties at marginal goods.
- Labor markets, goods markets, and trade balance clear.
- Labor is mobile across domestic sectors but immobile internationally.

## Equilibrium Concept or Solution Concept
A competitive general equilibrium. In the continuum model, an endogenous cutoff allocates goods across countries and a trade-balance condition determines the relative wage.

## Key Equations
Home has comparative advantage in good 1 in the two-good model if

\[
\frac{a_{1H}}{a_{2H}}<\frac{a_{1F}}{a_{2F}}.
\]

For the continuum model, define

\[
A(z)=\frac{a_F(z)}{a_H(z)}.
\]

Home produces good (z) when

\[
w_Ha_H(z)\leq w_Fa_F(z)
\quad\Longleftrightarrow\quad
\frac{w_H}{w_F}\leq A(z).
\]

If (A(z)) is monotone, the marginal good satisfies

\[
A(\tilde z)=\frac{w_H}{w_F}.
\]

## Main Mechanism
Relative rather than absolute productivity determines opportunity cost. The equilibrium wage prevents one country from being the cheapest supplier of every good and allocates goods according to comparative advantage; trade permits consumption beyond each autarky production possibility frontier.

## Common Propositions
- A country exports goods in which its relative unit labor requirement is lower.
- Both countries weakly gain from voluntary trade in the competitive one-factor benchmark.
- Relative wages are endogenous and lie within bounds implied by relative productivities.
- In the continuum model, technology or size changes shift both the wage and specialization cutoff.

## Comparative Statics Usually Available
- A Home productivity improvement expands its potential production range and raises labor demand; wage feedback attenuates the expansion.
- A larger Home labor supply lowers its relative wage on impact and expands the set of Home-produced goods.
- Iceberg costs create ranges of nontraded goods around the marginal specialization region.

## Data Requirements
- Sector- or product-level productivity or unit labor costs, output, employment, wages, and bilateral trade.
- Domestic absorption for welfare or general-equilibrium calibration.
- Trade-cost data if nontraded margins or bilateral counterfactuals are studied.

## Estimation or Calibration
Calibrate unit labor requirements from productivity and wage data, then discipline demand and trade costs with expenditure shares. Identifying technology from observed trade alone is not possible without cost and wage restrictions; quantitative multicountry work usually uses Eaton-Kortum.

## Counterfactual Analysis
Change technology, labor endowments, or trade costs; recompute the relative wage, specialization cutoff, trade, and consumption. Check trade balance rather than holding wages fixed.

## Welfare Implications
With one homogeneous factor, real-wage changes summarize within-country welfare and there is no factor-based distributional conflict. Terms-of-trade changes can reallocate gains across countries; extensions with multiple factors or adjustment costs change this conclusion.

## Welfare Decomposition
Separate productivity, specialization, and terms-of-trade/relative-wage effects. No unique decomposition follows from the two-good model alone because price normalization and shock sequencing matter.

## Common Modeling Pitfalls
- Confusing comparative with absolute advantage.
- Holding relative wages fixed in a general-equilibrium counterfactual.
- Using revealed comparative advantage as a direct technology measure.
- Applying one-factor welfare conclusions to worker groups or sector-specific capital.

## How to Extend the Model
- Eaton-Kortum for many countries and probabilistic specialization.
- Sector-specific factors or Heckscher-Ohlin factors for distribution.
- Trade in tasks, learning-by-doing, or dynamic technology.

## Example Research Questions This Model Can Support
- How does a sector-specific productivity shock change specialization and relative wages?
- Which goods become nontraded as transport costs rise?
- Can observed unit labor costs explain product-level export specialization?

## Closely Related Model Families
Eaton-Kortum; Heckscher-Ohlin; specific-factors trade; quantitative trade counterfactuals.

## When This Model Is Not Appropriate
Do not use the baseline when firm selection, increasing returns, input-output production, multiple-factor incidence, or dynamic adjustment is the primary mechanism.
