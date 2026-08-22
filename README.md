# IDEXX (idexx-labs)

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

IDEXX Laboratories is a global leader in veterinary diagnostics - reference laboratory testing, in-house analyzers (IDEXX VetLab Station), diagnostic imaging (IDEXX Web PACS), and practice management software (Cornerstone, Neo, and ezyVet, which IDEXX acquired in 2021). IDEXX connects a veterinary practice to its diagnostic ecosystem through **VetConnect PLUS** - a diagnostic results and ordering platform - and through partner integration APIs for Web PACS imaging and reference/in-house lab results.

**These developer integrations are partner-gated.** The developer portal at [developer.vetconnectplus.com](https://developer.vetconnectplus.com/) requires an authenticated login (the sign-in flow carries OAuth 2.0 parameters), and partner access is granted only after an approved IDEXX integration request submitted through IDEXX customer support or the [practice-management integration request form](https://www.idexx.com/en/veterinary/software-services/idexx-practice-management-software-integration-request-form/). IDEXX Web PACS "API Partner" integrations authenticate with a **Client ID, Client Secret, and Grant Type** issued by IDEXX customer support (OAuth 2.0-style client credentials).

IDEXX does **not** publish an open, unauthenticated API reference, OpenAPI description, or public API pricing. The logical APIs below are **modeled** from IDEXX's public product and integration pages and from PIMS partner configuration docs - not copied from a public endpoint reference.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/idexx-labs/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/idexx-labs/refs/heads/main/apis.yml)

## Access Model

- **Partner-gated:** no self-service signup; no public endpoint reference.
- **Prerequisite:** an IDEXX VetConnect PLUS account (obtained via IDEXX customer support).
- **Web PACS API Partner:** credentials (Client ID / Client Secret / Grant Type) issued by IDEXX support; the partner selects "API Partner" as the integration type in their PIMS.
- **Pricing:** contact-sales / quote-based for diagnostics and software; no public API pricing tier.

## Relationship to ezyVet

IDEXX owns **ezyVet** (acquired June 2021, including Vet Radar) alongside its Cornerstone and Neo PIMS. ezyVet is documented separately in this catalog (`all/ezyvet`) and has its own publicly documented, partner-gated RESTful API at developers.ezyvet.com. This IDEXX entry covers the IDEXX-branded diagnostic and imaging integration surfaces (VetConnect PLUS, Web PACS, reference/in-house labs), which are distinct from the ezyVet PIMS API.

## Tags

- Veterinary
- Diagnostics
- Reference Labs
- Diagnostic Imaging
- Animal Health
- Healthcare
- VetConnect PLUS
- Web PACS
- Partner Gated

## Timestamps

- **Created:** 2026-07-05
- **Modified:** 2026-07-05

## APIs (modeled - partner-gated, not from a public reference)

### IDEXX VetConnect PLUS Diagnostic Results API

Retrieve diagnostic results from IDEXX Reference Laboratories and IDEXX in-house analyzers (VetLab Station), including real-time test status updates and the full IDEXX diagnostic history for a patient, surfaced to practice management partners through VetConnect PLUS.

- **Human URL:** [https://www.idexx.com/en/veterinary/software-services/vetconnect-plus/](https://www.idexx.com/en/veterinary/software-services/vetconnect-plus/)
- **Base URL:** `https://developer.vetconnectplus.com`

### IDEXX VetConnect PLUS Diagnostic Orders API

Submit electronic test requests (orders) from a practice management system to IDEXX Reference Laboratories, configure in-house analyzer runs, and track order status through VetConnect PLUS.

- **Human URL:** [https://www.idexx.com/en/veterinary/software-services/vetconnect-plus/](https://www.idexx.com/en/veterinary/software-services/vetconnect-plus/)
- **Base URL:** `https://developer.vetconnectplus.com`

### IDEXX Web PACS Diagnostic Imaging API

The Web PACS "API Partner" integration lets an imaging or practice management partner send diagnostic imaging requests and link captured DICOM studies (x-ray, ultrasound, CT, MR, IO) back to the patient record for viewing in Web PACS. Authenticates with a Client ID, Client Secret, and Grant Type issued by IDEXX customer support.

- **Human URL:** [https://www.idexx.com/en/veterinary/diagnostic-imaging-telemedicine-consultants/web-pacs/](https://www.idexx.com/en/veterinary/diagnostic-imaging-telemedicine-consultants/web-pacs/)
- **Base URL:** `https://developer.vetconnectplus.com`

### IDEXX VetConnect PLUS Reference Data API

Reference resources that underpin ordering and results - the IDEXX test and panel catalog, analyte/test codes, units, and reference ranges - used to map a partner's requests and result displays to IDEXX diagnostics.

- **Human URL:** [https://www.idexx.com/en/veterinary/software-services/vetconnect-plus/](https://www.idexx.com/en/veterinary/software-services/vetconnect-plus/)
- **Base URL:** `https://developer.vetconnectplus.com`

### IDEXX VetConnect PLUS Authentication

OAuth 2.0-style authentication for IDEXX partner integrations. The developer portal is login-gated, and Web PACS API Partner integrations exchange a Client ID, Client Secret, and Grant Type (all issued by IDEXX customer support) for access.

- **Human URL:** [https://developer.vetconnectplus.com/](https://developer.vetconnectplus.com/)
- **Base URL:** `https://developer.vetconnectplus.com`

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/idexx-laboratories)
- [Website](https://www.idexx.com)
- [Documentation](https://developer.vetconnectplus.com/) (login-gated developer portal)
- [Software Integrations](https://software.idexx.com/integrations)
- [Integration Request](https://www.idexx.com/en/veterinary/software-services/idexx-practice-management-software-integration-request-form/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
