---
name: scope3-accounting
description: Calculate Scope 1, 2, and 3 GHG emissions for real estate using GHG Protocol and PCAF methodology. Covers Category 13 (downstream leased assets), Category 15 (investments/financed emissions), emission factor selection, and carbon inventory preparation for GRESB, TCFD, CDP, and SEC reporting. Use when asked about carbon accounting, Scope 3, emissions calculations, PCAF, financed emissions, or GHG inventory.
---

# Scope 3 Carbon Accounting for Real Estate

## Category Routing — REQUIRED FIRST QUESTION

Ask before any calculation: "Are you the direct owner/operator of the building, or do you hold an investment interest (equity, debt, fund unit) in an entity that owns it?"

- **Owner/operator** → Category 13 (Downstream Leased Assets) if tenants occupy, or Scope 1/2 if owner-occupied
- **Investment fund / equity holder** → Category 15 (Investments) under PCAF methodology

These use completely different calculation methods, attribution boundaries, and PCAF requirements. Misclassification produces materially wrong reported figures.

**PCAF Data Quality Score — always disclose:**
| Score | Basis |
|-------|-------|
| 1 | Actual utility meter data (highest quality) |
| 2 | Invoiced energy use by asset manager |
| 3 | Property-level physical activity data |
| 4 | Asset-level model estimates |
| 5 | Modeled from floor area and asset class (lowest quality) |

**US Electricity — use eGRID subregion factors (NOT national average):**
Range: 0.15 tCO2e/MWh (CAMX/California) to 0.70 tCO2e/MWh (SRVC/Southeast). Ask for building state.

**Scope 2 — always report BOTH:**
- Location-based: grid average emission factors
- Market-based: contractual instruments (RECs, PPAs) — may be zero with PPAs

CSRD (ESRS E1) and GHG Protocol require both Scope 2 methods to be disclosed.

## GHG Protocol Scopes for Real Estate

### Scope 1 — Direct Emissions
On-site fuel combustion: natural gas boilers, diesel generators, fuel oil, propane
Formula: Scope 1 (tCO2e) = Fuel Use (MMBtu) × Emission Factor (tCO2e/MMBtu)

Key emission factors:
- Natural gas: 0.0531 tCO2e/MMBtu (EPA)
- Fuel oil #2: 0.0732 tCO2e/MMBtu
- Diesel: 0.0737 tCO2e/MMBtu
- Propane: 0.0619 tCO2e/MMBtu

### Scope 2 — Indirect (Purchased Energy)

**Location-based** (use regional grid average):
- US: EPA eGRID factors by NERC region (lbs CO2/MWh → tCO2e/kWh)
- EU: AIB residual mix factors by country
- UK: BEIS conversion factors

**Market-based** (use contracted source):
- RECs/GOs: zero emission factor if verified
- Power Purchase Agreements (PPAs): use generator-specific factor
- Default if no instruments: residual mix factor (usually higher than location-based)

GRESB/CRREM: report both location-based and market-based

### Scope 3 — Value Chain Emissions

**Category 13: Downstream Leased Assets**
Applies to: building owners/landlords (not occupiers)
Includes: tenant energy use in spaces landlord does not control

Method 1 (preferred): actual tenant meter data × emission factor
Method 2: floor area × national average intensity × emission factor
Method 3: asset-level estimates from energy audits

**Category 15: Investments / Financed Emissions**
Applies to: REITs, funds, asset managers
PCAF Standard (2023 joint release with GRESB/CRREM):

Formula: Financed Emissions = (Outstanding Loan or Equity / Property Value) × Property Emissions

Attribution factor = debt or equity exposure / current property value
Total portfolio = Σ (attribution factor × asset Scope 1+2+3 emissions)

Data quality scoring (1-5):
- Score 1: physical energy consumption data + emission factors
- Score 5: national averages without asset data

## Emission Factor Sources

### Electricity (Scope 2 location-based)
- US: EPA eGRID 2022 (download subregion factors at epa.gov/egrid)
- EU: IEA World Energy Statistics or national TSOs
- UK: BEIS conversion factors (updated annually)
- Canada: Environment Canada NIR

### Fuel (Scope 1)
- US: EPA Emission Factors for GHG Inventories (Table 1)
- EU: IPCC default factors (acceptable for corporate reporting)
- UK: BEIS/DESNZ conversion factors

### National Building Averages (Scope 3 Cat 13 Method 2)
- US: CBECS 2018 (EIA) — energy use by building type and climate zone
- EU: Eurostat energy balances by building type
- UK: BEIS non-domestic energy consumption statistics

## Reporting Boundaries

**Operational Control:** Report all assets where you have operational control
**Financial Control:** Report all assets consolidated into financial statements  
**Equity Share:** Report % matching ownership stake

Most RE companies use Operational Control for Scope 1+2, Equity Share for Scope 3 Cat 15.

## Carbon Inventory Checklist
☐ Define reporting boundary (operational/financial/equity)
☐ Collect Scope 1 fuel consumption by asset
☐ Collect Scope 2 electricity by asset (kWh)
☐ Select appropriate emission factors (location vs market-based)
☐ Collect/estimate tenant energy (Cat 13)
☐ Calculate financed emissions if asset manager (Cat 15)
☐ Apply PCAF data quality scores
☐ Document methodology
☐ Third-party verification (for GRESB, SEC)

## PCAF Data Quality Score by Method
| Score | Method |
|-------|--------|
| 1 | Physical activity data + emission factors |
| 2 | Energy consumption from bills + factors |
| 3 | Energy performance certificate (EPC) data |
| 4 | Property-type proxy data |
| 5 | Asset-class/national average data |

Target: portfolio weighted average score < 3
