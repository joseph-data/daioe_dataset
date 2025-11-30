# DAIOE datasets

[![DOI](https://zenodo.org/badge/1106807158.svg)](https://doi.org/10.5281/zenodo.17765749)

This repository hosts the DAIOE (Direct AI Occupational Exposure) index in multiple occupational classifications. Each dataset folder includes three file formats for convenience: `.csv`, `.dta` (Stata), and `.xlsx` (Excel).

## Flavours (occupational classifications)
- `daioe_isco08`: ISCO-08 (international)
- `daioe_onetsoc2010`: O*NET-SOC 2010 (US)
- `daioe_soc2010`: SOC 2010 (US)
- `daioe_ssyk96`: SSYK 96 (Sweden)
- `daioe_ssyk2012`: SSYK 2012 (Sweden)

## File formats per folder
- `daioe_<flavour>.csv`
- `daioe_<flavour>.dta`
- `daioe_<flavour>.xlsx`

## Column layout (all files)
- Col A: occupational code  
- Col B: occupational title  
- Col C: year  
- Cols D–N: DAIOE index scores (overall + nine sub-domains + generative AI)  
- Cols O–Y: DAIOE percentile rankings (overall + nine sub-domains + generative AI)  

### Index structure
- Col D (O): overall DAIOE index (ranking)
- Cols E–M (P–X): nine sub-domain DAIOE indices (rankings)
- Col N (Y): generative AI DAIOE index (ranking)

### Notes
- Early rows may be empty for armed forces occupations or legislators where DAIOE cannot be computed due to missing O*NET observations.
- Scores allow comparison of AI exposure across occupations and over time; a one-unit change has no standalone interpretation.
