# DAIOE Datasets: Direct AI Occupational Exposure

This repository hosts the **Direct AI Occupational Exposure (DAIOE)** index across multiple international and national occupational classifications. The DAIOE index measures the exposure of various occupations to Artificial Intelligence by mapping AI capabilities to occupational task requirements.

Each dataset folder includes the data in `.csv`, `.dta` (Stata), and `.xlsx` (Excel) formats to ensure broad research accessibility.

## Classifications

- `daioe_isco08`: ISCO-08 (International Standard Classification of Occupations)
- `daioe_onetsoc2010`: O*NET-SOC 2010 (United States 🇺🇸)
- `daioe_soc2010`: SOC 2010 (United States 🇺🇸)
- `daioe_ssyk96`: SSYK 96 (Sweden 🇸🇪)
- `daioe_ssyk2012`: SSYK 2012 (Sweden 🇸🇪)

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

1. ♟️ **Strategic Games** (`stratgames`)
2. 🎮 **Video Games** (`videogames`)
3. 🖼️ **Image Recognition** (`imgrec`)
4. 🧩 **Image Compression** (`imgcompr`)
5. 🎨 **Image Generation** (`imggen`)
6. 📖 **Reading Comprehension** (`readcompr`)
7. ✍️ **Language Modeling** (`lngmod`)
8. 🌐 **Translation** (`translat`)
9. 🎙️ **Speech Recognition** (`speechrec`)
10. 🧠 **Generative AI** (`genai`) - *Specialized index*
11. 📚 **Overall Exposure** (`allapps`) - *Aggregated index*

## Important Notes

- **Data Gaps:** Some early rows may be empty for specific occupations (e.g., armed forces) where the DAIOE cannot be computed due to missing O*NET task observations.
- **Interpretation:** Scores are designed to allow comparison of AI exposure across different occupations and over time. Note that a one-unit change in the raw index score does not have a standalone physical interpretation; users should typically rely on percentile rankings for comparative analysis.

## Related Projects

- [Translation Helper Utility](https://github.com/joseph-data/07_translate_ssyk): Provides English translations for SSYK 2012 and SSYK 96 occupational titles.



## License

The dataset/data files are dedicated to the public domain under **CC BY 4.0**. See the [LICENSE](LICENSE) file for details.

## References

For further reading head to the [AI-Econ Lab Website](https://www.ai-econlab.com/ai-exposure-daioe).
