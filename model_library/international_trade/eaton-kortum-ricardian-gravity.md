# Eaton-Kortum Ricardian Gravity

## Model Family Name
Multicountry Ricardian Trade with Fréchet Productivity

## Canonical Economic Question
How do technology, geography, and comparative advantage jointly determine bilateral trade shares, prices, specialization, and the gains from trade?

## Verified References
- Eaton, Jonathan, and Samuel Kortum. 2002. “Technology, Geography, and Trade.” *Econometrica* 70(5): 1741-1779. [DOI](https://doi.org/10.1111/1468-0262.00352).

## When to Use This Model
- Use it for quantitative Ricardian trade with many countries and probabilistic specialization.
- Use it when bilateral trade shares and a single positive trade elasticity are central sufficient inputs.
- Use it as the technology-based foundation for multisector, spatial, or production-network trade models.

## Typical Primitives
- Countries (i,n=1,...,N), a continuum of goods (j), labor endowments (L_i), and representative consumers.
- Country technology scale (T_i>0) and common Fréchet shape parameter (\theta>0).
- Iceberg trade costs (d_{ni}\geq1), with (d_{ii}=1), and unit input costs (c_i), typically wages in the one-factor model.
- CES elasticity of substitution across goods (\sigma>1).

## Timing
Static. Productivities are drawn; producers quote delivered costs; each destination buys every good from its lowest-cost source; households consume; wages and goods markets clear.

## Information Structure
Productivity draws are independently distributed across goods and countries and are observed when sourcing occurs. Aggregate distributions and trade costs are common knowledge.

## Agent Heterogeneity
Countries differ in technology, labor supply, wages, and bilateral accessibility. Goods differ in realized country-specific productivity. Households are representative within countries.

## Choice Variables
- Producers choose output and destinations under perfect competition.
- Buyers choose the lowest delivered-cost supplier for each good.
- Households allocate expenditure across the CES composite; wages and trade shares are equilibrium objects.

## Constraints
- Delivering one unit from (i) to (n) requires shipping (d_{ni}) units.
- Labor and each country’s expenditure clear; the baseline imposes balanced trade.
- The Fréchet distribution and common shape parameter discipline comparative advantage and substitution across origins.

## Equilibrium Concept or Solution Concept
A competitive multicountry equilibrium with probabilistic specialization. Conditional on wages and trade costs, closed-form price indices and trade shares are combined with labor-market clearing and trade balance to determine wages.

## Key Equations
Country (i)'s productivity for a good has cumulative distribution

\[
F_i(z)=\exp(-T_i z^{-\theta}).
\]

The CES price index in destination (n) is

\[
P_n=\Gamma\left[\sum_i T_i(c_i d_{ni})^{-\theta}\right]^{-1/\theta},
\]

where (\Gamma) is a constant determined by (\sigma) and (\theta). The expenditure share on source (i) is

\[
\pi_{ni}=\frac{T_i(c_i d_{ni})^{-\theta}}
{\sum_k T_k(c_k d_{nk})^{-\theta}}.
\]

With balanced trade, (w_iL_i=\sum_n\pi_{ni}w_nL_n).

## Main Mechanism
Extreme-value productivity draws convert a discrete lowest-cost sourcing decision into smooth aggregate trade shares. Technology raises a country’s probability of being the cheapest source; wages and geography offset that advantage. The Fréchet shape (\theta) is the elasticity of trade with respect to delivered cost.

## Common Propositions
- Bilateral trade shares have a gravity form and depend on technology and delivered unit costs.
- A lower (\theta) means greater productivity dispersion and stronger comparative advantage but a smaller trade response to cost changes.
- The destination price distribution and source shares have closed forms.
- In the one-factor benchmark, the domestic expenditure share and (\theta) summarize the gains from trade under the ACR restrictions.

## Comparative Statics Usually Available
- Lower bilateral trade costs raise the exporter’s destination share with elasticity governed by (\theta), including general-equilibrium wage feedback.
- Higher (T_i) increases country (i)'s export shares and labor demand.
- Larger labor supply lowers relative wages on impact and expands comparative-advantage sectors until equilibrium feedback operates.

## Data Requirements
- Bilateral trade including domestic expenditure, output or absorption, wages, and labor endowments.
- Geographic trade-cost proxies or observed tariffs and freight costs.
- Price or productivity data if technology levels, rather than only counterfactual changes, are required.

## Estimation or Calibration
Estimate (\theta) from the response of trade shares to delivered-cost or price variation, preferably using exogenous tariff, freight, or geographic variation. Recover relative technology and trade-cost terms from trade shares only under explicit normalizations; otherwise use exact changes around the observed equilibrium.

## Counterfactual Analysis
Change iceberg costs, technologies, or labor supplies; solve for counterfactual wages satisfying market clearing and trade balance; then update price indices and trade shares. Report both partial-equilibrium sourcing responses and general-equilibrium wage effects.

## Welfare Implications
Real income is (W_n=w_n/P_n) in the one-factor benchmark. Under the ACR conditions, (\widehat W_n=\widehat\pi_{nn}^{-1/\theta}). This formula is not valid after adding unrestricted intermediates, multiple factors, markups, or unbalanced-trade closure without re-derivation.

## Welfare Decomposition
The baseline can separate technology, terms-of-trade/wage, and trade-cost contributions through the price index. The domestic-share formula gives the total exact change but does not by itself identify a unique causal decomposition.

## Common Modeling Pitfalls
- Reversing origin-destination indices in (\pi_{ni}).
- Treating (\theta) as the CES demand elasticity; it is the trade elasticity generated by productivity dispersion.
- Inferring technology from trade shares without accounting for wages and bilateral costs.
- Applying the one-factor welfare formula after adding sectoral input-output linkages.

## How to Extend the Model
- Sector-specific technologies and trade elasticities as in Caliendo-Parro.
- Intermediate inputs, production networks, multiple factors, tariffs, or spatial mobility.
- Firm-to-firm matching frictions as in Eaton-Kortum-Kramarz.

## Example Research Questions This Model Can Support
- How would a fall in shipping costs reallocate sourcing and welfare across countries?
- How much of bilateral trade reflects technology versus geography?
- What is the general-equilibrium effect of a country-specific productivity shock?

## Closely Related Model Families
Armington structural gravity; ACR sufficient-statistics welfare; Caliendo-Parro multisector trade; quantitative exact-hat counterfactuals.

## When This Model Is Not Appropriate
Do not use the baseline when firm entry, product scope, strategic pricing, contractual sourcing relationships, or dynamic adjustment is the primary mechanism. It also cannot identify the separate levels of technology and trade costs from trade shares alone.
