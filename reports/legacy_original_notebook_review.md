# Changes from the original Colab exploration

The original notebook contained data loading, cleaning, age-band totals, state/district comparisons and monthly/regional heatmaps. This project preserves that descriptive purpose while replacing repeated exploratory steps with one reusable script.

- Removed repeated Task/Subtask/Reasoning sections and duplicate loading/plotting code.
- Replaced personal Drive paths with configurable input/output directories.
- Removed unsupported final claims about fraud, rejection rates, operator correlations and trained anomaly-detection models.
- Kept update-service activity distinct from new enrolment activity.
- Used state-plus-district grouping and year–month periods.
- Retained exact repeats pending confirmation of row identity, unlike the original unconditional drop_duplicates step. Results can therefore differ from the original saved outputs.
- Did not reuse the incomplete regional mapping, which may misclassify geographic aliases as Unknown.
- Made missing biometric file coverage explicit.

The revised pipeline was run against the provided XLSX files. The original Colab notebook itself was not rerun end to end, and no private Drive access was used.
