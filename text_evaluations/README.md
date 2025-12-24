## responsesToPrompts

This folder contains everything related to **model responses** and their derived scores.

Key files and subfolders:

- `generated_prompts.csv` – prompts to send to models (copied from `questionsGeneration/`).  
- `process_prompts_gemini.py` – calls Gemini, writes `generated_responses_gemini.csv`.  
- `process_prompts_claude.py` – calls Claude, writes `generated_responses_claude.csv`.  
- `process_prompts_openai.py` – calls OpenAI, writes `generated_responses_openai.csv`.  
- `merge_csv_files.py` – merges the three response CSVs into `merged_csv.csv`.  
- `merged_csv.csv` – combined responses + shared metadata (input to scoring).  
- `master_scores.csv` – merged responses plus all automatic metrics
  (output of `master_evaluator.py`).  
- `llm_responses_txt/` – one plain‑text file per model response (used by some metrics).  
- `scores/` – partial or per‑metric CSVs (see its README).

In the **end‑to‑end pipeline**, this folder is where most intermediate and final data land.

