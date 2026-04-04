# AGENTS

## Repo purpose
Observability baseline repository for metrics, dashboards, and alert rules.

## Key paths
- stack/: observability stack components
- dashboards/: service/domain dashboard definitions
- alerts/: alert rules and thresholds

## Local commands
- Validate structure and referenced runbooks manually.

## CI/CD notes
- validate-observability workflow checks required repository layout.

## LLM editing rules
- Keep alert names/severity clear and actionable.
- Cross-reference runbooks when adding or changing alerts.
- Avoid undocumented dashboard metric changes.
