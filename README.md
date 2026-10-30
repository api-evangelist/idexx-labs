# IDEXX

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

IDEXX Laboratories is a global leader in veterinary diagnostics, offering reference laboratory testing, in-house analyzers (IDEXX VetLab Station), diagnostic imaging (IDEXX Web PACS), and practice management software (Cornerstone, Neo, and ezyVet, which IDEXX acquired in 2021). IDEXX connects the practice to its diagnostic ecosystem through VetConnect PLUS - a diagnostic results and ordering platform - and through partner integration APIs for Web PACS imaging and reference/in-house lab results. These developer integrations are partner-gated - the developer portal at developer.vetconnectplus.com requires an authenticated login, and partner access is granted only after an approved IDEXX integration request. Web PACS API Partner integrations authenticate with OAuth 2.0-style credentials (Client ID, Client Secret, and Grant Type) issued by IDEXX customer support. IDEXX does not publish an open, unauthenticated API reference, OpenAPI description, or pricing; the logical APIs below are modeled from IDEXX's public product and integration pages, not from a public endpoint reference.

**Areas:** Veterinary · Diagnostics · Reference Labs · Diagnostic Imaging · Animal Health · Healthcare · VetConnect PLUS · Web PACS

## IDEXX on APIs.io

Everything profiled for IDEXX is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/idexx-labs/](https://apis.io/providers/idexx-labs/)** — or go straight to one of the APIs or properties below.

### APIs (5)

- [IDEXX VetConnect PLUS Diagnostic Results API](https://apis.io/apis/idexx-labs/idexx-labs-vetconnect-plus-results-api/) — Retrieve diagnostic results from IDEXX Reference Laboratories and IDEXX in-house analyzers (VetLab Station), including real-time test status updates and the…
- [IDEXX VetConnect PLUS Diagnostic Orders API](https://apis.io/apis/idexx-labs/idexx-labs-vetconnect-plus-orders-api/) — Submit electronic test requests (orders) from a practice management system to IDEXX Reference Laboratories and configure in-house analyzer runs, then track…
- [IDEXX Web PACS Diagnostic Imaging API](https://apis.io/apis/idexx-labs/idexx-labs-web-pacs-imaging-api/) — The IDEXX Web PACS "API Partner" integration lets an imaging or practice management partner send diagnostic imaging requests and link captured DICOM studies…
- [IDEXX VetConnect PLUS Reference Data API](https://apis.io/apis/idexx-labs/idexx-labs-vetconnect-plus-reference-data-api/) — Reference resources that underpin ordering and results - the IDEXX test and panel catalog, analyte/test codes, units, and reference ranges - used to map a…
- [IDEXX VetConnect PLUS Authentication](https://apis.io/apis/idexx-labs/idexx-labs-vetconnect-plus-authentication/) — OAuth 2.0-style authentication for IDEXX partner integrations. The developer.vetconnectplus.com portal is login-gated (the sign-in flow carries OAuth…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Idexx Labs Domain Security](https://apis.io/security/idexx-labs/idexx-labs-domain-security/)
- [Idexx Labs Trust Center](https://apis.io/security/idexx-labs/idexx-labs-trust-center/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.idexx.com)
- [Documentation](https://developer.vetconnectplus.com/)
- [Blog](https://ir.idexx.com/news-events/press-releases)

## API Evangelist rating

**Kin Score 10.1** — minimal · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 0.0 |
| Contract governance | 0.0 |
| Operational transparency | 0.0 |
| Developer ergonomics | 9.5 |
| Access clarity | 7.9 |

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

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/idexx-labs/](https://apis.io/providers/idexx-labs/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for IDEXX: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/idexx-labs/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
