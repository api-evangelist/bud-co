# Bud Financial (bud-co)

Bud Financial (formerly Bud, thisisbud.com) is a UK-based fintech infrastructure company providing AI-driven Open Banking aggregation, transaction enrichment, categorization, affordability assessment, and payment initiation APIs. The Bud platform unifies Open Banking connections to UK and EU ASPSPs behind a single REST API and layers AI/ML-powered enrichment, categorization, merchant identification, affordability scoring, income and expenditure analysis, and actionable financial insights on top of raw transaction data. Banks, lenders, and consumer fintechs use Bud for KYC/AML checks, lending decisions, money management, and embedded payments.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

Open Banking, Transaction Enrichment, Categorization, Affordability, Payments, AISP, PISP, Financial Data, FinTech, UK, AI, Machine Learning

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Products

| Product | Description |
|---|---|
| Connect | Open Banking aggregation + first-party ingestion across UK and EU ASPSPs. |
| Intelligence | Enrichment, categorization, merchant ID, insights, characteristics, intelligent search. |
| Assess | Affordability reports and lending decision support. |
| Pay | PISP payment initiation (single, scheduled, standing order) via Bud Pay. |
| Check | KYC and verification services for businesses and individuals. |

## Common Resources

- [Website](https://bud.co)
- [Documentation](https://docs.thisisbud.com)
- [Developer Console](https://console.thisisbud.com)
- [Support Centre](https://support.thisisbud.com)
- [LinkedIn](https://www.linkedin.com/company/bud-financial/)
- [Public Developer Resources (GitHub)](https://github.com/thisisbud/bud-public-developer-resources)
- [llms.txt](https://docs.thisisbud.com/llms.txt)

## APIs

### Bud Connect API
Open Banking aggregation API providing unified access to UK and EU ASPSP connections via Bud Connect (hosted gateway) or native authorisation, refresh, consent, and reconfirmation endpoints.

- [Documentation](https://docs.thisisbud.com)
- [OpenAPI](openapi/bud-platform-openapi.yml)
- [Naftiko Capability - Open Banking](capabilities/connect-open-banking.yaml)
- [Naftiko Capability - Refresh](capabilities/connect-ingestion.yaml)

### Bud First-Party Ingestion API
Push first-party account and transaction data into the Bud platform for enrichment without an Open Banking consent.

- [OpenAPI](openapi/bud-platform-openapi.yml)
- [Naftiko Capability - Accounts](capabilities/ingestion-accounts.yaml)
- [Naftiko Capability - Transactions](capabilities/ingestion-transactions.yaml)

### Bud Customers Platform API
Create and manage end-user customer records on the Bud platform (V1, V2, V3) with idempotent identifiers and customer context.

- [OpenAPI](openapi/bud-platform-openapi.yml)
- [Naftiko Capability - Customers](capabilities/platform-customers.yaml)

### Bud Financial Data API
Retrieve enriched accounts, transactions, balances, and authorised payments with Bud's category, merchant, and recurrence metadata.

- [OpenAPI](openapi/bud-platform-openapi.yml)
- [JSON Schema - Transaction](json-schema/bud-transaction-schema.json)
- [JSON Schema - Account](json-schema/bud-account-schema.json)
- [JSON-LD](json-ld/bud-co-context.jsonld)
- [Naftiko Capability - Accounts](capabilities/financial-accounts.yaml)
- [Naftiko Capability - Transactions](capabilities/financial-transactions.yaml)
- [Naftiko Capability - Balances](capabilities/financial-balances.yaml)

### Bud Enrichment API
Category models, category and merchant taxonomies, aggregated category and merchant totals, essential-spending statistics, and category/merchant corrections.

- [OpenAPI](openapi/bud-platform-openapi.yml)
- [Naftiko Capability - Categories](capabilities/enrichment-categories.yaml)
- [Naftiko Capability - Merchants](capabilities/enrichment-merchants.yaml)
- [Naftiko Capability - Corrections](capabilities/enrichment-corrections.yaml)

### Bud Financial Insights API
Actionable balance, income, and spending insights; custom insights; subscription and recurring-transaction detection; income finder; future transactions; benefits; loans and debt-collection identification.

- [OpenAPI](openapi/bud-platform-openapi.yml)
- [Naftiko Capability - Actionable](capabilities/insights-actionable.yaml)
- [Naftiko Capability - Custom](capabilities/insights-custom.yaml)
- [Naftiko Capability - Recurring](capabilities/insights-recurring.yaml)

### Bud Intelligent Search API (beta)
AI-powered natural-language search across transactions returning matches and a derived insight.

- [OpenAPI](openapi/bud-platform-openapi.yml)
- [Naftiko Capability - Search](capabilities/search-transactions.yaml)

### Bud Affordability and Assess API
Affordability reports (V1 and V2), affordability transactions, risk insights (income-expenditure, merchants, unauthorised overdraft, income-health), and Assess customer applications.

- [OpenAPI](openapi/bud-platform-openapi.yml)
- [Example - Affordability Report](examples/bud-affordability-report-example.json)
- [Naftiko Capability - Affordability](capabilities/affordability-reports.yaml)
- [Naftiko Capability - Assess Applications](capabilities/assess-applications.yaml)

### Bud Customer Characteristics API
Derived behavioural characteristics across credit card, loan, overdraft, and saver dimensions for lending and risk models.

- [OpenAPI](openapi/bud-platform-openapi.yml)
- [Naftiko Capability - Characteristics](capabilities/characteristics-customer.yaml)

### Bud Goals and Budgets API
Savings goals (V2) and spending budgets (V1) for end-customer money management UIs.

- [OpenAPI](openapi/bud-platform-openapi.yml)
- [Naftiko Capability - Savings](capabilities/goals-savings.yaml)
- [Naftiko Capability - Budgets](capabilities/goals-budgets.yaml)

### Bud Payments API
PISP payment initiation - single payments, scheduled payments, standing orders - via the Bud-hosted Bud Pay URL or native API flow.

- [OpenAPI](openapi/bud-platform-openapi.yml)
- [Naftiko Capability - Single](capabilities/payments-single.yaml)
- [Naftiko Capability - Standing Order](capabilities/payments-standing-order.yaml)
- [Naftiko Capability - Scheduled](capabilities/payments-scheduled.yaml)

### Bud Embedded Widgets API
Signed URLs for embeddable widgets: accounts, balances over time, financial calendar, insight summary, intelligent search, recurring and forecasted transactions, savings goals, spending analysis, spending budgets.

- [OpenAPI](openapi/bud-platform-openapi.yml)
- [Naftiko Capability - Widget URLs](capabilities/widgets-urls.yaml)

## Examples

- [Enriched Transaction](examples/bud-transaction-example.json)
- [Affordability Report](examples/bud-affordability-report-example.json)

## Operational Artifacts

- [Plans and Pricing](plans/bud-co-plans-pricing.yml)
- [Rate Limits](rate-limits/bud-co-rate-limits.yml)
- [FinOps](finops/bud-co-finops.yml)
- [Spectral Rules](rules/bud-co-rules.yml)
- [Vocabulary](vocabulary/bud-co-vocabulary.yml)
