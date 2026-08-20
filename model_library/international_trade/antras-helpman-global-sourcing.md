# Antràs-Helpman Global Sourcing

## Model Family Name
Heterogeneous Firms, Incomplete Contracts, and Global Organizational Choice

## Canonical Economic Question
How do firm productivity, headquarter intensity, wage differences, fixed organizational costs, and property rights determine domestic versus foreign sourcing and integration versus outsourcing?

## Verified References
- Antràs, Pol, and Elhanan Helpman. 2004. “Global Sourcing.” *Journal of Political Economy* 112(3): 552-580. [DOI](https://doi.org/10.1086/383099).

## When to Use This Model
- Use it when sourcing location and ownership mode are jointly endogenous.
- Use it to study sorting of heterogeneous firms into domestic outsourcing, domestic integration, offshore outsourcing, and foreign integration.
- Use it when relationship-specific investments and incomplete contracts are essential.

## Typical Primitives
- Northern final-good producers and potential component suppliers in North and South.
- Firm productivity (\varphi), sector headquarter intensity (\eta), CES demand parameter (\alpha), and productivity distribution (G).
- Northern and Southern wages, organizational fixed costs (f_k^l), and bargaining shares (\beta_k^l).
- Contractible up-front transfers but noncontractible relationship-specific headquarters and component investments.

## Timing
A potential entrant pays an entry cost and draws productivity; the final producer chooses supplier country and ownership; an up-front transfer secures participation; both parties invest noncooperatively; they bargain ex post; output is sold.

## Information Structure
Productivity is learned after entry. Investments and realized revenue are observable to the parties but not fully contractible or verifiable by courts. Organizational costs and bargaining rules are common knowledge.

## Agent Heterogeneity
Firms differ in productivity. Sectors differ in headquarter intensity. Locations differ in wages and contracting effectiveness; organizational modes differ in fixed cost and the final producer’s revenue share.

## Choice Variables
- Final producers choose exit, supplier location, integration versus outsourcing, and headquarter investment.
- Suppliers choose component investment.
- Entry, organizational cutoffs, consumption indices, and numbers of active firms are equilibrium outcomes.

## Constraints
- Relationship-specific investments cannot be fully contracted ex ante.
- Ex post surplus is divided according to ownership- and location-specific bargaining shares.
- The supplier’s participation constraint is satisfied through an up-front transfer.
- Free entry equates expected operating profit to the entry cost.

## Equilibrium Concept or Solution Concept
A subgame-perfect organizational equilibrium within each sector plus free entry. Productivity cutoffs sort firms across exit and feasible organizational forms; sectoral expenditure and entry close the equilibrium.

## Key Equations
Final output combines headquarters (h) and components (m):

\[
x=\varphi\left(\frac{h}{\eta}\right)^{\eta}
\left(\frac{m}{1-\eta}\right)^{1-\eta}.
\]

Under CES demand, revenue can be written as

\[
R=X^{\mu-\alpha}\varphi^{\alpha}
\left(\frac{h}{\eta}\right)^{\alpha\eta}
\left(\frac{m}{1-\eta}\right)^{\alpha(1-\eta)}.
\]

For ownership (k) and supplier location (l), equilibrium operating profit has the reduced form

\[
\pi_k^l(\varphi)=A_k^l(\eta,X)\varphi^{\alpha/(1-\alpha)}-w_N f_k^l,
\]

so intersections of profit schedules generate productivity cutoffs across organizational forms.

## Main Mechanism
Integration raises the final producer’s residual control and bargaining share but can weaken the supplier’s investment incentives and has higher fixed cost. Southern sourcing saves variable labor cost but entails higher organizational fixed cost. More productive firms can amortize higher fixed costs, creating ordered organizational sorting.

## Common Propositions
- The least productive entrants exit.
- In component-intensive sectors, active firms tend to outsource; more productive firms are more likely to source from the South.
- In headquarter-intensive sectors, integration can arise because stronger headquarters incentives are more valuable.
- Productivity dispersion and sector characteristics determine the prevalence of each organizational form.

## Comparative Statics Usually Available
- A lower Southern wage expands foreign sourcing, especially among high-productivity firms.
- Higher foreign organizational fixed costs shrink offshore sourcing.
- Greater headquarter intensity raises the relative appeal of organizational forms that give headquarters a larger surplus share.
- Better contracting or altered outside options change bargaining shares and organizational cutoffs.

## Data Requirements
- Firm productivity or sales, ownership mode, related-party versus arm’s-length imports, and supplier location.
- Sector measures of headquarter intensity and contractibility.
- Wages, fixed-cost proxies, and the distribution of firm size or productivity.

## Estimation or Calibration
Use ordered organizational shares across productivity bins and sectors to discipline fixed-cost rankings, productivity dispersion, and surplus shares. Identification requires separating location from ownership and treating related-party trade as an imperfect proxy for integration.

## Counterfactual Analysis
Change wages, organizational fixed costs, contracting institutions, or trade costs; recompute productivity cutoffs, entry, organizational shares, trade, and sectoral expenditure. Report extensive organizational switching separately from within-mode output changes.

## Welfare Implications
Lower sourcing costs and better investment incentives can raise output and variety, but incomplete contracting causes underinvestment. Organizational choices are privately optimal given bargaining and fixed costs, not necessarily socially efficient.

## Welfare Decomposition
Separate variable-cost savings, fixed organizational costs, entry/variety, and contractual underinvestment. Not applicable as a simple closed-form sufficient statistic; welfare requires solving sectoral entry and organizational sorting.

## Common Modeling Pitfalls
- Equating foreign sourcing with vertical integration; location and ownership are distinct choices.
- Treating related-party trade as a perfect ownership measure.
- Ignoring the up-front transfer when assigning ex ante rents.
- Assuming integration always improves investment incentives for both parties.

## How to Extend the Model
- Multiple suppliers, sequential stages, endogenous supplier search, or richer property rights.
- Quantitative global sourcing sets and fixed country-entry costs.
- Tariffs, policy uncertainty, or dynamic relationship capital.

## Example Research Questions This Model Can Support
- Which firms offshore through affiliates rather than independent suppliers?
- How do contracting institutions interact with headquarter intensity to shape intrafirm trade?
- Does a fall in foreign wages induce organizational upgrading or only location switching?

## Closely Related Model Families
Grossman-Helpman outsourcing; Antràs-Chor global value chains; heterogeneous firms and trade; global sourcing with country sets.

## When This Model Is Not Appropriate
Do not use the baseline when supplier discovery, many-country sourcing sets, sequential production stages, or persistent relationship dynamics are the main outcome. It is a sorting model, not a firm-to-firm network formation model.
