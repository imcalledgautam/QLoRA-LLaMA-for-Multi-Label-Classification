# QLoRA + LLAMA Multi-Label Text Classification

An efficient implementation of a **multi-label text classification pipeline** leveraging QLoRA fine-tuning on a LLAMA-based language model.

---

## 📝 What is this?

This project fine-tunes a pre-trained LLAMA language model using **QLoRA (Quantized Low-Rank Adaptation)** for an NLP multi-label classification task.  
It covers:
- Data loading & preprocessing
- Model configuration & training
- Evaluation & predictions

---

## 📁 Project Structure

```
QLoRA_LLAMA_MultiLabel_Classification/
├── data/                       # Training and test datasets
│   ├── train.csv
│   └── test.csv
├── notebook/                   # Main notebook
│   └── QLoRA_LLAMA_MultiLabel_Classification.ipynb
├── outputs/                    # (optional: predictions, plots, logs)
├── custom_files/               # User-provided custom helper files
│   └── .gitkeep
├── requirements.txt            # Python dependencies
├── .gitignore
└── README.md
```

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/your-username/QLoRA_LLAMA_MultiLabel_Classification.git
cd QLoRA_LLAMA_MultiLabel_Classification
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the notebook
```bash
jupyter notebook notebook/QLoRA_LLAMA_MultiLabel_Classification.ipynb
```

---

## 🔷 Key Components

- `data/train.csv` – Training data
- `data/test.csv` – Test data
- `notebook/QLoRA_LLAMA_MultiLabel_Classification.ipynb` – End-to-end notebook with training & evaluation
- `requirements.txt` – List of Python packages needed

---

## 📌 Notes

- Make sure you have a CUDA-enabled GPU for faster training.
- You can save predictions or plots to the `outputs/` folder.
- Notebook runs fully from start to finish – no external scripts needed.

---

## 🔷 Custom Files

This project expects certain custom files to be placed in the `custom_files/` folder before running. These files are not included in the repository (they may be specific to your environment).

Expected files:
- `my_custom_functions.py` – custom helper functions
- `my_config.yaml` – configuration settings

Please ensure you place the appropriate files in `custom_files/` before executing the notebook.

### Example
```
custom_files/
├── my_custom_functions.py
├── my_config.yaml
```

Alternatively, you can set the path to your custom files via an environment variable:
```bash
export CUSTOM_FILES_PATH=/path/to/your/custom_files
```
The notebook will then use that path instead of the default.