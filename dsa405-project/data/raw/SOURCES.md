# Raw data sources

| File | Source | How obtained | Committed? |
|---|---|---|---|
| `eia_retail_sales_raw.csv` | U.S. Energy Information Administration, Open Data API v2, electricity retail sales, residential price by state, annual 2001-2025. https://www.eia.gov/opendata/ | API request in P2 (free key, never committed) | Yes (100 KB) |
| `LBNL_distributed_solar_dataset_public.zip` | Lawrence Berkeley National Laboratory, "U.S. Distributed Solar and Storage Data" (Tracking the Sun), public file dated 28-Jul-2026. https://emp.lbl.gov/tracking-the-sun/ | Downloaded once by hand from the link in LBNL's user guide (https://bit.ly/trackingthesun2026), because robots.txt on Google's download host disallows automated downloads. See the P3 notebook. | **No** (252 MB; listed in `.gitignore`) |
| `MANIFEST_LBNL.json` | Written by the P3 notebook | Records the zip's size and SHA-256 so a downloaded copy can be checked | Yes |

Terms of use are in the README ("Data sources and terms").
