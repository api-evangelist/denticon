# Denticon (denticon)

Denticon is a cloud-based dental practice management platform built for dental service organizations (DSOs) and multi-location group practices. It is owned and operated by **Planet DDS**, which also owns Cloud 9 Ortho and Apteryx imaging. The Denticon API program was relaunched in July 2024 on a new developer portal (developer.planetdds.com) powered by Azure API Management, exposing RESTful APIs, an event-driven webhook architecture, and batch data extracts across patient, appointment, financial/ledger, insurance and claims (Revenue Cycle Management), clinical, and practice/office data, with OAuth 2.0 authentication and writebacks into Denticon.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/denticon/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/denticon/refs/heads/main/apis.yml)

## Access Model (Partner-Gated)

This is an honestly-modeled entry. Denticon's API is **not openly self-serve**:

- **Vendor approval:** Planet DDS must approve a partner/vendor into the API program before keys are issued. Prospective vendors apply through the Planet DDS "Partner with Us" / integrations process; approved vendors receive a demo account.
- **Client authorization:** Each client practice must log into Denticon and configure API Vendor Settings (Setup → Offices) to authorize which vendors may access which office locations (OIDs).
- **Scoping:** Denticon runs a multi-location single-database model, so every request is scoped by practice group (PGID) and office (OID).
- **Auth:** The new portal uses OAuth 2.0 best practices; the legacy `api.denticon.com` libraries use a Vendor Key + Auth/Client Key + PGID.

Public documentation exists, but the interactive specification and downloadable OpenAPI are behind portal enrollment. For that reason every API in `apis.yml` is marked `endpointsModeled: true` - the logical API groupings and capabilities are sourced from Planet DDS's published category descriptions, and no full endpoint surface or OpenAPI/AsyncAPI document has been fabricated.

## Ownership

Denticon is a **Planet DDS** product. Planet DDS's portfolio also includes Cloud 9 Ortho and Apteryx XVWeb imaging, plus Planet DDS Pay.

## Tags

- Dental
- Practice Management
- Healthcare
- DSO
- EHR
- Patient Data
- Revenue Cycle Management
- Partner API

## Timestamps

- **Created:** 2026-07-04
- **Modified:** 2026-07-04

## APIs (Modeled)

Endpoint surfaces are modeled from published API categories; exact routes require developer portal enrollment.

### Denticon Patient API
Create new patients, update and synchronize patient demographics and medical history, and upload patient documents.

### Denticon Appointments API
Read the schedule, query open availability, and book, confirm, reschedule, or cancel appointments; appointment-status writebacks update Denticon from external systems.

### Denticon Revenue Cycle Management API
Retrieve insurance eligibility and claims data and post writebacks that automate insurance verification and RCM workflows.

### Denticon Financial Ledger API
Access patient ledger, account balance, and transaction data for analytics, billing, and payment reconciliation.

### Denticon Clinical API
Read clinical data (medical history, treatment plans, clinical notes) and write back updates to patient records.

### Denticon Practice API
Retrieve practice configuration - office locations (OIDs), providers, and setup data - to scope requests correctly across locations.

### Denticon Events and Webhooks API
Event-driven outbound HTTP webhooks that push synchronized patient and appointment updates when records are created, modified, or cancelled - removing the need for polling.

## Pricing

No public pricing. Access is contact-sales / partner-enrollment through Planet DDS (phone 800-861-5098) and the developer portal.

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/planet-dds)
- [Website](https://www.planetdds.com/denticon/)
- [Documentation](https://developer.planetdds.com/)
- [Documentation (Legacy Libraries)](https://api.denticon.com/Home/GettingStarted)
- [Sign Up / Developer Portal](https://developer.planetdds.com/)
- [Partners / Integrations](https://www.planetdds.com/integrations/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
