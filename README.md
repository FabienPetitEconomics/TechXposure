# TechXposure Database (v0.9.1)

[![DOI](https://zenodo.org/badge/750952450.svg)](https://zenodo.org/doi/10.5281/zenodo.10696075)

TechXposure is a database that provides information on the exposure of industries and occupations to 40 digital technologies that emerged over the last decade (2012–2021). The data are available for several industry and occupation classifications. 

The current version is v0.9.1. For more details on the methodology, see the [Working Paper](https://www.fabienpetit.com/wp/PPLCC_EmploymentImpactEmergingDigitalTechnologies_Oct2024.pdf). 

## International Classifications

- NACE Rev.2 Industries (from 1-digit to 3-digit)
- ISCO-08 Occupations (from 1-digit to 4-digit)

## US Classifications

- NAICS 2007 Industries (from 2-digit to 4-digit)
- ONET-SOC Occupations (from 2-digit to 8-digit)

For more details on the methodology on the US classifications, see the [Working Paper](https://www.fabienpetit.com/wp/PP_EmploymentImpactUS_Feb2025.pdf). 

## List of directories and files

Each directory contains a README file describing each file and subdirectory.

| DATA FILE         | DESCRIPTION                          |
|-------------------|--------------------------------------|
| `_classification` | Classifications used in the database |
| `_isco`           | ISCO-08 Occupation Exposure          |
| `_nace`           | NACE Rev.2 Industry Exposure         |
| `_naics`           | NAICS 2007 Industry Exposure         |
| `_soc`           | ONET-SOC 2010 Industry Exposure         |
| `PPLCC_EmploymentImpactEmergingDigitalTechnologies_Oct2024.pdf` | Working Paper |
| `PP_EmploymentImpactUS_Feb2025.pdf` | Working Paper |

## Citation

Please mention the data as the `TechXposure` database and cite as:

> Prytkova, E., Petit, F., Li, D., Chaturvedi, S., and Ciarli, T. (2024). The Employment Impact of Emerging Digital Technologies. Working Paper.

> Prytkova, E., and Petit, F. (2025). The Employment Impact of Emerging Digital Technologies: Evidence from US Labor Markets. Working Paper.

Citations in `bibtex` format:

```bibtex
@techreport{prytkova2024employment,
  title={{The Employment Impact of Emerging Digital Technologies}},
  author={Prytkova, Ekaterina and Petit, Fabien and Li, Deyu and Chaturvedi, Sugat and Ciarli, Tommaso},
  keywords= {{Occupation Exposure, Industry Exposure, Text as Data, Natural Language Processing, Sentence Transformers, Emerging Digital Technologies, Automation, Employment}},
  type={{Working Paper}},
  year={2024}
}

@techreport{prytkova2025employment,
  title={{The Employment Impact of Emerging Digital Technologies: Evidence from US Labor Markets}},
  author={Prytkova, Ekaterina and Petit, Fabien},
  keywords= {{Occupation Exposure, Industry Exposure, Text as Data, Natural Language Processing, Sentence Transformers, Emerging Digital Technologies, Automation, Employment}},
  type={{Working Paper}},
  year={2025}
}
```

## Feedback

We greatly appreciate feedback and insights from researchers and policymakers to continually improve the `TechXposure` Database. If you have suggestions, questions, or face any issues while using our data, please contact us without hesitation. Your input is vital in enhancing our database and supporting future research. We welcome comments on data accuracy, usability, or desired features. All feedback is valued and will be thoughtfully used to refine the `TechXposure` Database for all.

## Contacts

Ekaterina Prytkova ([ekaterina.prytkova@univ-cotedazur.fr](mailto:ekaterina.prytkova@univ-cotedazur.fr)) & Fabien Petit ([f.petit@ucl.ac.uk](mailto:f.petit@ucl.ac.uk) / [fabienpetit.com](https://www.fabienpetit.com/))

## Acknowledgements

This database is an outcome of [PATHWAYS TO INCLUSIVE LABOUR MARKETS (PILLARS)](https://doi.org/10.3030/101004703). This project received funding from the European Union’s Horizon 2020 Research and Innovation Programme under Grant Agreement No. 101004703.