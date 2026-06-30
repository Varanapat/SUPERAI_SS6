# SUPERAI_SS6

A collection of notebooks from **SUPER AI Engineer Season 6**, covering data analysis, machine learning, deep learning, NLP, OCR, computer vision, and hackathon-style submission workflows.

## Project Overview

This repository contains Jupyter Notebooks created for learning exercises and Mini Hackathons. The notebooks explore multiple AI and data science tasks, including:

- Exploratory Data Analysis (EDA) and data visualization
- Machine learning for tabular data
- Thai Natural Language Processing
- OCR and computer vision
- Retrieval-Augmented Generation (RAG)
- Deep learning for time-series/signal classification

## Notebooks

| File | Topic | Description |
| --- | --- | --- |
| `MiniHack1.ipynb` | Thai fishery import/export analysis | Analyzes `import_export.csv` with Polars and Plotly to answer questions about trade partners, major products, and trade trends. |
| `605558_Mini_Hackathon_1_Online.ipynb` | Tabular ML / Classification | Performs EDA, feature engineering, model comparison, SHAP analysis, and generates `submission.csv`. |
| `605558_Heart_disease.ipynb` | Heart Disease Prediction | Covers data cleaning, outlier detection, encoding, feature selection, model training, and prediction on `test.csv`. |
| `605558_Word_Segmentation.ipynb` | Thai Word Segmentation | Prepares data, builds features, trains a segmentation approach, evaluates F1-score, and creates submission files. |
| `MiniHack2.ipynb` | OCR | Uses OpenCV, PyTesseract, PyThaiNLP, and fuzzy matching to extract text from images and prepare a submission file. |
| `MiniHack3.ipynb` | RAG / Information Retrieval | Builds a retrieval pipeline with document loading, chunking, FAISS vector search, BM25, hybrid retrieval, reranking, and top-k selection. |
| `605558_SleepStage.ipynb` | Sleep Stage Classification | Processes time-series data, trains LSTM/GRU/BiLSTM models with TensorFlow/Keras, and generates test predictions. |
| `605558_House_Recognization.ipynb` | Image Classification | Uses a Vision Transformer (ViT) from Hugging Face Transformers for house image classification and submission generation. |

## Repository Structure

```text
SUPERAI_SS6/
├── 605558_Heart_disease.ipynb
├── 605558_House_Recognization.ipynb
├── 605558_Mini_Hackathon_1_Online.ipynb
├── 605558_SleepStage.ipynb
├── 605558_Word_Segmentation.ipynb
├── MiniHack1.ipynb
├── MiniHack2.ipynb
├── MiniHack3.ipynb
└── README.md
```

> Note: Large datasets and competition datasets are not included in this repository. Please download the required data separately according to each notebook's instructions.

## Getting Started

1. Clone the repository

```bash
git clone https://github.com/Varanapat/SUPERAI_SS6.git
cd SUPERAI_SS6
```

2. Create a virtual environment

```bash
python -m venv .venv
source .venv/bin/activate
```

For Windows:

```bash
.venv\Scripts\activate
```

3. Install common dependencies

```bash
pip install numpy pandas scikit-learn matplotlib seaborn jupyter
```

4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Then open the notebook you want to run.

## Main Dependencies

Each notebook may require different libraries depending on the task. Common dependencies used across the repository include:

- Data analysis: `numpy`, `pandas`, `polars`
- Visualization: `matplotlib`, `seaborn`, `plotly`
- Machine learning: `scikit-learn`, `lightgbm`, `joblib`, `shap`
- Deep learning: `tensorflow`, `torch`, `transformers`
- NLP / Thai NLP: `pythainlp`, `rank-bm25`, `sentence-transformers`
- Vector search: `faiss`
- OCR / image processing: `opencv-python`, `pytesseract`, `Pillow`, `thefuzz`
- Kaggle workflow: `kagglehub`

If a notebook reports a missing package, install it with:

```bash
pip install <package-name>
```

## Required Data

Several notebooks expect local files or Kaggle competition datasets, such as:

- `train.csv`, `test.csv`, `sample_submission.csv`
- `import_export.csv`
- `ws_test.txt`, `ws_sample_submission.csv`
- Image folders or files from Kaggle competitions
- Document files for the RAG pipeline

Place the data files in the paths expected by each notebook, or update the notebook paths to match your local environment.

## Generated Outputs

Some notebooks generate output files such as:

- Submission files: `submission.csv`, `submission_results.csv`, `sample_submission_V3.csv`
- Saved models: `.pkl`
- EDA and model diagnostic plots: `.png`
- Model prediction files: `test_predictions.csv`

These files are usually created after running the notebooks and may not be committed to the repository.

## Notes

- Some notebooks were developed on Kaggle or Google Colab, so they may contain environment-specific paths such as `/kaggle/input/...`.
- When running locally, you may need to adjust file paths and install additional system dependencies, such as Tesseract OCR for `pytesseract`.
- This repository is intended for learning, experimentation, and hackathon submission preparation.

