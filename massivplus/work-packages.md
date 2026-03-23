# MASSIV+ — Work packages

Project period: 2025–2028 (Vinnova grant)

| WP | Focus | Lead | Budget |
|----|-------|------|--------|
| AP1 | Regulated trust and governance structure | Handelshögskolan Göteborg | 9.8 MSEK |
| AP2 | Data model and infrastructure | Icons Of | 7.8 MSEK |
| AP3 | AI-based guidance | Icons Of | 5.1 MSEK |
| AP4 | Pilot and validation in industrial value chains | Icons Of | 11.4 MSEK |
| AP5 | Dissemination, business model, and commercialisation | Massivplus AB | 3.1 MSEK |
| AP6 | Project management | GU Ventures | 1.9 MSEK |

**Total: ~39.1 MSEK**

---

## AP1 — Regulated trust and governance structure
**Lead:** Handelshögskolan Göteborg

Covers the legal, regulatory, and governance framework for the data space. Defines how trust is established between participants, what rules govern data sharing, and how compliance with IDS/Gaia-X requirements is certified.

---

## AP2 — Data model and infrastructure
**Lead:** Icons Of

The core technical work package. Covers:

- CCDM (Common Composite Data Model) — the shared data standard
- API specifications for data exchange
- IDS connector implementation and configuration ("beacons")
- Hosted/managed connectors for SMEs
- Metadata broker / catalog for data discovery
- Interoperability with Catena-X and Manufacturing-X

See `massivplus/architecture/data-model.md` and `massivplus/architecture/data-spaces.md`.

---

## AP3 — AI-based guidance
**Lead:** Icons Of

The AI layer sitting on top of the data infrastructure. Primarily designed for SME users (Erik and Nisse personas). Covers:

- SME onboarding guidance — what data to collect and how
- Automated data structuring from raw inputs (energy bills, ERP exports)
- Data quality checks and anomaly flagging
- Action recommendations (what to prioritise to reduce footprint)
- RAG-based question answering on sustainability standards

See `massivplus/architecture/ai-agent.md`.

---

## AP4 — Pilot and validation in industrial value chains
**Lead:** Icons Of

Runs the industrial pilots that validate the platform in real conditions. Targets:

- Minimum Viable Data Space: 2 large companies + 3 SMEs (TRL 7)
- Scaling to 50+ SMEs during the project period
- Pilot environment: automotive industry (Volvo Cars, Polestar as anchor companies)

See `massivplus/deliverables/pilot-plan.md`.

---

## AP5 — Dissemination, business model, and commercialisation
**Lead:** Massivplus AB

Covers how the initiative reaches beyond the project consortium, how it becomes financially self-sustaining, and how the governance and incentive model is designed for long-term operation.

Long-term structure:
- **Non-profit association** — governs the standard and collaboration framework
- **Massivplus AB** — commercially manages and develops data infrastructure, AI guidance, and value-added services

---

## AP6 — Project management
**Lead:** GU Ventures

Overall project coordination, reporting to Vinnova, and ensuring cross-WP alignment.
