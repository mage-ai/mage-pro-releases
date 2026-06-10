# Observability Upgrades

A more confident control room for teams that need to know what changed, what is late, and what needs attention.

## Highlights

- Spot late-running pipelines before SLAs are missed.
- Compare block output changes across recent runs.
- Send clearer status summaries to operators and stakeholders.

## Pipeline Monitoring

Pipeline run pages now put the highest-signal information closer to the top. Teams can scan run health, recent failures, and delayed schedules without opening every pipeline one by one.

## Data Observability

Block output previews are easier to compare across runs. This helps teams understand whether a pipeline changed because of code, source data, configuration, or a downstream dependency.

## Alerts That Read Better

Operational summaries now use clearer labels and grouped details so Slack and email updates are easier to skim. The goal is to make the next action obvious:

- Retry a failed block.
- Escalate a stale dependency.
- Confirm a late run is still within tolerance.
- Share an incident-ready summary with stakeholders.

## Example Runbook Snippet

```text
If a critical pipeline is late:
1. Open the latest pipeline run.
2. Check the slowest block and upstream dependency.
3. Retry only the failed block when inputs are unchanged.
4. Share the generated status summary.
```
