# Relational Trade and Relationship Capital

## Model Family Name
Repeated Relational Contracting with Reputation and Limited Enforcement

## Canonical Economic Question
How can repeated buyer-seller relationships sustain trade when formal contracts are incomplete or weakly enforced, and how does accumulated relationship value affect deliveries during supply shocks?

## Verified References
- Macchiavello, Rocco, and Ameet Morjaria. 2015. “The Value of Relationships: Evidence from a Supply Shock to Kenyan Rose Exports.” *American Economic Review* 105(9): 2911-2945. [DOI](https://doi.org/10.1257/aer.20120141).
- Barrot, Jean-Noël, and Julien Sauvagnat. 2016. “Input Specificity and the Propagation of Idiosyncratic Shocks in Production Networks.” *Quarterly Journal of Economics* 131(3): 1543-1592. [DOI](https://doi.org/10.1093/qje/qjw018). The second paper is a related propagation application, not the canonical relational-contract model.

## When to Use This Model
- Use it when formal enforcement is limited and future trade disciplines current behavior.
- Use it when relationship age, reputation, or relationship-specific capital affects quantities, quality, or reliability.
- Use it to study how a negative supply shock is allocated across buyers of different relationship strength.

## Typical Primitives
- A buyer and seller who can trade repeatedly; outside options and spot-market alternatives.
- Relationship state (h_t): age, reputation, belief about reliability, or accumulated specific capital.
- Current order/delivery (q_t), transfer (p_t), stochastic supply capacity (s_t), and discount factor (\delta).
- Limited enforceability: a party can renege, underdeliver, delay payment, or terminate the relationship.
- Continuation values (V^C(h)) under cooperation and (V^P(h)) after deviation/punishment.

## Timing
1. The inherited relationship state and current supply/demand shock are observed.
2. The buyer places an order or promises a transfer.
3. The seller chooses production, quality, or delivery, possibly under a capacity shock.
4. Payment and observable performance occur.
5. Beliefs/reputation and relationship capital update; the relationship continues or terminates.

## Information Structure
Actions may be observable to the pair but not contractible in court. Reliability can be imperfectly known, so buyers update beliefs from delivery histories. The public/private nature of histories must be specified in extensions with multiple partners.

## Agent Heterogeneity
Relationships differ in age, accumulated surplus, outside options, buyer importance, seller reliability beliefs, and input specificity. Firms may maintain several relationships with different continuation values.

## Choice Variables
- Contracted and delivered quantity, quality, timing, and transfer.
- Whether to honor, renegotiate, or terminate the relationship.
- Relationship-specific investment and allocation of scarce supply across buyers.

## Constraints
- Physical supply/capacity: (\sum_b q_{bt}\leq s_t).
- Participation: each party’s relational value must exceed its outside option.
- Self-enforcement: continuation surplus must deter profitable one-shot deviations.
- Beliefs or relationship capital update according to observed histories.

## Equilibrium Concept or Solution Concept
A perfect public, perfect Bayesian, or sequential equilibrium of a repeated relational contract, depending on observability and hidden type/action. The canonical enforcement condition compares the gain from deviation with the discounted loss of future relationship surplus.

## Key Equations
For the seller, a generic self-enforcement condition is

\[
u_S(q_t,p_t,h_t)+\delta E_t[V_S^C(h_{t+1})]
\geq
u_S^D(q_t,p_t,h_t)+\delta E_t[V_S^P(h_{t+1})].
\]

The relationship value satisfies

\[
V_S(h_t)=\pi_S(h_t)+\delta E_t[V_S(h_{t+1})],
\]

with an analogous equation for the buyer. Cooperation is sustainable when

\[
\text{one-shot deviation gain}
\leq
\delta\,[V^C(h_{t+1})-V^P(h_{t+1})].
\]

Under a capacity shock, deliveries solve a constrained allocation problem over relationships, with the enforcement bound for each buyer acting as a relationship-specific lower or upper constraint.

## Main Mechanism
Current opportunism destroys future quasi-rents. Older or more successful relationships have larger continuation surplus and therefore support more trade or stronger reliability. During a negative supply shock, the seller trades off current scarcity against the future value of each relationship; this can generate nonmonotonic deliveries by relationship age when reputation-building and established-surplus channels pull in opposite directions.

## Common Propositions
- Limited enforcement caps trade at the quantity sustainable by continuation surplus.
- Relationship value and sustainable trade generally rise with a sufficiently favorable history or age.
- More patient parties, worse outside options after termination, or more relationship-specific surplus expand the self-enforcing set.
- A supply shock can reveal relationship value through differential delivery rather than only through prices.

## Comparative Statics Usually Available
- (\delta\uparrow) relaxes enforcement constraints and supports more trade/investment.
- Better outside options after deviation tighten relational enforcement.
- Greater relationship specificity raises the loss from termination but can also worsen holdup before investment.
- Higher shock persistence changes the value of preserving a relationship and the allocation of scarce supply.

## Data Requirements
- Relationship-level panel data with buyer and seller identities, start date/age, orders, deliveries, prices, quality, and termination.
- Exogenous supply disruptions and measures of outside options or market tightness.
- Input-specificity or relationship-investment measures when holdup is studied.

## Estimation or Calibration
Use exogenous supply shocks to infer which relationships receive priority and how this varies with age. Estimate survival/continuation values from relationship duration and switching. Structural estimation requires a specified punishment path, belief-updating rule, and outside-option process; these cannot be inferred from cross-sectional link data alone.

## Counterfactual Analysis
Change enforcement quality, discounting, outside options, shock frequency, or portability of relationship capital. Simulate delivery, termination, and investment policies over the relationship state distribution.

## Welfare Implications
Relational contracts permit mutually beneficial trade that formal enforcement cannot support, but they may lock firms into incumbent partners and discourage entry. Relationship-specific investment creates surplus while exposing investors to holdup.

## Welfare Decomposition
Decompose total surplus into current match surplus, enforcement-constrained unrealized surplus, relationship-specific investment returns, shock-sharing benefits, and switching/termination costs. Aggregate general-equilibrium effects are not identified by the bilateral model alone and are therefore not applicable without an embedding market model.

## Common Modeling Pitfalls
- Treating relationship age as exogenous; good matches survive longer.
- Equating reputation, relationship capital, and physical input specificity without defining the state variable.
- Writing an informal “trust” mechanism without an explicit deviation payoff and punishment path.
- Inferring relational enforcement from persistent trade when formal long-term contracts could generate the same pattern.

## How to Extend the Model
- Many buyers competing for a capacity-constrained seller.
- Endogenous partner search, switching costs, and portable versus nonportable capital.
- Private quality or hidden action with imperfect public monitoring.
- Embed bilateral relationships in a trade or production-network general equilibrium.

## Example Research Questions This Model Can Support
- Which buyers receive scarce deliveries after an exporter experiences a supply shock?
- Does stronger contract enforcement substitute for or complement relationship capital?
- How does supplier-specific investment affect switching after a tariff or geopolitical shock?

## Closely Related Model Families
Incomplete-contract global sourcing; Grossman-Helpman outsourcing; supplier switching; buyer-supplier search; input-specific shock propagation.

## When This Model Is Not Appropriate
Do not use it when transactions are fully enforceable, interactions are one-shot, partner discovery rather than enforcement is the only friction, or network propagation can be modeled without relationship-level continuation values.
