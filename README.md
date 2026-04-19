# Allianz Trade (allianz-trade-online)

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
