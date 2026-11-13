# UIDAI Aadhaar Data Analysis

Exploratory analysis of Aadhaar enrolment, biometric updates and demographic updates using Python, Pandas, Matplotlib and Seaborn.

[**View the original notebook**](notebooks/UIDAI_EDA.ipynb) · [**Open in Google Colab**](https://colab.research.google.com/github/AishwaryB-SATI/UIDAI-Data-Analysis/blob/main/notebooks/UIDAI_EDA.ipynb)

## Analysis covered

- State-wise and district-wise activity comparisons.
- Yearly and monthly trends for enrolment, biometric updates and demographic updates.
- Age-group activity comparisons.
- State-versus-month heatmaps.
- **Region-versus-month heatmaps** for all three services, using North, South, East, West, Central and North-East groupings to make geographic patterns easier to compare.
- Regional interpretation and discussion of uneven activity.

The notebook preserves the original 208 cells, analysis code, narrative and available saved outputs.

## Run the notebook

Open the notebook in Google Colab. The original workflow mounts Google Drive and uses paths under `/content/drive/MyDrive/Aadhar_Dataset`, with some earlier setup cells referencing `Aadhar_Data`. Configure the input paths for your environment and provide the expected source exports or matching intermediate cleaned datasets. The original notebook includes setup retries and repeated exploratory steps; review the selected input path before running.

For local execution, install `requirements.txt`, replace Colab-specific Drive setup with local paths, and use Jupyter or a Python notebook kernel in VS Code.

The original notebook includes data-loading and cleaning steps that establish its analysis variables. A separate cleaning repository is planned; those dependencies remain preserved until its outputs and interface are available.

## Saved outputs and reproducibility

Available original outputs are embedded in the notebook. **The regional heatmap code is present, but its cells have no saved outputs in the original file.** Rendering those heatmaps requires executing their dependencies with the corresponding data.

The existing tables in `reports/` are supplemental aggregates. Separate monthly totals and state totals cannot reconstruct state-by-month or region-by-month heatmaps. They must not be substituted for the original joint data.

`reports/analysis_validation.json` documents checks on the supplemental aggregate-based notebook edition. It does not establish execution or validation of this original notebook.

## Data and interpretation

The project uses aggregate activity exports reported as obtained from UIDAI. Original input filenames and schemas are recorded in `reports/input_manifest.json`; source exports are not bundled here.

- Biometric coverage in the supplied file manifest is partial.
- Activity counts are not unique residents or population-normalized coverage rates.
- The original geographic mapping sends unmatched state labels to `Unknown`; inspect those labels when interpreting regional totals.
- Month-based grouping can combine years; verify the date coverage before interpreting trends.
- Descriptive patterns do not independently establish recurring seasonality, fraud, operational causes or resource shortages. Proposed interventions and narrative claims require separate validation.

## Repository contents

| Location | Contents |
|---|---|
| `notebooks/UIDAI_EDA.ipynb` | Original Colab project, including trend plots and regional heatmap code |
| `reports/` | Supplemental aggregates, charts, provenance and validation records |
| `DATA_DICTIONARY.md` | Schema of the supplemental aggregate tables |
| `requirements.txt` | Python analysis dependencies |
