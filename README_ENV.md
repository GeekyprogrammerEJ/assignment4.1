# Python environment for LSTM Regression Assignment

**Note:** TensorFlow supports Python 3.9–3.12. If your default `python3` is 3.14+, use `python3.12` or `python3.11` to create the venv (e.g. `python3.12 -m venv .venv`).

## Option 1: venv (recommended)

From the project folder in a terminal:

```bash
# Create virtual environment (use Python 3.10–3.12 for TensorFlow compatibility)
python3.12 -m venv .venv
# or: python3.11 -m venv .venv
# or: python3 -m venv .venv   # only if python3 is 3.9–3.12

# Activate it
# On macOS/Linux:
source .venv/bin/activate
# On Windows (Command Prompt):
# .venv\Scripts\activate.bat
# On Windows (PowerShell):
# .venv\Scripts\Activate.ps1

# Upgrade pip, then install dependencies
pip install --upgrade pip
pip install -r requirements.txt

# Register the env as a Jupyter kernel (so you can pick it in the notebook)
python -m ipykernel install --user --name=lstm-assignment --display-name "Python (LSTM Assignment)"
```

Then in Jupyter/Cursor: open the notebook, choose kernel **"Python (LSTM Assignment)"**, and run.

## Option 2: conda

```bash
conda create -n lstm-assignment python=3.11 -y
conda activate lstm-assignment
pip install -r requirements.txt
python -m ipykernel install --user --name=lstm-assignment --display-name "Python (LSTM Assignment)"
```

## Verify

```bash
python -c "import keras; import pandas; import numpy; import matplotlib; print('OK')"
```
