# Allianz Trade (allianz-trade-online)

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

Allianz Trade APIs enable businesses to automate trade credit insurance management including cover requests, credit limit monitoring, payment overdue reporting, claims management, and company credit grading. Built on secure REST architecture with OAuth2, the APIs support three business lines: Trade Credit Insurance, E-Commerce B2B, and Surety/Guarantee.

**Portal:** [https://developers.allianz-trade.com/](https://developers.allianz-trade.com/)

## APIs

### Allianz Trade Payment Overdues API

Report payment overdues, request extension periods, and manage debt rescheduling for trade credit insurance policies. Supports three overdue category types: OVD (report default), EXP (extension period), and RES (rescheduling/repayment plan).

- **Documentation:** [https://developers.allianz-trade.com/welcome-trade-credit-insurance-api-world/payment-overdues](https://developers.allianz-trade.com/welcome-trade-credit-insurance-api-world/payment-overdues)
- **OpenAPI:** [openapi/allianz-trade-payment-overdues.yaml](openapi/allianz-trade-payment-overdues.yaml)
- **JSON Schema:** [json-schema/trade-payment-overdues-overdue-schema.json](json-schema/trade-payment-overdues-overdue-schema.json)
- **JSON-LD Context:** [json-ld/allianz-trade-payment-overdues-context.jsonld](json-ld/allianz-trade-payment-overdues-context.jsonld)
- **Capability:** [capabilities/shared/payment-overdues.yaml](capabilities/shared/payment-overdues.yaml)

### Allianz Trade Company Grade API

Retrieve creditworthiness grades for clients and prospects after cover requests. Supports bulk operations for grading multiple companies simultaneously, enabling automated credit risk assessment within ERP systems.

- **OpenAPI:** [openapi/allianz-trade-company-grade.yaml](openapi/allianz-trade-company-grade.yaml)
- **JSON Schema:** [json-schema/trade-company-grade-company_grade-schema.json](json-schema/trade-company-grade-company_grade-schema.json)
- **JSON-LD Context:** [json-ld/allianz-trade-company-grade-context.jsonld](json-ld/allianz-trade-company-grade-context.jsonld)
- **Capability:** [capabilities/shared/company-grade.yaml](capabilities/shared/company-grade.yaml)

### Allianz Trade Claims API

Access and manage all insurance claims declared to Allianz Trade from within your ERP system. Retrieve claim status, submit new claims, and track claim progression for trade credit insurance policies.

- **OpenAPI:** [openapi/allianz-trade-claims.yaml](openapi/allianz-trade-claims.yaml)
- **JSON Schema:** [json-schema/trade-claims-claim-schema.json](json-schema/trade-claims-claim-schema.json)
- **JSON-LD Context:** [json-ld/allianz-trade-claims-context.jsonld](json-ld/allianz-trade-claims-context.jsonld)
- **Capability:** [capabilities/shared/claims.yaml](capabilities/shared/claims.yaml)

### Allianz Trade Policy API

Manage your trade credit insurance policy portfolio. Retrieve policy details, create joint insured policies, and manage policy configurations directly from your ERP or credit management system.

- **OpenAPI:** [openapi/allianz-trade-policy.yaml](openapi/allianz-trade-policy.yaml)
- **JSON Schema:** [json-schema/trade-policy-policy-schema.json](json-schema/trade-policy-policy-schema.json)
- **JSON-LD Context:** [json-ld/allianz-trade-policy-context.jsonld](json-ld/allianz-trade-policy-context.jsonld)
- **Capability:** [capabilities/shared/policy.yaml](capabilities/shared/policy.yaml)

## Generated Artifacts

| Directory | Count | Description |
|-----------|-------|-------------|
| `openapi/` | 4 | OpenAPI 3.0.3 specifications |
| `json-schema/` | 22 | JSON Schema (draft 2020-12) files |
| `json-structure/` | 22 | JSON Structure documentation files |
| `json-ld/` | 4 | JSON-LD 1.1 context files |
| `examples/` | 22 | Example request/response JSON files |
| `capabilities/shared/` | 4 | Per-API Naftiko capability definitions |
| `capabilities/` | 1 | Workflow capability composition |
| `rules/` | 1 | Spectral ruleset (22 rules) |
| `vocabulary/` | 1 | Domain vocabulary and taxonomy |

## Workflow Capabilities

The [trade-credit-management.yaml](capabilities/trade-credit-management.yaml) capability composition supports three business workflows:

- **Credit Risk Monitoring** — Grade buyer creditworthiness and report payment defaults
- **Claims Declaration** — Submit and track insurance claims after payment default
- **Policy Onboarding** — Register subsidiaries as joint insureds under policies

## Authentication

All APIs use OAuth2 client credentials flow:

- **Token URL:** `https://api.allianz-trade.com/oauth2/token`
- **Scopes:** `overdues:read`, `overdues:write`, `grades:read`, `grades:write`, `claims:read`, `claims:write`, `policy:read`, `policy:write`

## API Patterns

- **Pagination:** `pageSize` / `page` / `totalRequired` query parameters; `Total-Items` / `Total-Pages` response headers
- **Async Operations:** POST/PATCH/DELETE return `202 Accepted` with a `jobId`; poll `GET /jobs/{jobId}` until `status: processed`
- **Overdue Categories:** OVD (default), EXP (extension), RES (rescheduling)

## Common Resources

- **Website:** [https://www.allianz-trade.com/](https://www.allianz-trade.com/)
- **Developer Portal:** [https://developers.allianz-trade.com/](https://developers.allianz-trade.com/)
- **Getting Started:** [https://developers.allianz-trade.com/docs/getting-started](https://developers.allianz-trade.com/docs/getting-started)
- **Change Log:** [https://developers.allianz-trade.com/whatsnew](https://developers.allianz-trade.com/whatsnew)
- **Support:** api@allianz-trade.com

## Maintainer

Kin Lane — kin@apievangelist.com
