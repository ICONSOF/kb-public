# Data model — CCDM

## What it is

The **CCDM (Common Composite Data Model)** is the shared data standard at the heart of MASSIV+. It defines how climate data is structured, calculated, and exchanged between participants in the data space.

## Foundations

CCDM builds on existing frameworks with MASSIV+-specific extensions:

- **WBCSD/PACT** — Partnership for Carbon Transparency; product-level carbon accounting
- **Carbon Call** — cross-industry initiative for consistent carbon accounting
- **Asset Administration Shell (AAS)** — IEC/ISO standard for digital representation of assets

MASSIV+ extensions cover:
- Organisational-level emissions
- Asset-level emissions
- Product-level emissions (PCF)

## Scope

The CCDM focuses on **Scope 1 and Scope 2** emissions:
- **Scope 1** — direct emissions from owned or controlled sources
- **Scope 2** — indirect emissions from purchased energy

When shared across the supply chain, these become the building blocks for Scope 3 calculations by downstream companies.

## Alignment with reporting standards

The data model is designed to be compatible with:
- GHG Protocol (see `standards/ghg-protocol.md`)
- ISO 14067 (PCF calculation)
- ESRS E1 (see `standards/esrs-e1.md`)
- CSRD reporting requirements

---

*This file needs to be populated with the actual CCDM entity model, field definitions, and calculation methodology as AP2 progresses. Add schema diagrams, entity relationships, and worked examples.*
