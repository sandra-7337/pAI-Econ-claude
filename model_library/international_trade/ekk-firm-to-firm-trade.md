# EKK Firm-to-Firm Trade

## Model Family Name
Quantitative General Equilibrium with Random Buyer-Seller Matching

## Canonical Economic Question
How do iceberg trade costs and buyer-seller matching frictions jointly determine granular firm-to-firm trade, input sourcing, labor shares, and the distributional effects of integration?

## Verified References
- Eaton, Jonathan, Samuel S. Kortum, and Francis Kramarz. 2026. “Firm-to-Firm Trade: Imports, Exports, and the Labor Market.” *Econometrica* 94(4): 1135-1170. [DOI](https://doi.org/10.3982/ECTA20506).
- Eaton, Jonathan, Samuel S. Kortum, and Francis Kramarz. 2022. “Firm-to-Firm Trade: Imports, Exports, and the Labor Market.” NBER Working Paper 29685. [Working-paper DOI](https://doi.org/10.3386/w29685). The 2022 item is the working-paper version of the 2026 published article.

## When to Use This Model
- Use it when matched importer-exporter relationships and partner counts are outcomes, not incidental data.
- Use it to distinguish iceberg costs from matching frictions in gravity.
- Use it when imported and domestic intermediates compete with heterogeneous labor tasks.

## Typical Primitives
- Countries, heterogeneous potential producers, retailers, and multiple labor/task types.
- Producer efficiency (z), number of tasks (m), task labor requirements, and destination-specific cost shocks.
- Iceberg costs (d_{ni}), bilateral matching intensity (\lambda_{ni}), buyer congestion (\phi), and seller congestion (\gamma).
- Task shares (\beta_{k,i}), task substitution elasticity (\sigma), and Pareto/Fréchet tail parameter (\theta).

## Timing
Static. Potential producers draw efficiency and costs; active buyers and sellers meet randomly; buyers compare supplier quotes with in-house labor costs; production, retailing, trade, and labor-market clearing follow.

## Information Structure
Firms observe their own costs, tasks, and received matches/quotes. Aggregate distributions and matching technologies are known. Granularity survives at the firm level even though aggregate measures are smooth.

## Agent Heterogeneity
Producers differ in efficiency, tasks, labor requirements, destination shocks, supplier access, and buyer counts. Workers differ by task type. Countries differ in technologies, wages, matching access, and trade costs.

## Choice Variables
- Buyers choose the cheapest encountered supplier or perform a task in house with labor.
- Producers supply destinations in which they obtain buyers.
- Equilibrium determines active producer masses, partner distributions, trade shares, task outsourcing, wages, and expenditures.

## Constraints
- Production has constant returns with task-type Cobb-Douglas shares summing to one.
- A firm can buy only from suppliers it encounters; matches are Poisson.
- Potential producers become active only after obtaining at least one buyer.
- Goods, services, and labor markets clear in general equilibrium.

## Equilibrium Concept or Solution Concept
A competitive quantitative general equilibrium with random matching. A fixed point jointly determines the distribution of producer costs, buyer presence, active firms, matching outcomes, trade shares, labor shares, wages, and expenditures.

## Key Equations
A producer (j) from (i) delivers to (n) at unit cost

\[
c_{ni}(j)=\delta_n(j)\frac{d_{ni}C_i(j)}{z(j)}.
\]

For task type (k), the intensity with which a buyer in (n) meets a seller from (i) with cost (c) is

\[
\lambda_{k,ni}(c)=\lambda_k\lambda_{ni}B_n^{-\phi}S_n(c)^{-\gamma}.
\]

The model’s bilateral trade share is

\[
\pi_{ni}=\frac{\lambda_{ni}d_{ni}^{-\theta}T_i\Xi_i}
{\sum_{i'}\lambda_{ni'}d_{ni'}^{-\theta}T_{i'}\Xi_{i'}}.
\]

Thus matching intensity and iceberg costs enter gravity multiplicatively but affect partner counts differently.

## Main Mechanism
Buyers sample only a finite set of potential suppliers. Market access therefore depends on both shipping costs and the chance of forming relationships. Supplier encounters also determine whether production tasks use intermediates or labor, linking firm-to-firm trade to heterogeneous labor shares and worker incidence.

## Common Propositions
- Relationship counts, rather than sales per relationship alone, explain much cross-market variation in exports.
- Both lower iceberg costs and higher bilateral matching intensity raise trade shares.
- The two frictions are separately identified because they imply different partner-count and sales patterns.
- Cheaper or better-connected sellers obtain more buyers and are more likely to become active.

## Comparative Statics Usually Available
- Lower (d_{ni}) or higher (\lambda_{ni}) raises bilateral trade, but matching changes also shift the number and distribution of relationships.
- Greater buyer congestion (\phi) reduces encounters per buyer as market thickness rises.
- Greater seller congestion (\gamma) strengthens the advantage of low-cost sellers and changes the effective cost tail.
- Trade integration changes demand for task-specific labor through substitution toward imported intermediates.

## Data Requirements
- Matched exporter-importer customs transactions with values and partner identifiers.
- Firm production accounts, intermediate purchases, and task- or skill-specific labor payments.
- Bilateral trade, market size, wages, input-output information, and a policy episode or cross-sectional cost variation.

## Estimation or Calibration
Use partner-count distributions, exporters per market, buyers per exporter, sales per relationship, labor-share distributions, and aggregate trade shares. The published application disciplines matching and iceberg frictions separately and calibrates the model to French firms and EU destinations.

## Counterfactual Analysis
Change (d_{ni}) and/or (\lambda_{ni}), recompute active firms, matches, input costs, trade shares, labor shares, wages, and welfare. The 2004 EU enlargement is a canonical application; report separate iceberg and matching contributions.

## Welfare Implications
Lower barriers can benefit workers overall while generating unequal gains across task types; workers whose tasks compete most directly with imports can gain less or lose. Welfare requires the model’s services and labor-market closure, not trade shares alone.

## Welfare Decomposition
Decompose aggregate and worker-type welfare into changes due to iceberg costs, matching frictions, goods prices, wages, and task substitution. Because the counterfactual is nonlinear, decomposition order should be reported or a path-independent method used.

## Common Modeling Pitfalls
- Calling every Eaton-Kortum-Kramarz paper “EKK”; this card refers specifically to the 2026 firm-to-firm matching article.
- Treating observed links as a fixed network rather than outcomes of random matching.
- Identifying matching frictions from aggregate gravity alone.
- Adding fixed relationship costs without re-deriving the zero-variable-profit matching structure.

## How to Extend the Model
- Persistent relationships, directed search, bargaining, or supplier switching costs.
- Endogenous investments in match formation or quality.
- Multiple sectors, inventories, tariffs, and dynamic labor adjustment.

## Example Research Questions This Model Can Support
- How much of distance-related trade resistance reflects shipping versus difficulty finding partners?
- How does a trade agreement change exporters per market and buyers per exporter?
- Which worker tasks are most exposed when imported intermediates become easier to source?

## Closely Related Model Families
Eaton-Kortum; buyer-supplier search and matching; production-network formation; trade-labor adjustment; dynamic sourcing.

## When This Model Is Not Appropriate
Do not use it when relationships are persistent strategic contracts, firms deliberately search over known suppliers, or fixed relationship investments are the main mechanism unless those elements are explicitly added. Aggregate trade data alone are insufficient to discipline its key frictions.
