# Acemoglu-Azar Endogenous Production Networks

## Model Family Name
Endogenous Input Adoption and Technology Choice in Multisector General Equilibrium

## Canonical Economic Question
How do industries choose which products to use as inputs, how do prices and distortions reshape the resulting production network, and can the arrival of new products generate sustained growth by expanding the space of input combinations?

## Verified References
- Acemoglu, Daron, and Pablo D. Azar. 2020. “Endogenous Production Networks.” *Econometrica* 88(1): 33-82. [DOI](https://doi.org/10.3982/ECTA15899).

## When to Use This Model
- Use it when sectors can adopt or drop input categories and the network itself is an equilibrium object.
- Use it when technology benefits depend on the entire chosen subset of inputs, not only on bilateral link costs.
- Use its dynamic version when new product arrival expands the combinatorial set of feasible production techniques.

## Typical Primitives
- Industries (i=1,\ldots,n), a representative household, labor, and a menu of feasible input sets (S_i\subseteq\{1,\ldots,n\}).
- Set-specific productivity (A_i(S_i)), unit-cost function (K_i(S_i,A_i(S_i),\mathbf P)), and distortion/markup (\mu_i).
- For Cobb-Douglas implementations, endogenous shares (\alpha_{ij}(S_i)) and the resulting matrix (\alpha(S)).
- State variables in the dynamic model: the set of products/industries available at date (t) and inherited techniques.
- Frictions: adoption costs or productivity trade-offs across input combinations, product-market distortions, and possibly resource losses from distortions.

## Timing
Static baseline: technologies and distortions are given; industries choose input sets while taking prices as given; firms choose quantities; markets clear. Dynamic extension: new products arrive, existing industries update technologies using the expanded menu, prices adjust, and the process repeats.

## Information Structure
Complete information about feasible input combinations, set-specific productivity, prices, and distortions. Choices are decentralized but not strategic in the game-theoretic sense.

## Agent Heterogeneity
Industries differ in feasible input sets, gains from adoption, production shares, productivity, and distortions. Consumers are represented by a single household.

## Choice Variables
- Each industry chooses an input set (S_i) or a technology associated with that set.
- Conditional on (S_i), firms choose labor and intermediate quantities.
- The household chooses consumption; equilibrium determines prices and revenues.

## Constraints
- Unit costs must be feasible under the selected technology and input prices.
- Chosen input shares satisfy constant returns in the Cobb-Douglas case.
- Goods, labor, and household budget constraints clear.
- The network must be consistent with every industry’s cost-minimizing set at equilibrium prices.

## Equilibrium Concept or Solution Concept
A competitive equilibrium with endogenous technology choices: a price vector, allocation, and network (S^*=(S_1^*,\ldots,S_n^*)) such that each industry selects a cost-minimizing technology, all agents optimize, and all markets clear. Under the paper’s technology-price single-crossing and regularity conditions, equilibrium prices are unique and technology choices are generically unique.

## Key Equations
Industry (i)'s equilibrium unit-price condition is

\[
P_i=(1+\mu_i)\min_{S_i}K_i(S_i,A_i(S_i),\mathbf P).
\]

For the Cobb-Douglas specialization, define (a_i(S_i)=\log A_i(S_i)), (m_i=\log(1+\mu_i)), and (L(S)=[I-\alpha(S)]^{-1}). Equilibrium log prices satisfy

\[
\mathbf p^*=-L(S^*)[\mathbf a(S^*)-\mathbf m].
\]

The network choice condition is

\[
S_i^*\in\arg\min_{S_i}K_i(S_i,A_i(S_i),\mathbf P^*).
\]

## Main Mechanism
An input becomes more attractive when it raises set-specific productivity enough to offset its direct and indirect cost. Adopting it lowers the buyer’s unit cost, which lowers prices faced by downstream industries and can induce further adoption. In the dynamic model, one new product doubles each incumbent industry’s possible subsets, creating combinatorial technology opportunities and a network-driven growth channel.

## Common Propositions
- Equilibrium exists under the stated regularity assumptions; prices are unique and technology choices are generically unique.
- A productivity improvement or distortion reduction lowers prices through the Leontief inverse.
- Under technology-price single crossing, lower input prices or better technologies lead to weakly denser input sets.
- Laissez-faire network choices need not be efficient when distortions differ across industries or destroy resources.
- With suitable arrival and adoption conditions, the dynamic model can sustain growth through new input combinations.

## Comparative Statics Usually Available
- Lower (\mu_i) or higher (A_i(S_i)) lowers (P_i), directly and through downstream propagation.
- Lower prices of candidate inputs make supersets (S_i'\supset S_i) more attractive under single crossing.
- Larger complementarities among inputs make adoption responses more discontinuous and potentially more clustered.
- Faster arrival of new products increases the growth potential from recombination.

## Data Requirements
- Detailed input-output tables over time or firm/sector transaction data capable of identifying new input adoption.
- Prices, productivity, markups/taxes, sales, intermediate expenditure, and product entry dates.
- For dynamic validation: repeated observations on changes in input combinations and sector productivity growth.

## Estimation or Calibration
Map observed input expenditure shares into (\alpha(S)); estimate or calibrate set-productivity gains using input adoption events and productivity changes. Distortions can be mapped from markups, taxes, or wedges. The original quantitative exercise is illustrative; causal identification of adoption gains requires exogenous changes in input availability or price.

## Counterfactual Analysis
Change productivities, distortions, or the set of available inputs; recompute both network choices and equilibrium prices. Report fixed-network and endogenous-network counterfactuals separately to isolate the adjustment margin.

## Welfare Implications
Network adaptation can magnify productivity improvements by lowering input costs economy-wide. It can also be inefficient because private cost minimization does not internalize downstream gains and because heterogeneous distortions alter the social value of adoption.

## Welfare Decomposition
Decompose welfare changes into direct productivity/distortion effects evaluated at the initial network and the contribution of network reoptimization. A universal scalar formula is not available for arbitrary set technologies; the full equilibrium or a local envelope calculation is required.

## Common Modeling Pitfalls
- Treating (S_i) as a continuous input share when it is a discrete technology/input-set choice.
- Assuming denser networks are always efficient; extra inputs may be privately attractive but socially distorted.
- Ignoring genericity conditions and claiming unique link choices at knife-edge prices.
- Attributing observed adoption-productivity correlations causally without an input-availability or price instrument.

## How to Extend the Model
- Add countries and iceberg trade costs.
- Add firm heterogeneity within sectors, bilateral search, or fixed relationship costs.
- Introduce uncertainty over supplier productivity as in Kopytov et al.
- Allow directed innovation to determine which new products arrive.

## Example Research Questions This Model Can Support
- Do tariff reductions induce sectors to adopt new imported input categories and thereby lower downstream prices?
- Can the diffusion of digital services generate growth by expanding feasible input combinations?
- How do heterogeneous sectoral markups distort the density of an economy’s production network?

## Closely Related Model Families
Fixed input-output production networks; Oberfield input-output architecture; Kopytov et al. networks under uncertainty; Arkolakis-Huneeus-Miyauchi production-network formation.

## When This Model Is Not Appropriate
Do not use it when the main issue is matching particular buyers and suppliers, relationship-specific bargaining, delivery risk along known links, or high-frequency inventory adjustment. A fixed-network model is preferable when observed input sets are effectively invariant.
