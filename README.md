# observability-platform

Observability assets for AxiomNode services.

## Scope

- Baseline stack definitions for metrics, logs, and tracing.
- Dashboard packs by domain and service.
- Alerting rules and operational thresholds.

## Structure

- `stack/`: core observability components.
- `dashboards/`: service and business dashboards.
- `alerts/`: alert rules and severity mapping.

## Workflow

- `validate-observability.yml`
	- Trigger: push (`main`, `develop`), pull request, manual dispatch.
	- Purpose: validates repository layout and required observability folders.
