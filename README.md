# MATH 170 — Lecture Notebooks

Emory University, Fall 2026. Notebooks that go with the lectures, one file per
chapter of Sundnes, *Introduction to Scientific Programming with Python*.

**Nothing here is submitted.** These are yours to work in. Labs are a separate
repository and go through Gradescope.

Full instructions are on the Canvas "Lecture notebooks" page. Short version:

## Setup (once)

You already have Anaconda, VS Code, the Python extension and Git from Lab 01.

In VS Code, **Terminal → New Terminal**:

```
git clone https://github.com/jimena-martin-emory/math170-lectures.git
```

Then **File → Open Folder** and choose `math170-lectures`.

## Working in a notebook

**Copy it first. Never type into the file inside `notebooks/`.**

```
mkdir -p work
cp notebooks/02_computing_with_formulas.ipynb work/
```

Open the copy in `work/`. The first time, click **Select Kernel** at the top
right → **Python Environments** → the Anaconda one. Run cells with
**Shift+Enter**.

You should not need to install packages — Anaconda already has NumPy, SciPy and
Matplotlib. If a cell says something is missing, ask rather than guessing at an
install.

The `work/` folder is ignored by Git, so your answers are safe there and updates
never overwrite them.

## Getting new chapters

```
git pull
```

## If `git pull` gives an error

*"local changes would be overwritten"* means you typed into a file inside
`notebooks/`. Rescue it:

```
git stash
git pull
git stash pop
```

Then copy the notebook into `work/` and continue there. Bring it to Friday lab
if it does not clear up — do not spend an evening on it.
