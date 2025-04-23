# NAICS (2007) Industry Exposure

This directory contains all the NAICS (2007) Industry Exposure data.

## List of directories and files

| DATA FILE               | SOURCE                    | DESCRIPTION               | PROVIDED |
| ----------------------- | ------------------------- | ------------------- | -------- |
| `techXposure_naics2d_by_tech.csv`  | Dataset | 2-digit NAICS Industry Exposure | Authors |
| `techXposure_naics3d_by_tech.csv`  | Dataset | 3-digit NAICS Industry Exposure | Authors |
| `techXposure_naics4d_by_tech.csv`  | Dataset | 4-digit NAICS Industry Exposure | Authors |

## Data structure

Each data file has the same data structure.

| VARIABLE               | TYPE                    | DESCRIPTION               | MERGE WITH |
| ----------------------- | ------------------------- | ------------------- | -------- |
| `naicsXd`  | Integer | NAICS code at the `X`-digit level | `_classification/classification_naics.csv` |
| `naicsXd_label`  | String | NAICS label at the `X`-digit level | `_classification/classification_naics.csv` |
| `tech40_id`  | Integer | Technology identifier | `_classification/classification_tech40.csv` |
| `tech40_label`  | String | Technology label | `_classification/classification_tech40.csv` |
| `cosineXd`  | Numeric | Cosine similarity score at the `X`-digit level |  |
| `n_patent`  | Integer | Number of patents |  |
| `xposureXd`  | Numeric | Exposure score at the `X`-digit level |  |