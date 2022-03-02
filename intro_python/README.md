# Introduction to virtual environments, package management, and Python

## Setup modular environments for working in Python, R, and other bioinformatics and data science tools

### Install conda

Anaconda vs Miniconda: https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html#anaconda-or-miniconda

We will download and install Miniconda: https://docs.conda.io/en/latest/miniconda.html, but later feel free to download and
install Anaconda: https://docs.anaconda.com/anaconda/install/index.html

### Add community channels

```bash
conda config --append channels conda-forge
conda config --append channels bioconda

```

### Install mamba

```bash
conda install -n base -c conda-forge mamba

```

### Create an environment

```bash
mamba create -n datasci python

```

### Activate and test the environment

```bash
python -c 'import sys; print(sys.executable)'

conda activate datasci

python -c 'import sys; print(sys.executable)'

```

### Deactivate and delete the environment

```bash
conda deactivate datasci

conda env remove -n datasci

```

### List available environments

```bash
conda env list

```

### Create a new environment with Jupyter

```bash
mamba create -n datasci python=3.8 nb_conda jupyterlab ipympl nodejs

```

## Introduction to the interactive Jupyter notebook environment

```bash
conda activate datasci

jupyter lab

```

### Install additional package

```bash
mamba install scikit-bio

```

## Introduction to Python
