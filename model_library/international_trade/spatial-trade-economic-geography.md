# Spatial Trade and Economic Geography

## Model Family Name
Continuous-Space Structural Gravity with Labor Mobility and Local Externalities

## Canonical Economic Question
How do trade costs, productivity, amenities, agglomeration, and congestion determine the spatial distribution of population, wages, market access, and welfare?

## Verified References
- Allen, Treb, and Costas Arkolakis. 2014. “Trade and the Topography of the Spatial Economy.” *Quarterly Journal of Economics* 129(3): 1085-1140. [DOI](https://doi.org/10.1093/qje/qju016).

## When to Use This Model
- Use it for infrastructure, market-access, or regional-development counterfactuals on a continuous or finely discretized geography.
- Use it when workers move across locations and local amenities and productivity jointly shape location choice.
- Use it to establish existence, uniqueness, or stability conditions for spatial equilibria.

## Typical Primitives
- Locations (i,j∈S), total mobile labor (L), iceberg cost function (T(i,j)), and one origin-specific variety per location.
- Exogenous productivity (\bar A(i)) and amenity (\bar u(i)).
- Productivity spillover (A(i)=\bar A(i)L(i)^\alpha) and amenity/congestion spillover (u(i)=\bar u(i)L(i)^\beta).
- CES elasticity across location varieties (σ>1).

## Timing
Static. Workers choose locations; competitive producers hire local labor; consumers source varieties from all locations; wages, price indices, population, trade, and utility equalization solve simultaneously.

## Information Structure
Complete information about geography, productivities, amenities, and trade costs. Workers are identical in the baseline and move until no inhabited location offers higher welfare.

## Agent Heterogeneity
Locations differ in productivity, amenities, connectivity, wages, and population. Workers are identical; discrete-choice taste heterogeneity can provide an isomorphic interpretation of amenity congestion.

## Choice Variables
- Workers choose residence.
- Consumers choose quantities of every location variety.
- Competitive firms choose labor and output.
- Population density, wages, trade flows, and welfare are equilibrium outcomes.

## Constraints
- Population integrates to the fixed aggregate labor supply.
- Income equals sales in every location.
- Utility is equalized across inhabited locations and no higher in uninhabited locations.
- Iceberg costs satisfy (T(i,i)=1); counterfactual routes must preserve a coherent bilateral cost surface.

## Equilibrium Concept or Solution Concept
A competitive spatial equilibrium satisfying goods-market clearing, aggregate labor clearing, and spatial utility equalization. Under stated restrictions, integral-operator methods establish existence, uniqueness, stability, and an iterative solution.

## Key Equations
Bilateral trade from (i) to (j) is

\[
X(i,j)=
\left[\frac{T(i,j)w(i)}{A(i)P(j)}\right]^{1-\sigma}
w(j)L(j),
\]

with price index

\[
P(j)^{1-\sigma}
=\int_S T(s,j)^{1-\sigma}A(s)^{\sigma-1}
w(s)^{1-\sigma}ds.
\]

Location welfare and market clearing are

\[
W(i)=\frac{w(i)}{P(i)}u(i),
\qquad
w(i)L(i)=\int_S X(i,s)ds,
\qquad
\int_S L(s)ds=L.
\]

## Main Mechanism
Geography affects consumer prices and producer market access through the entire trade-cost surface. Workers move toward high real wages and amenities. Productivity agglomeration attracts population, while congestion or deteriorating amenities disperse it; their balance governs uniqueness and stability.

## Common Propositions
- With exogenous productivity and amenities and regular geography, the spatial equilibrium is unique and can be computed iteratively.
- With endogenous spillovers, sufficient restrictions on dispersion relative to agglomeration deliver uniqueness and pointwise local stability.
- The local price index is a sufficient statistic for geographic location conditional on local fundamentals in the symmetric-cost case.
- Infrastructure can have effects through both direct trade-cost reductions and endogenous population relocation.

## Comparative Statics Usually Available
- Lower route costs improve market access and consumer access but reallocate population and wages across all connected locations.
- Stronger productivity spillovers increase spatial concentration and may create multiple equilibria.
- Stronger congestion/amenity dispersion stabilizes and spreads population.
- A larger (σ) makes trade flows more sensitive to route costs.

## Data Requirements
- Bilateral shipments among fine geographic units, population, wages/income, and local prices where available.
- Transportation networks, travel costs, terrain, or route-quality data.
- Local productivity and amenity proxies; land or housing data if congestion is structurally modeled.

## Estimation or Calibration
Estimate trade-cost topography from bilateral flows and transportation geography; recover productivity and amenity residuals from equilibrium conditions. Separating amenities from productivity requires population and wage information plus normalizations or excluded variation.

## Counterfactual Analysis
Modify the transportation network, local productivity, amenities, or spillover parameters; rebuild least-cost bilateral routes; solve wages and population until markets clear and utility equalizes. Check uniqueness or report alternative equilibria when agglomeration is strong.

## Welfare Implications
Welfare combines nominal wages, the CES price index, and amenities. Infrastructure benefits include market access and relocation effects; construction resource costs and externalities must be added before a policy is declared welfare improving.

## Welfare Decomposition
Decompose changes into consumer access/price index, producer market access/wages, amenities, productivity spillovers, and population reallocation. With externalities, competitive welfare changes need not equal social surplus changes.

## Common Modeling Pitfalls
- Holding population fixed in a model whose central equilibrium condition is labor mobility.
- Treating straight-line distance as the counterfactual cost when the network changes least-cost routes.
- Ignoring multiple equilibria under strong agglomeration.
- Double counting recovered productivity or amenities as independent observed fundamentals.

## How to Extend the Model
- Forward-looking capital and migration dynamics.
- Multiple sectors, input-output linkages, housing, land, commuting, or heterogeneous workers.
- International borders and policy barriers on top of physical geography.

## Example Research Questions This Model Can Support
- How does a highway change regional population and welfare through market access?
- How much spatial income variation is attributable to geographic location?
- When do productivity spillovers overturn the uniqueness of regional equilibrium?

## Closely Related Model Families
Armington structural gravity; dynamic spatial general equilibrium; quantitative trade counterfactuals; network general equilibrium.

## When This Model Is Not Appropriate
Do not use the static baseline when capital accumulation, migration transition costs, firm-level sourcing, or short-run immobility is the research object. Coarse regional data may also be inadequate for identifying route-level topography.
