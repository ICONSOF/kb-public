# MASSIV+ — User personas

The project defines four distinct user types representing the full spectrum of the supply chain. All design and UX decisions should be evaluated against these personas.

---

## Ronja — Large corporation

**Persona:** Ronja Windahl, Sustainability Procurement Manager, Volvo Cars

**User story:**
Ronja manages many thousands of suppliers, small and large, but mainly the 2,500 largest. Once a year she sends out a questionnaire for reporting to all suppliers. She then spends a lot of time reminding them to send in data, co-operating with buyers to chase responses. Low response rates, poor data quality, and immaturity among suppliers make it hard to gather, use, and compare data.

**Needs:**

- *Supplier data gathering* — a digital solution that intuitively guides suppliers and automatically sends out digital reminders. All supplier data using the same calculation method and format for comparability (also complementary and aligned with existing standards like Catena-X)
- *Data analysis* — customisable supply chain mapping to set up a value chain; capability for hotspot analysis to find where to focus supplier discussions and take actions with the greatest emissions impact

**Pain points:**
- Data today is inconsistent, incomplete, or simply absent
- Manual collection doesn't scale to 2,500 suppliers
- Needs to trust data quality before using it in statutory CSRD reports

---

## Anna — Large supplier (dual role)

**Persona:** Anna Celsing, Chief Sustainability Officer, Alfa Laval

**User story:**
Most probably has Microsoft Sustainability Manager, Position Green, or a similar system for internal data gathering. MASSIV+ solves her main problem: standardising data format and data sharing, both upstream to suppliers and downstream to clients. To save time and for comparability to make decisions in her own supply chain.

**Needs:**

- *Data input and sharing* — reporting to clients (Volvo Cars, AB Volvo, SKF, Maersk, etc.) is requested in many different shapes and forms. She wants to input data once and be able to share it, controlling what, how, and to whom
- *Supplier data gathering* — Anna has a lot of suppliers to collect data from in the same way. She needs the same type of solution as Ronja

**Pain points:**
- Simultaneously a data consumer (collecting from her own suppliers) and a data provider (sharing with her customers)
- Currently submits the same data in different formats to different customers
- Hard to stay consistent when standards and request formats differ per customer

---

## Erik — SME supplier

**Persona:** Erik Larsson, Tier 1 supplier of steel components to automotive OEM, 250 employees

**User story:**
Makes steel components mainly for Volvo AB and Scania trucks. Has increasing pressure from customers, stakeholders, and regulations to understand and report sustainability performance. Puts large effort into filling in manual supplier quality assurance forms on sustainability — considers the questions and their own answers to be rather arbitrary. No alignment across industry/customers; many different formats.

Has started collecting climate data from their own suppliers using custom surveys and Excel. Aims to add this data to their ERP. Three suppliers responded with 32, 78, and 99 CO2-eqv. per component. But what does that mean? 32 what? Not sure how to ask or what to do with the data.

**Needs:**
- Access to knowledge, capabilities, and resources
- To establish reliable and cost-efficient ESG accounting practices and tools
- Better understanding of what is important and what actions to take — ESG is a vast area

**Pain points:**
- No dedicated sustainability person; sustainability is someone's part-time hat
- Filling in different forms for each customer; answers feel arbitrary
- Has started collecting supplier data but can't interpret it

---

## Nisse — Small supplier (Kurts Mekaniska)

**Persona:** Nisse Jonsson, Kurts Mekaniska i Eslöv AB, Kundansvarig *(fictive)*

**User story:**
Kurts Mekaniska i Eslöv AB sells products (e.g. screws) to Volvo Cars from one factory in Skåne. They have no system, no knowledge about CO2 emissions, emission factors, CSRD, or sustainability. Don't have any resources or staff dedicated to it. They see reporting as a "necessary evil" — something they do to keep their clients or get a bank loan. They receive energy bills with kWh from their energy company but don't know how to re-calculate that into emissions.

**Needs:**

- *Data input and sharing* — simple guidance on how to gather data from energy bills. How to upload data and share it to clients. How to understand what their clients are even asking for
- Just wants to solve the client's ask and then not think more about it. When a client (e.g. Volvo Cars or Alfa Laval) asks for data — being able to say: "look here"

**Pain points:**
- No IT systems, no sustainability knowledge, no dedicated staff
- Can't afford to spend time or money on new systems
- One bad experience will cause permanent disengagement

---

## Design implications

- The AI guidance layer (AP3) is primarily designed around Erik and Nisse
- Hosted connectors exist specifically so Nisse doesn't have to run his own infrastructure
- The 15-minute onboarding target is benchmarked against Nisse's scenario
- Ronja and Anna are the primary users of the data space discovery and sharing features
- Anna's dual role (consumer + provider) is a key driver of the "input once, share to many" architecture requirement
