# Multiproduct Firms and Trade Liberalization

## Model Family Name
Heterogeneous Multiproduct, Multidestination Firms with Endogenous Product Scope

## Canonical Economic Question
How do firm ability, product attributes, market-entry costs, and trade costs determine which firms export, which products they sell in each destination, and how product scope changes after liberalization?

## Verified References
- Bernard, Andrew B., Stephen J. Redding, and Peter K. Schott. 2011. “Multiproduct Firms and Trade Liberalization.” *Quarterly Journal of Economics* 126(3): 1271-1318. [DOI](https://doi.org/10.1093/qje/qjr021).

## When to Use This Model
- Use it when firm-product-destination margins are central.
- Use it to study product dropping, core products, destination scope, and within-firm reallocation after trade liberalization.
- Use it when a single-product Melitz model omits empirically important product composition.

## Typical Primitives
- Countries, industries, a continuum of products, CES preferences, and monopolistic competition.
- Firm ability (\varphi), firm-product or firm-product-destination attributes (\lambda_{jk}), and elasticity of substitution (\sigma>1).
- Sunk firm entry cost, destination fixed cost, product-destination fixed cost, and iceberg trade cost (\tau_{ij}).
- General continuous distributions in symmetric analysis and Pareto distributions for tractable asymmetric gravity.

## Timing
Static baseline. A firm pays a sunk entry cost, observes ability and product attributes, then decides whether to operate, which destinations to serve, and which products to supply in each market.

## Information Structure
Ability and product attributes are unknown before sunk entry and observed afterward. In the baseline they are independent across firms and products; attributes may be common across destinations or destination specific.

## Agent Heterogeneity
Firms differ in common ability; products within a firm differ in attributes; destination-specific attributes may add a third dimension. Countries differ in size, wages, trade costs, and fixed market-access costs.

## Choice Variables
- Firms choose exit, destination participation, and the set of products supplied to each destination.
- Conditional on entry, firms set constant-markup prices under CES monopolistic competition.
- Entry masses, cutoffs, wages, price indices, and trade shares are equilibrium outcomes.

## Constraints
- Variable profit from a product must cover its product-destination fixed cost.
- The sum of profitable products must cover the fixed cost of serving a destination.
- Expected operating profits equal the sunk entry cost under free entry.
- Labor and goods markets clear.

## Equilibrium Concept or Solution Concept
A monopolistically competitive general equilibrium characterized by firm-ability cutoffs for operation and exporting and product-attribute cutoffs conditional on firm ability and destination. Under Pareto assumptions, aggregates and gravity margins have closed forms.

## Key Equations
Within a destination, CES demand can be represented by

\[
C_j=\left[\sum_i\int_{\omega\in\Omega_{ij}}
(\lambda_{ij}(\omega)c_{ij}(\omega))^{\rho}d\omega\right]^{1/\rho},
\qquad \sigma=\frac{1}{1-\rho}.
\]

With constant marginal cost (w_i/\varphi) and iceberg cost (\tau_{ij}), a firm charges the CES markup

\[
p_{ij}(\varphi)=\frac{\sigma}{\sigma-1}\frac{w_i\tau_{ij}}{\varphi}.
\]

A product is supplied only if

\[
\pi_{ijk}(\varphi,\lambda_{jk})
=\frac{r_{ijk}(\varphi,\lambda_{jk})}{\sigma}-w_i f_{ijk}\geq0,
\]

which defines a product-attribute cutoff that falls with firm ability.

## Main Mechanism
A common firm attribute creates selection across firms and destinations; idiosyncratic product attributes create selection within firms. Lower trade costs intensify competition and change cutoffs, causing surviving firms to shed weak products and reallocate sales toward stronger products and destinations.

## Common Propositions
- Higher-ability firms serve more destinations and sell more products in each market.
- A firm’s best products serve weakly more destinations than its marginal products under common product attributes.
- Trade liberalization raises the ability cutoff and product cutoffs, generating exit across firms and product dropping within firms.
- With Pareto distributions, domestic trade share can be sufficient for welfare; this need not hold under general distributions.

## Comparative Statics Usually Available
- Lower variable trade costs increase exporting firms, products per exporter, and sales of a firm-product to a destination before general-equilibrium selection effects.
- Lower fixed destination costs primarily expand destination participation.
- Lower product fixed costs expand product scope conditional on serving a market.
- Greater dispersion of product attributes changes within-firm concentration and extensive-margin elasticities.

## Data Requirements
- Firm-product-destination transaction data with trade values and quantities if prices are studied.
- Domestic firm-product shipments and firm entry/exit where product dropping is an outcome.
- Tariffs or other trade costs, destination size, wages, and market/product fixed-cost proxies.

## Estimation or Calibration
Use distributions of products per firm, destinations per firm, product sales ranks, and gravity decompositions into firms, products, and intensive margins. Identify liberalization effects using exogenous tariff changes and discipline Pareto shapes with firm and product sales tails.

## Counterfactual Analysis
Change variable or fixed trade costs; recompute firm, destination, and product cutoffs, entry, price indices, wages, and trade. Report within-firm product reallocation separately from across-firm exit and entry.

## Welfare Implications
Trade can raise welfare through lower prices and selection, while product dropping changes available variety. Under the special Pareto version, the ACR domestic-share result applies; outside it, welfare requires the full distribution and equilibrium.

## Welfare Decomposition
Decompose welfare into price-index changes from imported varieties, firm selection, product selection within firms, and wage/terms-of-trade effects. Product-count changes alone are not welfare because dropped products are selected on profitability and attributes.

## Common Modeling Pitfalls
- Confusing the Bernard-Redding-Schott model with Eckel-Neary’s oligopolistic flexible-manufacturing model.
- Treating products as symmetric within firms when product selection is the mechanism.
- Using export data without domestic product scope to infer total product dropping.
- Applying the Pareto welfare statistic under arbitrary ability and product-attribute distributions.

## How to Extend the Model
- Correlated product attributes, cannibalization, variable markups, quality, or capacity.
- Dynamic product innovation, product switching, and sunk destination entry.
- Multiproduct input sourcing or firm-to-firm networks.

## Example Research Questions This Model Can Support
- Do tariff reductions cause firms to concentrate on their core products?
- Why do firms exporting more products also serve more destinations?
- How much aggregate productivity growth comes from within-firm product reallocation?

## Closely Related Model Families
Melitz firm heterogeneity; dynamic export entry; multiproduct oligopoly; ACR welfare sufficient statistics.

## When This Model Is Not Appropriate
Do not use the baseline when cannibalization, strategic multiproduct pricing, innovation dynamics, or input sourcing is the central mechanism. A single-product Melitz model is preferable when product scope is unobserved and not substantively relevant.
