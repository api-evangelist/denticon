# Denticon (denticon)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
