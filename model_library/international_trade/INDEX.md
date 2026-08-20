# International Trade Model Library Index

This file is a routing index, not a model card. Stage 3b must exclude it from model-family scoring.

## Cross-Library Routing Rule

When Stage 3b activates the international-trade route, it must scan the specialized cards below and the retained root trade cards, then jointly consider these general model cards:

| General card | Combine when |
|---|---|
| `../search-models.md` | Supplier discovery, reservation rules, or costly search is central |
| `../matching-models.md` | Partner selection, rematching, match surplus, or stability is central |
| `../dynamic-optimization-bellman.md` | Inherited relationships, switching costs, or transition paths are central |
| `../general-equilibrium-basics.md` | Prices, wages, output, market clearing, or aggregate welfare feed back across markets |

The matching card is a structural comparator, not an automatic substitute for trade-specific buyer-supplier formation. If a general card is not applicable, the Stage 3b scan record must explain why.

## Foundations and Quantitative Trade

| Model card | Primary use |
|---|---|
| `eaton-kortum-ricardian-gravity.md` | Multicountry Ricardian trade, gravity, technology and trade costs |
| `armington-structural-gravity.md` | National product differentiation, multilateral resistance, structural gravity |
| `acr-welfare-sufficient-statistics.md` | Gains from trade from domestic expenditure shares and trade elasticity |
| `caliendo-parro-multisector-trade.md` | Multisector input-output trade and tariff counterfactuals |
| `quantitative-trade-counterfactuals.md` | Exact-hat algebra and disciplined counterfactual implementation |

## Firms, Sourcing, and Global Value Chains

| Model card | Primary use |
|---|---|
| `ekk-firm-to-firm-trade.md` | Importer-exporter matching and firm-level labor-market incidence |
| `multiproduct-firms-trade.md` | Product scope, core competence, and product dropping after liberalization |
| `antras-helpman-global-sourcing.md` | Organizational form, incomplete contracts, and heterogeneous firms |
| `grossman-helpman-outsourcing.md` | Search, matching, and integration-versus-outsourcing equilibrium |
| `antras-chor-global-value-chains.md` | Sequential production, contractibility, and stage allocation |

## Production Networks and Supply Chains

| Model card | Primary use |
|---|---|
| `input-output-production-networks.md` | Exogenous input-output networks and shock propagation |
| `acemoglu-azar-endogenous-production-networks.md` | Endogenous supplier sets and sectoral network adjustment |
| `oberfield-input-output-architecture.md` | Firm-level supplier choice and emergent input-output architecture |
| `production-network-formation-trade-welfare.md` | Multicountry network formation, trade, and welfare |
| `buyer-supplier-search-matching.md` | Geographic supplier search and endogenous buyer-seller links |
| `relational-trade-and-relationship-capital.md` | Relational contracts, relationship capital, and holdup |
| `supplier-switching-and-network-reconfiguration.md` | Switching costs and transition paths after supply-chain shocks |
| `supply-chain-resilience-diversification.md` | Endogenous diversification and resilience investment |
| `network-general-equilibrium-welfare.md` | Nonlinear propagation, wedges, and welfare decomposition |

## Trade Policy

| Model card | Primary use |
|---|---|
| `trade-policy-shocks-quantitative-ge.md` | Tariff shocks in quantitative general equilibrium |
| `trade-policy-uncertainty.md` | Irreversible export entry under uncertain future policy |
| `tariff-pass-through-incidence.md` | Border-to-price transmission and distributional incidence |
| `comparative-advantage-optimal-trade-policy.md` | Optimal taxes in Ricardian comparative-advantage models |

## Dynamics and Space

| Model card | Primary use |
|---|---|
| `dynamic-export-market-entry.md` | Sunk export costs and dynamic participation |
| `spatial-trade-economic-geography.md` | Trade, geography, amenities, and spatial equilibrium |

## Existing Root Cards Retained for Compatibility

| Existing card | Relationship to this library |
|---|---|
| `../comparative-advantage-ricardian.md` | Classical Ricardian baseline |
| `../heckscher-ohlin.md` | Factor-endowment baseline |
| `../new-trade-theory-krugman.md` | Increasing returns and love of variety |
| `../melitz-firm-heterogeneity.md` | Heterogeneous-firm baseline |
| `../dynamic-spatial-general-equilibrium.md` | Dynamic spatial adjustment baseline |
| `../trade-labor-dynamics-china-shock.md` | Trade shocks and labor-market adjustment baseline |
