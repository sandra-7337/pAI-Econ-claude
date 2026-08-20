# Oberfield Input-Output Architecture

## Model Family Name
Endogenous Firm-Level Supplier Choice and Input-Output Architecture

## Canonical Economic Question
How do decentralized choices over whom to buy from generate an aggregate production network, and how does the distribution of producer efficiency shape supplier concentration, input shares, and aggregate productivity?

## Verified References
- Oberfield, Ezra. 2018. “A Theory of Input-Output Architecture.” *Econometrica* 86(2): 559-589. [DOI](https://doi.org/10.3982/ECTA10731).

## When to Use This Model
- Use it when each producer selects a particular upstream supplier or technique and those choices jointly create the network.
- Use it to connect micro heterogeneity in production efficiency to star suppliers, supply-chain depth, and aggregate productivity.
- Use it when bilateral surplus division matters but the central object is network architecture rather than search effort.

## Typical Primitives
- A population of entrepreneurs, each producing a differentiated good.
- Labor and exactly one intermediate input in the baseline technology.
- A technique (\phi) specifies a buyer (b(\phi)), supplier (s(\phi)), and technique productivity (z(\phi)).
- Intermediate-input exponent (\alpha\in(0,1)); labor has exponent (1-\alpha).
- Heterogeneous entrepreneurial efficiencies and a feasible set of supply techniques/chains.
- Friction: decentralized bilateral surplus division; no exogenous input-output matrix.

## Timing
Static. Feasible techniques and efficiencies are realized; entrepreneurs choose supply chains/techniques; connected buyers and suppliers agree on quantities and transfers; labor, goods, and relationship-level trades clear.

## Information Structure
Complete information about feasible techniques and efficiencies. The equilibrium concept allows coalitional deviations along countable supply chains rather than private-information screening.

## Agent Heterogeneity
Entrepreneurs differ in productivity and in the techniques available to them. Endogenous heterogeneity arises in network position, customer count, labor demand, output, and surplus.

## Choice Variables
- Buyers choose which supplier/technique to use.
- Linked firms choose production and intermediate quantities and divide bilateral surplus.
- Entrepreneurs choose labor input; prices/transfers and outputs are equilibrium objects.

## Constraints
- Each entrepreneur uses labor and one chosen intermediate supplier.
- A feasible supply chain must link the supplier of each technique to the buyer of the next technique.
- Production feasibility must hold recursively along the entire chain.
- Labor use across all entrepreneurs cannot exceed the aggregate endowment.

## Equilibrium Concept or Solution Concept
Countably stable equilibrium: no countable coalition along a feasible supply chain can deviate in a way that makes all coalition members weakly better off and at least one strictly better off. Under the paper’s assumptions, stable allocations are productively efficient; surplus division is not always uniquely pinned down.

## Key Equations
For a buyer (j=b(\phi)) using supplier (s(\phi)), the baseline production relation is

\[
y_j=z(\phi)\,l_j^{1-\alpha}x_{j,s(\phi)}^{\alpha}.
\]

A feasible supply chain (\omega=(\phi_0,\phi_1,\ldots)) for (j) satisfies (b(\phi_0)=j) and (s(\phi_k)=b(\phi_{k+1})). Its recursively compounded productivity is

\[
q_j(\omega)=\prod_{k=0}^{\infty}z(\phi_k)^{\alpha^k},
\qquad
q_j=\sup_{\omega\in\Omega_j}q_j(\omega).
\]

The powers (\alpha^k) discount increasingly remote upstream efficiencies while preserving their cumulative effect.

## Main Mechanism
A productive supplier lowers the cost of its buyers, which can make those buyers attractive suppliers farther downstream. Recursive supplier choice therefore creates chains and hubs. The input exponent (\alpha) controls how strongly upstream productivity is transmitted and how the efficiency distribution maps into supplier concentration.

## Common Propositions
- Every countably stable equilibrium is efficient under the baseline feasibility and transfer assumptions.
- More efficient entrepreneurs are selected as suppliers more often, generating star suppliers.
- The distribution of efficiencies shapes the aggregate intermediate-input cost share and the degree distribution.
- Productivity improvements propagate recursively through chosen chains rather than through a fixed Leontief matrix.

## Comparative Statics Usually Available
- Higher (\alpha) increases the importance of upstream efficiency and lengthens the effective reach of supply chains.
- A thicker upper tail of efficiency raises supplier concentration and the prevalence of hubs.
- Greater supplier bargaining power can raise the observed intermediate expenditure share above the technological exponent (\alpha).
- Improving a central supplier raises output of direct and indirect downstream users.

## Data Requirements
- Firm-to-firm buyer-supplier links, firm employment, sales, productivity proxies, input expenditures, and possibly negotiated prices.
- Network degree distributions and buyer-supplier size correlations.
- Data distinguishing technological input shares from payment shares when bargaining is present.

## Estimation or Calibration
Calibrate (\alpha) from technological input intensity rather than mechanically from expenditure shares when surplus division matters. Fit the efficiency distribution to firm size and supplier-degree distributions. Identification of bargaining shares requires prices, margins, or relationship-level surplus information.

## Counterfactual Analysis
Change the efficiency distribution, individual supplier productivity, the input exponent, or feasible techniques; recompute optimal chains and a stable allocation. Network rewiring must be allowed unless the counterfactual explicitly fixes links.

## Welfare Implications
Efficient decentralized chain formation is possible under transferable surplus and the paper’s stability concept. Wedges, contracting limits, search costs, or nontransferable relationship investments can break this efficiency result.

## Welfare Decomposition
In the baseline, welfare changes can be decomposed into changes in compounded chain productivity and labor allocation. Not applicable as a universal closed-form sufficient-statistics decomposition: topology changes discretely and surplus division is not fully identified by technology alone.

## Common Modeling Pitfalls
- Equating the production exponent (\alpha) with the observed expenditure share when suppliers have bargaining power.
- Using pairwise Nash stability when profitable deviations require an entire upstream chain.
- Treating supplier hubs as exogenous instead of outcomes of efficiency draws and technique choice.
- Adding search costs without changing the equilibrium concept and welfare analysis.

## How to Extend the Model
- Geographic supplier search and trade costs.
- Multiple intermediates, CES supplier bundles, or sectoral heterogeneity.
- Relationship-specific investment, incomplete contracts, or disruption risk.
- Dynamic entry and supplier replacement.

## Example Research Questions This Model Can Support
- Why do a small number of highly productive firms become suppliers to many downstream firms?
- How does a technology improvement at a hub propagate when firms may rewire their supply chains?
- Why can observed input expenditure shares differ from engineering production elasticities?

## Closely Related Model Families
Acemoglu-Azar input-set choice; Bernard-Moxnes-Saito supplier search; fixed input-output networks; endogenous networks under uncertainty.

## When This Model Is Not Appropriate
Do not use it when firms require many simultaneous differentiated inputs, supplier discovery is the principal friction, contracts are incomplete, or dynamic disruption and rebuilding are central. Those settings require search, matching, or dynamic network models.
