# MATH 170 — Lecture Notebooks

Emory University, Fall 2026. Notebooks that go with the lectures, one file per
chapter of Sundnes, *Introduction to Scientific Programming with Python*.

**Nothing here is submitted.** These are yours to work in. Labs are a separate
repository and go through Gradescope.

## Setup (once)

You already installed Git and Python 3.10+ in Lab 01.

```
git clone https://github.com/jimena-martin-emory/math170-lectures.git
cd math170-lectures
pip install -r requirements.txt
```

## Working in a notebook

**Copy it first. Never type into the file inside `notebooks/`.**

```
mkdir -p work
cp notebooks/02_computing_with_formulas.ipynb work/
jupyter lab
```

Open the copy in `work/` and do everything there. The `work/` folder is ignored
by Git, so your answers are safe and updates never overwrite them.

## Getting new chapters

```
git pull
```

## If `git pull` gives an error

An error mentioning *"local changes would be overwritten"* means you typed into
a file inside `notebooks/`. Rescue it:

```
git stash
git pull
git stash pop
```

Then copy the notebook into `work/` and continue there. Bring it to Friday lab
if it does not clear up — do not spend an evening on it.
