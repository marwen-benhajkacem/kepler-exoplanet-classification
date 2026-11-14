# Data

`exoplanets.csv` — Kepler Objects of Interest (KOI) cumulative table, **9,564 rows × 49 columns**, exported from the [NASA Exoplanet Archive](https://exoplanetarchive.ipac.caltech.edu/) (Kaggle copy). NASA asks users to acknowledge the archive when using its data:
*This research has made use of the NASA Exoplanet Archive, operated by the California Institute of Technology under contract with NASA.*

| Item | Value |
|---|---|
| Target | `koi_disposition`: FALSE POSITIVE (4,840 / 50.6%), CANDIDATE (2,367 / 24.7%), CONFIRMED (2,357 / 24.6%) |
| Duplicates | 0 exact duplicates |
| Empty columns | `koi_teq_err1`, `koi_teq_err2` (100% missing) |
| Columns at risk of data leakage | `koi_pdisposition`, `koi_score`, `koi_fpflag_nt/ss/co/ec`, `kepler_name` |
| Anomaly | `koi_fpflag_nt = 465` in one row (should be 0 or 1) |

| `data/processed/koi_binary_clean.csv` | Output of notebook 02: kepid, binary target, 13 features (7,197 rows) |
