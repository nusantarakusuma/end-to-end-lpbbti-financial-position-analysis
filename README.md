# End-to-End LPBBTI Financial Position Analysis

Exploratory analysis of the monthly financial position of LPBBTI providers in Indonesia, using OJK statistics (Table 2), 2021–2025. The main analysis covers 2022–2025. The full write-up, with research questions, findings and limitations, is in the notebook.

## Project structure

```
├── data/
│   ├── raw/      # OJK source files (input, not included)
│   ├── clean/    # analytics dataset (output)
│   └── README.md # data source and notes
├── figures/      # saved charts (output)
├── notebook/
│   └── end-to-end-lpbbti-financial-position-analysis.ipynb
├── requirements.txt
└── README.md
```

## Data

The OJK files are not included. Download them and save them in `data/raw/` as described in [data/README.md](data/README.md).

## How to run

1. Use Python 3.11 or newer (tested with 3.11).
2. Install the packages:
    ```
    pip install -r requirements.txt
    ```
3. Open `notebook/end-to-end-lpbbti-financial-position-analysis.ipynb` and run all cells from top to bottom. The notebook uses relative paths (`../data/...`), so start Jupyter from inside `notebook/` or open it from there.

## Outputs

- `data/clean/Statistik LPBBTI 2022-2025.xlsx`: the long-format dataset (Year, Account, Period, Billion) used for the analysis. Created when the notebook runs, not included in the repository.
- `figures/`: the three RQ 1 charts (Section 11.3).