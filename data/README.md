# Data

## Source

Otoritas Jasa Keuangan (OJK), [LPBBTI statistics](https://ojk.go.id/id/kanal/iknb/data-dan-statistik/fintech/default.aspx), including the [December 2025 publication](https://ojk.go.id/id/kanal/iknb/data-dan-statistik/fintech/Pages/Statistik-LPBBTI-Desember-2025.aspx). Accessed 20 August 2026.

Cite as: Otoritas Jasa Keuangan, *Statistik LPBBTI*, December 2021 to December 2025 publications, accessed 20 August 2026.

## Files in `data/raw/`

The raw files are not included. Download the December publication of each year (2021–2025) and save it as:
`STATISTIK LPBBTI Desember <year>.xlsx`

The notebook builds the paths from these names, so keep them unchanged. It reads sheet `2` (Table 2) with the header on the second row.

## Notes

- Values are monthly balances in billion rupiah, not annual flows. The 2021 report starts in May, and blank months are unavailable data, not zero.
- Raw files are never overwritten. Adjustments are made on an in-memory copy and logged in `adjustment_log`.
- OJK may revise published data. The analysis used the versions downloaded on the access date.
- The data belongs to OJK, including the reshaped copy in `data/clean/`. OJK's terms (*Syarat dan Kondisi*) allow quoting its information with a full citation, but do not explicitly address redistributing whole files, so `data/raw/*.xlsx` and `data/clean/*.xlsx` are in `.gitignore`.
- This is an independent analysis, not affiliated with or endorsed by OJK.