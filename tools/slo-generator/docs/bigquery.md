# BigQuery

## Exporter

The BigQuery exporter will export SLO reports to a BigQuery table. This allows teams to conduct historical analysis of SLO reports, and figure out what to do to improve on the long-run (months, years).

### Example

> We want to query the last year of SLO reports to see how often we meet our targets. This way we can know if we need to adjust some targets to be more realistic and save our SREs some time.
>
> -- <cite>SRE Lead</cite>

```yaml
exporters:
  - class: Bigquery
    project_id: "${BIGQUERY_HOST_PROJECT}"
    dataset_id: "${BIGQUERY_DATASET_ID}"
    table_id: "${BIGQUERY_TABLE_ID}"
```
