# Analysis of supplied Aadhaar service exports

These results were computed from the 11 supplied XLSX files. Counts refer to aggregate records and recorded service activity, not unique people. Biometric coverage is partial.

| Service | Rows | Exact repeated rows (retained) | Recorded activity | Date span |
|---|---:|---:|---:|---|
| enrolment | 1,006,029 | 22,957 | 5,435,702 | 2025-03-02 to 2025-12-31 |
| biometric | 1,361,108 | 62,846 | 61,776,326 | 2025-03-01 to 2025-12-29 |
| demographic | 2,071,700 | 473,601 | 49,295,187 | 2025-03-01 to 2025-12-29 |

## Findings and limits

### Enrolment

The largest source state label by recorded activity is **Uttar Pradesh** (1,018,629). The highest supplied monthly total is **2025-09**. These rankings retain source aliases and should be considered provisional.

There are 0 unparseable dates and 0 rows with missing, nonnumeric or negative age counts. 0 rows are excluded from activity aggregation. The raw missing-value counts are preserved in summary.json.

Observed date coverage by month:

- 2025-03: 9 observed date labels
- 2025-04: 1 observed date labels
- 2025-05: 1 observed date labels
- 2025-06: 1 observed date labels
- 2025-07: 1 observed date labels
- 2025-09: 30 observed date labels
- 2025-10: 18 observed date labels
- 2025-11: 20 observed date labels
- 2025-12: 11 observed date labels

Exact repeated rows contribute 103,943 recorded activity. This measures sensitivity to a potential deduplication policy, not confirmed overcounting.

### Biometric

The largest source state label by recorded activity is **Uttar Pradesh** (8,385,428). The highest supplied monthly total is **2025-07**. These rankings retain source aliases and should be considered provisional.

There are 0 unparseable dates and 0 rows with missing, nonnumeric or negative age counts. 0 rows are excluded from activity aggregation. The raw missing-value counts are preserved in summary.json.

Observed date coverage by month:

- 2025-03: 1 observed date labels
- 2025-04: 1 observed date labels
- 2025-05: 1 observed date labels
- 2025-06: 1 observed date labels
- 2025-07: 1 observed date labels
- 2025-09: 20 observed date labels
- 2025-10: 18 observed date labels
- 2025-11: 7 observed date labels
- 2025-12: 19 observed date labels

Exact repeated rows contribute 973,587 recorded activity. This measures sensitivity to a potential deduplication policy, not confirmed overcounting.

### Demographic

The largest source state label by recorded activity is **Uttar Pradesh** (8,542,328). The highest supplied monthly total is **2025-03**. These rankings retain source aliases and should be considered provisional.

There are 0 unparseable dates and 0 rows with missing, nonnumeric or negative age counts. 0 rows are excluded from activity aggregation. The raw missing-value counts are preserved in summary.json.

Observed date coverage by month:

- 2025-03: 1 observed date labels
- 2025-04: 1 observed date labels
- 2025-05: 1 observed date labels
- 2025-06: 1 observed date labels
- 2025-07: 1 observed date labels
- 2025-09: 20 observed date labels
- 2025-10: 18 observed date labels
- 2025-11: 24 observed date labels
- 2025-12: 28 observed date labels

Exact repeated rows contribute 12,697,629 recorded activity. This measures sensitivity to a potential deduplication policy, not confirmed overcounting.

## Interpretation

Months differ substantially in observed date coverage. Monthly peaks do not establish recurring seasonality or comparable full-month service volumes. The supplied biometric files omit the 1,000,000–1,500,000 portion, so biometric totals are subset totals. State labels require validated alias mapping before definitive state rankings. No fraud-detection, forecasting, waiting-time or staffing conclusion is established by this EDA.

Source provenance: the owner reports official-site downloads; exact URL and reuse terms remain unverified.