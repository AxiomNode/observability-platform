# observability-platform

Last updated: 2026-05-03.

Observability assets for AxiomNode services.

## Responsibility

- Baseline stack definitions for metrics, logs, and tracing.
- Dashboard packs by domain and service.
- Alerting rules and operational thresholds.

## Runtime role

### Ownership boundary

This repository owns shared observability assets for the platform.

It should document:

- what telemetry assets exist centrally
- how alerts and dashboards are organized
- which validation guarantees are enforced before changes land

It should not restate per-service metrics semantics that belong in the owning service repositories.

## Runtime surface

### Structure

- `stack/`: core observability components.
- `dashboards/`: service and business dashboards.
- `alerts/`: alert rules and severity mapping.

### Main consumers

- operators using `backoffice`
- platform operators validating staging or production health
- incident workflows described in the central `docs` repository

## Local setup

### Workflow

- `validate-observability.yml`
	- Trigger: push (`main`, `develop`), pull request, manual dispatch.
	- Purpose: validates repository layout and checks alert rule files for valid YAML structure (`groups`, `rules`, `alert`, `expr`).

## Documentation

- `stack/README.md`
- `dashboards/README.md`
- `alerts/README.md`

## Deployment and operations notes

### Documentation scope

Keep this repository documentation concrete about stacks, dashboards, alert assets, and repository-local validation. Cross-repository incident process belongs in the central `docs` repository.

## References
