# Setup Guide: Python Environment & Jupyter Notebooks

To run the lecture materials, use a Python virtual environment so course packages stay isolated from the rest of your system.

In a terminal, go to the course folder (this repo’s root), then:

## 1. Create the environment (first time only)

**macOS / Linux:**

```bash
python3 -m venv venv
```

**Windows (Command Prompt or PowerShell):**

```bash
python -m venv venv
```

## 2. Activate the environmentw

You must activate **before** installing packages or starting Jupyter so the notebooks use this Python.

**macOS / Linux:**

```bash
source venv/bin/activate
```

**Windows (Command Prompt):**

```bash
venv\Scripts\activate.bat
```

**Windows (PowerShell):**

```bash
venv\Scripts\Activate.ps1
```

Your prompt usually shows `(venv)` when it is active.

## 3. Install dependencies

With the environment activated:

```bash
pip install -r requirements.txt
```

## 4. Open the lecture notebooks

Still with `venv` active:

```bash
jupyter lab
```

or:

```bash
jupyter notebook
```

Then open the lecture `.ipynb` files from the file browser.

**Deactivate** when you are done (optional):

```bash
deactivate
```
