# Fertilizer Quantity Prediction from Soil and Geospatial Features

Master's/Bachelor's thesis project: multi-output regression models that predict
recommended fertilizer quantities (MOP, DAP, urea, organic, zinc, boron) for
crops in Nepal from soil properties and geospatial features.

> **License: All rights reserved.** This repository is public for viewing and
> evaluation only. Reuse of the code, figures or data requires written
> permission. See [LICENSE](LICENSE).

## Repository layout

| Folder | Contents |
|---|---|
| `notebooks/01_main_model/` | Data loading, feature/target setup, model comparison (Linear, Ridge, Random Forest, LightGBM, ...). `v3_latest` is the current version; v1/v2 are earlier iterations. |
| `notebooks/02_hyperparameter_tuning/` | Hyperparameter search for the selected models. |
| `notebooks/03_ablation_studies/` | Feature ablations: removing/keeping lat-lon, elevation and a third feature group. |
| `results/figures/` | Ablation comparison plots. |
| `data/sample/` | 100-row random sample of the dataset (full data of ~384k rows, 57 columns is not published). |

## Data

Columns include coordinates (`lon`, `lat`, `elevation`), soil properties (pH,
organic matter, N, K, P2O5, B, Zn, sand/clay/silt) and administrative region
(province, district, palika), plus fertilizer-recommendation targets per crop.
Notebooks expect `cleaned_df_4lakh.csv` in the working directory; only the
sample is provided here, so the notebooks are shown **without outputs** and
cannot be fully re-run.

## Not included

Trained model files, the full dataset and training logs are intentionally
withheld.

## Citation

See [CITATION.cff](CITATION.cff).

## Contact

Kritin Youpane
