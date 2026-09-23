# Dataset Information

This project uses publicly available gene-expression data from the [NCBI Gene Expression Omnibus (GEO)](https://www.ncbi.nlm.nih.gov/geo/).

The original datasets are not included in this repository. The accession pages below are the official source and download location for the data used in this project.

---

## Parkinson's Disease — GSE99039

| Field | Details |
|---|---|
| **Source** | NCBI Gene Expression Omnibus (GEO) |
| **Accession** | GSE99039 |
| **Organism** | *Homo sapiens* |
| **Platform** | GPL570 — Affymetrix Human Genome U133 Plus 2.0 Array |
| **Sample type** | Whole blood |

**Official GEO record:** https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE99039

**Data file used:** `GSE99039_series_matrix.txt.gz`

The analysis uses the processed expression values provided in the GEO Series Matrix file. The raw `GSE99039_RAW.tar` archive was not used.

For the Parkinson's disease analysis, the original dataset was filtered to retain idiopathic Parkinson's disease and control samples. Other neurological and genetic/mutation-related groups were excluded according to the analysis protocol.

---

## Alzheimer's Disease — GSE85426

| Field | Details |
|---|---|
| **Source** | NCBI Gene Expression Omnibus (GEO) |
| **Accession** | GSE85426 |
| **Organism** | *Homo sapiens* |
| **Platform** | GPL14550 — Agilent-028004 SurePrint G3 Human GE 8x60K Microarray |
| **Sample type** | Peripheral blood |

**Official GEO record:** https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE85426

**Data file used:** `GSE85426_series_matrix.txt.gz`

The analysis uses the processed expression values provided in the GEO Series Matrix file.

The GEO record describes 180 peripheral-blood samples: 90 Alzheimer's disease samples and 90 non-demented controls.

---

## Local Data Directory

Downloaded datasets should be placed in `data/raw/` relative to the project root.

**Expected files:**

```
project-root/
├── data/
│   └── raw/
│       ├── GSE99039_series_matrix.txt.gz
│       └── GSE85426_series_matrix.txt.gz
├── src/
├── studies/
└── README.md
```

The analysis code may further process or transform these files during execution.

---

## Data Usage

The downloaded GEO files are used locally for preprocessing and analysis. They are intentionally not committed to this repository.

This repository contains:

- preprocessing and analysis code
- study-specific notebooks and scripts
- derived results and evaluation tables
- documentation of the data sources and analysis protocols

The original datasets remain available from their official NCBI GEO records above.

---

## Reproducibility

To reproduce the analyses:

1. Open the relevant GEO accession page above.
2. Download the corresponding Series Matrix file.
3. Place the downloaded file in `data/raw/` in the project root.
4. Follow the instructions in the main project README and the corresponding study analysis.

---

**Data source:** [NCBI Gene Expression Omnibus (GEO)](https://www.ncbi.nlm.nih.gov/geo/)

**Project:** Explainable Machine Learning for Cross-Neurodegenerative Disease Biomarker Discovery from Blood Transcriptomics
