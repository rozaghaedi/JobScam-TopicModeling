# JobScam-TopicModeling

NLP analysis of **fraudulent vs legitimate job postings** using **LDA topic modeling** and **TF-IDF** to surface recurring scam narratives and cues.

## Why this matters
Fraud job ads are a real online-harms vector (identity theft, advance-fee scams). This repo shows how **unsupervised NLP** can reveal patterns in text—skills directly transferable to **misinformation / extremist narrative** analysis.

## What’s inside
- `notebooks/LDA_TopicModelling.ipynb` – build corpus, train LDA, show top words per topic, basic pyLDAvis.
- `notebooks/TFIDF_FraudulentJobs.ipynb` – TF-IDF for the *fraud* subset (+ n-grams) to rank salient terms.
- `data/` – small CSVs for reproducibility (`fake_job_postings.csv`, `FradulentJobs.csv`, `Industry_Count.csv`, `stopwords.txt`).
- `outputs/reqExperience_results.txt` – example cluster/topic keywords dump (“Cluster 0…9”).

> Note: The repo includes **small example files** so notebooks run quickly. Use original datasets locally for full experiments.

## Quickstart
```bash
pip install -r requirements.txt
jupyter notebook notebooks/LDA_TopicModelling.ipynb
jupyter notebook notebooks/TFIDF_FraudulentJobs.ipynb
