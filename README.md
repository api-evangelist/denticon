# Denticon

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

Denticon is a cloud-based dental practice management platform built for dental service organizations (DSOs) and multi-location group practices, owned and operated by Planet DDS (which also owns Cloud 9 Ortho and Apteryx imaging). The Denticon API program - relaunched in July 2024 on a new developer portal powered by Azure API Management - exposes RESTful APIs, webhooks, and batch data extracts covering patient, appointment, financial/ledger, insurance and claims (Revenue Cycle Management), clinical, and practice/office data, with OAuth 2.0 auth, an event-driven architecture for synchronized updates, and writebacks into Denticon. API access is partner-gated - Planet DDS must approve vendors and each client practice authorizes vendor access to specific office locations (OIDs). Public documentation exists, but keys and interactive access require program enrollment, so the endpoint surface below is modeled from the published API categories rather than a downloadable OpenAPI specification.

**Areas:** Dental · Practice Management · Healthcare · DSO · Electronic Health Records · Patient Data · Revenue Cycle Management · Partner API

## Denticon on APIs.io

Everything profiled for Denticon is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/denticon/](https://apis.io/providers/denticon/)** — or go straight to one of the APIs or properties below.

### APIs (7)

- [Denticon Patient API](https://apis.io/apis/denticon/denticon-patient-api/) — Create new patients, update and synchronize patient demographics and medical history, and upload patient documents into Denticon. Access is partner approved…
- [Denticon Appointments API](https://apis.io/apis/denticon/denticon-appointments-api/) — Read appointments on the schedule, query open scheduling availability, and book, confirm, reschedule, or cancel appointments to increase chair utilization.…
- [Denticon Revenue Cycle Management API](https://apis.io/apis/denticon/denticon-revenue-cycle-management-api/) — Retrieve insurance eligibility and claims data and post writebacks that automate insurance verification and revenue cycle workflows. Part of the July 2024…
- [Denticon Financial Ledger API](https://apis.io/apis/denticon/denticon-financial-ledger-api/) — Access patient ledger, account balance, and transaction data for analytics, patient billing, and payment reconciliation, with ledger writebacks into…
- [Denticon Clinical API](https://apis.io/apis/denticon/denticon-clinical-api/) — Read clinical data including medical history, treatment plans, and clinical notes, and write back updates to patient medical history and documents. Part of…
- [Denticon Practice API](https://apis.io/apis/denticon/denticon-practice-api/) — Retrieve practice configuration - office locations (OIDs), providers, and setup data - so that every query can be scoped to the correct location in…
- [Denticon Events and Webhooks API](https://apis.io/apis/denticon/denticon-events-webhooks-api/) — Event-driven architecture that pushes synchronized patient and appointment updates to partner-registered webhook endpoints when records are created,…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Denticon Domain Security](https://apis.io/security/denticon/denticon-domain-security/)
- [Denticon Trust Center](https://apis.io/security/denticon/denticon-trust-center/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.planetdds.com/denticon/)
- [Documentation](https://developer.planetdds.com/)
- [Sign up](https://developer.planetdds.com/)
- [Blog](https://www.planetdds.com/blog/)

## API Evangelist rating

**Kin Score 14.6** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 0.0 |
| Contract governance | 0.0 |
| Operational transparency | 0.0 |
| Developer ergonomics | 19.0 |
| Access clarity | 21.1 |

**Agent readiness 0.0** — human-only

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | — |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 8.6** — Health

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/denticon/](https://apis.io/providers/denticon/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Denticon: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/denticon/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
