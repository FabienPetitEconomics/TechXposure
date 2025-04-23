# TechXposure Classifications

This directory contains all the classifications used in the `TechXposure` database. 

## List of directories and files

| DATA FILE               | TYPE                    | DESCRIPTION               | SOURCE |
| ----------------------- | ------------------------- | ------------------- | -------- |
| `classification_isco.csv`  | Dataset | This dataset includes the ISCO-08 occupation codes and their labels from the 1-digit to the 4-digit level. | [ILO](https://www.ilo.org/public/english/bureau/stat/isco/) |
| `classification_isco.pdf`  | Document | This document presents the ISCO-08 classification. | [ILO](https://www.ilo.org/public/english/bureau/stat/isco/) |
| `classification_nace.csv`  | Dataset | This dataset includes the NACE Rev.2 industry codes and their labels from the 1-digit to the 3-digit level. | [Eurostat](https://ec.europa.eu/eurostat/statistics-explained/index.php?title=Glossary:Statistical_classification_of_economic_activities_in_the_European_Community_(NACE)) |
| `classification_nace.pdf`  | Document | This document presents the NACE Rev.2 industry classification. |  [Eurostat](https://ec.europa.eu/eurostat/statistics-explained/index.php?title=Glossary:Statistical_classification_of_economic_activities_in_the_European_Community_(NACE)) |
| `classification_naics.csv`  | Dataset | This dataset includes the NAICS (2007) industry codes and their labels from the 2-digit to the 4-digit level. | [BLS](https://www.bls.gov/cew/classifications/industry/naics-2007.htm) |
| `classification_soc.csv`  | Dataset | This dataset includes the ONET-SOC (2010) occupation codes and their labels from the 2-digit to the 8-digit level. | [BLS](https://www.bls.gov/soc/2010/2010_major_groups.htm) |
| `classification_tech40.csv`  | Dataset | This dataset includes the classification of emerging digital technologies. | Authors |

## Data structure

### `classification_isco.csv`

| VARIABLE               | TYPE                    | DESCRIPTION               | MERGE WITH |
| ----------------------- | ------------------------- | ------------------- | -------- |
| `iscoXd`  | Integer | ISCO-08 code at the `X`-digit level | All `techXposure_isco` files |
| `iscoXd_label`  | String | ISCO-08 label at the `X`-digit level | All `techXposure_isco` files |

### `classification_nace.csv`

| VARIABLE               | TYPE                    | DESCRIPTION               | MERGE WITH |
| ----------------------- | ------------------------- | ------------------- | -------- |
| `naceXd`  | String / Numeric[^1] | NACE Rev.2 code at the `X`-digit level | All `techXposure_nace` files |
| `naceXd_label`  | String | NACE Rev.2 label at the `X`-digit level | All `techXposure_nace` files |

### `classification_naics.csv`

| VARIABLE               | TYPE                    | DESCRIPTION               | MERGE WITH |
| ----------------------- | ------------------------- | ------------------- | -------- |
| `naicsXd`  | Integer | NAICS (2007) code at the `X`-digit level | All `techXposure_naics` files |
| `naicsXd_label`  | String | NAICS (2007) label at the `X`-digit level | All `techXposure_naics` files |


### `classification_soc.csv`

| VARIABLE               | TYPE                    | DESCRIPTION               | MERGE WITH |
| ----------------------- | ------------------------- | ------------------- | -------- |
| `socXd`  | Numeric | ONET-SOC (2010) code at the `X`-digit level | All `techXposure_soc` files |
| `socXd_label`  | String | ONET-SOC (2010) label at the `X`-digit level | All `techXposure_soc` files |

### `classification_tech40.csv`

| VARIABLE               | TYPE                    | DESCRIPTION               | MERGE WITH |
| ----------------------- | ------------------------- | ------------------- | -------- |
| `family40_id`  | Integer | Technology family identifier | |
| `family40_label`  | String | Technology family label | |
| `tech40_id`  | Integer | Technology identifier | All `techXposure` files |
| `tech40_label`  | String | Technology label | All `techXposure` files |
| `tech40_labelshort`  | String | Technology label (short version) | |
| `cluster40_id`  | String | Technology cluster identifier | Primary data |
| `description`  | String | Technology description | |


[^1]: The NACE Rev.2 code is a string variable at the 1-digit level and a numeric variable at the 2-digit and 3-digit levels.