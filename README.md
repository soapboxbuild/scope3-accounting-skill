# Scope 3 Accounting Skill

GHG Protocol and PCAF real estate carbon accounting for Claude Code.

## What It Does

This skill teaches Claude to calculate and document greenhouse gas emissions for real estate portfolios per GHG Protocol and PCAF standards. It covers:

- **Scope 1** — Direct fuel combustion (natural gas, diesel, fuel oil, propane)
- **Scope 2** — Purchased electricity, both location-based and market-based
- **Scope 3 Category 13** — Downstream leased assets (tenant energy)
- **Scope 3 Category 15** — Financed emissions (PCAF methodology for REITs/funds)

Supports reporting for GRESB, TCFD, CDP, and SEC climate disclosure.

## Commands

| Command | Description |
|---------|-------------|
| `/calculate` | Full GHG inventory for a property or portfolio |
| `/financed-emissions` | PCAF Category 15 financed emissions for a portfolio |
| `/methodology` | Draft GHG accounting methodology statement for disclosure |

## Installation

```bash
npx skills add soapboxbuild/scope3-accounting-skill
```

## License

Apache-2.0
