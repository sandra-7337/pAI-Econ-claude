# Caliendo-Parro Multisector Trade

## Model Family Name
Multicountry Multisector Ricardian Trade with Input-Output Linkages and Tariffs

## Canonical Economic Question
How do sector-specific tariff changes propagate across countries and industries through comparative advantage, intermediate-input trade, and input-output linkages, and what are their trade and welfare effects?

## Verified References
- Caliendo, Lorenzo, and Fernando Parro. 2015. “Estimates of the Trade and Welfare Effects of NAFTA.” *Review of Economic Studies* 82(1): 1-44. [DOI](https://doi.org/10.1093/restud/rdu035).

## When to Use This Model
- Use it for tariff counterfactuals requiring country-sector heterogeneity and traded intermediates.
- Use it when input-output linkages transmit trade policy across sectors.
- Use it when exact changes are preferable to recovering technology and iceberg-cost levels.

## Typical Primitives
- Countries (n,i=1,\ldots,N), sectors (j,k=1,\ldots,J), labor (L_n), and a representative household in each country.
- Sectoral productivity draws (z_n^j(\omega)) distributed Fréchet with scale (T_n^j) and shape (\theta_j).
- Labor value-added share (\gamma_n^j), input share (\gamma_n^{k,j}), and final expenditure share (\alpha_n^j).
- Iceberg costs (d_{ni}^j\geq1), gross tariff factor (1+\tau_{ni}^j), and trade deficit/transfer (D_n).
- Competitive intermediate producers and CES/EK sourcing over varieties.

## Timing
Static. Tariffs and fundamentals are given; producers source each variety from its lowest delivered-cost country; firms demand labor and sectoral materials; households consume; wages, price indices, trade shares, tariff revenue, and expenditures clear simultaneously.

## Information Structure
Complete information over distributions and aggregate fundamentals. Individual variety productivity draws are realized and sourcing selects the lowest delivered cost.

## Agent Heterogeneity
Countries differ in technology, labor, deficits, tariffs, and production structure. Sectors differ in trade elasticity, value-added share, intermediate composition, and tradability. Varieties differ in realized productivity.

## Choice Variables
- Intermediate producers choose labor and sectoral material inputs.
- Composite producers choose the lowest-cost origin for each variety.
- Households choose sectoral consumption; equilibrium determines wages, expenditures, and tariff revenue.

## Constraints
- Cobb-Douglas production shares satisfy (\gamma_n^j+\sum_k\gamma_n^{k,j}=1).
- Goods and labor markets clear in every country and sector.
- Income equals labor income, tariff rebates, and the specified trade deficit/transfer.
- Bilateral expenditures must be consistent with sourcing probabilities and tariffs.

## Equilibrium Concept or Solution Concept
A competitive multicountry-multisector equilibrium. For a counterfactual tariff matrix, the model is solved in relative changes from an observed baseline. The exact-hat system determines wage, price, expenditure, and trade-share changes without separately identifying levels of (T_n^j) or (d_{ni}^j).

## Key Equations
Unit input cost in country (n), sector (j), is

\[
c_n^j=\Upsilon_n^j w_n^{\gamma_n^j}
\prod_{k=1}^J(P_n^k)^{\gamma_n^{k,j}}.
\]

Let (\kappa_{ni}^j=d_{ni}^j(1+\tau_{ni}^j)). The EK price index and expenditure share are

\[
P_n^j=\Gamma_j\left[\sum_iT_i^j(c_i^j\kappa_{ni}^j)^{-\theta_j}\right]^{-1/\theta_j},
\]

\[
\pi_{ni}^j=
\frac{T_i^j(c_i^j\kappa_{ni}^j)^{-\theta_j}}
{\sum_hT_h^j(c_h^j\kappa_{nh}^j)^{-\theta_j}}.
\]

In exact changes,

\[
\widehat\pi_{ni}^j=
\frac{(\widehat c_i^j\widehat\kappa_{ni}^j)^{-\theta_j}}
{\sum_h\pi_{nh}^j(\widehat c_h^j\widehat\kappa_{nh}^j)^{-\theta_j}}.
\]

Real income is nominal income divided by the Cobb-Douglas final price index, (W_n=I_n/\prod_j(P_n^j)^{\alpha_n^j}).

## Main Mechanism
A tariff changes the delivered cost of a sectoral input, reallocating sourcing according to (\theta_j). The price change enters every downstream sector through (\gamma_n^{j,k}), changes comparative costs, wages, tariff revenue, and terms of trade, and feeds back into bilateral sourcing. Sectoral heterogeneity and input-output loops can magnify or redirect the initial shock.

## Common Propositions
- Bilateral sectoral shares have gravity form with elasticity (\theta_j).
- Exact counterfactual changes require baseline shares, production structure, tariffs, deficits, and (\theta_j), but not productivity or iceberg-cost levels.
- Welfare changes can be decomposed into terms-of-trade and volume-of-trade components.
- Removing intermediate goods or sectoral linkages can materially change quantitative tariff effects.

## Comparative Statics Usually Available
- A larger (\theta_j) produces a larger sourcing response to a given tariff change.
- Higher intermediate shares transmit a sectoral tariff to more downstream prices.
- Higher domestic expenditure shares reduce immediate foreign exposure but may reflect high underlying trade costs.
- Deficit closure and tariff-revenue treatment affect wage and welfare responses.

## Data Requirements
- Country-sector bilateral trade including domestic sales.
- Gross output, value added, final expenditure, and input-output tables.
- Applied bilateral tariffs before and after the policy, labor income, and trade deficits/transfers.

## Estimation or Calibration
Compute (\pi,\gamma,\alpha) from trade and input-output data. Estimate sectoral (\theta_j) from tariff variation in a multiplicative gravity equation without requiring symmetric bilateral trade costs. Balance the baseline social accounting matrix before solving.

## Counterfactual Analysis
Replace (\tau) by a counterfactual tariff matrix; iterate on wages and expenditures until trade, goods, and labor markets clear. Report sectoral trade changes, real wages, tariff revenue, terms of trade, volume of trade, and welfare. Test sensitivity to deficits and sectoral elasticities.

## Welfare Implications
Tariff reductions lower imported-input costs and expand sourcing but can worsen a country’s terms of trade. Welfare need not move in the same direction for all agreement members. Input-output linkages make policy effects depend on the full production structure.

## Welfare Decomposition
Decompose real-income changes into terms-of-trade and volume-of-trade effects, with sector-level contributions. Tariff revenue is a domestic transfer; iceberg costs are resources lost. Also report results without materials and without cross-sector linkages to measure amplification.

## Common Modeling Pitfalls
- Applying a one-sector trade elasticity to every sector without sensitivity analysis.
- Omitting domestic sales from bilateral expenditure shares.
- Confusing tariffs with iceberg costs in the resource and revenue accounting.
- Holding intermediate price indices fixed after a tariff change.
- Reporting a converged numerical fixed point without checking market clearing.

## How to Extend the Model
- Multiple factors and distributional incidence.
- Regional labor mobility and dynamics as in Caliendo-Dvorkin-Parro.
- Endogenous firm entry, supplier networks, or variable markups.
- Optimal tariff or industrial-policy choice.

## Example Research Questions This Model Can Support
- How do sector-specific tariff cuts in a regional agreement affect each member’s welfare?
- Which downstream industries bear an upstream steel tariff through intermediate prices?
- How much do input-output linkages change the gains from eliminating a tariff war?

## Closely Related Model Families
Eaton-Kortum; Armington structural gravity; quantitative exact-hat counterfactuals; trade-policy shocks; network general-equilibrium welfare.

## When This Model Is Not Appropriate
Do not use it when firm entry, market power, relationship switching, uncertainty, or dynamic labor adjustment is the primary mechanism. A one-sector model may suffice when sectoral input-output structure is empirically irrelevant.
