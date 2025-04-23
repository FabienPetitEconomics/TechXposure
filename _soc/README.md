# ONET-SOC (2010) Occupation Exposure

This directory contains all the ONET-SOC (2010) Occupation Exposure data.

## List of directories and files

| DATA FILE               | TYPE                    | DESCRIPTION               | SOURCE |
| ----------------------- | ------------------------- | ------------------- | -------- |
| `techXposure_soc2d_by_tech.csv`  | Dataset | 2-digit ONET-SOC Occupation Exposure | Authors |
| `techXposure_soc3d_by_tech.csv`  | Dataset | 3-digit ONET-SOC Occupation Exposure | Authors |
| `techXposure_soc5d_by_tech.csv`  | Dataset | 5-digit ONET-SOC Occupation Exposure | Authors |
| `techXposure_soc6d_by_tech.csv`  | Dataset | 6-digit ONET-SOC Occupation Exposure | Authors |
| `techXposure_soc8d_by_tech.csv`  | Dataset | 8-digit ONET-SOC Occupation Exposure | Authors |

## Data structure

Each data file has the same data structure.

| VARIABLE               | TYPE                    | DESCRIPTION               | MERGE WITH |
| ----------------------- | ------------------------- | ------------------- | -------- |
| `socXd`  | Integer | ONET-SOC code at the `X`-digit level | `_classification/classification_soc.csv` |
| `socXd_label`  | String | ONET-SOC label at the `X`-digit level | `_classification/classification_soc.csv` |
| `tech40_id`  | Integer | Technology identifier | `_classification/classification_tech40.csv` |
| `tech40_label`  | String | Technology label | `_classification/classification_tech40.csv` |
| `cosineXd`  | Numeric | Cosine similarity score at the `X`-digit level |  |
| `n_patent`  | Integer | Number of patents |  |
| `xposureXd`  | Numeric | Exposure score at the `X`-digit level |  |