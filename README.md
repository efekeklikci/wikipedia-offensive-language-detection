# Toxic Language Detection (Multi-Label) — TF-IDF Baseline vs DistilBERT

This project builds a **multi-label toxic comment classifier** (e.g., toxic, obscene, threat, insult, identity_hate, severe_toxic).  
I compare a classical baseline (**TF-IDF + Logistic Regression**) with a transformer model (**fine-tuned DistilBERT**) and provide a simple inference function to score new text.

## Highlights
- Multi-label classification (one comment can belong to multiple toxicity categories)
- Baseline: TF-IDF + One-vs-Rest Logistic Regression
- Transformer: DistilBERT fine-tuning
- Evaluation with micro/macro F1 and per-label metrics
- Inference helper to print label probabilities and flagged labels

## Project Structure (suggested)

## Dataset
This project uses a toxic comment dataset with the following labels:
`toxic, severe_toxic, obscene, threat, insult, identity_hate`.

## Setup
### Option A: Run in Google Colab (recommended)
- Open the notebook in Colab and run cells in order.
- If you save models to Google Drive, mount Drive when prompted.

### Option B: Run locally
1. Create and activate a virtual environment
2. Install dependencies:
```bash
pip install -r requirements.txt
