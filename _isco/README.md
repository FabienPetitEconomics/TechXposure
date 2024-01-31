# ISCO-08 Occupation Exposure

This directory contains all the ISCO-08 Occupation Exposure data.

## List of directories and files

| DATA FILE               | TYPE                    | DESCRIPTION               | SOURCE |
| ----------------------- | ------------------------- | ------------------- | -------- |
| `techXposure_isco1d_by_tech.csv`  | Dataset | 1-digit ISCO-08 Occupation Exposure | Authors |
| `techXposure_isco2d_by_tech.csv`  | Dataset | 2-digit ISCO-08 Occupation Exposure | Authors |
| `techXposure_isco3d_by_tech.csv`  | Dataset | 3-digit ISCO-08 Occupation Exposure | Authors |
| `techXposure_isco4d_by_tech.csv`  | Dataset | 4-digit ISCO-08 Occupation Exposure | Authors |

## Data structure

Each data file has the same data structure.

| VARIABLE               | TYPE                    | DESCRIPTION               | MERGE WITH |
| ----------------------- | ------------------------- | ------------------- | -------- |
| `iscoXd`  | Integer | ISCO-08 code at the `X`-digit level | `_classification/classification_isco.csv` |
| `iscoXd_label`  | String | ISCO-08 label at the `X`-digit level | `_classification/classification_isco.csv` |
| `tech40_id`  | Integer | Technology identifier | `_classification/classification_tech40.csv` |
| `tech40_label`  | String | Technology label | `_classification/classification_tech40.csv` |
| `cosineXd`  | Numeric | Cosine similarity score at the `X`-digit level |  |
| `n_patent`  | Integer | Number of patents |  |
| `xposureXd`  | Numeric | Exposure score at the `X`-digit level |  |