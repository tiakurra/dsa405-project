# dsa405-project
Author: Tanmayi Kurra (tkurra)

This repository contains the dataset and notebook for DSA 405 Milestone 3.

## P3: Acquisition and Integration

- **Notebook:** `DSA405_002_FA26_P3_tkurra.ipynb`
- **Source 1:** EIA retail sales API (collected and cleaned in P2): `data/clean/eia_retail_sales_clean.csv`
- **Source 2:** Berkeley Lab, U.S. Distributed Solar and Storage Data (Tracking the Sun), 2026 Update, public project-level CSV. Credit: Lawrence Berkeley National Laboratory. The project page states no license; the Data.gov catalog record for Tracking the Sun lists CC BY 4.0.
- **Not in the repo:** the 241 MB zip (`LBNL_distributed_solar_dataset_public.zip`), which is git-ignored. To reproduce, download it from https://bit.ly/trackingthesun2026 (Google Drive shows a virus-scan warning page for large files, so download it once by hand) and place it in `data/raw/`. The notebook checks it against the size and checksums recorded in `data/raw/MANIFEST_LBNL.json`.
- **Needs:** Python with pandas and requests, and the `unzip` command (macOS has it). The CSV uses Deflate64 compression, so Python's `zipfile` cannot read it.
- **Outputs:** `data/clean/tts_state_year_capacity.csv` (state-year cumulative solar capacity) and `data/clean/tts_accounting.json` (row counts by drop reason).
- **Result:** the join keeps all 1,275 EIA rows; 675 match solar data (27 jurisdictions) and 600 are `NA` (24 jurisdictions the public file does not cover).
- **Run:** open the notebook, Restart, Run All.
