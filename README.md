# Bud Financial (bud-co)

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

Bud Financial (formerly Bud, thisisbud.com) is a UK-based fintech infrastructure company providing AI-driven Open Banking aggregation, transaction enrichment, categorization, affordability assessment, and payment initiation APIs. The Bud platform unifies Open Banking connections to UK and EU ASPSPs behind a single REST API and layers AI/ML-powered enrichment, categorization, merchant identification, affordability scoring, income/expenditure analysis, and actionable financial insights on top of raw transaction data. Banks, lenders, and consumer fintechs use Bud for KYC/AML checks, lending decisions, money management, and embedded payments.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/apis.yml)

## Tags

- Open Banking
- Transaction Enrichment
- Categorization
- Affordability
- Payments
- AISP
- PISP
- Financial Data
- FinTech
- UK
- AI
- Machine Learning

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Bud Connect API

Open Banking aggregation API providing unified access to UK and EU ASPSP connections. Initiate consents through Bud's hosted Bud Connect gateway or build a native flow with the underlying authorisation, refresh, consent management, and reconfirmation endpoints. Bud handles the heterogeneity of ASPSP integrations behind a single set of asynchronous task-based endpoints, with webhook callbacks for connection, refresh, and consent events.

- **Human URL:** [https://docs.thisisbud.com](https://docs.thisisbud.com)
- **Base URL:** `https://api-sandbox.thisisbud.com`

#### Tags

- Open Banking
- AISP
- Account Aggregation
- Consent

#### Properties

- [Documentation](https://docs.thisisbud.com)
- [OpenAPI](openapi/bud-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bud-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bud-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bud First-Party Ingestion API

Push your own first-party account and transaction data into the Bud platform for enrichment, categorization, and insights without requiring an Open Banking consent. Supports synchronous and asynchronous ingestion, account open/close/reopen, and transaction book/decline lifecycle events.

- **Human URL:** [https://docs.thisisbud.com](https://docs.thisisbud.com)
- **Base URL:** `https://api-sandbox.thisisbud.com`

#### Tags

- Ingestion
- Transactions
- Accounts

#### Properties

- [Documentation](https://docs.thisisbud.com)
- [OpenAPI](openapi/bud-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bud-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bud-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bud Customers Platform API

Create, retrieve, batch-create, and manage end-user customer records on the Bud platform. Supports V1, V2, and V3 customer endpoints, idempotent identifiers, customer context configuration, and asynchronous task tracking.

- **Human URL:** [https://docs.thisisbud.com](https://docs.thisisbud.com)
- **Base URL:** `https://api-sandbox.thisisbud.com`

#### Tags

- Customers
- Identity
- Platform

#### Properties

- [Documentation](https://docs.thisisbud.com)
- [OpenAPI](openapi/bud-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bud-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bud-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bud Financial Data API

Retrieve enriched accounts, transactions, balances, and authorised payments. Bud's AI/ML enrichment engine attaches category, merchant, geolocation, and recurrence metadata to every transaction. Financial V3 endpoints expose the latest enriched schema with transaction-date ranges and per-account balance history.

- **Human URL:** [https://docs.thisisbud.com](https://docs.thisisbud.com)
- **Base URL:** `https://api-sandbox.thisisbud.com`

#### Tags

- Accounts
- Transactions
- Balances
- Enrichment

#### Properties

- [Documentation](https://docs.thisisbud.com)
- [OpenAPI](openapi/bud-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bud-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bud-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/bud-transaction-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/bud-account-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/bud-co-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Bud Enrichment API

Access Bud's enrichment resources: category models, category and merchant taxonomies, aggregated category and merchant totals, essential-spending statistics, and correction endpoints for re-labelling categories and merchants on individual transactions. Custom buckets let you group categories or merchants into your own reporting groupings.

- **Human URL:** [https://docs.thisisbud.com](https://docs.thisisbud.com)
- **Base URL:** `https://api-sandbox.thisisbud.com`

#### Tags

- Enrichment
- Categorization
- Merchants
- Aggregations

#### Properties

- [Documentation](https://docs.thisisbud.com)
- [OpenAPI](openapi/bud-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bud-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bud-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bud Financial Insights API

Generate deep insights from transaction data: actionable balance, income, and spending insights; custom insight management; subscription and recurring-transaction detection; income finder; future-transaction forecasting; benefit transactions; loan and debt-collection identification; and the Insights Product Finder.

- **Human URL:** [https://docs.thisisbud.com](https://docs.thisisbud.com)
- **Base URL:** `https://api-sandbox.thisisbud.com`

#### Tags

- Insights
- Analytics
- Recurring Payments
- Subscriptions
- Income

#### Properties

- [Documentation](https://docs.thisisbud.com)
- [OpenAPI](openapi/bud-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bud-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bud-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bud Intelligent Search API

Beta intelligent search across transactions with AI-generated insights. Submit a natural language query, retrieve matching transactions and a derived narrative insight referencing the matched set.

- **Human URL:** [https://docs.thisisbud.com](https://docs.thisisbud.com)
- **Base URL:** `https://api-sandbox.thisisbud.com`

#### Tags

- Search
- AI
- Natural Language
- Beta

#### Properties

- [Documentation](https://docs.thisisbud.com)
- [OpenAPI](openapi/bud-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bud-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bud-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bud Affordability and Assess API

Pre-fill affordability forms and power lending decisions with structured income and expenditure breakdowns. Generate affordability reports (V1 and V2), drill into affordability transactions, retrieve beta risk insights (income-expenditure, merchants, unauthorised overdraft, income-health), and manage Assess customer applications with linked customer references.

- **Human URL:** [https://docs.thisisbud.com](https://docs.thisisbud.com)
- **Base URL:** `https://api-sandbox.thisisbud.com`

#### Tags

- Affordability
- Lending
- Assess
- Risk

#### Properties

- [Documentation](https://docs.thisisbud.com)
- [OpenAPI](openapi/bud-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bud-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bud-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bud Customer Characteristics API

Retrieve derived behavioural characteristics for a customer across credit card, loan, overdraft, and saver lenses. Designed to feed lending models and risk decisioning with explainable feature sets calculated from enriched transaction history.

- **Human URL:** [https://docs.thisisbud.com](https://docs.thisisbud.com)
- **Base URL:** `https://api-sandbox.thisisbud.com`

#### Tags

- Characteristics
- Risk
- Credit
- Lending

#### Properties

- [Documentation](https://docs.thisisbud.com)
- [OpenAPI](openapi/bud-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bud-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bud-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bud Goals and Budgets API

Manage savings goals (V2) and spending budgets (V1) for end customers. Create, retrieve, list, and delete goals, attach contributing transactions to a budget, and track progress against a target amount and time horizon.

- **Human URL:** [https://docs.thisisbud.com](https://docs.thisisbud.com)
- **Base URL:** `https://api-sandbox.thisisbud.com`

#### Tags

- Budgets
- Savings
- Goals
- Money Management

#### Properties

- [Documentation](https://docs.thisisbud.com)
- [OpenAPI](openapi/bud-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bud-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bud-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bud Payments API

Initiate authorised single payments, scheduled payments, and standing orders directly from a customer's bank account using Bud's PISP service. Either redirect users to a Bud-hosted Bud Pay URL or drive the flow yourself with native authorisation-code, confirmation, and status endpoints.

- **Human URL:** [https://docs.thisisbud.com](https://docs.thisisbud.com)
- **Base URL:** `https://api-sandbox.thisisbud.com`

#### Tags

- Payments
- PISP
- Open Banking
- Standing Orders

#### Properties

- [Documentation](https://docs.thisisbud.com)
- [OpenAPI](openapi/bud-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bud-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bud-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bud Embedded Widgets API

Request signed URLs for Bud's embeddable frontend widgets - accounts, balances over time, financial calendar, insight summary, intelligent search, recurring and forecasted transactions, savings goals, spending analysis, and spending budgets - drop them into your app without rebuilding the UI.

- **Human URL:** [https://docs.thisisbud.com](https://docs.thisisbud.com)
- **Base URL:** `https://api-sandbox.thisisbud.com`

#### Tags

- Widgets
- Embeddable
- UI
- Frontend

#### Properties

- [Documentation](https://docs.thisisbud.com)
- [OpenAPI](openapi/bud-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bud-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bud-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Web Site](https://bud.co)
- [Documentation](https://docs.thisisbud.com)
- [Console](https://console.thisisbud.com)
- [Support](https://support.thisisbud.com)
- [LinkedIn](https://www.linkedin.com/company/bud-financial/)
- [Git Hub](https://github.com/thisisbud/bud-public-developer-resources)
- [L L M S Tx T](https://docs.thisisbud.com/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
