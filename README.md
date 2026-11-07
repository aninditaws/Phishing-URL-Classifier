# Phishing URL Classifier

A Python/Jupyter team project comparing custom K-Nearest Neighbour (KNN) and Gaussian Naive Bayes classifiers with scikit-learn implementations on phishing URL data.

**Anindita's contribution:** Data cleaning, preprocessing, and pipeline assembly. Classifier implementation responsibilities are listed in the contribution table below.

[Portfolio case study](https://aninditaws.github.io/projects/phishing-classifier/)

## Project scope

- Prepare training/test data and handle missing values.
- Apply preprocessing and compare classification approaches.
- Evaluate predictions using classification metrics in the notebook.

This is an academic project for IF3070 Dasar Inteligensi Buatan at ITB. Results depend on the dataset, split, and preprocessing choices; this repository does not establish production phishing-detection performance.

## Run the notebook

Requires Python, pip, and Jupyter. Run the notebook from `src/` so the relative `../data/` paths resolve correctly.

```bash
git clone https://github.com/aninditaws/Phishing-URL-Classifier.git
cd Phishing-URL-Classifier
python -m venv .venv
```

Activate the environment:

```bash
# macOS / Linux
source .venv/bin/activate
```

```powershell
# Windows PowerShell
.venv\\Scripts\\Activate.ps1
```

Install the notebook's third-party dependencies, then start Jupyter:

```bash
python -m pip install notebook pandas numpy scikit-learn imbalanced-learn
cd src
jupyter notebook IF3070_DAI_TugasBesar2_finalboss.ipynb
```

The repository does not pin dependency versions. These commands describe the notebook's imports and file layout; package compatibility and a complete notebook execution should be checked in your environment. Full runs can take time for the custom models.

## Repository structure

```text
README.md
data/
  sample_submission.csv
  test.csv
  train.csv
doc/
  Tubes2_finalboss.pdf
models/
  gnb.pkl
  knn.pkl
src/
  IF3070_DAI_TugasBesar2_finalboss.ipynb
```

## Team contributions

| NIM      | Nama Lengkap           | Tugas                                                                                     |
|----------|------------------------|-------------------------------------------------------------------------------------------|
| 18222113 | Angelica Aliwinata     | Modelling Naive Bayes                                                                     |
| 18222116 | Jason Jahja            | Modelling KNN                                                                             |
| 18222123 | Melissa Trenggono      | Modelling Naive Bayes                                                                     |
| 18222128 | Anindita Widya Santoso | Data Cleaning & Preprocessing, Compile Pipeline                                           |
