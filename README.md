# Smallworld Demo — Data Workflow (SQLite → Master Dataset → Validation → Curated Export)

This demo notebook shows an end-to-end data workflow:

1. Load an SQLite database  
2. Inspect source tables  
3. Join into a master dataset using `Field_ID` (explicit column selection)  
4. Validate data quality (duplicates, missingness, range sanity, simple rule checks)  
5. Curate the schema and export a clean dataset  

## Output
- `smallworld_curated.csv` — the final curated dataset ready for analysis and modeling

---

## Run in Google Colab

1. Open the notebook in Google Colab  
2. Run the first cell and upload the `.db` file when prompted  
3. Run all cells from top to bottom  

---

## Run locally

```bash
python -m venv .venv
source .venv/bin/activate   # On Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook
