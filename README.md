# CareerOS Analytics Service

Produce privacy-conscious aggregates and operational metrics for the job-search journey.

## Scope

- **Owns:** Derived aggregates, metric definitions and non-identifying reporting views.
- **Inputs:** Minimized lifecycle events and authorized reporting queries.
- **Outputs:** Aggregated indicators without raw CV or application content.
- **Dependencies:** versioned events from operational services.

## Safety baseline

This public repository must never contain secrets, real resumes, real applications or personal data. External communication and application submission always require explicit user approval.

## Documentation

See [docs/overview.md](docs/overview.md) and the central [CareerOS workspace](https://github.com/FievezRomain/careeros-workspace).

## Status

Architecture and security baseline. Functional implementation will be added incrementally with tests and versioned contracts.

## License

Apache-2.0.