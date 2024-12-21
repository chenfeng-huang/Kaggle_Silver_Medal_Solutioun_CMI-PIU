## Data source and usage

Data for this project comes from the Kaggle competition [Child Mind Institute — Problematic Internet Use](https://www.kaggle.com/competitions/child-mind-institute-problematic-internet-use/data).

### What to download

- `train.csv`, `test.csv`, `sample_submission.csv`
- `series_train.parquet/` and `series_test.parquet/`, each containing per‑participant folders like `id=<participant_id>/part-0.parquet`

### Where to place the files

Place all files under `dataset/` with the following layout:

```
dataset/
├─ train.csv
├─ test.csv
├─ sample_submission.csv
├─ series_train.parquet/
│  └─ id=<participant_id>/part-0.parquet
└─ series_test.parquet/
   └─ id=<participant_id>/part-0.parquet
```

### Git policy (large files)

This repository ignores large competition artifacts to respect size and licensing:

- Ignored: `dataset/train.csv`, `dataset/test.csv`, `dataset/series_train.parquet/`, `dataset/series_test.parquet/`
- Tracked: `dataset/sample_submission.csv`

See `.gitignore` for details.

### Competition data rules (summary)

- The competition data consists of public and private test sets; which is which is not disclosed to participants.
- Access and use are allowed for non‑commercial purposes only (participation, research, education) during the competition; terms may change thereafter.
- Phenotypic/tabular survey data are de‑identified. You must not redistribute the data, attempt re‑identification, or probe the test labels. Report any PII findings to organizers via Kaggle forums.
- Keep data secure; do not share it with non‑participants. Notify Kaggle of any unauthorized access or transmission.
- External data may be used only if it is publicly available, equally accessible to all participants, and free of charge, and all other competition rules still apply.

### Citation

If you reference or use the dataset, include the following citation:

“CMI 2024 Problematic Internet Use Detection Challenge”

Adam Santorelli, Arianna Zuanazzi, Michael Leyden, Logan Lawler, Maggie Devkin, Yuki Kotani, and Gregory Kiar. Child Mind Institute — Problematic Internet Use. https://kaggle.com/competitions/child-mind-institute-problematic-internet-use, 2024. Kaggle.

BibTeX:

```bibtex
@misc{child-mind-institute-problematic-internet-use,
    author = {Adam Santorelli and Arianna Zuanazzi and Michael Leyden and Logan Lawler and Maggie Devkin and Yuki Kotani and Gregory Kiar},
    title = {Child Mind Institute — Problematic Internet Use},
    year = {2024},
    howpublished = {\url{https://kaggle.com/competitions/child-mind-institute-problematic-internet-use}},
    note = {Kaggle}
}
```