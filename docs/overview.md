# CareerOS Analytics Service â€” service overview

## Responsibility

Produce privacy-conscious aggregates and operational metrics for the job-search journey.

## Data ownership

Derived aggregates, metric definitions and non-identifying reporting views.

## Interfaces

- Inputs: Minimized lifecycle events and authorized reporting queries.
- Outputs: Aggregated indicators without raw CV or application content.
- Dependencies: versioned events from operational services.

## Example

For one authorized user journey, the service can derive a funnel such as: 42 jobs analyzed, 12 shortlisted, 5 resumes validated, 3 applications submitted and 1 interview recorded. It stores the metric dimensions and aggregate counts, not the raw resume or application text.

## Contract rules

- APIs and events are versioned.
- Consumers must be idempotent where retries are possible.
- Correlation identifiers are propagated without logging sensitive payloads.
- Authorization and ownership are checked at the service boundary.

## Non-goals

This service does not absorb responsibilities owned by another CareerOS service. Cross-service workflows are coordinated through explicit contracts rather than shared databases.

## Security and privacy

Persist the minimum data required, record provenance, define retention, redact logs and use synthetic examples in this public repository.
