# DAIOE Datasets: Direct AI Occupational Exposure

[![DOI](https://zenodo.org/badge/1106807158.svg)](https://doi.org/10.5281/zenodo.17765749)

This repository hosts the **Direct AI Occupational Exposure (DAIOE)** index across multiple international and national occupational classifications. The DAIOE index measures the exposure of various occupations to Artificial Intelligence by mapping AI capabilities to occupational task requirements.

Each dataset folder includes the data in `.csv`, `.dta` (Stata), and `.xlsx` (Excel) formats to ensure broad research accessibility.

## Classifications

- `daioe_isco08`: ISCO-08 (International Standard Classification of Occupations)
- `daioe_onetsoc2010`: O*NET-SOC 2010 (United States)
- `daioe_soc2010`: SOC 2010 (United States)
- `daioe_ssyk96`: SSYK 96 (Sweden)
- `daioe_ssyk2012`: SSYK 2012 (Sweden)

## Data Structure

All files follow a standardized column layout across the index scores and percentile rankings.

### Column Mapping

| Column(s) | Variable Type | Description |
| :--- | :--- | :--- |
| A | `occ_code` | Occupational classification code |
| B | `occ_title` | Occupational title |
| C | `year` | Reference year |
| D-N | `daioe_*` | Index Scores (Overall, Sub-domains, and Generative AI) |
| O-Y | `pctl_rank_*` | Percentile Rankings (Overall, Sub-domains, and Generative AI) |

### AI Applications (Sub-domains)

The index is built from the following specific AI capability domains:

1. **Strategic Games** (`stratgames`)
2. **Video Games** (`videogames`)
3. **Image Recognition** (`imgrec`)
4. **Image Compression** (`imgcompr`)
5. **Image Generation** (`imggen`)
6. **Reading Comprehension** (`readcompr`)
7. **Language Modeling** (`lngmod`)
8. **Translation** (`translat`)
9. **Speech Recognition** (`speechrec`)
10. **Generative AI** (`genai`) - *Specialized index*
11. **Overall Exposure** (`allapps`) - *Aggregated index*

## Important Notes

- **Data Gaps:** Some early rows may be empty for specific occupations (e.g., armed forces or certain legislators) where the DAIOE cannot be computed due to missing O*NET task observations.
- **Interpretation:** Scores are designed to allow comparison of AI exposure across different occupations and over time. Note that a one-unit change in the raw index score does not have a standalone physical interpretation; users should typically rely on percentile rankings for comparative analysis.

## Related Projects

- [Translation Helper Utility](https://github.com/joseph-data/07_translate_ssyk): Provides English translations for SSYK 2012 and SSYK 96 occupational titles.

## Citation

If you use this dataset in your research, please cite it as follows:

```bibtex
@dataset{joseph_nyajuoga_2025_17765750,
  author       = {Joseph Nyajuoga},
  title        = {joseph-data/daioe_dataset: AI-Econ Lab, Örebro University},
  month        = nov,
  year         = 2025,
  publisher    = {Zenodo},
  version      = {v1.0.0},
  doi          = {10.5281/zenodo.17765750},
  url          = {https://doi.org/10.5281/zenodo.17765750},
}
```

## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.
