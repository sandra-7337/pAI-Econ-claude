# Supply-Chain Resilience and Supplier Diversification

## Model Family Name
Endogenous Resilience Investment, Network Thickness, and Risk-Sensitive Supplier Choice

## Canonical Economic Question
How much should firms invest ex ante in supplier survival and diversification across multiple production tiers, how does uncertainty reshape network structure, and why can private resilience differ from the social optimum?

## Verified References
- Grossman, Gene M., Elhanan Helpman, and Alejandro Sabal. 2024. “Optimal Resilience in Multitier Supply Chains.” *Quarterly Journal of Economics* 139(4): 2377-2425. [DOI](https://doi.org/10.1093/qje/qjae024).
- Kopytov, Alexandr, Bineet Mishra, Kristoffer Nimark, and Mathieu Taschereau-Dumouchel. 2024. “Endogenous Production Networks Under Supply Chain Uncertainty.” *Econometrica* 92(5): 1621-1659. [DOI](https://doi.org/10.3982/ECTA20629).

## When to Use This Model
- Use it when firms choose protective capacity and the number/diversity of suppliers before disruptions occur.
- Use it when disruptions propagate across multiple vertical tiers and resilience creates externalities downstream.
- Use the Kopytov et al. variant when firms trade expected productivity against supplier stability.

## Typical Primitives
- Tiers (s=0,\ldots,S), (N_s) potential firms per tier, and a representative household consuming differentiated final goods.
- Protective investment (r_s), survival probability (\phi_s(r_s)), and network thickness (\eta_s).
- Active firms (n_s=\phi_s(r_s)N_s) and active upstream relationships per buyer.
- Nested CES/Cobb-Douglas production, tier-specific labor/input shares (\gamma_s), substitution elasticities (\sigma_s), and final-demand elasticity (\varepsilon).
- Bilateral Nash-in-Nash bargaining and sequential bargaining across tiers.
- In the uncertainty variant: beliefs about mean productivity (\mu) and covariance (\Sigma), risk aversion (\rho), and endogenous input-share matrix (\alpha).

## Timing
1. Firms invest ex ante in protective capabilities and supplier links.
2. Disruptions realize and determine which firms survive.
3. Surviving firms bargain sequentially across adjacent tiers.
4. Inputs flow downstream, final goods are produced, and households consume.
5. The planner or government may choose transaction, resilience, and link-formation policies ex ante.

## Information Structure
Firms know disruption probabilities and network technology when investing but not survival realizations. In the beliefs-based model they price expected input costs and covariance with the stochastic discount factor, then choose techniques before productivity shocks realize.

## Agent Heterogeneity
Tiers differ in production shares, substitution elasticities, bargaining weights, disruption risk, and downstream importance. The baseline multitier model is symmetric within tier; the uncertainty model permits sector-specific mean productivity and covariance.

## Choice Variables
- Protective investment (r_s) and link/network thickness (\eta_s).
- Supplier/input quantities and bilateral transfers after survival.
- In the uncertainty model, input shares or production techniques (\alpha_i).
- Policy instruments: transaction, protection, and network-formation subsidies/taxes.

## Constraints
- Aggregate labor covers manufacturing, protective investment, and link formation:

\[
\sum_{s=0}^S N_s r_s+\sum_{s=1}^S N_s k_s\eta_sN_{s-1}
+\sum_{s=0}^S\phi_s(r_s)N_s l_s\leq L.
\]

- Each tier’s downstream deliveries cannot exceed output of surviving upstream firms.
- Bargaining outcomes must be bilaterally optimal given negotiations in other links.
- Survival probabilities and matching/link counts must be feasible.

## Equilibrium Concept or Solution Concept
A general equilibrium with ex-ante resilience and link investments, stochastic survival, and sequential Nash-in-Nash bargaining. The planner’s allocation internalizes all downstream effects. In Kopytov et al., equilibrium is a choice of production techniques and stochastic prices/allocations satisfying firm, household, unit-cost, and market-clearing conditions; under their assumptions it is unique and efficient.

## Key Equations
The number of surviving firms and upstream relationships for a tier-(s) producer are

\[
n_s=\phi_s(r_s)N_s,
\qquad
n_s^u=\eta_s\phi_{s-1}(r_{s-1})N_{s-1}.
\]

With symmetric final varieties, the household’s CES welfare index is

\[
W=n_S^{\varepsilon/(\varepsilon-1)}x_S.
\]

The optimal transaction subsidy factor in Grossman-Helpman-Sabal satisfies, for (s\geq1),

\[
T_s=\frac{1}{\gamma_s+(1-\gamma_s)\mu_{s-1}}<1,
\]

where (\mu_{s-1}) is the inherited bargaining markup term; the most-upstream transaction has (T_0=1) in the baseline.

In the uncertainty model, the first-order welfare response to mean productivity remains Domar-weighted:

\[
\frac{dW}{d\mu_i}=\omega_i,
\]

while equilibrium network reorganization changes expected GDP and its variance beyond the fixed-network response.

## Main Mechanism
Protecting or adding an upstream supplier benefits not only its direct customer but every downstream tier. Bilateral bargaining and decentralized investment generally fail to internalize this cascade. Under uncertainty, firms substitute toward stable but potentially expensive suppliers, lowering volatility at the cost of average output. Resilience therefore trades productive efficiency against exposure and depends on network position.

## Common Propositions
- Private and social incentives differ for transaction quantities, protective investment, and network thickness.
- Efficient resilience and link investment depend on cumulative downstream input shares and substitution elasticities.
- When transaction subsidies are unavailable, second-best resilience subsidies are typically larger farther upstream under the paper’s bargaining-weight condition.
- Greater uncertainty tilts sourcing toward stable suppliers, often reducing macro volatility and expected output simultaneously.

## Comparative Statics Usually Available
- More effective protection (\phi_s'(r_s)) raises optimal resilience investment.
- Lower substitutability among inputs increases the social value of supplier survival and network thickness.
- Larger downstream input shares raise the value of protecting upstream tiers.
- Higher covariance with bad aggregate states makes a supplier less attractive even at a low expected price.

## Data Requirements
- Multitier supplier-customer data, firm/tier locations, disruption and survival histories, input shares, and bargaining/payment information.
- Protective investment, inventories, dual sourcing, qualification costs, and link counts.
- For uncertainty calibration: time series of sectoral productivity means/covariances and input-output shares.

## Estimation or Calibration
Calibrate tier technologies and elasticities from input-output accounts; survival technologies from disruption and investment data; network thickness from supplier counts; bargaining weights from price/cost margins. Estimate risk-sensitive network responses from changes in input shares following shifts in supplier volatility.

## Counterfactual Analysis
Compare laissez-faire, first-best, and restricted second-best policies. Shock disruption probabilities, covariance, protection effectiveness, or supplier concentration. Resolve both ex-ante investments and post-disruption bargaining rather than changing survival probabilities while holding the network fixed.

## Welfare Implications
Resilience is not synonymous with maximum redundancy. Extra links and protection consume resources; optimal policy balances these costs against downstream survival and variety benefits. Private firms can underinvest because they do not capture downstream gains, although business-stealing and bargaining wedges can create offsetting forces.

## Welfare Decomposition
Separate expected consumption/variety, manufacturing output, protection cost, link-formation cost, disruption losses, double marginalization, bargaining transfers, and network externalities. In risk-sensitive models also separate expected output from output variance and the household’s risk adjustment.

## Common Modeling Pitfalls
- Treating diversification, inventory, capacity, geographic relocation, and protective investment as one undifferentiated “resilience” variable.
- Counting transfer payments or tariff revenue as real resource losses.
- Ignoring tier position when applying a uniform resilience subsidy.
- Inferring optimal diversification from lower volatility without valuing the associated expected-output cost.

## How to Extend the Model
- International sourcing, tariffs, geopolitical hazards, and correlated regional disruptions.
- Dynamic rebuilding, learning, and supplier switching costs.
- Asymmetric firms within tiers and endogenous vertical integration.
- Inventories, capacity reservation, financial constraints, and default.

## Example Research Questions This Model Can Support
- Should upstream semiconductor suppliers receive larger resilience subsidies than downstream assemblers?
- How does correlated geopolitical risk change optimal supplier diversification?
- When does dual sourcing reduce welfare because qualification and relationship costs are large?

## Closely Related Model Families
Supplier switching; Kopytov et al. endogenous networks under uncertainty; fixed input-output propagation; network welfare; global sourcing.

## When This Model Is Not Appropriate
Do not use it when disruptions are realized before any investment, when sourcing is frictionless spot purchasing, or when the research question concerns ordinary price substitution without failure risk or network externalities.
