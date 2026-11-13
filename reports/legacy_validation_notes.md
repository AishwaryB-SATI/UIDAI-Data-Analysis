# Validation

The analysis script is executed against the supplied Excel exports. Notebook code cells are syntax-checked; the notebook is a thin interactive entry point to the same script, rather than a separate analysis implementation. No original Colab state or cached outputs are used.

Reconciliation checks compare each service's monthly, state, district and age aggregates to its recorded total. Input row counts are reconciled to the per-file manifest. See validation_results.json for the results.

Source data coverage is measured using distinct observed dates per month. Absence of a date cannot distinguish no activity from missing reporting. The recorded date format is interpreted as day-month-year, matching the original notebook; definitive source metadata was not supplied.
