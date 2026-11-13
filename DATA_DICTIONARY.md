# Analysis input contract

All analysis inputs are bundled in `reports/`. Each service is one of `enrolment`, `biometric`, or `demographic`.

| File | Fields | Meaning |
|---|---|---|
| `<service>_monthly.csv` | period, activity, observed_days, rows | Year-month total, distinct observed dates and contributing rows |
| `<service>_states.csv` | state, activity | Total by source state label |
| `<service>_districts.csv` | state, district, activity | Total by state and district together |
| `<service>_ages.csv` | source age field, activity | Totals by source age-count column; the first CSV header is blank and Pandas reads it as `Unnamed: 0` |
| `<service>_state_case_variants.csv` | normalized case key, source labels | Case-variant diagnostics |
| `summary.json` | service, rows, total_activity and quality/coverage fields | Previously prepared raw-source quality summary |
| `input_manifest.json` | file, service, rows, columns | Provenance of previously processed source files |

These are different aggregation levels of the same activity. Do not add totals across tables or join them as though they were independent records. Do not infer district-by-month or age-by-district counts from separate marginal summaries. The future cleaning repository can publish these same analysis inputs, or provide a separately documented row-level dataset.
