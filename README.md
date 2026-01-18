# Applied Valuation and Credit Risk Models

This repository contains self-directed financial modelling projects focused on asset-based valuation and credit risk analysis in capital-intensive businesses. The work emphasises discounted cash flow modelling, capital recovery dynamics, and scenario-based stress testing, with commercial aviation used as a primary case study due to its exposure to operating leverage, residual value risk, and structured financing.

The objective was not to produce stylised academic outputs, but to build internally consistent models that reflect how valuation and risk assessment are approached in practice across real assets.

---

## 1. Aircraft Asset Valuation Model (Excel)

### Purpose
The objective of this model is to value a single commercial aircraft using a discounted cash flow framework similar to those applied by aircraft lessors and structured finance teams. The analysis adopts a long-term ownership perspective and explicitly links lease economics, depreciation behaviour, and exit assumptions.

### Modelling Approach
- Lease cash flows are forecast explicitly over the assumed lease term.
- Aircraft value evolution is modelled using an economic depreciation approach, reflecting age, utilisation, and market maturity rather than accounting conventions.
- Residual value is estimated under base, downside, and stress scenarios and discounted as a terminal cash flow.
- The discount rate is constructed transparently using a weighted average cost of capital, with sensitivities used to test exposure to capital market assumptions.
- Lease Rate Factors are calibrated to ensure consistency between pricing, return requirements, and residual risk.

The model is structured to allow full transparency of assumptions and to make the interaction between lease pricing, residual value, and required return explicit.

### Files
- `Aircraft_Valuation_Model.xlsx`
- `Aircraft_Valuation_Methodology.pdf`

---

## 2. Airline Default Risk Model (Python)

### Purpose
This model assesses relative airline financial strength and potential distress risk through ratio analysis and scenario-based stress testing. The intent is not to predict bankruptcy mechanically, but to compare resilience across carriers under varying operating conditions.

### Methodology
- Financial statement data is ingested and processed using pandas.
- Liquidity, leverage, coverage, efficiency, and cash sustainability metrics are computed consistently across airlines.
- A scoring framework aggregates these indicators into a comparative risk ranking.
- Base, downside, and severe stress scenarios are applied to reflect adverse movements in demand, cost structure, and margins.
- Results are visualised to highlight cross-airline differences and sensitivity to stress assumptions.

The notebook is fully reproducible and structured to make each transformation and assumption explicit.

### Files
- `Airline_Default_Risk_Model.ipynb`

---

## Notes
All assumptions are documented directly within the models. Data used for the airline analysis is drawn from publicly available financial disclosures. The work is intended for academic demonstration and skills development rather than investment recommendation.
