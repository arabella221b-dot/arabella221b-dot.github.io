# arabella221b-dot.github.io

## What this repository is

This repository contains my Quarto website and two posts analyzing the Palmer Penguins dataset: 
one written in R and one written in Python.

## What to install first

The website was built with:

- Quarto 1.8.27
- uv 0.12.18
- R 4.6.1
- Python 3.14

## Reproduce the website

Run these commands in a terminal:

```bash
git clone https://github.com/arabella221b-dot/arabella221b-dot.github.io.git
cd arabella221b-dot.github.io
uv sync
Rscript -e 'renv::restore()'
uv run quarto render
```
Then rendered website is saved in `docs/`. On macOS, open it with:
```bash
open docs/index.html
```

# Data

Both posts use the [Palmer Penguins dataset](https://allisonhorst.github.io/palmerpenguins/). The R post loads it from the `palmerpenguins` R package, and the Python post loads it from the `palmerpenguins` Python package.

An internet connection is needed to clone the repository and install the packages when setting up the project.