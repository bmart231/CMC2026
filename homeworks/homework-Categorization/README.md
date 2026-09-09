# Setup — Categorization Homework
PSY/COS 360, Computational Models of Cognition

You need Python plus a few packages (numpy, pandas, scipy, matplotlib, seaborn,
Jupyter). If you already run Jupyter notebooks regularly, skip to step 3.

## 1. Check whether you already have Python

Open a terminal (macOS: Terminal app; Windows: PowerShell) and run:

```
python --version
```

If it prints `Python 3.9` or higher, skip to step 3. Otherwise, do step 2.

## 2. Install Python (Miniconda)

1. Download the Miniconda installer for your OS: <https://www.anaconda.com/download/success>
2. Run it with the default options.
3. Close and reopen the terminal. Check it worked: `conda --version`

## 3. Install the dependencies

In the terminal, go to this folder (the one with `requirements.txt`):

```
cd path/to/homework-Categorization
```

Then:

```
conda create -n ccm python=3.11 -y
conda activate ccm
pip install -r requirements.txt
```

Run `conda activate ccm` again each time you open a new terminal for this homework.

## 4. Open the notebooks

From this folder, with `ccm` activated:

```
jupyter notebook
```

Your browser opens a file list. Click `Homework-Categorization-PartA.ipynb`, then
run cells top to bottom with Shift+Enter. Do Part B the same way.

Keep all the files in this folder together — Part B imports `exemplarproto.py` and
both parts read from `data/`.

## If a notebook says a package is missing

The notebook is using the wrong Python. Close Jupyter, run `conda activate ccm`,
then `jupyter notebook` again from this folder. Still stuck? Post on the Ed
forum with the exact command and full error text.