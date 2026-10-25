# Week 6 — Large Language Models & Embeddings

This repository contains the Jupyter Notebook solution for the IIT Week 6 Graded Mini Project on Large Language Models (LLMs) and embeddings.

The notebook is included exactly as supplied by the author; it has not been edited during repository preparation.

## Project scope

The assignment explores text generation, tokenisation, prompt engineering, word embeddings, sentence-level similarity, and a transformer application.

### Section A — LLM Foundations & Hugging Face
- Loads the `distilgpt2` text-generation model.
- Generates three continuations for the prompt `AI is transforming industries by`.
- Tokenises the sentence `LLMs are powerful tools for natural language understanding.` and displays tokens, token IDs, and sequence length.

### Section B — Prompt Engineering
- Experiments with prompts for summarisation, factual question answering, and creative text generation.
- The assignment asks for a 100–150 word reflection comparing how prompt rephrasing changes outputs. Check the notebook against this requirement before treating the submission as complete; the notebook is preserved unchanged in this repository.

### Section C — Embeddings with Gensim
- Loads the `glove-wiki-gigaword-50` vectors through Gensim.
- Displays vector values and nearest words for `king`, `queen`, and `diamond`.
- Creates simple average-word-vector representations for five sentences and compares them with cosine similarity.

### Section D — Transformer Application
- Runs a Hugging Face sentiment-analysis pipeline on two example texts.
- Includes a short reflection on potential business use and a list of real-world embedding/vector-search applications.

## Tech stack

- Python
- Jupyter Notebook
- Hugging Face Transformers
- DistilGPT-2
- Gensim and GloVe (`glove-wiki-gigaword-50`)
- NumPy
- pandas
- scikit-learn
- PyTorch (used by the Transformers model pipeline)

## Repository contents

- `Week6.ipynb` — original assignment notebook, unchanged.
- `README.md` — project overview and setup instructions.
- `requirements.txt` — Python package dependencies.
- `.gitignore` — common Python/Jupyter exclusions.

## Setup

Use Python 3.10 or 3.11 for a practical starting point, then create a virtual environment.

### Windows PowerShell

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
jupyter notebook
```

Open `Week6.ipynb` and run the cells in order.

## Model downloads and execution notes

The notebook downloads pretrained models and embeddings on first use:
- Hugging Face model: `distilgpt2`
- Hugging Face sentiment-analysis pipeline model (the Transformers default for that pipeline)
- Gensim dataset: `glove-wiki-gigaword-50`

These downloads require an internet connection and can take time. Model outputs may vary by model version, generation settings, and runtime environment. The notebook may use additional disk space for cached model files.

## Limitations and reproducibility

- This is an educational exploration notebook, not a deployed application.
- The notebook was not modified as part of preparing this repository
- Running the notebook requires installing the listed packages and downloading pretrained model/embedding files.

## Suggested future improvements

- Add the missing prompt-rephrasing reflection if it is not present in the submitted version.
- Add a short explanation of how to interpret cosine similarity values.
- Record the tested Python and package versions for more reproducible execution.
- Add screenshots or a short project summary PDF if desired for portfolio presentation.
