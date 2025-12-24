## responsesToPrompts/scores

This folder holds **derived score tables** built from `merged_csv.csv` and `master_scores.csv`.

Examples (content depends on which helper scripts were run):

- `merged_with_taales.csv` – merged responses with TAALES indices attached.  
- `merged_with_taaco.csv` – merged responses with TAACO cohesion metrics.  
- `merged_with_readability_flesch_only.csv` – merged responses with Flesch scores only.  
- `master_scores.csv` – a copy of the main master score table for convenience.

These files are *convenience outputs* for analysis. The canonical inputs for plotting are:

- `responsesToPrompts/merged_csv.csv`  
- `responsesToPrompts/master_scores.csv`

