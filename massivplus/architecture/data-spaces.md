# Data space architecture — MASSIV+

This document covers the IDS/Gaia-X infrastructure as it applies specifically to MASSIV+. For a broader explanation of data spaces, IDS, and Gaia-X, see `standards/ids-gaia-x.md`.

## How MASSIV+ uses the data space stack

MASSIV+ builds on IDS/Gaia-X principles but is scoped specifically to climate data (Scope 1–2) in manufacturing value chains.

```
┌─────────────────────────────────────────────────┐
│                  EU Data Strategy                │
│            (Data Act, Data Governance Act)        │
├─────────────────────────────────────────────────┤
│                    Gaia-X                        │
│          (Principles, federation, trust)          │
├─────────────────────────────────────────────────┤
│           IDS (International Data Spaces)         │
│    (Reference architecture, Dataspace Protocol,   │
│     Connectors, Metadata Broker, Rulebook)        │
├──────────┬──────────┬───────────┬───────────────┤
│ Catena-X │Factory-X │  Chem-X   │  MASSIV+      │
│(automotv)│(manufact)│ (chemical)│ (climate data)│
│          │          │           │  IDS/Gaia-X + │
│          │          │           │  AI guidance  │
│          │          │           │  + SME focus  │
└──────────┴──────────┴───────────┴───────────────┘
```

## Connectors ("beacons")

The IDS Connector is the core technical building block. In MASSIV+, connectors are called **beacons**. A beacon is a secure "data port" between a company's internal systems and the data space ecosystem. It handles authentication, access control, and usage policies.

**Implementation:** Eclipse Data Connector (EDC) — the same component used by Catena-X.

**Deployment options:**
- Large companies (Ronja, Anna personas) run their own connectors
- SMEs (Erik, Nisse personas) use hosted/managed connectors operated on their behalf — connector-as-a-service

This is a key differentiator from Catena-X, which assumes participants can run their own infrastructure.

## Metadata broker / catalog

A central catalog for discovering what data is available — without storing the actual data. This is how Ronja (Volvo Cars) can find that Erik and Nisse's Scope 1–2 data exists and request access to it.

## Data flow

```
Nisse's energy bill
        ↓
  AI guidance layer (AP3)
  [structures raw data → CCDM format]
        ↓
  Hosted beacon (IDS Connector)
  [Nisse's data, under his sovereignty]
        ↓
  Metadata broker
  [Ronja can discover it exists]
        ↓
  Ronja's beacon
  [requests access, receives data peer-to-peer]
        ↓
  Ronja's Scope 3 calculation
```

## Relationship to Catena-X

MASSIV+ is intentionally interoperable with Catena-X:
- Shared connectors: both use Eclipse Data Connector (EDC)
- Shared use cases: PCF (Product Carbon Footprint) overlaps
- Altiro Consulting and Mobility Sweden (MASSIV+ partners) are the Swedish Catena-X representatives

**Key difference:** Catena-X has been criticised for high complexity and low SME adoption. MASSIV+ explicitly addresses this by combining the same technical standard with simpler onboarding and AI-based guidance.

## Relevant standards

- Dataspace Protocol (DSP) v1.0.0 — published July 2025
- IDS Reference Architecture Model (RAM) — version 5 under development
- EU Data Act — entered into force September 2025

See `standards/ids-gaia-x.md` for deeper technical reference.
