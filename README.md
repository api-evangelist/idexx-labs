# IDEXX (idexx-labs)

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
