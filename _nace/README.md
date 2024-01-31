# NACE Rev.2 Industry Exposure

This directory contains all the NACE Rev.2 Industry Exposure data.

## List of directories and files

| DATA FILE               | SOURCE                    | DESCRIPTION               | PROVIDED |
| ----------------------- | ------------------------- | ------------------- | -------- |
| `techXposure_nace1d_by_tech.csv`  | Dataset | 1-digit NACE Rev.2 Industry Exposure | Authors |
| `techXposure_nace2d_by_tech.csv`  | Dataset | 2-digit NACE Rev.2 Industry Exposure | Authors |
| `techXposure_nace3d_by_tech.csv`  | Dataset | 3-digit NACE Rev.2 Industry Exposure | Authors |

## Data structure

Each data file has the same data structure.

| VARIABLE               | TYPE                    | DESCRIPTION               | MERGE WITH |
| ----------------------- | ------------------------- | ------------------- | -------- |
| `naceXd`  | String / Numeric[^1] | NACE Rev.2 code at the `X`-digit level | `_classification/classification_nace.csv` |
| `naceXd_label`  | String | NACE Rev.2 label at the `X`-digit level | `_classification/classification_nace.csv` |
| `tech40_id`  | Integer | Technology identifier | `_classification/classification_tech40.csv` |
| `tech40_label`  | String | Technology label | `_classification/classification_tech40.csv` |
| `cosineXd`  | Numeric | Cosine similarity score at the `X`-digit level |  |
| `n_patent`  | Integer | Number of patents |  |
| `xposureXd`  | Numeric | Exposure score at the `X`-digit level |  |

[^1]: The NACE Rev.2 code is a string variable at the 1-digit level and a numeric variable at the 2-digit and 3-digit levels.