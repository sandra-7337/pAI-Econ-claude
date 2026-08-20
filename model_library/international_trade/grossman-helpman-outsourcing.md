# Grossman-Helpman Outsourcing in Industry Equilibrium

## Model Family Name
Search, Matching, Incomplete Contracts, and Vertical Organization

## Canonical Economic Question
When does an industry organize production through arm’s-length outsourcing rather than vertical integration once search thickness, hold-up, fixed costs, and product-market competition are jointly determined?

## Verified References
- Grossman, Gene M., and Elhanan Helpman. 2002. “Integration versus Outsourcing in Industry Equilibrium.” *Quarterly Journal of Economics* 117(1): 85-120. [DOI](https://doi.org/10.1162/003355302753399454).

## When to Use This Model
- Use it when industry-wide outsourcing depends on the thickness of the market for specialized suppliers.
- Use it to combine incomplete contracting with endogenous entry and two-sided search.
- Use it when vertical integration and outsourcing are alternative equilibrium modes rather than firm-specific labels imposed from the data.

## Typical Primitives
- Differentiated final-good varieties under CES demand and industry spending share (\mu_j).
- Specialized final producers, specialized component producers, and vertically integrated firms.
- Entry/search costs (k_s,k_m), integrated fixed cost (k_v), integrated unit cost (\ell), and supplier bargaining weight (\nu).
- Matching function (n(s,m)) between masses of final producers (s) and component suppliers (m).

## Timing
Firms enter and pay type-specific fixed costs; specialized firms search and match; suppliers produce relationship-specific inputs; matched parties bargain ex post; final goods are assembled and sold.

## Information Structure
Input quality is observable to the parties but not court-verifiable, preventing complete ex ante quality contracts. Matching is random and its technology is known. Households diversify firm risk.

## Agent Heterogeneity
The baseline firms of a given type are identical; heterogeneity comes from organizational role and match realization. Industries differ in demand elasticity, fixed costs, governance cost, bargaining power, and matching conditions.

## Choice Variables
- Entrants choose integrated, specialized-final, or specialized-input status.
- Specialized suppliers choose input quantity/quality after matching.
- Entry masses determine market thickness and match probabilities; final firms set prices through CES markups.

## Constraints
- Specialized production requires a successful match.
- Relationship-specific inputs have no outside value in the simple model.
- Ex post bargaining divides revenue after input production, creating hold-up.
- Free entry imposes zero expected profit for every active organizational type; product and labor markets clear.

## Equilibrium Concept or Solution Concept
A free-entry general equilibrium with random matching and ex post Nash bargaining. Industry organization is a fixed point in entrant masses, match probabilities, demand, and expected profits. Stable equilibria can feature pervasive outsourcing or pervasive integration.

## Key Equations
With constant-returns matching, let (r=m/s) and let the final producer’s match probability be

\[
h(r)=n(1,r),
\]

while a component supplier matches with probability (h(r)/r). Under outsourcing, the CES price and quantity are

\[
p_s=\frac{1}{\alpha\nu},
\qquad
y_s=A(\alpha\nu)^{1/(1-\alpha)}.
\]

Expected profits of specialized final and input producers are

\[
\pi_s=h(r)(1-\nu)A(\alpha\nu)^{\alpha/(1-\alpha)}-k_s,
\]

\[
\pi_m=\frac{h(r)}{r}(1-\alpha)\nu A(\alpha\nu)^{\alpha/(1-\alpha)}-k_m.
\]

Free entry sets active types’ expected profits to zero.

## Main Mechanism
Outsourcing suffers from hold-up and failed-search risk, but specialization avoids bureaucratic production costs. More entrants on the opposite side raise a firm’s matching probability, generating a market-thickness complementarity. Product-market entry then feeds back through the demand shifter.

## Common Propositions
- With identical firms and constant returns in matching, mixed organizational equilibria are generically knife-edge.
- Outsourcing is viable only when the zero-profit conditions for both sides of the specialized market are jointly satisfied.
- Industry size and matching returns can create thickness effects and multiple or unstable equilibria.
- Greater bargaining power for suppliers improves their investment incentives but redistributes surplus and changes entry on both sides.

## Comparative Statics Usually Available
- Lower search costs raise specialized entry and the probability of a match.
- Higher integrated unit or governance costs favor outsourcing.
- Changes in bargaining power have nonmonotone industry effects because investment and entry incentives move differently.
- Increasing returns in matching strengthen agglomeration and thickness effects.

## Data Requirements
- Industry organization, vertical ownership, supplier counts, partner formation, and entry/exit.
- Measures of search costs, input specificity, bargaining conditions, and integrated production costs.
- Industry demand elasticities, firm counts, prices, output, and geographic market thickness.

## Estimation or Calibration
Discipline matching using match rates and the ratio of supplier to final-producer entrants. Use organizational shares and entry responses to estimate fixed costs and governance penalties. Causal identification of thickness effects requires exogenous variation in local supplier availability or search costs.

## Counterfactual Analysis
Change search technology, fixed costs, bargaining power, or integration costs; solve zero-profit, matching, demand, and labor-market equations. Check equilibrium existence, multiplicity, and local stability rather than reporting only one numerical root.

## Welfare Implications
Outsourcing can exploit specialization but creates hold-up and matching losses; integration avoids failed search and changes incentives but can have higher governance or production cost. Free entry does not generally eliminate contractual inefficiency.

## Welfare Decomposition
Separate specialization cost savings, search failures, hold-up distortions, fixed entry/search resources, product variety, and integrated governance costs. No single sufficient statistic summarizes these components.

## Common Modeling Pitfalls
- Treating matching as a reduced-form fixed probability instead of an equilibrium outcome.
- Ignoring the short-side/long-side distinction in match probabilities.
- Assuming a stable mixed equilibrium in the homogeneous-firm constant-returns baseline.
- Calling the model international sourcing without adding countries, wages, or trade costs.

## How to Extend the Model
- North-South sourcing and heterogeneous firms as in Antràs-Helpman.
- Partial input specialization, endogenous outside options, repeat relationships, or directed search.
- Geographic supplier clusters, trade costs, and policy shocks.

## Example Research Questions This Model Can Support
- Can supplier-market thickness explain why outsourcing clusters geographically?
- How do lower search costs change the boundary of the firm?
- When does a policy that subsidizes specialized entry coordinate an outsourcing equilibrium?

## Closely Related Model Families
Antràs-Helpman global sourcing; buyer-supplier search and matching; relationship-specific investment; endogenous production networks.

## When This Model Is Not Appropriate
Do not use the simple baseline for firm-level sorting by productivity, many-country sourcing, or observed persistent buyer-supplier links without adding the relevant heterogeneity and dynamics.
