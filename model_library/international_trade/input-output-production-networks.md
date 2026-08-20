# Input-Output Production Networks

## Model Family Name
Static Multisector General Equilibrium with an Exogenous Production Network

## Canonical Economic Question
How do sector- or firm-level supply and demand shocks propagate through direct and indirect input-output linkages, and when can microeconomic disturbances generate aggregate fluctuations?

## Verified References
- Carvalho, Vasco M., and Alireza Tahbaz-Salehi. 2019. “Production Networks: A Primer.” *Annual Review of Economics* 11: 635-663. [DOI](https://doi.org/10.1146/annurev-economics-080218-030212).
- Acemoglu, Daron, Vasco M. Carvalho, Asuman Ozdaglar, and Alireza Tahbaz-Salehi. 2012. “The Network Origins of Aggregate Fluctuations.” *Econometrica* 80(5): 1977-2016. [DOI](https://doi.org/10.3982/ECTA9623).

## When to Use This Model
- Use it when buyer-supplier or sectoral input shares can be treated as fixed over the counterfactual horizon.
- Use it to trace direct and indirect propagation, construct exposure measures, or aggregate productivity shocks.
- Use it as the fixed-network benchmark before adding supplier choice, substitution, search, or relationship dynamics.

## Typical Primitives
- Industries (i,j=1,\ldots,n), one primary factor (labor in the baseline), and a representative household.
- Hicks-neutral productivity (z_i>0), labor share (\alpha_i>0), input shares (a_{ij}\geq0), and final-demand shares (\beta_i\geq0).
- Cobb-Douglas constant-returns production and logarithmic final demand in the canonical baseline.
- The input-output matrix (A=[a_{ij}]), with row sums below one so that its spectral radius is below one.
- State/shock variables: sectoral productivity (\log z_i), final-demand shocks, or wedges. The network (A) is a parameter, not a choice.

## Timing
Static. Productivities and demand shifters are realized; competitive firms choose inputs; the household chooses consumption; prices and quantities clear simultaneously.

## Information Structure
Complete information. Firms and households observe technologies, shocks, prices, and the fixed input-output matrix. There is no strategic or private information.

## Agent Heterogeneity
Industries differ in productivity, labor shares, input dependence, final-demand weights, sales, and network centrality. Firms within an industry are represented by a competitive sectoral producer.

## Choice Variables
- Firms choose labor (l_i) and intermediate quantities (x_{ij}).
- The household chooses final consumption (c_i).
- Prices (p_i), the wage (w), output (y_i), and expenditures are equilibrium objects.

## Constraints
- Technology: constant returns require (\alpha_i+\sum_j a_{ij}=1).
- Firm budget/profit condition under perfect competition: revenue equals labor plus intermediate expenditure.
- Goods-market clearing: (y_j=c_j+\sum_i x_{ij}).
- Labor-market clearing: total labor demand equals the household endowment.

## Equilibrium Concept or Solution Concept
A competitive general equilibrium in which the household maximizes utility, each sector minimizes unit cost or maximizes profit, and all goods and factor markets clear. Given the baseline Cobb-Douglas assumptions and (\rho(A)<1), relative prices and Domar weights have closed forms involving the Leontief inverse.

## Key Equations
Baseline production:

\[
y_i=z_i\,\zeta_i l_i^{\alpha_i}\prod_{j=1}^n x_{ij}^{a_{ij}}.
\]

Let (\widehat p_i=\log(p_i/w)), (\varepsilon_i=\log z_i), and (L=(I-A)^{-1}=\sum_{k=0}^{\infty}A^k). Unit-cost pricing gives

\[
\widehat{\mathbf p}=A\widehat{\mathbf p}-\boldsymbol\varepsilon,
\qquad
\widehat{\mathbf p}=-L\boldsymbol\varepsilon.
\]

With Cobb-Douglas final demand, Domar weights satisfy

\[
\boldsymbol\lambda=(I-A^\top)^{-1}\boldsymbol\beta,
\qquad
\lambda_i=\frac{p_i y_i}{GDP}.
\]

The first-order aggregate productivity result is

\[
d\log GDP=\sum_i\lambda_i\,d\log z_i.
\]

## Main Mechanism
A supply shock raises the affected input’s price and propagates downstream to customers, customers’ customers, and so on. The relevant exposure is the Leontief inverse rather than the direct input share. In the Cobb-Douglas one-factor benchmark, demand shocks instead propagate upstream because higher demand raises purchases from direct and indirect suppliers.

## Common Propositions
- The Leontief inverse exists and is nonnegative if the network matrix has spectral radius below one.
- The response of sector (i)'s log output or price to sector (j)'s productivity shock is governed by (L_{ij}).
- A sector’s Domar weight is a sufficient statistic for the first-order effect of its productivity shock on aggregate real value added.
- Network asymmetry and concentration can prevent idiosyncratic shocks from averaging out.

## Comparative Statics Usually Available
- A larger (a_{ij}) raises sector (i)'s direct and indirect exposure to shocks from (j).
- Longer or denser upstream chains increase relevant elements of (L) and amplify downstream supply shocks.
- Lower substitution elasticities than Cobb-Douglas generally strengthen quantity responses to adverse bottleneck shocks.
- Greater concentration of Domar weights raises the variance contribution of micro shocks.

## Data Requirements
- National or international input-output tables, use tables, or firm-to-firm transaction data.
- Gross output, value added, intermediate expenditures, final demand, employment, prices, and sectoral productivity shocks.
- For international applications: country-sector bilateral intermediate flows and trade costs.

## Estimation or Calibration
Calibrate (A) from intermediate expenditure shares, (\beta) from final expenditure shares, and factor shares from national accounts. Identify shocks using productivity residuals, natural disasters, tariff changes, or other exogenous supply/demand variation. Elasticities outside the Cobb-Douglas benchmark require external estimates or structural estimation.

## Counterfactual Analysis
Hold (A) fixed, change productivities, final demand, factor supplies, or wedges, and resolve prices and quantities. Report both direct effects and effects propagated by (L). Large shocks should be solved nonlinearly if technologies are not Cobb-Douglas.

## Welfare Implications
In an efficient competitive benchmark, real-income changes reflect productivity and terms-of-trade effects. With markups, taxes, rationing, or other wedges, the same physical network may amplify misallocation as well as shocks.

## Welfare Decomposition
At first order in an efficient economy, welfare/output changes decompose into Domar-weighted productivity shocks. For distorted or large-shock economies, this first-order decomposition is incomplete; reallocation, substitution, and wedge-interaction terms must be added. Use `network-general-equilibrium-welfare.md` for that case.

## Common Modeling Pitfalls
- Treating a direct input coefficient as total exposure instead of using the Leontief inverse.
- Reversing matrix orientation: (a_{ij}) is input (j)'s share in producer (i)'s costs.
- Applying Hulten’s first-order result to large shocks or distorted equilibria without qualification.
- Holding input shares fixed when the research question is explicitly about supplier switching or network formation.

## How to Extend the Model
- CES or nested-CES technologies with endogenous expenditure shares.
- Multiple primary factors, inventories, capacity constraints, markups, or financial frictions.
- Endogenous link formation as in Acemoglu-Azar, Oberfield, or Arkolakis-Huneeus-Miyauchi.
- Country-sector trade blocks and tariffs as in Caliendo-Parro or Baqaee-Farhi.

## Example Research Questions This Model Can Support
- Which upstream sectors contribute most to the aggregate effect of a semiconductor disruption?
- How do foreign sectoral shocks propagate through domestic intermediate-input use?
- Does observed network concentration make aggregate volatility sensitive to a small set of suppliers?

## Closely Related Model Families
Acemoglu-Azar endogenous networks; Oberfield input-output architecture; Caliendo-Parro multisector trade; Baqaee-Farhi nonlinear network welfare; supply-chain resilience models.

## When This Model Is Not Appropriate
Do not use the fixed-network baseline when link creation, supplier replacement, inventories, strategic bargaining, default cascades, or endogenous product scope is the central outcome. It is also inadequate for large counterfactuals when input substitution materially changes (A).
