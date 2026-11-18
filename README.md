*English · [Русский](README.ru.md)*

# Hi, I'm Sergey Karmanov!

MSc, Novosibirsk State University (Faculty of Natural Sciences, 2026). ML experience with biological and biomedical data.

[kainanasarlil@gmail.com](mailto:kainanasarlil@gmail.com) · [LinkedIn](https://www.linkedin.com/in/sergey-karmanov/) · [Telegram](https://t.me/Kain8800)

---

## Tech stack

### Confident
- **Python:** NumPy, pandas, matplotlib, scikit-learn
- **HPC:** cluster computing (PBS), conda environments, GPU model inference
- **Data:** processing and cleaning, exploratory analysis, visualization, feature engineering
- **Document processing:** data extraction from PDF (`pdfplumber`)
- **Validation:** homology stratification (MMseqs2), data-leakage control, control experiments on shuffled labels
- **Tools & databases:** Git, SQL, Linux
- **Bioinformatics:** sequences, annotations, biological databases (UniProt, RefSeq, KEGG, ODB)

### Learning
- **LLM / RAG:** prompt engineering, RAG pipelines, OpenAI API
- **Pipelines:** Docker, Nextflow
- **Backend for ML services:** FastAPI

---

## Education

### Novosibirsk State University (NSU)
- MSc in bioinformatics, Faculty of Natural Sciences, 2023–2026
- Thesis: "EC-number prediction for enzymes with operon structure using AI"

### Saratov State University (N. G. Chernyshevsky)
- Professional retraining program "Data Processing Specialist", Digital Department, 2022–2023
- Final project (co-authored): "Cancer diagnostics from biomarkers using machine learning"

---

## Projects & experience

### Master's thesis: EC-number prediction for enzymes
Pipeline: data collection from four sources, predictions from off-the-shelf models (ProteInfer, CLEAN), a verification filter based on operon context, and stratified quality evaluation.
- Macro-F1 **0.807 → 0.887**, accuracy 0.967 → 0.982; coverage drops from 0.879 to 0.716 because the filter rejects uncertain predictions
- The largest gain is where the model is weakest: **+0.124 F1** on low-homology proteins
- Validation: homology stratification (MMseqs2), per-sequence leakage exclusion, a reproducible pipeline
- Data sources: ODB, RefSeq, UniProtKB, KEGG; PDF parsing (`pdfplumber`)
- Repository: [prokaryotic-ec-operon-filter](https://github.com/Kain8800/prokaryotic-ec-operon-filter)

### Spotify Churn Analysis: diagnosing the absence of signal in data
Negative result: the data carries no signal for predicting churn.
- ROC-AUC **0.50** across all models and preprocessing strategies; the tuned model loses to a constant predictor
- Five control experiments confirm the result: a pipeline check on data with a known signal, comparing real labels against deliberately shuffled ones, an examination of what class balancing does, calibration of the mutual-information estimate, and a demonstration of overfitting
- Practical takeaway: how to tell "the model is undertrained" from "there is no signal in the data" before spending time on tuning
- Repository: [spotify-churn-analysis](https://github.com/Kain8800/spotify-churn-analysis)

### Navi: a Telegram bot for channel navigation
- Post indexing, full-text search, and navigation through an inline interface
- Asynchronous architecture (aiohttp, Telethon, asyncio) in webhook mode, running in production on Render
- Repository: [Navi](https://github.com/Kain8800/Navi)

### Research Assistant | AI Centre, NSU
- Preparing and processing datasets for research
- Taking part in planning and running experiments
- Exploratory analysis of metabolomic data: searching for correlations between metabolites
- Drafting and reviewing part of a research paper (co-author, see Publications)

### Hackathons
**Sistema Hack: Novosibirsk** (MTS and the Sistema Charitable Foundation, hosted at NSU), 14–16 November 2025. Team of four, CDEK case: a tool for diagnosing and preventing employee burnout. I was responsible for defining the metrics, justifying the applicability of the burnout criteria, and the ML part.

**Cookie Fest**, Novosibirsk, 29 November – 2 December 2024. Team of two, predicting employee burnout from HR data (18,590 records). I was responsible for data preparation and exploratory analysis, and for presenting the solution.

---

## Publications

**Gene networks and metabolomic screening analysis revealed specific pathways of amino acid and acylcarnitine profile alterations in blood plasma of patients with Parkinson's disease and vascular parkinsonism**

Makarova A.A., Melnikova P.M., Rogachev A.D., Demenkov P.S., Ivanisenko T.V., Predtechenskaya E.V., **Karmanov S.Yu.**, Koval V.V., Pokrovsky A.G., Lavrik I.N., Kolchanov N.A., Ivanisenko V.A. // Vavilov Journal of Genetics and Breeding. 2024. Vol. 28, no. 8, pp. 927–939.

Metabolomic screening of amino acids and acylcarnitines in blood plasma and reconstruction of regulatory gene networks to find mechanisms specific to Parkinson's disease and vascular parkinsonism. Indexed in PubMed and Scopus, open access.

[DOI: 10.18699/vjgb-24-100](https://doi.org/10.18699/vjgb-24-100)

---

## Career goal

Seeking a Junior/Mid-level role in one of the following areas:
- Bioinformatics: NGS data analysis, pipeline development, genomics
- Data Science / ML: models on tabular and biological data, model validation, data and metric quality control
- LLM / RAG: LLM-based applications and RAG systems
