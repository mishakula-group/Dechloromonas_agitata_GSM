*Dechloromonas agitata* Genome-Scale Metabolic Model

This repository contains files for the *Dechloromonas agitata* is5 genome-scale metabolic model (GSM), including intermediate and final SBML models, model-quality reports, community-modeling inputs and results, and supplementary tables.

## Directory Index

- [`iMM643/`](#imm643) — *D. agitata* model variants, reports, and final model files.
  - [`final_files/`](#imm643final_files) — final SBML model, metabolic map, and report.
- [`MICOM_results/`](#micom_results) — MICOM notebook, community models, serialized communities, result archives, tables, and interactive visualizations.
  - [`final_res_with_sample_id/`](#micom_resultsfinal_res_with_sample_id) — aggregated MICOM results.
  - [`grow_results_micom/`](#micom_resultsgrow_results_micom) — per-sample MICOM result archives.
  - [`methanotrophs_models/`](#micom_resultsmethanotrophs_models) — partner-model SBML files.
- [`PyCoMo_results/`](#pycomo_results) — PyCoMo community-model result sets.
  - [`20zr_community/`](#pycomo_results20zr_community) — *D. agitata*–20ZR results.
  - [`album_community/`](#pycomo_resultsalbum_community) — *D. agitata*–*Methylobacterium album* results.
  - [`mcaps_community/`](#pycomo_resultsmcaps_community) — *D. agitata*–M. capsulatus results.
- [`Supplementary/`](#supplementary) — supplementary workbook.

## `iMM643/`

This directory stores the *D. agitata* is5 SBML model files and their HTML reports.

- `agitata_vjgb_1.xml`, `agitata_vjgb_2.xml`, and `agitata_vjgb_3.xml` are three versioned SBML model files.
- `agitata_vjgb_cleaned.xml` is a cleaned SBML model variant.
- `report_agitata_vjgb_1.html`, `report_agitata_vjgb_2.html`, `report_agitata_vjgb_3.html`, and `report_agitata_vjgb_cleaned.html` are the corresponding HTML reports.

### `iMM643/final_files/`

- `iMM643.xml` — final SBML model file.
- `agitata_micro_map.json` — JSON metabolic-map file.
- `report_iMM643.html` — HTML report for `iMM643.xml`.

## `MICOM_results/`

This directory contains a Python notebook and output files from MICOM community-modeling analyses. The notebook builds serialized community models, defines media, runs growth workflows, aggregates results, and produces MICOM visualizations.

- `community_agitata.ipynb` — executable analysis notebook. Paths in the notebook point to a Google Drive working location and should be updated before rerunning elsewhere.
- `community_micom_complete.csv` — community composition table. 
- `com_growth_on_medium.csv` — community growth results on the medium defined in the notebook.
- `manifest.csv` — manifest of serialized communities with reaction and metabolite counts and sample IDs.
- `sample_1_1.pickle` through `sample_1_11.pickle`, `sample_2_1.pickle` through `sample_2_11.pickle`, and `sample_3_1.pickle` through `sample_3_11.pickle` — serialized MICOM community objects.
- `consumption_st.html`, `growth_rates_st.html`, and `niche_st.html` — interactive MICOM visualization outputs for exchange consumption, growth rates, and taxon-level 