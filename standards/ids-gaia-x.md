# IDS and Gaia-X — Technical standards

## What is a data space?

A data space is a shared, trusted environment for data exchange between organisations. Unlike a centralised database or data warehouse, no data is stored centrally — each participant keeps their data on their own infrastructure and shares it selectively through standardised interfaces. Think of it as a protocol rather than a platform: just as HTTP enables web pages without owning the content, a data space enables data sharing without owning the data.

Core principles:

- **Data sovereignty** — each organisation retains full control over its data and decides who gets access, to what, and under what conditions
- **Federated architecture** — no central data store; data is exchanged directly between participants (peer-to-peer)
- **Interoperability** — standardised interfaces, data models, and protocols allow different systems to communicate
- **Trust** — certified components, identity management, and usage policies ensure data exchange is secure and reliable

## IDS (International Data Spaces)

IDS is the technical standard and reference architecture that defines *how* data spaces work. Developed by the International Data Spaces Association (IDSA), founded in 2016 with roots in the Fraunhofer Institute.

Key components:

- **IDS Reference Architecture Model (RAM)** — defines roles, components, and information model. Version 5 under development
- **IDS Connector** — the core technical building block. Acts as a secure "data port" between a company's internal systems and the data space ecosystem. Handles authentication, access control, and usage policies
- **Dataspace Protocol (DSP)** — standardised protocol for data exchange, published as version 1.0.0 in July 2025. IDSA describes it as potentially as transformative as HTTP was for the internet
- **Metadata Broker** — central catalog for discovering what data is available, without storing the actual data
- **IDSA Rulebook** — covers functional, technical, operational, and legal requirements for designing and operating data spaces

IDS is industry-agnostic — it defines the *infrastructure* that all sector-specific data spaces are built on.

## Gaia-X

Gaia-X is a European initiative (launched 2019 by France and Germany) to create an open, federated, and interoperable data infrastructure based on European values of digital sovereignty. It is not a technical product but a framework of principles and specifications.

Gaia-X and IDS complement each other:
- Gaia-X defines the overarching European vision and principles
- IDS provides the concrete reference architecture and protocols
- Data spaces being built should be "Gaia-X compliant" and use IDS components

## Catena-X

Catena-X is the first large-scale data space implemented in practice, specifically for the automotive industry. Founded in 2021, it is the first end-to-end, multi-tier collaborative platform for open data exchange in the automotive industry.

Key aspects:

- Built on IDS architecture and follows Gaia-X specifications
- Founded by BMW, Mercedes-Benz, Siemens, Bosch, SAP, Fraunhofer, and others
- Uses the **Eclipse Data Connector (EDC)** as the technical component for data exchange

Use cases: Product Carbon Footprint (PCF), Traceability, Quality Management, Battery Passport.

Catena-X has become the reference model for the entire Manufacturing-X family.

## Manufacturing-X

Manufacturing-X is the umbrella initiative for data spaces across European manufacturing. Sector-specific initiatives under it:

- **Catena-X** — automotive (the pioneer)
- **Factory-X** — mechanical engineering / manufacturing
- **Chem-X** — chemical industry
- **Semiconductor-X** — semiconductor industry
- **MASSIV+** — climate data across manufacturing value chains

## EU Data Act

Entered into force September 2025. Sets global standards for data flows and sovereignty. Legislates the principles that data spaces already implement technically — the right to control your data and the conditions for sharing it.

## Architecture stack

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
└──────────┴──────────┴───────────┴───────────────┘
```

## MASSIV+ in this context

MASSIV+ builds on IDS/Gaia-X but focuses specifically on climate data (Scope 1–2) in manufacturing value chains.

Shared with Catena-X:
- Same underlying IDS architecture and Gaia-X compliance
- Focus on automotive industry as pilot environment
- PCF as a common use case
- Same connector technology (Eclipse Data Connector)

Differentiated from Catena-X:
- Catena-X has been criticised for high complexity and low SME adoption — MASSIV+ explicitly focuses on simple onboarding and AI-based guidance
- Narrower focus (climate data) but deeper (from energy data all the way to PCF calculation)
- Addresses the practical gap: how an SME without an IT department can actually participate

See `massivplus/architecture/data-spaces.md` for how these standards are implemented in the MASSIV+ platform.
