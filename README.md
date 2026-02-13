# Text-to-Python Code Generation using Seq2Seq Models

A comprehensive comparative study of sequence-to-sequence architectures (Vanilla RNN, LSTM, LSTM with Attention, and Transformer) for automatic Python code generation from natural language descriptions.

## 🔧 Requirements

### Software Dependencies

```
Python >= 3.8
PyTorch >= 2.0
transformers >= 4.30
datasets >= 2.12
numpy >= 1.24
pandas >= 2.0
matplotlib >= 3.7
sacrebleu >= 2.3
evaluate >= 0.4
```

### Hardware Requirement:2x NVIDIA T4 GPUs 


---

## 📂 Dataset

### Source
**CodeSearchNet Python Dataset** [Dataset](https://huggingface.co/datasets/Nan-Do/code-search-net-python)

### Automatic Download (via Hugging Face)

The notebook automatically downloads the dataset:

```python
from datasets import load_dataset
ds = load_dataset("Nan-Do/code-search-net-python")
```

### Dataset Specifications
- **Total samples:** 10,000 (filtered from full dataset)
- **Filtering criteria:** 
  - Docstring length ≤ 50 tokens
  - Code length ≤ 80 tokens
- **Split:** Train (60%) / Val (20%) / Test (20%)
---

## Running the Project

### Option 1: Run Locally (Jupyter Notebook)

1. **Open the notebook:**
```bash
jupyter notebook "text_to_code.ipynb"
```
2. **Run all cells sequentially:**
   - Environment setup and data loading
   - Data preprocessing and tokenization
   - Model 1 (Vanilla RNN) - Training & Evaluation
   - Training & Evaluation
   - Model 3 (LSTM + Attention) - Training & Evaluation
   - Model 4 (Transformer) - Training & Evaluation
   - Comparative analysis and visualization

### Option 2: Run on Kaggle (Cloud)

**Source Code:** [Kaggle Notebook](https://www.kaggle.com/code/amitroy13/text-to-code2)

1. Open the Kaggle notebook link
2. Click **"Copy & Edit"** to create your own version
3. Enable GPU: Settings → Accelerator → GPU T4 x2
4. Click **"Run All"** to execute all cells
5. Download trained models from output section

**Advantages:**
- Free GPU access (30 hours/week)
- No local setup required
- Pre-configured environment

---

## 💾 Pre-trained Models

**Download Link:** [Google Drive - Trained Models](https://drive.google.com/drive/folders/1ESjnyWN9-6Lq1aDG_Q9i_PuUJkNnuq05?usp=drive_link)

## Acknowledgments

- CodeSearchNet dataset by GitHub and Microsoft Research
- Hugging Face for Transformers library and dataset hosting
- PyTorch team for the deep learning framework
- Kaggle for providing free GPU resources



