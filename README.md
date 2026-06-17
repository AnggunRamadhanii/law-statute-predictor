# ⚖️ Law Statute Predictor using Case-Based Reasoning (CBR)

This repository implements a Case-Based Reasoning (CBR) system for legal document similarity matching (Case Retrieval) and statute prediction using TF-IDF Vectorizer and Cosine Similarity.

---

## End-to-End Pipeline

The entire workflow is integrated into one notebook (`notebooks/Penalaran_Komputer_Final.ipynb`) and includes:

1. Case Base Construction
   - Collect, clean, and organize past legal cases into `data/processed/cases.csv`.

2. Case Representation
   - Transform case text into numerical feature vectors using TF-IDF.

3. Case Retrieval
   - Compute similarity scores between new queries and past cases using Cosine Similarity.

4. Case Prediction
   - Recommend statutes from the most similar past cases.
   - Save predictions to `data/results/predictions.csv`.

5. Model Evaluation
   - Evaluate system performance using `data/eval/queries.json`.
   - Save metrics to `data/eval/`.

---

## Installation & Usage

### 1. Install Requirements
Ensure Python 3.8+ is installed. From the project root, run:

pip install -r requirements.txt

### 2. Run the Pipeline

Option A: Jupyter Notebook (Browser)
-----------------------------------
jupyter notebook

- Navigate to `notebooks/`
- Open `Penalaran_Komputer_Final.ipynb`
- Run cells sequentially

Option B: VS Code
-----------------
1. Open this folder in VS Code.
2. Open `notebooks/Penalaran_Komputer_Final.ipynb`.
3. Select the correct Python kernel.
4. Click **Run All** to execute the pipeline.

---

## Output Verification
Successful execution generates:

- `data/results/predictions.csv`
- `data/eval/retrieval_metrics.csv`
- `data/eval/prediction_metrics.csv`

---
## 👥 Contributors / Team Members
- Anggun Ramadhani (202310370311077)


