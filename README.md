# *Dechloromonas agitata* Genome-Scale Metabolic Model

This repository contains the genome-scale metabolic model (GSM) of *Dechloromonas agitata* strain is5, model curation notebooks, and results from MICOM and PyCoMo community-modeling analyses.

## Repository structure

- `iEK643/` — SBML model versions, HTML model reports, and final model files.
  - `agitata_vjgb_1.xml`, `agitata_vjgb_2.xml`, `agitata_vjgb_3.xml` — versioned model files.
  - `agitata_vjgb_cleaned.xml` — cleaned model.
  - `report_agitata_vjgb_1.html`, `report_agitata_vjgb_2.html`, `report_agitata_vjgb_3.html`, `report_agitata_vjgb_cleaned.html` — model reports.
  - `final_files/iEK643.xml` — final SBML model.
  - `final_files/report_iEK643.html` — report for the final model.
  - `final_files/agitata_micro_map.json` — metabolic map data.
- `Jupyter-notebooks/` — notebooks for model curation and aerobic community analysis.
  - `curation_iEK643.ipynb`
  - `aerobic_community_agitata.ipynb`
- `MICOM_results/` — MICOM community models, input tables, growth results, and visualizations.
  - `community_agitata.ipynb` — MICOM analysis notebook.
  - `community_models/` — serialized community models (`sample_*.pickle`).
  - `final_res_with_sample_id/` — aggregated results, annotations, exchanges, and growth rates.
  - `grow_results_micom/` — per-sample growth result archives.
  - `html_reports/` — interactive reports for consumption, growth rates, and interactions.
  - `methanotrophs_models/` — partner models used to build communities.
  - `community_micom_complete.csv`, `com_growth_on_medium.csv`, `manifest.csv` — community composition, growth results, and model manifest.
- `PyCoMo_results/` — PyCoMo community-model results for three partner organisms.
  - `20zr_community/` — *D. agitata*–20ZR models, tables, and plots.
  - `album_community/` — *D. agitata*–*Methylobacterium album* models, tables, and plots.
  - `mcaps_community/` — *D. agitata*–*Methylobacterium capsulatus* models, tables, and plots.
- `Supplementary/` — supplementary figures, `supplementary_figures.pdf`, and `supplementary_tables.xlsx`.

Notebook paths may refer to the original working environment and may need updating before running on another computer.