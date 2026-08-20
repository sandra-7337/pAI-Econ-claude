# Heckscher-Ohlin Model

## Model Family Name
Factor-Endowment Trade with Stolper-Samuelson, Rybczynski, and Factor-Price Equalization

## Canonical Economic Question
How do cross-country differences in factor endowments determine trade patterns, production, and the distribution of real income across factors?

## Verified References
- Heckscher, Eli F. 1919. “The Effect of Foreign Trade on the Distribution of Income.” *Ekonomisk Tidskrift*; English translation in *Readings in the Theory of International Trade* (1949), 272-300. [ZBW catalog record](https://www.econbiz.de/10003573813).
- Ohlin, Bertil. 1933. *Interregional and International Trade*. Cambridge, MA: Harvard University Press. [Bibliographic record](https://books.google.com/books/about/Interregional_and_International_Trade.html?id=k60LAQAAIAAJ).
- Stolper, Wolfgang F., and Paul A. Samuelson. 1941. “Protection and Real Wages.” *Review of Economic Studies* 9(1): 58-73. [DOI](https://doi.org/10.2307/2967638).

## When to Use This Model
- Use it when relative factor abundance and sectoral factor intensity drive comparative advantage.
- Use it for real factor-return and distributional effects of goods-price or trade-policy changes.
- Use it to distinguish output responses to endowment changes from price responses to trade shocks.

## Typical Primitives
- Two countries, two goods, and two factors (capital K and labor L) in the canonical 2×2×2 model.
- Identical constant-returns technologies across countries and homothetic preferences.
- Sectoral unit-cost functions (c_j(w,r)) and no factor-intensity reversal.
- Factors mobile across domestic sectors and immobile internationally.

## Timing
Static. Firms choose cost-minimizing factor inputs; goods and factor prices and outputs solve simultaneously; trade clears world goods markets.

## Information Structure
Complete information and competitive price taking. There is no uncertainty or strategic interaction.

## Agent Heterogeneity
Countries differ in relative factor endowments; sectors differ in factor intensity; factor owners differ by ownership of capital or labor.

## Choice Variables
- Firms choose factor intensities and output.
- Households choose consumption.
- Goods prices, factor returns, production, and trade are equilibrium outcomes.

## Constraints
- Full employment: (\sum_jK_j=K) and (\sum_jL_j=L).
- Zero profit in active sectors: (p_j=c_j(w,r)).
- Goods-market clearing and trade balance.
- No factor-intensity reversal for the clean 2×2 theorems.

## Equilibrium Concept or Solution Concept
A competitive general equilibrium. Zero-profit conditions map goods prices into factor prices; full-employment conditions map endowments into outputs. Diversified countries inside the same cone can share factor prices.

## Key Equations
For active sectors,

\[
p_1=c_1(w,r),\qquad p_2=c_2(w,r).
\]

Cost-minimizing factor demands satisfy

\[
L_j=y_j\frac{\partial c_j(w,r)}{\partial w},
\qquad
K_j=y_j\frac{\partial c_j(w,r)}{\partial r}.
\]

Full employment gives

\[
\begin{bmatrix}
a_{L1}&a_{L2}\\
a_{K1}&a_{K2}
\end{bmatrix}
\begin{bmatrix}y_1\\y_2\end{bmatrix}
=
\begin{bmatrix}L\\K\end{bmatrix}.
\]

## Main Mechanism
An abundant factor is relatively cheap, lowering the relative unit cost of the good that uses it intensively. Trade raises the relative price of that export good, which feeds back into real factor returns through zero profit and into output through full employment.

## Common Propositions
- Heckscher-Ohlin: a factor-abundant country exports the good intensive in that factor under the theorem’s assumptions.
- Stolper-Samuelson: a rise in a good’s relative price raises the real return of its intensive factor and lowers the other factor’s real return.
- Rybczynski: at fixed goods prices, an increase in a factor endowment expands the output of its intensive good and contracts the other good.
- Factor-price equalization requires common technology, diversification, and common goods prices.

## Comparative Statics Usually Available
- Trade-induced goods-price changes map into magnified factor-price changes in the 2×2 diversified cone.
- Capital accumulation expands capital-intensive output at fixed prices.
- A labor endowment increase expands labor-intensive output at fixed prices.
- Complete specialization breaks the clean factor-price-equalization result.

## Data Requirements
- Sectoral factor inputs, factor payments, output, prices, and bilateral or net trade.
- Country factor endowments and sector factor intensities.
- Tariffs or other price shifters for causal tests of Stolper-Samuelson mechanisms.

## Estimation or Calibration
Calibrate unit input coefficients or production functions and recover factor abundance consistently across countries. Factor-content tests require compatible input-output and endowment data. Causal incidence needs exogenous goods-price or policy variation, not simple wage-trade correlations.

## Counterfactual Analysis
Change endowments, tariffs, or world goods prices; solve zero-profit and full-employment equations; check whether countries remain diversified. If a cone boundary is crossed, allow specialization and re-solve piecewise.

## Welfare Implications
Aggregate gains from trade can coexist with losses for owners of the scarce factor. Stolper-Samuelson is a local 2×2 result and does not guarantee a one-to-one winner/loser mapping with many goods, factors, nontraded goods, or mobility frictions.

## Welfare Decomposition
Decompose aggregate real-income change into terms of trade and production efficiency, then allocate income changes across factor owners. Compensation is not automatic; potential Pareto gains differ from actual household welfare.

## Common Modeling Pitfalls
- Conflating the HO trade-pattern theorem with Stolper-Samuelson incidence.
- Ignoring diversification cones and specialization.
- Assuming identical technologies when measured productivity differs.
- Applying the 2×2 sign theorem mechanically in a many-factor economy.

## How to Extend the Model
- Heckscher-Ohlin-Vanek factor content with many goods and factors.
- Specific factors for short-run immobility.
- Firm heterogeneity within comparative-advantage sectors.
- Skill-biased technology and nonhomothetic demand.

## Example Research Questions This Model Can Support
- Does a tariff-induced goods-price change benefit the factor used intensively in that sector?
- How does capital accumulation shift a country’s export composition?
- Are observed factor contents of trade consistent with measured endowment differences?

## Closely Related Model Families
Ricardian trade; specific-factors trade; Melitz with comparative advantage; trade and labor adjustment.

## When This Model Is Not Appropriate
Do not use the canonical model when technology differences, firm selection, increasing returns, input networks, or short-run sector-specific adjustment dominate endowment-driven comparative advantage.
